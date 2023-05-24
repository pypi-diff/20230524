# Comparing `tmp/edc-device-0.3.8.tar.gz` & `tmp/edc-device-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-device-0.3.8.tar", last modified: Thu Aug 11 23:21:59 2022, max compression
+gzip compressed data, was "edc-device-0.3.9.tar", last modified: Thu Sep  8 11:45:34 2022, max compression
```

## Comparing `edc-device-0.3.8.tar` & `edc-device-0.3.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:21:59.906700 edc-device-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       89 2020-03-04 22:50:07.000000 edc-device-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 17:40:44.000000 edc-device-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:21:59.896143 edc-device-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:21:59.899323 edc-device-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 11:17:52.000000 edc-device-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1397 2022-06-23 20:39:40.000000 edc-device-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-10 11:17:52.000000 edc-device-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 11:17:52.000000 edc-device-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 20:39:40.000000 edc-device-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 20:39:40.000000 edc-device-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    18047 2020-03-04 22:48:42.000000 edc-device-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      115 2022-06-23 20:39:40.000000 edc-device-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     8090 2022-08-11 23:21:59.906819 edc-device-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     7107 2021-02-04 17:40:44.000000 edc-device-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-11 23:21:52.000000 edc-device-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-10 11:17:52.000000 edc-device-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:21:59.901479 edc-device-0.3.8/edc_device/
--rw-r--r--   0 erikvw     (501) staff       (20)      286 2021-02-04 17:40:44.000000 edc-device-0.3.8/edc_device/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1782 2021-02-04 17:40:44.000000 edc-device-0.3.8/edc_device/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      120 2022-07-08 06:55:39.000000 edc-device-0.3.8/edc_device/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3926 2022-08-10 11:17:52.000000 edc-device-0.3.8/edc_device/device.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3887 2021-02-04 17:40:44.000000 edc-device-0.3.8/edc_device/device_permission.py
--rw-r--r--   0 erikvw     (501) staff       (20)      148 2021-07-28 02:58:17.000000 edc-device-0.3.8/edc_device/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      334 2020-03-04 22:50:07.000000 edc-device-0.3.8/edc_device/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)      943 2021-02-04 17:40:44.000000 edc-device-0.3.8/edc_device/signals.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:21:59.896366 edc-device-0.3.8/edc_device/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:21:59.896407 edc-device-0.3.8/edc_device/templates/edc_device/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:21:59.902442 edc-device-0.3.8/edc_device/templates/edc_device/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)     1691 2022-08-10 11:17:52.000000 edc-device-0.3.8/edc_device/templates/edc_device/bootstrap3/home.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:21:59.903143 edc-device-0.3.8/edc_device/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       49 2020-03-04 22:50:07.000000 edc-device-0.3.8/edc_device/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      703 2022-08-10 11:17:52.000000 edc-device-0.3.8/edc_device/tests/device_test_helper.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:21:59.905379 edc-device-0.3.8/edc_device/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:24:02.000000 edc-device-0.3.8/edc_device/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:24:02.000000 edc-device-0.3.8/edc_device/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-09 16:24:02.000000 edc-device-0.3.8/edc_device/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-09 16:24:02.000000 edc-device-0.3.8/edc_device/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-09 16:24:02.000000 edc-device-0.3.8/edc_device/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-09 16:24:02.000000 edc-device-0.3.8/edc_device/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:24:02.000000 edc-device-0.3.8/edc_device/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:24:02.000000 edc-device-0.3.8/edc_device/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-04 22:50:07.000000 edc-device-0.3.8/edc_device/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:21:59.906255 edc-device-0.3.8/edc_device/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-28 02:58:17.000000 edc-device-0.3.8/edc_device/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4275 2022-06-23 20:39:40.000000 edc-device-0.3.8/edc_device/tests/tests/test_device.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6105 2021-07-28 02:58:17.000000 edc-device-0.3.8/edc_device/tests/tests/test_device_permission.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2991 2021-07-28 02:58:17.000000 edc-device-0.3.8/edc_device/tests/tests/test_model.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1505 2022-05-25 02:47:55.000000 edc-device-0.3.8/edc_device/tests/tests/test_views.py
--rw-r--r--   0 erikvw     (501) staff       (20)      478 2020-03-04 22:50:07.000000 edc-device-0.3.8/edc_device/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2021-02-04 17:40:44.000000 edc-device-0.3.8/edc_device/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      976 2022-06-23 20:39:40.000000 edc-device-0.3.8/edc_device/view_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      833 2022-06-23 20:39:40.000000 edc-device-0.3.8/edc_device/views.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:21:59.902302 edc-device-0.3.8/edc_device.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     8090 2022-08-11 23:21:59.000000 edc-device-0.3.8/edc_device.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1361 2022-08-11 23:21:59.000000 edc-device-0.3.8/edc_device.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-11 23:21:59.000000 edc-device-0.3.8/edc_device.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 22:50:07.000000 edc-device-0.3.8/edc_device.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-08-11 23:21:59.000000 edc-device-0.3.8/edc_device.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1722 2022-08-10 11:17:52.000000 edc-device-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2531 2022-08-11 23:21:51.000000 edc-device-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1244 2022-08-11 23:21:59.907242 edc-device-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:45:34.349020 edc-device-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       89 2020-03-04 22:50:07.000000 edc-device-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 17:40:44.000000 edc-device-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:45:34.340676 edc-device-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:45:34.343598 edc-device-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 11:17:52.000000 edc-device-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1397 2022-06-23 20:39:40.000000 edc-device-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-10 11:17:52.000000 edc-device-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 11:17:52.000000 edc-device-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 20:39:40.000000 edc-device-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 20:39:40.000000 edc-device-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    18047 2020-03-04 22:48:42.000000 edc-device-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      115 2022-06-23 20:39:40.000000 edc-device-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     8090 2022-09-08 11:45:34.349134 edc-device-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     7107 2021-02-04 17:40:44.000000 edc-device-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-08 11:45:26.000000 edc-device-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-10 11:17:52.000000 edc-device-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:45:34.345708 edc-device-0.3.9/edc_device/
+-rw-r--r--   0 erikvw     (501) staff       (20)      286 2021-02-04 17:40:44.000000 edc-device-0.3.9/edc_device/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1782 2021-02-04 17:40:44.000000 edc-device-0.3.9/edc_device/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      120 2022-07-08 06:55:39.000000 edc-device-0.3.9/edc_device/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3926 2022-08-10 11:17:52.000000 edc-device-0.3.9/edc_device/device.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3887 2021-02-04 17:40:44.000000 edc-device-0.3.9/edc_device/device_permission.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      148 2021-07-28 02:58:17.000000 edc-device-0.3.9/edc_device/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      334 2020-03-04 22:50:07.000000 edc-device-0.3.9/edc_device/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      943 2021-02-04 17:40:44.000000 edc-device-0.3.9/edc_device/signals.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:45:34.340896 edc-device-0.3.9/edc_device/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:45:34.340937 edc-device-0.3.9/edc_device/templates/edc_device/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:45:34.346449 edc-device-0.3.9/edc_device/templates/edc_device/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1691 2022-08-10 11:17:52.000000 edc-device-0.3.9/edc_device/templates/edc_device/bootstrap3/home.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:45:34.347047 edc-device-0.3.9/edc_device/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       49 2020-03-04 22:50:07.000000 edc-device-0.3.9/edc_device/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      703 2022-08-10 11:17:52.000000 edc-device-0.3.9/edc_device/tests/device_test_helper.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:45:34.348141 edc-device-0.3.9/edc_device/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:24:02.000000 edc-device-0.3.9/edc_device/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:24:02.000000 edc-device-0.3.9/edc_device/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-09 16:24:02.000000 edc-device-0.3.9/edc_device/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-09 16:24:02.000000 edc-device-0.3.9/edc_device/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-09 16:24:02.000000 edc-device-0.3.9/edc_device/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-09 16:24:02.000000 edc-device-0.3.9/edc_device/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:24:02.000000 edc-device-0.3.9/edc_device/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:24:02.000000 edc-device-0.3.9/edc_device/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-04 22:50:07.000000 edc-device-0.3.9/edc_device/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:45:34.348808 edc-device-0.3.9/edc_device/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-28 02:58:17.000000 edc-device-0.3.9/edc_device/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4275 2022-06-23 20:39:40.000000 edc-device-0.3.9/edc_device/tests/tests/test_device.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6105 2021-07-28 02:58:17.000000 edc-device-0.3.9/edc_device/tests/tests/test_device_permission.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2991 2021-07-28 02:58:17.000000 edc-device-0.3.9/edc_device/tests/tests/test_model.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1505 2022-05-25 02:47:55.000000 edc-device-0.3.9/edc_device/tests/tests/test_views.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      478 2020-03-04 22:50:07.000000 edc-device-0.3.9/edc_device/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2021-02-04 17:40:44.000000 edc-device-0.3.9/edc_device/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      976 2022-06-23 20:39:40.000000 edc-device-0.3.9/edc_device/view_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      833 2022-06-23 20:39:40.000000 edc-device-0.3.9/edc_device/views.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:45:34.346344 edc-device-0.3.9/edc_device.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     8090 2022-09-08 11:45:34.000000 edc-device-0.3.9/edc_device.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1361 2022-09-08 11:45:34.000000 edc-device-0.3.9/edc_device.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-08 11:45:34.000000 edc-device-0.3.9/edc_device.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 22:50:07.000000 edc-device-0.3.9/edc_device.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-09-08 11:45:34.000000 edc-device-0.3.9/edc_device.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1722 2022-08-10 11:17:52.000000 edc-device-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2618 2022-09-08 11:45:26.000000 edc-device-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1244 2022-09-08 11:45:34.349442 edc-device-0.3.9/setup.cfg
```

### Comparing `edc-device-0.3.8/.github/workflows/build.yml` & `edc-device-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/.gitignore` & `edc-device-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/.pre-commit-config.yaml` & `edc-device-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/LICENSE` & `edc-device-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/PKG-INFO` & `edc-device-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-device
-Version: 0.3.8
+Version: 0.3.9
 Summary: Get info on a data collection device for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-device
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-device-0.3.8/README.rst` & `edc-device-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/apps.py` & `edc-device-0.3.9/edc_device/apps.py`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/device.py` & `edc-device-0.3.9/edc_device/device.py`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/device_permission.py` & `edc-device-0.3.9/edc_device/device_permission.py`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/signals.py` & `edc-device-0.3.9/edc_device/signals.py`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/templates/edc_device/bootstrap3/home.html` & `edc-device-0.3.9/edc_device/templates/edc_device/bootstrap3/home.html`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/tests/device_test_helper.py` & `edc-device-0.3.9/edc_device/tests/device_test_helper.py`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/tests/etc/user-rsa-local-private.pem` & `edc-device-0.3.9/edc_device/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/tests/etc/user-rsa-restricted-private.pem` & `edc-device-0.3.9/edc_device/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/tests/tests/test_device.py` & `edc-device-0.3.9/edc_device/tests/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/tests/tests/test_device_permission.py` & `edc-device-0.3.9/edc_device/tests/tests/test_device_permission.py`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/tests/tests/test_model.py` & `edc-device-0.3.9/edc_device/tests/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/tests/tests/test_views.py` & `edc-device-0.3.9/edc_device/tests/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/view_mixins.py` & `edc-device-0.3.9/edc_device/view_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device/views.py` & `edc-device-0.3.9/edc_device/views.py`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/edc_device.egg-info/PKG-INFO` & `edc-device-0.3.9/edc_device.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-device
-Version: 0.3.8
+Version: 0.3.9
 Summary: Get info on a data collection device for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-device
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-device-0.3.8/edc_device.egg-info/SOURCES.txt` & `edc-device-0.3.9/edc_device.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/pyproject.toml` & `edc-device-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-device-0.3.8/runtests.py` & `edc-device-0.3.9/runtests.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         "django.contrib.staticfiles",
         "django.contrib.sites",
         "django_crypto_fields.apps.AppConfig",
         "django_revision.apps.AppConfig",
         "multisite",
         "edc_appointment.apps.AppConfig",
         "edc_action_item.apps.AppConfig",
-        "adverse_event_app.apps.AppConfig",
         "edc_adverse_event.apps.AppConfig",
         "edc_auth.apps.AppConfig",
         "edc_notification.apps.AppConfig",
         "edc_consent.apps.AppConfig",
         "edc_crf.apps.AppConfig",
         "edc_data_manager.apps.AppConfig",
         "edc_device.apps.AppConfig",
@@ -54,15 +53,18 @@
         "edc_protocol.apps.AppConfig",
         "edc_randomization.apps.AppConfig",
         "edc_registration.apps.AppConfig",
         "edc_sites.apps.AppConfig",
         "edc_timepoint.apps.AppConfig",
         "edc_visit_schedule.apps.AppConfig",
         "edc_visit_tracking.apps.AppConfig",
+        "edc_listboard.apps.AppConfig",
+        "edc_review_dashboard.apps.AppConfig",
         "edc_subject_dashboard.apps.AppConfig",
+        "adverse_event_app.apps.AppConfig",
         "edc_dashboard.apps.AppConfig",
     ],
     add_dashboard_middleware=True,
     use_test_urls=True,
 ).settings
```

### Comparing `edc-device-0.3.8/setup.cfg` & `edc-device-0.3.9/setup.cfg`

 * *Files identical despite different names*

