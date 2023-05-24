# Comparing `tmp/edc-navbar-0.3.8.tar.gz` & `tmp/edc-navbar-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-navbar-0.3.8.tar", last modified: Thu Jun 23 21:30:24 2022, max compression
+gzip compressed data, was "edc-navbar-0.3.9.tar", last modified: Fri Aug 12 12:09:59 2022, max compression
```

## Comparing `edc-navbar-0.3.8.tar` & `edc-navbar-0.3.9.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.575842 edc-navbar-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      100 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 16:01:54.000000 edc-navbar-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.563096 edc-navbar-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.566673 edc-navbar-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-19 02:12:43.000000 edc-navbar-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)      955 2022-06-23 21:29:55.000000 edc-navbar-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 21:29:55.000000 edc-navbar-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 21:29:55.000000 edc-navbar-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-04 23:34:19.000000 edc-navbar-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      115 2022-06-23 21:29:55.000000 edc-navbar-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     6268 2022-06-23 21:30:24.575974 edc-navbar-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     5423 2021-02-08 16:01:54.000000 edc-navbar-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-06-23 21:29:55.000000 edc-navbar-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-08 16:01:54.000000 edc-navbar-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.569135 edc-navbar-0.3.8/edc_navbar/
--rw-r--r--   0 erikvw     (501) staff       (20)      172 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      614 2021-09-09 00:27:54.000000 edc-navbar-0.3.8/edc_navbar/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1264 2021-09-09 02:40:23.000000 edc-navbar-0.3.8/edc_navbar/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      758 2022-01-08 16:14:32.000000 edc-navbar-0.3.8/edc_navbar/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2022-06-23 21:29:55.000000 edc-navbar-0.3.8/edc_navbar/get_default_navbar.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.570520 edc-navbar-0.3.8/edc_navbar/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)      595 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      397 2021-04-23 11:57:02.000000 edc-navbar-0.3.8/edc_navbar/migrations/0002_auto_20210423_1451.py
--rw-r--r--   0 erikvw     (501) staff       (20)      352 2021-09-12 17:11:43.000000 edc-navbar-0.3.8/edc_navbar/migrations/0003_alter_navbar_options.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      338 2021-09-09 00:27:54.000000 edc-navbar-0.3.8/edc_navbar/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2137 2021-02-08 16:01:54.000000 edc-navbar-0.3.8/edc_navbar/navbar.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4989 2022-06-23 21:29:55.000000 edc-navbar-0.3.8/edc_navbar/navbar_item.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1098 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4253 2022-06-23 21:29:55.000000 edc-navbar-0.3.8/edc_navbar/site_navbars.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.563366 edc-navbar-0.3.8/edc_navbar/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.563464 edc-navbar-0.3.8/edc_navbar/templates/edc_navbar/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.570747 edc-navbar-0.3.8/edc_navbar/templates/edc_navbar/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      516 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/templates/edc_navbar/bootstrap3/edc_navbar.html
--rw-r--r--   0 erikvw     (501) staff       (20)      762 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/templates/edc_navbar/bootstrap3/navbar_item.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.570927 edc-navbar-0.3.8/edc_navbar/templates/edc_navbar/bootstrap4/
--rw-r--r--   0 erikvw     (501) staff       (20)      732 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/templates/edc_navbar/bootstrap4/navbar_item.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.572649 edc-navbar-0.3.8/edc_navbar/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      816 2022-06-23 21:29:55.000000 edc-navbar-0.3.8/edc_navbar/templatetags/edc_navbar_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.574101 edc-navbar-0.3.8/edc_navbar/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2021-02-08 16:01:54.000000 edc-navbar-0.3.8/edc_navbar/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.575327 edc-navbar-0.3.8/edc_navbar/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      522 2020-03-06 15:50:39.000000 edc-navbar-0.3.8/edc_navbar/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      478 2020-03-06 15:50:39.000000 edc-navbar-0.3.8/edc_navbar/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.575634 edc-navbar-0.3.8/edc_navbar/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4935 2022-06-23 21:29:55.000000 edc-navbar-0.3.8/edc_navbar/tests/tests/test_navbar.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1127 2021-02-08 16:01:54.000000 edc-navbar-0.3.8/edc_navbar/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      531 2021-02-08 16:01:54.000000 edc-navbar-0.3.8/edc_navbar/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1452 2022-06-09 17:32:34.000000 edc-navbar-0.3.8/edc_navbar/view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      398 2020-03-04 23:34:40.000000 edc-navbar-0.3.8/edc_navbar/wsgi.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 21:30:24.569885 edc-navbar-0.3.8/edc_navbar.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     6268 2022-06-23 21:30:24.000000 edc-navbar-0.3.8/edc_navbar.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1627 2022-06-23 21:30:24.000000 edc-navbar-0.3.8/edc_navbar.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-06-23 21:30:24.000000 edc-navbar-0.3.8/edc_navbar.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:34:44.000000 edc-navbar-0.3.8/edc_navbar.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-06-23 21:30:24.000000 edc-navbar-0.3.8/edc_navbar.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1581 2022-06-23 21:29:55.000000 edc-navbar-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2788 2021-09-09 00:27:54.000000 edc-navbar-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1138 2022-06-23 21:30:24.577333 edc-navbar-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.801326 edc-navbar-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      100 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 16:01:54.000000 edc-navbar-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.791636 edc-navbar-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.794755 edc-navbar-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-12 12:09:51.000000 edc-navbar-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)      955 2022-06-23 21:29:55.000000 edc-navbar-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-12 12:09:51.000000 edc-navbar-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-12 12:09:51.000000 edc-navbar-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 21:29:55.000000 edc-navbar-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 21:29:55.000000 edc-navbar-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-04 23:34:19.000000 edc-navbar-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      115 2022-06-23 21:29:55.000000 edc-navbar-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     6397 2022-08-12 12:09:59.801426 edc-navbar-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     5423 2021-02-08 16:01:54.000000 edc-navbar-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-12 12:09:51.000000 edc-navbar-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-12 12:09:51.000000 edc-navbar-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.797041 edc-navbar-0.3.9/edc_navbar/
+-rw-r--r--   0 erikvw     (501) staff       (20)      172 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      614 2021-09-09 00:27:54.000000 edc-navbar-0.3.9/edc_navbar/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1264 2021-09-09 02:40:23.000000 edc-navbar-0.3.9/edc_navbar/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      758 2022-01-08 16:14:32.000000 edc-navbar-0.3.9/edc_navbar/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      253 2022-06-23 21:29:55.000000 edc-navbar-0.3.9/edc_navbar/get_default_navbar.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.798193 edc-navbar-0.3.9/edc_navbar/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)      595 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      397 2022-08-12 12:09:51.000000 edc-navbar-0.3.9/edc_navbar/migrations/0002_auto_20210423_1451.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      352 2021-09-12 17:11:43.000000 edc-navbar-0.3.9/edc_navbar/migrations/0003_alter_navbar_options.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      338 2021-09-09 00:27:54.000000 edc-navbar-0.3.9/edc_navbar/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2137 2021-02-08 16:01:54.000000 edc-navbar-0.3.9/edc_navbar/navbar.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4989 2022-06-23 21:29:55.000000 edc-navbar-0.3.9/edc_navbar/navbar_item.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1098 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4253 2022-06-23 21:29:55.000000 edc-navbar-0.3.9/edc_navbar/site_navbars.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.791905 edc-navbar-0.3.9/edc_navbar/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.791997 edc-navbar-0.3.9/edc_navbar/templates/edc_navbar/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.798409 edc-navbar-0.3.9/edc_navbar/templates/edc_navbar/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      516 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/templates/edc_navbar/bootstrap3/edc_navbar.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      762 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/templates/edc_navbar/bootstrap3/navbar_item.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.798622 edc-navbar-0.3.9/edc_navbar/templates/edc_navbar/bootstrap4/
+-rw-r--r--   0 erikvw     (501) staff       (20)      732 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/templates/edc_navbar/bootstrap4/navbar_item.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.798868 edc-navbar-0.3.9/edc_navbar/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      816 2022-06-23 21:29:55.000000 edc-navbar-0.3.9/edc_navbar/templatetags/edc_navbar_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.799570 edc-navbar-0.3.9/edc_navbar/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       73 2021-02-08 16:01:54.000000 edc-navbar-0.3.9/edc_navbar/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.800917 edc-navbar-0.3.9/edc_navbar/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      522 2020-03-06 15:50:39.000000 edc-navbar-0.3.9/edc_navbar/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      478 2020-03-06 15:50:39.000000 edc-navbar-0.3.9/edc_navbar/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.801173 edc-navbar-0.3.9/edc_navbar/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4935 2022-06-23 21:29:55.000000 edc-navbar-0.3.9/edc_navbar/tests/tests/test_navbar.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1127 2021-02-08 16:01:54.000000 edc-navbar-0.3.9/edc_navbar/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      531 2021-02-08 16:01:54.000000 edc-navbar-0.3.9/edc_navbar/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1452 2022-06-09 17:32:34.000000 edc-navbar-0.3.9/edc_navbar/view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      398 2020-03-04 23:34:40.000000 edc-navbar-0.3.9/edc_navbar/wsgi.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:09:59.797734 edc-navbar-0.3.9/edc_navbar.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     6397 2022-08-12 12:09:59.000000 edc-navbar-0.3.9/edc_navbar.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1661 2022-08-12 12:09:59.000000 edc-navbar-0.3.9/edc_navbar.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-12 12:09:59.000000 edc-navbar-0.3.9/edc_navbar.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:34:44.000000 edc-navbar-0.3.9/edc_navbar.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-08-12 12:09:59.000000 edc-navbar-0.3.9/edc_navbar.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1722 2022-08-12 12:09:51.000000 edc-navbar-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2725 2022-08-12 12:09:51.000000 edc-navbar-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1236 2022-08-12 12:09:59.801747 edc-navbar-0.3.9/setup.cfg
```

### Comparing `edc-navbar-0.3.8/.github/workflows/build.yml` & `edc-navbar-0.3.9/.github/workflows/build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,70 @@
+---
 name: build
 
 on: [push, pull_request]
 
 jobs:
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.9']
-        django-version: ['3.2']
+        python-version: ['3.9', '3.10']
+        django-version: ['3.2', '4.0', '4.1', 'dev']
 
     services:
-
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
           - 3306:3306
         options: --health-cmd="mysqladmin ping" --health-interval=10s --health-timeout=5s --health-retries=3
 
     steps:
-    - name: Install pycups and words dependency
-      run: |
-        sudo apt-get install libcups2-dev wamerican
-
-    - uses: actions/checkout@v2
-
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-
-    - name: Get pip cache dir
-      id: pip-cache
-      run: |
-        echo "::set-output name=dir::$(pip cache dir)"
-
-    - name: Cache
-      uses: actions/cache@v2
-      with:
-        path: ${{ steps.pip-cache.outputs.dir }}
-        key:
-          ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
-        restore-keys: |
-          ${{ matrix.python-version }}-v1-
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        python -m pip install -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
-
-
-    - name: Tox tests
-      run: |
-        tox -v
-      env:
-        DJANGO: ${{ matrix.django-version }}
-
-    - name: Upload coverage
-      uses: codecov/codecov-action@v1
-      with:
-        name: Python ${{ matrix.python-version }}
+      - name: Install pycups and words dependency
+        run: |
+          sudo sed -i 's/azure\.//' /etc/apt/sources.list
+          sudo apt-get -y update
+          sudo apt-get install libcups2-dev wamerican
+
+      - uses: actions/checkout@v2
+
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Get pip cache dir
+        id: pip-cache
+        run: |
+          echo "::set-output name=dir::$(pip cache dir)"
+
+      - name: Cache
+        uses: actions/cache@v2
+        with:
+          path: ${{ steps.pip-cache.outputs.dir }}
+          key:
+            ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
+          restore-keys: |
+            ${{ matrix.python-version }}-v1-
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          python -m pip install -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
+
+
+      - name: Tox tests
+        run: |
+          tox -v
+        env:
+          DJANGO: ${{ matrix.django-version }}
+
+      - name: Upload coverage
+        uses: codecov/codecov-action@v1
+        with:
+          name: Python ${{ matrix.python-version }}
```

### Comparing `edc-navbar-0.3.8/.gitignore` & `edc-navbar-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/LICENSE` & `edc-navbar-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/PKG-INFO` & `edc-navbar-0.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: edc-navbar
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple navbar classes in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-navbar
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc navbar,clinicedc,clinical trials
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
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-navbar-0.3.8/README.rst` & `edc-navbar-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/apps.py` & `edc-navbar-0.3.9/edc_navbar/apps.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/auth_objects.py` & `edc-navbar-0.3.9/edc_navbar/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/auths.py` & `edc-navbar-0.3.9/edc_navbar/auths.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/migrations/0001_initial.py` & `edc-navbar-0.3.9/edc_navbar/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/navbar.py` & `edc-navbar-0.3.9/edc_navbar/navbar.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/navbar_item.py` & `edc-navbar-0.3.9/edc_navbar/navbar_item.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/navbars.py` & `edc-navbar-0.3.9/edc_navbar/navbars.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/site_navbars.py` & `edc-navbar-0.3.9/edc_navbar/site_navbars.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/templates/edc_navbar/bootstrap3/edc_navbar.html` & `edc-navbar-0.3.9/edc_navbar/templates/edc_navbar/bootstrap3/edc_navbar.html`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/templates/edc_navbar/bootstrap3/navbar_item.html` & `edc-navbar-0.3.9/edc_navbar/templates/edc_navbar/bootstrap3/navbar_item.html`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/templates/edc_navbar/bootstrap4/navbar_item.html` & `edc-navbar-0.3.9/edc_navbar/templates/edc_navbar/bootstrap4/navbar_item.html`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/templatetags/edc_navbar_extras.py` & `edc-navbar-0.3.9/edc_navbar/templatetags/edc_navbar_extras.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/tests/etc/user-rsa-local-private.pem` & `edc-navbar-0.3.9/edc_navbar/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/tests/etc/user-rsa-restricted-private.pem` & `edc-navbar-0.3.9/edc_navbar/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/tests/holidays.csv` & `edc-navbar-0.3.9/edc_navbar/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/tests/tests/test_navbar.py` & `edc-navbar-0.3.9/edc_navbar/tests/tests/test_navbar.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/tests/urls.py` & `edc-navbar-0.3.9/edc_navbar/tests/urls.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/urls.py` & `edc-navbar-0.3.9/edc_navbar/urls.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar/view_mixin.py` & `edc-navbar-0.3.9/edc_navbar/view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-navbar-0.3.8/edc_navbar.egg-info/PKG-INFO` & `edc-navbar-0.3.9/edc_navbar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: edc-navbar
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple navbar classes in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-navbar
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc navbar,clinicedc,clinical trials
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
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-navbar-0.3.8/edc_navbar.egg-info/SOURCES.txt` & `edc-navbar-0.3.9/edc_navbar.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

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

### Comparing `edc-navbar-0.3.8/pyproject.toml` & `edc-navbar-0.3.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -28,39 +28,47 @@
 skip_covered = true
 omit = ["requirements.txt"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{39}-dj{32,dev},
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
+    4.0: dj40
+    4.1: dj41
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
     dj32: Django>=3.2,<3.3
+    dj40: Django>=4.0,<4.1
+    dj41: Django>=4.1,<4.2
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

### Comparing `edc-navbar-0.3.8/runtests.py` & `edc-navbar-0.3.9/runtests.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,16 +29,14 @@
         "django.contrib.admin",
         "django.contrib.auth",
         "django.contrib.contenttypes",
         "django.contrib.sessions",
         "django.contrib.messages",
         "django.contrib.staticfiles",
         "django.contrib.sites",
-        "django_celery_beat",
-        "django_celery_results",
         "django_crypto_fields.apps.AppConfig",
         "edc_action_item.apps.AppConfig",
         "edc_auth.apps.AppConfig",
         "edc_crf.apps.AppConfig",
         "edc_navbar.apps.AppConfig",
         "edc_adverse_event.apps.AppConfig",
         "edc_appointment.apps.AppConfig",
```

### Comparing `edc-navbar-0.3.8/setup.cfg` & `edc-navbar-0.3.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django Edc navbar, clinicedc, clinical trials
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
 	edc_navbar.tests*
 
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

