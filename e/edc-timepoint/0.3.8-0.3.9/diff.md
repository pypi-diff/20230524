# Comparing `tmp/edc-timepoint-0.3.8.tar.gz` & `tmp/edc-timepoint-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-timepoint-0.3.8.tar", last modified: Sun Sep 25 22:25:35 2022, max compression
+gzip compressed data, was "edc-timepoint-0.3.9.tar", last modified: Tue Oct  4 02:59:17 2022, max compression
```

## Comparing `edc-timepoint-0.3.8.tar` & `edc-timepoint-0.3.9.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:25:35.942753 edc-timepoint-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       98 2020-03-04 22:51:04.000000 edc-timepoint-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 13:57:22.000000 edc-timepoint-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:25:35.934661 edc-timepoint-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:25:35.937797 edc-timepoint-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-12 00:24:13.000000 edc-timepoint-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)      954 2022-06-23 19:55:19.000000 edc-timepoint-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-25 22:25:28.000000 edc-timepoint-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-12 00:24:13.000000 edc-timepoint-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 19:55:19.000000 edc-timepoint-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 19:55:19.000000 edc-timepoint-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      159 2022-06-23 19:55:19.000000 edc-timepoint-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     5737 2022-09-25 22:25:35.942847 edc-timepoint-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     4704 2022-08-12 00:24:13.000000 edc-timepoint-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 22:25:28.000000 edc-timepoint-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-12 00:24:13.000000 edc-timepoint-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:25:35.939486 edc-timepoint-0.3.8/edc_timepoint/
--rw-r--r--   0 erikvw     (501) staff       (20)       87 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1831 2022-08-12 00:24:13.000000 edc-timepoint-0.3.8/edc_timepoint/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      182 2021-02-04 13:57:22.000000 edc-timepoint-0.3.8/edc_timepoint/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      947 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/form_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4906 2022-09-25 22:25:28.000000 edc-timepoint-0.3.8/edc_timepoint/model_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:25:35.940400 edc-timepoint-0.3.8/edc_timepoint/models/
--rw-r--r--   0 erikvw     (501) staff       (20)       51 2022-08-12 00:24:13.000000 edc-timepoint-0.3.8/edc_timepoint/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1505 2022-08-12 00:24:13.000000 edc-timepoint-0.3.8/edc_timepoint/models/signals.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:25:35.941359 edc-timepoint-0.3.8/edc_timepoint/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      357 2021-02-04 13:57:22.000000 edc-timepoint-0.3.8/edc_timepoint/tests/consents.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:25:35.942449 edc-timepoint-0.3.8/edc_timepoint/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      522 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     2277 2021-02-04 13:57:22.000000 edc-timepoint-0.3.8/edc_timepoint/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:25:35.942655 edc-timepoint-0.3.8/edc_timepoint/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7046 2022-09-25 22:25:28.000000 edc-timepoint-0.3.8/edc_timepoint/tests/tests/test_timepoints.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-02-04 13:57:22.000000 edc-timepoint-0.3.8/edc_timepoint/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1277 2021-02-04 13:57:22.000000 edc-timepoint-0.3.8/edc_timepoint/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      678 2021-02-04 13:57:22.000000 edc-timepoint-0.3.8/edc_timepoint/timepoint.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1068 2021-02-04 13:57:22.000000 edc-timepoint-0.3.8/edc_timepoint/timepoint_collection.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1727 2021-02-04 13:57:22.000000 edc-timepoint-0.3.8/edc_timepoint/timepoint_lookup.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:25:35.940172 edc-timepoint-0.3.8/edc_timepoint.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     5737 2022-09-25 22:25:35.000000 edc-timepoint-0.3.8/edc_timepoint.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1380 2022-09-25 22:25:35.000000 edc-timepoint-0.3.8/edc_timepoint.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-25 22:25:35.000000 edc-timepoint-0.3.8/edc_timepoint.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 22:50:09.000000 edc-timepoint-0.3.8/edc_timepoint.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-09-25 22:25:35.000000 edc-timepoint-0.3.8/edc_timepoint.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1728 2022-08-12 00:24:13.000000 edc-timepoint-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1966 2022-09-25 22:25:28.000000 edc-timepoint-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1298 2022-09-25 22:25:35.943146 edc-timepoint-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-04 02:59:17.007310 edc-timepoint-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       98 2020-03-04 22:51:04.000000 edc-timepoint-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 13:57:22.000000 edc-timepoint-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-04 02:59:16.999029 edc-timepoint-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-04 02:59:17.002020 edc-timepoint-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-12 00:24:13.000000 edc-timepoint-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)      954 2022-06-23 19:55:19.000000 edc-timepoint-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-25 22:25:28.000000 edc-timepoint-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-12 00:24:13.000000 edc-timepoint-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 19:55:19.000000 edc-timepoint-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 19:55:19.000000 edc-timepoint-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      159 2022-06-23 19:55:19.000000 edc-timepoint-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     5737 2022-10-04 02:59:17.007407 edc-timepoint-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     4704 2022-08-12 00:24:13.000000 edc-timepoint-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-10-04 02:59:09.000000 edc-timepoint-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-12 00:24:13.000000 edc-timepoint-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-04 02:59:17.003707 edc-timepoint-0.3.9/edc_timepoint/
+-rw-r--r--   0 erikvw     (501) staff       (20)       87 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1831 2022-08-12 00:24:13.000000 edc-timepoint-0.3.9/edc_timepoint/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      182 2021-02-04 13:57:22.000000 edc-timepoint-0.3.9/edc_timepoint/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      947 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/form_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4906 2022-09-25 22:25:28.000000 edc-timepoint-0.3.9/edc_timepoint/model_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-04 02:59:17.004666 edc-timepoint-0.3.9/edc_timepoint/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)       51 2022-08-12 00:24:13.000000 edc-timepoint-0.3.9/edc_timepoint/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1505 2022-08-12 00:24:13.000000 edc-timepoint-0.3.9/edc_timepoint/models/signals.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-04 02:59:17.005942 edc-timepoint-0.3.9/edc_timepoint/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      357 2021-02-04 13:57:22.000000 edc-timepoint-0.3.9/edc_timepoint/tests/consents.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-04 02:59:17.007008 edc-timepoint-0.3.9/edc_timepoint/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      522 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     2355 2022-10-04 02:59:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      424 2022-10-04 02:59:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/reference_configs.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-04 02:59:17.007217 edc-timepoint-0.3.9/edc_timepoint/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7863 2022-10-04 02:59:09.000000 edc-timepoint-0.3.9/edc_timepoint/tests/tests/test_timepoints.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-02-04 13:57:22.000000 edc-timepoint-0.3.9/edc_timepoint/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1277 2021-02-04 13:57:22.000000 edc-timepoint-0.3.9/edc_timepoint/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      678 2021-02-04 13:57:22.000000 edc-timepoint-0.3.9/edc_timepoint/timepoint.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1068 2021-02-04 13:57:22.000000 edc-timepoint-0.3.9/edc_timepoint/timepoint_collection.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1727 2021-02-04 13:57:22.000000 edc-timepoint-0.3.9/edc_timepoint/timepoint_lookup.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-04 02:59:17.004433 edc-timepoint-0.3.9/edc_timepoint.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5737 2022-10-04 02:59:16.000000 edc-timepoint-0.3.9/edc_timepoint.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1421 2022-10-04 02:59:16.000000 edc-timepoint-0.3.9/edc_timepoint.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-10-04 02:59:16.000000 edc-timepoint-0.3.9/edc_timepoint.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 22:50:09.000000 edc-timepoint-0.3.9/edc_timepoint.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-10-04 02:59:16.000000 edc-timepoint-0.3.9/edc_timepoint.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1728 2022-08-12 00:24:13.000000 edc-timepoint-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2006 2022-10-04 02:59:09.000000 edc-timepoint-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1298 2022-10-04 02:59:17.007698 edc-timepoint-0.3.9/setup.cfg
```

### Comparing `edc-timepoint-0.3.8/.github/workflows/build.yml` & `edc-timepoint-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/.gitignore` & `edc-timepoint-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/.pre-commit-config.yaml` & `edc-timepoint-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/LICENSE` & `edc-timepoint-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/PKG-INFO` & `edc-timepoint-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-timepoint
-Version: 0.3.8
+Version: 0.3.9
 Summary: Lock a timepoint from further editing once data is cleaned and reviewed in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-timepoint
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc timepoint,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-timepoint-0.3.8/README.rst` & `edc-timepoint-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint/apps.py` & `edc-timepoint-0.3.9/edc_timepoint/apps.py`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint/form_mixin.py` & `edc-timepoint-0.3.9/edc_timepoint/form_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint/model_mixins.py` & `edc-timepoint-0.3.9/edc_timepoint/model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint/models/signals.py` & `edc-timepoint-0.3.9/edc_timepoint/models/signals.py`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint/tests/etc/user-rsa-local-private.pem` & `edc-timepoint-0.3.9/edc_timepoint/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint/tests/etc/user-rsa-restricted-private.pem` & `edc-timepoint-0.3.9/edc_timepoint/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint/tests/holidays.csv` & `edc-timepoint-0.3.9/edc_timepoint/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint/tests/models.py` & `edc-timepoint-0.3.9/edc_timepoint/tests/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from edc_consent.field_mixins import IdentityFieldsMixin, PersonalFieldsMixin
 from edc_consent.model_mixins import ConsentModelMixin
+from edc_crf.model_mixins import CrfModelMixin
 from edc_identifier.managers import SubjectIdentifierManager
 from edc_identifier.model_mixins import UniqueSubjectIdentifierFieldMixin
+from edc_metadata.model_mixins.creates import CreatesMetadataModelMixin
 from edc_model.models import BaseUuidModel
+from edc_reference.model_mixins import ReferenceModelMixin
 from edc_registration.model_mixins import UpdatesOrCreatesRegistrationModelMixin
 from edc_sites.models import SiteModelMixin
 from edc_visit_schedule.model_mixins import OffScheduleModelMixin, OnScheduleModelMixin
-from edc_visit_tracking.model_mixins import VisitModelMixin, VisitTrackingCrfModelMixin
+from edc_visit_tracking.model_mixins import VisitModelMixin
 
 from ..model_mixins import TimepointLookupModelMixin
 from ..timepoint_lookup import TimepointLookup
 
 
 class VisitTimepointLookup(TimepointLookup):
     timepoint_model = "edc_appointment.appointment"
@@ -18,67 +21,63 @@
 
 
 class CrfTimepointLookup(TimepointLookup):
     timepoint_model = "edc_appointment.appointment"
 
 
 class SubjectConsent(
+    SiteModelMixin,
     ConsentModelMixin,
     PersonalFieldsMixin,
     IdentityFieldsMixin,
     UniqueSubjectIdentifierFieldMixin,
     UpdatesOrCreatesRegistrationModelMixin,
-    SiteModelMixin,
     BaseUuidModel,
 ):
-
-    objects = SubjectIdentifierManager()
-
     def natural_key(self):
         return (self.subject_identifier,)
 
-
-# class SubjectVisit(
-#     VisitModelMixin,
-#     ReferenceModelMixin,
-#     CreatesMetadataModelMixin,
-#     SiteModelMixin,
-#     BaseUuidModel,
-# ):
-#
-#     subject_identifier = models.CharField(max_length=50)
+    class Meta(ConsentModelMixin.Meta, BaseUuidModel.Meta):
+        pass
 
 
-class SubjectVisit(VisitModelMixin, TimepointLookupModelMixin, BaseUuidModel):
+class SubjectVisit(
+    SiteModelMixin,
+    VisitModelMixin,
+    ReferenceModelMixin,
+    CreatesMetadataModelMixin,
+    TimepointLookupModelMixin,
+    BaseUuidModel,
+):
 
     timepoint_lookup_cls = VisitTimepointLookup
 
     class Meta(VisitModelMixin.Meta):
         pass
 
 
-class CrfOne(VisitTrackingCrfModelMixin, TimepointLookupModelMixin, BaseUuidModel):
+class CrfOne(CrfModelMixin, TimepointLookupModelMixin, BaseUuidModel):
 
     timepoint_lookup_cls = CrfTimepointLookup
 
 
-class CrfTwo(VisitTrackingCrfModelMixin, TimepointLookupModelMixin, BaseUuidModel):
+class CrfTwo(CrfModelMixin, TimepointLookupModelMixin, BaseUuidModel):
 
     timepoint_lookup_cls = CrfTimepointLookup
 
 
-class OnSchedule(OnScheduleModelMixin, BaseUuidModel):
+class OnSchedule(SiteModelMixin, OnScheduleModelMixin, BaseUuidModel):
 
     pass
 
 
-class OffSchedule(OffScheduleModelMixin, BaseUuidModel):
+class OffSchedule(SiteModelMixin, OffScheduleModelMixin, BaseUuidModel):
 
     pass
 
 
-class DeathReport(UniqueSubjectIdentifierFieldMixin, BaseUuidModel):
+class DeathReport(SiteModelMixin, UniqueSubjectIdentifierFieldMixin, BaseUuidModel):
 
     objects = SubjectIdentifierManager()
 
     def natural_key(self):
         return (self.subject_identifier,)
```

### Comparing `edc-timepoint-0.3.8/edc_timepoint/tests/tests/test_timepoints.py` & `edc-timepoint-0.3.9/edc_timepoint/tests/tests/test_timepoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 from django.apps import apps as django_apps
 from django.test import TestCase
 from edc_appointment.constants import COMPLETE_APPT
 from edc_appointment.creators import UnscheduledAppointmentCreator
 from edc_appointment.models import Appointment
 from edc_consent.site_consents import site_consents
 from edc_facility.import_holidays import import_holidays
+from edc_reference import site_reference_configs
 from edc_utils import get_utcnow
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
+from edc_visit_tracking.constants import SCHEDULED
 
 from ...constants import CLOSED_TIMEPOINT, OPEN_TIMEPOINT
 from ...model_mixins import UnableToCloseTimepoint
 from ...timepoint import TimepointClosed
 from ..consents import v1
 from ..models import CrfOne, CrfTwo, SubjectConsent, SubjectVisit
+from ..reference_configs import register_to_site_reference_configs
 from ..visit_schedule import visit_schedule1
 
 
 class Helper:
     def __init__(self, subject_identifier=None, now=None):
         self.subject_identifier = subject_identifier
         self.now = now or get_utcnow()
@@ -63,14 +66,18 @@
 
         return super().setUpClass()
 
     def setUp(self):
         self.subject_identifier = "12345"
         site_visit_schedules._registry = {}
         site_visit_schedules.register(visit_schedule=visit_schedule1)
+        register_to_site_reference_configs()
+        site_reference_configs.register_from_visit_schedule(
+            visit_models={"edc_appointment.appointment": "edc_timepoint.subjectvisit"}
+        )
         self.helper = self.helper_cls(
             subject_identifier=self.subject_identifier,
             now=get_utcnow() - relativedelta(years=1),
         )
         self.helper.consent_and_put_on_schedule()
         appointments = Appointment.objects.filter(
             subject_identifier=self.subject_identifier
@@ -94,41 +101,49 @@
         self.assertEqual(self.appointment.timepoint_status, OPEN_TIMEPOINT)
         self.assertRaises(UnableToCloseTimepoint, self.appointment.timepoint_close_timepoint)
 
     def test_timepoint_status_closed_blocks_everything(self):
         """Assert timepoint closes because appointment status
         is "closed" and blocks further changes.
         """
-        subject_visit = SubjectVisit.objects.create(appointment=self.appointment)
+        subject_visit = SubjectVisit.objects.create(
+            appointment=self.appointment, reason=SCHEDULED
+        )
         CrfOne.objects.create(subject_visit=subject_visit)
         CrfTwo.objects.create(subject_visit=subject_visit)
         self.appointment.appt_status = COMPLETE_APPT
         self.appointment.save()
         self.appointment.timepoint_close_timepoint()
         self.assertRaises(TimepointClosed, self.appointment.save)
 
     def test_timepoint_status_close_attempt_ok(self):
         """Assert timepoint closes because appointment status
         is "closed".
         """
-        subject_visit = SubjectVisit.objects.create(appointment=self.appointment)
+        subject_visit = SubjectVisit.objects.create(
+            appointment=self.appointment, reason=SCHEDULED
+        )
         crf_obj = CrfOne.objects.create(subject_visit=subject_visit)
+        CrfTwo.objects.create(subject_visit=subject_visit)
         self.appointment.appt_status = COMPLETE_APPT
         self.appointment.save()
         self.appointment.refresh_from_db()
+        self.assertEqual(self.appointment.appt_status, COMPLETE_APPT)
         self.appointment.timepoint_close_timepoint()
         self.assertRaises(TimepointClosed, self.appointment.save)
         self.assertRaises(TimepointClosed, subject_visit.save)
         self.assertRaises(TimepointClosed, crf_obj.save)
 
     def test_timepoint_status_attrs(self):
         """Assert timepoint closes because appointment status
         is COMPLETE_APPT and blocks further changes.
         """
-        subject_visit = SubjectVisit.objects.create(appointment=self.appointment)
+        subject_visit = SubjectVisit.objects.create(
+            appointment=self.appointment, reason=SCHEDULED
+        )
         CrfOne.objects.create(subject_visit=subject_visit)
         CrfTwo.objects.create(subject_visit=subject_visit)
         self.appointment.appt_status = COMPLETE_APPT
         self.appointment.save()
         self.appointment.timepoint_close_timepoint()
         self.assertEqual(self.appointment.appt_status, COMPLETE_APPT)
         self.assertEqual(
@@ -137,27 +152,33 @@
         self.assertGreater(
             self.appointment.timepoint_closed_datetime,
             self.appointment.timepoint_opened_datetime,
         )
         self.assertEqual(self.appointment.timepoint_status, CLOSED_TIMEPOINT)
 
     def test_timepoint_lookup_blocks_crf_create(self):
-        subject_visit = SubjectVisit.objects.create(appointment=self.appointment)
-        self.appointment.appt_status = COMPLETE_APPT
-        self.appointment.save()
+        subject_visit = SubjectVisit.objects.create(
+            appointment=self.appointment, reason=SCHEDULED
+        )
         subject_visit = SubjectVisit.objects.get(pk=subject_visit.pk)
+        CrfTwo.objects.create(subject_visit=subject_visit)
         try:
             crf_obj = CrfOne.objects.create(subject_visit=subject_visit)
         except TimepointClosed:
             self.fail("TimepointError unexpectedly raised.")
+        self.appointment.appt_status = COMPLETE_APPT
+        self.appointment.save()
         self.appointment.timepoint_close_timepoint()
         self.assertRaises(TimepointClosed, crf_obj.save)
 
     def test_timepoint_lookup_blocks_update(self):
-        subject_visit = SubjectVisit.objects.create(appointment=self.appointment)
+        subject_visit = SubjectVisit.objects.create(
+            appointment=self.appointment, reason=SCHEDULED
+        )
         crf_obj = CrfOne.objects.create(subject_visit=subject_visit)
+        CrfTwo.objects.create(subject_visit=subject_visit)
         self.appointment.appt_status = COMPLETE_APPT
         self.appointment.save()
         self.appointment.timepoint_close_timepoint()
 
         self.assertRaises(TimepointClosed, crf_obj.save)
         self.assertRaises(TimepointClosed, subject_visit.save)
```

### Comparing `edc-timepoint-0.3.8/edc_timepoint/tests/visit_schedule.py` & `edc-timepoint-0.3.9/edc_timepoint/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint/timepoint.py` & `edc-timepoint-0.3.9/edc_timepoint/timepoint.py`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint/timepoint_collection.py` & `edc-timepoint-0.3.9/edc_timepoint/timepoint_collection.py`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint/timepoint_lookup.py` & `edc-timepoint-0.3.9/edc_timepoint/timepoint_lookup.py`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/edc_timepoint.egg-info/PKG-INFO` & `edc-timepoint-0.3.9/edc_timepoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-timepoint
-Version: 0.3.8
+Version: 0.3.9
 Summary: Lock a timepoint from further editing once data is cleaned and reviewed in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-timepoint
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc timepoint,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-timepoint-0.3.8/edc_timepoint.egg-info/SOURCES.txt` & `edc-timepoint-0.3.9/edc_timepoint.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 edc_timepoint.egg-info/top_level.txt
 edc_timepoint/models/__init__.py
 edc_timepoint/models/signals.py
 edc_timepoint/tests/__init__.py
 edc_timepoint/tests/consents.py
 edc_timepoint/tests/holidays.csv
 edc_timepoint/tests/models.py
+edc_timepoint/tests/reference_configs.py
 edc_timepoint/tests/urls.py
 edc_timepoint/tests/visit_schedule.py
 edc_timepoint/tests/etc/user-aes-local.key
 edc_timepoint/tests/etc/user-aes-restricted.key
 edc_timepoint/tests/etc/user-rsa-local-private.pem
 edc_timepoint/tests/etc/user-rsa-local-public.pem
 edc_timepoint/tests/etc/user-rsa-restricted-private.pem
```

### Comparing `edc-timepoint-0.3.8/pyproject.toml` & `edc-timepoint-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-timepoint-0.3.8/runtests.py` & `edc-timepoint-0.3.9/runtests.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         "edc_appointment.apps.AppConfig",
         "edc_notification.apps.AppConfig",
         "edc_offstudy.apps.AppConfig",
         "edc_visit_schedule.apps.AppConfig",
         "edc_protocol.apps.AppConfig",
         "edc_consent.apps.AppConfig",
         "edc_metadata.apps.AppConfig",
+        "edc_reference.apps.AppConfig",
         "edc_registration.apps.AppConfig",
         "edc_identifier.apps.AppConfig",
         "edc_facility.apps.AppConfig",
         "edc_visit_tracking.apps.AppConfig",
         "edc_timepoint.apps.AppConfig",
     ],
     add_dashboard_middleware=True,
```

### Comparing `edc-timepoint-0.3.8/setup.cfg` & `edc-timepoint-0.3.9/setup.cfg`

 * *Files identical despite different names*

