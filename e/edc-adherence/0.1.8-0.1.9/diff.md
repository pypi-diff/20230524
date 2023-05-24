# Comparing `tmp/edc-adherence-0.1.8.tar.gz` & `tmp/edc-adherence-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-adherence-0.1.8.tar", last modified: Sun Jul  3 20:24:32 2022, max compression
+gzip compressed data, was "edc-adherence-0.1.9.tar", last modified: Fri Jul  8 18:24:01 2022, max compression
```

## Comparing `edc-adherence-0.1.8.tar` & `edc-adherence-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-03 20:24:32.176847 edc-adherence-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-03 20:24:32.169163 edc-adherence-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-03 20:24:32.172158 edc-adherence-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-19 02:12:43.000000 edc-adherence-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1836 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-15 05:10:58.000000 edc-adherence-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1549 2022-07-03 20:24:32.176946 edc-adherence-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      688 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-07-03 20:24:15.000000 edc-adherence-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-03 20:24:32.173773 edc-adherence-0.1.8/edc_adherence/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      228 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      348 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1435 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      635 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-03 20:24:32.174612 edc-adherence-0.1.8/edc_adherence/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     1690 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2216 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/model_form_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1830 2022-07-03 20:24:15.000000 edc-adherence-0.1.8/edc_adherence/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      237 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-03 20:24:32.175457 edc-adherence-0.1.8/edc_adherence/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      697 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-03 20:24:32.176528 edc-adherence-0.1.8/edc_adherence/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      640 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     2293 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-03 20:24:32.176729 edc-adherence-0.1.8/edc_adherence/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5087 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/tests/test_adherence.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1073 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/edc_adherence/tests/visit_schedules.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-03 20:24:32.174363 edc-adherence-0.1.8/edc_adherence.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1549 2022-07-03 20:24:31.000000 edc-adherence-0.1.8/edc_adherence.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1388 2022-07-03 20:24:32.000000 edc-adherence-0.1.8/edc_adherence.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-07-03 20:24:31.000000 edc-adherence-0.1.8/edc_adherence.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-15 05:31:20.000000 edc-adherence-0.1.8/edc_adherence.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-07-03 20:24:32.000000 edc-adherence-0.1.8/edc_adherence.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1587 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2483 2022-05-07 01:23:14.000000 edc-adherence-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1157 2022-07-03 20:24:32.177239 edc-adherence-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-08 18:24:01.364862 edc-adherence-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/.coveragrc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-08 18:24:01.357317 edc-adherence-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-08 18:24:01.360022 edc-adherence-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1759 2022-07-08 18:23:43.000000 edc-adherence-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1836 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-15 05:10:58.000000 edc-adherence-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1549 2022-07-08 18:24:01.364951 edc-adherence-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      688 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-07-08 18:23:44.000000 edc-adherence-0.1.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-08 18:24:01.361773 edc-adherence-0.1.9/edc_adherence/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      228 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      348 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1435 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      635 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-08 18:24:01.362659 edc-adherence-0.1.9/edc_adherence/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1690 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2216 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/model_form_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1840 2022-07-08 18:23:43.000000 edc-adherence-0.1.9/edc_adherence/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      237 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-08 18:24:01.363520 edc-adherence-0.1.9/edc_adherence/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      697 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-08 18:24:01.364541 edc-adherence-0.1.9/edc_adherence/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      640 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     2293 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-08 18:24:01.364744 edc-adherence-0.1.9/edc_adherence/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5087 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/tests/test_adherence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1073 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/edc_adherence/tests/visit_schedules.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-08 18:24:01.362411 edc-adherence-0.1.9/edc_adherence.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1549 2022-07-08 18:24:01.000000 edc-adherence-0.1.9/edc_adherence.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1388 2022-07-08 18:24:01.000000 edc-adherence-0.1.9/edc_adherence.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-07-08 18:24:01.000000 edc-adherence-0.1.9/edc_adherence.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-15 05:31:20.000000 edc-adherence-0.1.9/edc_adherence.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-07-08 18:24:01.000000 edc-adherence-0.1.9/edc_adherence.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1647 2022-07-08 18:23:43.000000 edc-adherence-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2483 2022-05-07 01:23:14.000000 edc-adherence-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1157 2022-07-08 18:24:01.365246 edc-adherence-0.1.9/setup.cfg
```

### Comparing `edc-adherence-0.1.8/.github/workflows/build.yml` & `edc-adherence-0.1.9/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.9']
-        django-version: ['3.2']
+        django-version: ['3.2', '4.0', 'dev']
 
     services:
 
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
```

### Comparing `edc-adherence-0.1.8/.gitignore` & `edc-adherence-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/LICENSE` & `edc-adherence-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/PKG-INFO` & `edc-adherence-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-adherence
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes to manage adherence in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-adherence
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc adherendce,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-adherence-0.1.8/README.rst` & `edc-adherence-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence/form_validator_mixin.py` & `edc-adherence-0.1.9/edc_adherence/form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence/list_data.py` & `edc-adherence-0.1.9/edc_adherence/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence/migrations/0001_initial.py` & `edc-adherence-0.1.9/edc_adherence/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence/model_admin_mixin.py` & `edc-adherence-0.1.9/edc_adherence/model_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence/model_mixins.py` & `edc-adherence-0.1.9/edc_adherence/model_mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     )
 
     pill_count_performed = models.CharField(
         verbose_name="Was a pill count performed", max_length=5, choices=YES_NO, default=YES
     )
 
     pill_count_not_performed_reason = models.TextField(
-        verbose_name="Was a pill count performed",
+        verbose_name="If not performed, please explain ...",
         null=True,
         blank=True,
     )
 
     pill_count = models.IntegerField(
         verbose_name="Number of pills left in the bottle", null=True, blank=True
     )
```

### Comparing `edc-adherence-0.1.8/edc_adherence/tests/admin.py` & `edc-adherence-0.1.9/edc_adherence/tests/admin.py`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence/tests/etc/user-rsa-local-private.pem` & `edc-adherence-0.1.9/edc_adherence/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence/tests/etc/user-rsa-restricted-private.pem` & `edc-adherence-0.1.9/edc_adherence/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence/tests/forms.py` & `edc-adherence-0.1.9/edc_adherence/tests/forms.py`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence/tests/models.py` & `edc-adherence-0.1.9/edc_adherence/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence/tests/tests/test_adherence.py` & `edc-adherence-0.1.9/edc_adherence/tests/tests/test_adherence.py`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence/tests/visit_schedules.py` & `edc-adherence-0.1.9/edc_adherence/tests/visit_schedules.py`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/edc_adherence.egg-info/PKG-INFO` & `edc-adherence-0.1.9/edc_adherence.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-adherence
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes to manage adherence in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-adherence
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc adherendce,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-adherence-0.1.8/edc_adherence.egg-info/SOURCES.txt` & `edc-adherence-0.1.9/edc_adherence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/pyproject.toml` & `edc-adherence-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 [tool.isort]
 profile = "black"
 py_version = "39"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
-parallel = true
+parallel = false
 branch = true
 source = ["edc_adherence"]
 
 [tool.coverage.paths]
 source = ["edc_adherence"]
 
 [tool.coverage.report]
@@ -28,39 +28,42 @@
 skip_covered = true
 omit = ["requirements.txt"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{39}-dj{32,dev},
+    py{39}-dj{32,40,dev},
     lint
 isolated_build = true
 
 [gh-actions]
 python =
     3.9: py39, lint
 
 [gh-actions:env]
 DJANGO =
     3.2: dj32, lint
+    4.0: dj40
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
     dj32: Django>=3.2,<3.3
+    dj40: Django>=4.0,<4.1
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

### Comparing `edc-adherence-0.1.8/runtests.py` & `edc-adherence-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-adherence-0.1.8/setup.cfg` & `edc-adherence-0.1.9/setup.cfg`

 * *Files identical despite different names*

