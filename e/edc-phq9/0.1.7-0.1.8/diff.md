# Comparing `tmp/edc-phq9-0.1.7.tar.gz` & `tmp/edc-phq9-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-phq9-0.1.7.tar", last modified: Fri Aug 26 02:19:56 2022, max compression
+gzip compressed data, was "edc-phq9-0.1.8.tar", last modified: Sun Sep 25 22:11:23 2022, max compression
```

## Comparing `edc-phq9-0.1.7.tar` & `edc-phq9-0.1.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:19:56.946112 edc-phq9-0.1.7/
--rw-r--r--   0 erikvw     (501) staff       (20)       84 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:19:56.938460 edc-phq9-0.1.7/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:19:56.941659 edc-phq9-0.1.7/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-23 02:17:52.000000 edc-phq9-0.1.7/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 22:19:44.000000 edc-phq9-0.1.7/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-23 02:17:52.000000 edc-phq9-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-23 02:17:52.000000 edc-phq9-0.1.7/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 22:19:44.000000 edc-phq9-0.1.7/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-06-01 22:19:44.000000 edc-phq9-0.1.7/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-01-05 14:54:30.000000 edc-phq9-0.1.7/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 22:19:44.000000 edc-phq9-0.1.7/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1617 2022-08-26 02:19:56.946206 edc-phq9-0.1.7/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      650 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-26 02:19:49.000000 edc-phq9-0.1.7/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-23 02:17:52.000000 edc-phq9-0.1.7/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:19:56.944024 edc-phq9-0.1.7/edc_phq9/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      891 2022-08-23 02:17:52.000000 edc-phq9-0.1.7/edc_phq9/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      396 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      383 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      305 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      351 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      126 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      622 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1140 2022-06-01 22:19:44.000000 edc-phq9-0.1.7/edc_phq9/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      885 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/model_admin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3236 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      655 2022-06-01 22:19:44.000000 edc-phq9-0.1.7/edc_phq9/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:19:56.944718 edc-phq9-0.1.7/edc_phq9/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:19:56.945705 edc-phq9-0.1.7/edc_phq9/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:19:56.945996 edc-phq9-0.1.7/edc_phq9/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      449 2022-08-26 02:19:49.000000 edc-phq9-0.1.7/edc_phq9/tests/tests/test_auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1329 2022-06-01 22:19:44.000000 edc-phq9-0.1.7/edc_phq9/tests/tests/tests.py
--rw-r--r--   0 erikvw     (501) staff       (20)      283 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      379 2022-01-06 03:46:37.000000 edc-phq9-0.1.7/edc_phq9/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:19:56.944625 edc-phq9-0.1.7/edc_phq9.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1617 2022-08-26 02:19:56.000000 edc-phq9-0.1.7/edc_phq9.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1155 2022-08-26 02:19:56.000000 edc-phq9-0.1.7/edc_phq9.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-26 02:19:56.000000 edc-phq9-0.1.7/edc_phq9.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-01-05 15:20:02.000000 edc-phq9-0.1.7/edc_phq9.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        9 2022-08-26 02:19:56.000000 edc-phq9-0.1.7/edc_phq9.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1718 2022-08-23 02:17:52.000000 edc-phq9-0.1.7/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2085 2022-08-26 02:19:49.000000 edc-phq9-0.1.7/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1228 2022-08-26 02:19:56.946495 edc-phq9-0.1.7/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.312485 edc-phq9-0.1.8/
+-rw-r--r--   0 erikvw     (501) staff       (20)       84 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/.coveragrc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.303979 edc-phq9-0.1.8/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.307394 edc-phq9-0.1.8/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-23 02:17:52.000000 edc-phq9-0.1.8/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-25 22:11:15.000000 edc-phq9-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-23 02:17:52.000000 edc-phq9-0.1.8/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-01-05 14:54:30.000000 edc-phq9-0.1.8/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1617 2022-09-25 22:11:23.312598 edc-phq9-0.1.8/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      650 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 22:11:15.000000 edc-phq9-0.1.8/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-23 02:17:52.000000 edc-phq9-0.1.8/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.309925 edc-phq9-0.1.8/edc_phq9/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      891 2022-08-23 02:17:52.000000 edc-phq9-0.1.8/edc_phq9/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      396 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      383 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      305 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      351 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      126 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      622 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1156 2022-09-25 22:11:15.000000 edc-phq9-0.1.8/edc_phq9/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      885 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/model_admin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3236 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      655 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/edc_phq9/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.310700 edc-phq9-0.1.8/edc_phq9/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.311805 edc-phq9-0.1.8/edc_phq9/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.312320 edc-phq9-0.1.8/edc_phq9/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      449 2022-08-26 02:19:49.000000 edc-phq9-0.1.8/edc_phq9/tests/tests/test_auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1329 2022-06-01 22:19:44.000000 edc-phq9-0.1.8/edc_phq9/tests/tests/tests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      283 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      379 2022-01-06 03:46:37.000000 edc-phq9-0.1.8/edc_phq9/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:11:23.310606 edc-phq9-0.1.8/edc_phq9.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1617 2022-09-25 22:11:23.000000 edc-phq9-0.1.8/edc_phq9.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1155 2022-09-25 22:11:23.000000 edc-phq9-0.1.8/edc_phq9.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-25 22:11:23.000000 edc-phq9-0.1.8/edc_phq9.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-01-05 15:20:02.000000 edc-phq9-0.1.8/edc_phq9.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        9 2022-09-25 22:11:23.000000 edc-phq9-0.1.8/edc_phq9.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1718 2022-08-23 02:17:52.000000 edc-phq9-0.1.8/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2085 2022-08-26 02:19:49.000000 edc-phq9-0.1.8/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1228 2022-09-25 22:11:23.312945 edc-phq9-0.1.8/setup.cfg
```

### Comparing `edc-phq9-0.1.7/.github/workflows/build.yml` & `edc-phq9-0.1.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/.gitignore` & `edc-phq9-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/.pre-commit-config.yaml` & `edc-phq9-0.1.8/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black
-        language_version: python3.8
+        language_version: python3.9
 
   - repo: https://github.com/pycqa/flake8
     rev: 5.0.4
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
```

### Comparing `edc-phq9-0.1.7/LICENSE` & `edc-phq9-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/PKG-INFO` & `edc-phq9-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-phq9
-Version: 0.1.7
+Version: 0.1.8
 Summary: Classes for PHQ9 in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-phq9
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc phq9,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-phq9-0.1.7/README.rst` & `edc-phq9-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/edc_phq9/admin.py` & `edc-phq9-0.1.8/edc_phq9/admin.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/edc_phq9/fieldsets.py` & `edc-phq9-0.1.8/edc_phq9/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/edc_phq9/forms.py` & `edc-phq9-0.1.8/edc_phq9/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django import forms
 from django.conf import settings
 from edc_constants.constants import NO, YES
-from edc_crf.forms import CrfFormValidatorMixin
+from edc_crf.form_validator_mixins import CrfFormValidatorMixin
 from edc_form_validators import FormValidatorMixin
 from edc_form_validators.form_validator import FormValidator
 from edc_visit_schedule.utils import raise_if_not_baseline
 
 from edc_phq9.fieldsets import get_phq9_fields
 
 from .utils import get_phq9_model_cls
```

### Comparing `edc-phq9-0.1.7/edc_phq9/model_admin_mixins.py` & `edc-phq9-0.1.8/edc_phq9/model_admin_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/edc_phq9/model_mixins.py` & `edc-phq9-0.1.8/edc_phq9/model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/edc_phq9/models.py` & `edc-phq9-0.1.8/edc_phq9/models.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/edc_phq9/tests/etc/user-rsa-local-private.pem` & `edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/edc_phq9/tests/etc/user-rsa-restricted-private.pem` & `edc-phq9-0.1.8/edc_phq9/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/edc_phq9/tests/tests/tests.py` & `edc-phq9-0.1.8/edc_phq9/tests/tests/tests.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/edc_phq9.egg-info/PKG-INFO` & `edc-phq9-0.1.8/edc_phq9.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-phq9
-Version: 0.1.7
+Version: 0.1.8
 Summary: Classes for PHQ9 in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-phq9
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc phq9,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-phq9-0.1.7/edc_phq9.egg-info/SOURCES.txt` & `edc-phq9-0.1.8/edc_phq9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/pyproject.toml` & `edc-phq9-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/runtests.py` & `edc-phq9-0.1.8/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-phq9-0.1.7/setup.cfg` & `edc-phq9-0.1.8/setup.cfg`

 * *Files identical despite different names*

