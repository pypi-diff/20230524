# Comparing `tmp/edc-transfer-0.3.8.tar.gz` & `tmp/edc-transfer-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-transfer-0.3.8.tar", last modified: Thu Aug 11 00:02:07 2022, max compression
+gzip compressed data, was "edc-transfer-0.3.9.tar", last modified: Thu Aug 11 19:16:40 2022, max compression
```

## Comparing `edc-transfer-0.3.8.tar` & `edc-transfer-0.3.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 00:02:07.769099 edc-transfer-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       95 2021-01-23 15:27:13.000000 edc-transfer-0.3.8/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 20:33:23.000000 edc-transfer-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 00:02:07.760873 edc-transfer-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 00:02:07.764090 edc-transfer-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 12:23:10.000000 edc-transfer-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1844 2022-06-01 23:48:52.000000 edc-transfer-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-10 12:23:10.000000 edc-transfer-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 12:23:10.000000 edc-transfer-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)       37 2022-06-01 23:48:52.000000 edc-transfer-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:48:52.000000 edc-transfer-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-01-21 23:37:43.000000 edc-transfer-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:48:52.000000 edc-transfer-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1692 2022-08-11 00:02:07.769228 edc-transfer-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      687 2021-02-04 20:33:23.000000 edc-transfer-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-11 00:01:58.000000 edc-transfer-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 12:23:10.000000 edc-transfer-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 00:02:07.765907 edc-transfer-0.3.8/edc_transfer/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-01-21 23:38:05.000000 edc-transfer-0.3.8/edc_transfer/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      770 2021-02-04 20:33:23.000000 edc-transfer-0.3.8/edc_transfer/action_items.py
--rw-r--r--   0 erikvw     (501) staff       (20)      149 2021-01-21 23:44:04.000000 edc-transfer-0.3.8/edc_transfer/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      181 2021-01-23 15:27:13.000000 edc-transfer-0.3.8/edc_transfer/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       87 2021-01-23 15:27:13.000000 edc-transfer-0.3.8/edc_transfer/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3420 2021-08-26 01:01:17.000000 edc-transfer-0.3.8/edc_transfer/form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2135 2022-07-03 20:28:49.000000 edc-transfer-0.3.8/edc_transfer/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1976 2022-08-11 00:01:58.000000 edc-transfer-0.3.8/edc_transfer/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      629 2021-04-23 01:08:26.000000 edc-transfer-0.3.8/edc_transfer/modelform_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-01-23 15:27:13.000000 edc-transfer-0.3.8/edc_transfer/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 00:02:07.767387 edc-transfer-0.3.8/edc_transfer/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-01-21 23:56:42.000000 edc-transfer-0.3.8/edc_transfer/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2021-04-23 01:08:26.000000 edc-transfer-0.3.8/edc_transfer/tests/admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 00:02:07.768651 edc-transfer-0.3.8/edc_transfer/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-01-21 23:56:54.000000 edc-transfer-0.3.8/edc_transfer/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-01-21 23:56:54.000000 edc-transfer-0.3.8/edc_transfer/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-01-21 23:56:54.000000 edc-transfer-0.3.8/edc_transfer/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-01-21 23:56:54.000000 edc-transfer-0.3.8/edc_transfer/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-01-21 23:56:53.000000 edc-transfer-0.3.8/edc_transfer/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-01-21 23:56:53.000000 edc-transfer-0.3.8/edc_transfer/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-01-21 23:56:54.000000 edc-transfer-0.3.8/edc_transfer/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-01-21 23:56:54.000000 edc-transfer-0.3.8/edc_transfer/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      636 2021-04-23 01:08:26.000000 edc-transfer-0.3.8/edc_transfer/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      508 2021-04-23 01:08:26.000000 edc-transfer-0.3.8/edc_transfer/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      597 2021-04-23 01:08:26.000000 edc-transfer-0.3.8/edc_transfer/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 00:02:07.768875 edc-transfer-0.3.8/edc_transfer/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-01-21 23:58:11.000000 edc-transfer-0.3.8/edc_transfer/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1178 2022-06-01 23:48:52.000000 edc-transfer-0.3.8/edc_transfer/tests/tests/tests.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-02-04 20:33:23.000000 edc-transfer-0.3.8/edc_transfer/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 00:02:07.766502 edc-transfer-0.3.8/edc_transfer.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1692 2022-08-11 00:02:07.000000 edc-transfer-0.3.8/edc_transfer.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1290 2022-08-11 00:02:07.000000 edc-transfer-0.3.8/edc_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-11 00:02:07.000000 edc-transfer-0.3.8/edc_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-01-22 01:48:58.000000 edc-transfer-0.3.8/edc_transfer.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       13 2022-08-11 00:02:07.000000 edc-transfer-0.3.8/edc_transfer.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1726 2022-08-10 12:23:10.000000 edc-transfer-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2442 2022-06-01 23:48:52.000000 edc-transfer-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1269 2022-08-11 00:02:07.769631 edc-transfer-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 19:16:40.619127 edc-transfer-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       95 2021-01-23 15:27:13.000000 edc-transfer-0.3.9/.coveragrc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 20:33:23.000000 edc-transfer-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 19:16:40.610750 edc-transfer-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 19:16:40.614396 edc-transfer-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 12:23:10.000000 edc-transfer-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1844 2022-06-01 23:48:52.000000 edc-transfer-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-10 12:23:10.000000 edc-transfer-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 12:23:10.000000 edc-transfer-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)       37 2022-06-01 23:48:52.000000 edc-transfer-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:48:52.000000 edc-transfer-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-01-21 23:37:43.000000 edc-transfer-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:48:52.000000 edc-transfer-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1692 2022-08-11 19:16:40.619254 edc-transfer-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      687 2021-02-04 20:33:23.000000 edc-transfer-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-11 19:16:31.000000 edc-transfer-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 12:23:10.000000 edc-transfer-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 19:16:40.616263 edc-transfer-0.3.9/edc_transfer/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-01-21 23:38:05.000000 edc-transfer-0.3.9/edc_transfer/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      770 2021-02-04 20:33:23.000000 edc-transfer-0.3.9/edc_transfer/action_items.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      149 2021-01-21 23:44:04.000000 edc-transfer-0.3.9/edc_transfer/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      181 2021-01-23 15:27:13.000000 edc-transfer-0.3.9/edc_transfer/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       87 2021-01-23 15:27:13.000000 edc-transfer-0.3.9/edc_transfer/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3420 2021-08-26 01:01:17.000000 edc-transfer-0.3.9/edc_transfer/form_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2135 2022-07-03 20:28:49.000000 edc-transfer-0.3.9/edc_transfer/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1976 2022-08-11 00:01:58.000000 edc-transfer-0.3.9/edc_transfer/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      629 2021-04-23 01:08:26.000000 edc-transfer-0.3.9/edc_transfer/modelform_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-01-23 15:27:13.000000 edc-transfer-0.3.9/edc_transfer/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 19:16:40.617580 edc-transfer-0.3.9/edc_transfer/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-01-21 23:56:42.000000 edc-transfer-0.3.9/edc_transfer/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2021-04-23 01:08:26.000000 edc-transfer-0.3.9/edc_transfer/tests/admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 19:16:40.618750 edc-transfer-0.3.9/edc_transfer/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-01-21 23:56:54.000000 edc-transfer-0.3.9/edc_transfer/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-01-21 23:56:54.000000 edc-transfer-0.3.9/edc_transfer/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-01-21 23:56:54.000000 edc-transfer-0.3.9/edc_transfer/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-01-21 23:56:54.000000 edc-transfer-0.3.9/edc_transfer/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-01-21 23:56:53.000000 edc-transfer-0.3.9/edc_transfer/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-01-21 23:56:53.000000 edc-transfer-0.3.9/edc_transfer/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-01-21 23:56:54.000000 edc-transfer-0.3.9/edc_transfer/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-01-21 23:56:54.000000 edc-transfer-0.3.9/edc_transfer/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      636 2021-04-23 01:08:26.000000 edc-transfer-0.3.9/edc_transfer/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2021-04-23 01:08:26.000000 edc-transfer-0.3.9/edc_transfer/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      597 2021-04-23 01:08:26.000000 edc-transfer-0.3.9/edc_transfer/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 19:16:40.618965 edc-transfer-0.3.9/edc_transfer/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-01-21 23:58:11.000000 edc-transfer-0.3.9/edc_transfer/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1178 2022-06-01 23:48:52.000000 edc-transfer-0.3.9/edc_transfer/tests/tests/tests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-02-04 20:33:23.000000 edc-transfer-0.3.9/edc_transfer/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 19:16:40.616842 edc-transfer-0.3.9/edc_transfer.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1692 2022-08-11 19:16:40.000000 edc-transfer-0.3.9/edc_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1290 2022-08-11 19:16:40.000000 edc-transfer-0.3.9/edc_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-11 19:16:40.000000 edc-transfer-0.3.9/edc_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-01-22 01:48:58.000000 edc-transfer-0.3.9/edc_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       13 2022-08-11 19:16:40.000000 edc-transfer-0.3.9/edc_transfer.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1742 2022-08-11 19:16:31.000000 edc-transfer-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2442 2022-06-01 23:48:52.000000 edc-transfer-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1269 2022-08-11 19:16:40.619590 edc-transfer-0.3.9/setup.cfg
```

### Comparing `edc-transfer-0.3.8/.github/workflows/build.yml` & `edc-transfer-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/.gitignore` & `edc-transfer-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/.pre-commit-config.yaml` & `edc-transfer-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/LICENSE` & `edc-transfer-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/PKG-INFO` & `edc-transfer-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-transfer
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple classes related to the django sites framework for clinicedc projects
 Home-page: https://github.com/clinicedc/edc-transfer
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc sites,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-transfer-0.3.8/README.rst` & `edc-transfer-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/edc_transfer/action_items.py` & `edc-transfer-0.3.9/edc_transfer/action_items.py`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/edc_transfer/form_validators.py` & `edc-transfer-0.3.9/edc_transfer/form_validators.py`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/edc_transfer/model_mixins.py` & `edc-transfer-0.3.9/edc_transfer/model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/edc_transfer/modeladmin_mixins.py` & `edc-transfer-0.3.9/edc_transfer/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/edc_transfer/modelform_mixins.py` & `edc-transfer-0.3.9/edc_transfer/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/edc_transfer/tests/etc/user-rsa-local-private.pem` & `edc-transfer-0.3.9/edc_transfer/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/edc_transfer/tests/etc/user-rsa-restricted-private.pem` & `edc-transfer-0.3.9/edc_transfer/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/edc_transfer/tests/forms.py` & `edc-transfer-0.3.9/edc_transfer/tests/forms.py`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/edc_transfer/tests/models.py` & `edc-transfer-0.3.9/edc_transfer/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/edc_transfer/tests/tests/tests.py` & `edc-transfer-0.3.9/edc_transfer/tests/tests/tests.py`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/edc_transfer.egg-info/PKG-INFO` & `edc-transfer-0.3.9/edc_transfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-transfer
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple classes related to the django sites framework for clinicedc projects
 Home-page: https://github.com/clinicedc/edc-transfer
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc sites,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-transfer-0.3.8/edc_transfer.egg-info/SOURCES.txt` & `edc-transfer-0.3.9/edc_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/pyproject.toml` & `edc-transfer-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

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
 source = ["edc_transfer"]
 
 [tool.coverage.paths]
 source = ["edc_transfer"]
 
 [tool.coverage.report]
@@ -58,15 +58,15 @@
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
     dj32: Django>=3.2,<3.3
     dj40: Django>=4.0,<4.1
     dj41: Django>=4.1,<4.2
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

### Comparing `edc-transfer-0.3.8/runtests.py` & `edc-transfer-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-transfer-0.3.8/setup.cfg` & `edc-transfer-0.3.9/setup.cfg`

 * *Files identical despite different names*

