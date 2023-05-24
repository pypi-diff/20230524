# Comparing `tmp/edc-listboard-0.1.8.tar.gz` & `tmp/edc-listboard-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-listboard-0.1.8.tar", last modified: Fri May 12 04:32:31 2023, max compression
+gzip compressed data, was "edc-listboard-0.1.9.tar", last modified: Wed May 24 16:54:07 2023, max compression
```

## Comparing `edc-listboard-0.1.8.tar` & `edc-listboard-0.1.9.tar`

### file list

```diff
@@ -1,85 +1,84 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.763881 edc-listboard-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.748431 edc-listboard-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.752426 edc-listboard-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1821 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:32:24.000000 edc-listboard-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-08-23 20:00:32.000000 edc-listboard-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)      902 2023-05-12 04:32:31.763967 edc-listboard-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)       40 2022-08-25 03:17:45.000000 edc-listboard-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-26 00:16:33.000000 edc-listboard-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.753416 edc-listboard-0.1.8/edc_listboard/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      348 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      174 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/dashboard_templates.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.755675 edc-listboard-0.1.8/edc_listboard/filters/
--rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/filters/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1093 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/filters/listboard_filter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1566 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/filters/listboard_view_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)      853 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/middleware.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.756022 edc-listboard-0.1.8/edc_listboard/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     3713 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      299 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      397 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/system_checks.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.748844 edc-listboard-0.1.8/edc_listboard/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.748895 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.756124 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.756857 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/
--rw-r--r--   0 erikvw     (501) staff       (20)     1244 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/buttons_column.html
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/columns.html
--rw-r--r--   0 erikvw     (501) staff       (20)      297 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/results_body.html
--rw-r--r--   0 erikvw     (501) staff       (20)      197 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/results_header.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2549 2022-11-17 00:02:13.000000 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.757441 edc-listboard-0.1.8/edc_listboard/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.758758 edc-listboard-0.1.8/edc_listboard/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      113 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/django_crypto_fields
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1119 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.758990 edc-listboard-0.1.8/edc_listboard/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4469 2022-09-15 01:52:48.000000 edc-listboard-0.1.8/edc_listboard/tests/tests/test_view_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      928 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.760026 edc-listboard-0.1.8/edc_listboard/view_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      301 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2645 2022-09-26 00:16:33.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/listboard_filter_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      924 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/querystring_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1152 2022-09-26 00:16:33.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/search_form_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3316 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/search_listboard_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      254 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/site_queryset_view_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.760334 edc-listboard-0.1.8/edc_listboard/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      127 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9546 2022-09-26 00:16:00.000000 edc-listboard-0.1.8/edc_listboard/views/listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.762330 edc-listboard-0.1.8/edc_listboard/views/screen/
--rw-r--r--   0 erikvw     (501) staff       (20)      105 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/views/screen/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      678 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/views/screen/listboard_view_filter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2581 2022-08-26 02:01:49.000000 edc-listboard-0.1.8/edc_listboard/views/screen/screening_listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.763772 edc-listboard-0.1.8/edc_listboard/views/subject/
--rw-r--r--   0 erikvw     (501) staff       (20)       57 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/views/subject/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2246 2023-05-12 04:32:24.000000 edc-listboard-0.1.8/edc_listboard/views/subject/subject_listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.755129 edc-listboard-0.1.8/edc_listboard.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)      902 2023-05-12 04:32:31.000000 edc-listboard-0.1.8/edc_listboard.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2404 2023-05-12 04:32:31.000000 edc-listboard-0.1.8/edc_listboard.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-12 04:32:31.000000 edc-listboard-0.1.8/edc_listboard.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-23 20:16:36.000000 edc-listboard-0.1.8/edc_listboard.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2023-05-12 04:32:31.000000 edc-listboard-0.1.8/edc_listboard.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1709 2023-05-12 04:32:24.000000 edc-listboard-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1856 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1154 2023-05-12 04:32:31.764290 edc-listboard-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.816197 edc-listboard-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/.coveragrc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.804726 edc-listboard-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.808880 edc-listboard-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:53:59.000000 edc-listboard-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1821 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:53:59.000000 edc-listboard-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-08-23 20:00:32.000000 edc-listboard-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)      903 2023-05-24 16:54:07.816301 edc-listboard-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)       40 2022-08-25 03:17:45.000000 edc-listboard-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.809787 edc-listboard-0.1.9/edc_listboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      348 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      174 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/dashboard_templates.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.810850 edc-listboard-0.1.9/edc_listboard/filters/
+-rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/filters/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1093 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/filters/listboard_filter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1566 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/filters/listboard_view_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      853 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/middleware.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.811106 edc-listboard-0.1.9/edc_listboard/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     3712 2023-05-24 16:53:59.000000 edc-listboard-0.1.9/edc_listboard/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2023-05-24 16:53:59.000000 edc-listboard-0.1.9/edc_listboard/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      397 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/system_checks.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.805120 edc-listboard-0.1.9/edc_listboard/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.805165 edc-listboard-0.1.9/edc_listboard/templates/edc_listboard/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.811196 edc-listboard-0.1.9/edc_listboard/templates/edc_listboard/bootstrap3/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.811849 edc-listboard-0.1.9/edc_listboard/templates/edc_listboard/bootstrap3/include/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1244 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/templates/edc_listboard/bootstrap3/include/buttons_column.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/templates/edc_listboard/bootstrap3/include/columns.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      297 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/templates/edc_listboard/bootstrap3/include/results_body.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      197 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/templates/edc_listboard/bootstrap3/include/results_header.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2549 2022-11-17 00:02:13.000000 edc-listboard-0.1.9/edc_listboard/templates/edc_listboard/bootstrap3/listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.812350 edc-listboard-0.1.9/edc_listboard/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.813753 edc-listboard-0.1.9/edc_listboard/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      113 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/etc/django_crypto_fields
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1119 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.813982 edc-listboard-0.1.9/edc_listboard/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4469 2022-09-15 01:52:48.000000 edc-listboard-0.1.9/edc_listboard/tests/tests/test_view_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      928 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.814983 edc-listboard-0.1.9/edc_listboard/view_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      301 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/view_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2644 2023-05-24 16:53:59.000000 edc-listboard-0.1.9/edc_listboard/view_mixins/listboard_filter_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      924 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/view_mixins/querystring_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1151 2023-05-24 16:53:59.000000 edc-listboard-0.1.9/edc_listboard/view_mixins/search_form_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3315 2023-05-24 16:53:59.000000 edc-listboard-0.1.9/edc_listboard/view_mixins/search_listboard_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      254 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/view_mixins/site_queryset_view_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.815296 edc-listboard-0.1.9/edc_listboard/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      127 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9545 2023-05-24 16:53:59.000000 edc-listboard-0.1.9/edc_listboard/views/listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.815689 edc-listboard-0.1.9/edc_listboard/views/screen/
+-rw-r--r--   0 erikvw     (501) staff       (20)      105 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/views/screen/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      677 2023-05-24 16:53:59.000000 edc-listboard-0.1.9/edc_listboard/views/screen/listboard_view_filter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2580 2023-05-24 16:53:59.000000 edc-listboard-0.1.9/edc_listboard/views/screen/screening_listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.815960 edc-listboard-0.1.9/edc_listboard/views/subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)       57 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/edc_listboard/views/subject/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2246 2023-05-12 04:32:24.000000 edc-listboard-0.1.9/edc_listboard/views/subject/subject_listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:07.810483 edc-listboard-0.1.9/edc_listboard.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)      903 2023-05-24 16:54:07.000000 edc-listboard-0.1.9/edc_listboard.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2396 2023-05-24 16:54:07.000000 edc-listboard-0.1.9/edc_listboard.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 16:54:07.000000 edc-listboard-0.1.9/edc_listboard.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-23 20:16:36.000000 edc-listboard-0.1.9/edc_listboard.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2023-05-24 16:54:07.000000 edc-listboard-0.1.9/edc_listboard.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1772 2023-05-24 16:53:59.000000 edc-listboard-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1856 2022-08-25 03:16:05.000000 edc-listboard-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1155 2023-05-24 16:54:07.816607 edc-listboard-0.1.9/setup.cfg
```

### Comparing `edc-listboard-0.1.8/.github/workflows/build.yml` & `edc-listboard-0.1.9/.github/workflows/build.yml`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,19 @@
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.9', '3.10']
-        django-version: ['3.2', '4.0', '4.1', 'dev']
-
+        python-version: ['3.10', '3.11']
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
@@ -27,28 +29,27 @@
     steps:
       - name: Install pycups and words dependency
         run: |
           sudo sed -i 's/azure\.//' /etc/apt/sources.list
           sudo apt-get -y update
           sudo apt-get install libcups2-dev wamerican
 
-      - uses: actions/checkout@v2
-
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Get pip cache dir
         id: pip-cache
         run: |
-          echo "::set-output name=dir::$(pip cache dir)"
+          echo "dir=$(pip cache dir)" >>$GITHUB_OUTPUT
 
       - name: Cache
-        uses: actions/cache@v2
+        uses: actions/cache@v3
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key:
             ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
           restore-keys: |
             ${{ matrix.python-version }}-v1-
 
@@ -60,11 +61,11 @@
 
       - name: Tox tests
         run: |
           tox -v
         env:
           DJANGO: ${{ matrix.django-version }}
 
-      - name: Upload coverage
-        uses: codecov/codecov-action@v1
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v3
         with:
           name: Python ${{ matrix.python-version }}
```

### Comparing `edc-listboard-0.1.8/.gitignore` & `edc-listboard-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/.pre-commit-config.yaml` & `edc-listboard-0.1.9/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
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
@@ -38,12 +38,12 @@
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

### Comparing `edc-listboard-0.1.8/LICENSE` & `edc-listboard-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/PKG-INFO` & `edc-listboard-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-listboard
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes for Listboard views in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-listboard
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc listboard,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
@@ -12,14 +12,14 @@
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 # edc-listboard
 Listboard class for edc
```

### Comparing `edc-listboard-0.1.8/edc_listboard/filters/listboard_filter.py` & `edc-listboard-0.1.9/edc_listboard/filters/listboard_filter.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard/filters/listboard_view_filters.py` & `edc-listboard-0.1.9/edc_listboard/filters/listboard_view_filters.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard/middleware.py` & `edc-listboard-0.1.9/edc_listboard/middleware.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard/migrations/0001_initial.py` & `edc-listboard-0.1.9/edc_listboard/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import django_audit_fields.fields.userfield
 import django_audit_fields.fields.uuid_auto_field
 import django_audit_fields.models.audit_model_mixin
 import django_revision.revision_field
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Listboard",
```

### Comparing `edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/buttons_column.html` & `edc-listboard-0.1.9/edc_listboard/templates/edc_listboard/bootstrap3/include/buttons_column.html`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/listboard.html` & `edc-listboard-0.1.9/edc_listboard/templates/edc_listboard/bootstrap3/listboard.html`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-local-private.pem` & `edc-listboard-0.1.9/edc_listboard/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-restricted-private.pem` & `edc-listboard-0.1.9/edc_listboard/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard/tests/models.py` & `edc-listboard-0.1.9/edc_listboard/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard/tests/tests/test_view_mixins.py` & `edc-listboard-0.1.9/edc_listboard/tests/tests/test_view_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard/tests/urls.py` & `edc-listboard-0.1.9/edc_listboard/tests/urls.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard/view_mixins/listboard_filter_view_mixin.py` & `edc-listboard-0.1.9/edc_listboard/view_mixins/listboard_filter_view_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from edc_dashboard import url_names
 
 from ..filters import ListboardViewFilters
 
 
 class ListboardFilterViewMixin:
-
     listboard_view_filters = ListboardViewFilters()
     listboard_filter_url = None
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.listboard_view_exclude_filter_applied = False
         self.listboard_view_include_filter_applied = False
```

### Comparing `edc-listboard-0.1.8/edc_listboard/view_mixins/querystring_view_mixin.py` & `edc-listboard-0.1.9/edc_listboard/view_mixins/querystring_view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard/view_mixins/search_form_view_mixin.py` & `edc-listboard-0.1.9/edc_listboard/view_mixins/search_form_view_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 
 class SearchFormViewError(Exception):
     pass
 
 
 class SearchFormViewMixin:
-
     search_form_url = None
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context.update(search_form_url_reversed=self.search_form_url_reversed)
         return context
```

### Comparing `edc-listboard-0.1.8/edc_listboard/view_mixins/search_listboard_view_mixin.py` & `edc-listboard-0.1.9/edc_listboard/view_mixins/search_listboard_view_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django.db.models import Q
 from django.utils.html import escape
 from django.utils.text import slugify
 
 
 class SearchListboardMixin:
-
     search_fields = ["slug"]
 
     default_querystring_attrs = "q"
     alternate_search_attr = "subject_identifier"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `edc-listboard-0.1.8/edc_listboard/views/listboard_view.py` & `edc-listboard-0.1.9/edc_listboard/views/listboard_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 
 class ListboardViewError(Exception):
     pass
 
 
 class BaseListboardView(TemplateRequestContextMixin, ListView):
-
     cleaned_search_term: str | None = None
     context_object_name: str = "results"
     empty_queryset_message: str = _("Nothing to display.")
     listboard_template: str | None = None  # an existing key in request.context_data
     # if self.listboard_url declared through another mixin.
     listboard_url: str | None = None  # an existing key in request.context_data
     listboard_back_url: str | None = None
```

### Comparing `edc-listboard-0.1.8/edc_listboard/views/screen/listboard_view_filter.py` & `edc-listboard-0.1.9/edc_listboard/views/screen/listboard_view_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from ...filters import ListboardFilter
 from ...filters import ListboardViewFilters as Base
 
 
 class ScreeningListboardViewFilters(Base):
-
     all = ListboardFilter(name="all", label="All", lookup={})
 
     eligible = ListboardFilter(label="Eligible", position=10, lookup={"eligible": True})
 
     not_eligible = ListboardFilter(
         label="Not Eligible", position=11, lookup={"eligible": False}
     )
```

### Comparing `edc-listboard-0.1.8/edc_listboard/views/screen/screening_listboard_view.py` & `edc-listboard-0.1.9/edc_listboard/views/screen/screening_listboard_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 class ScreeningListboardView(
     EdcViewMixin,
     NavbarViewMixin,
     ListboardFilterViewMixin,
     SearchFormViewMixin,
     ListboardView,
 ):
-
     listboard_model = get_subject_screening_model()
     model_wrapper_cls = SubjectScreeningModelWrapper
     listboard_view_filters = ScreeningListboardViewFilters()
 
     listboard_template = "screening_listboard_template"
     listboard_url = "screening_listboard_url"
     listboard_panel_style = "info"
```

### Comparing `edc-listboard-0.1.8/edc_listboard/views/subject/subject_listboard_view.py` & `edc-listboard-0.1.9/edc_listboard/views/subject/subject_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/edc_listboard.egg-info/PKG-INFO` & `edc-listboard-0.1.9/edc_listboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-listboard
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes for Listboard views in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-listboard
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc listboard,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
@@ -12,14 +12,14 @@
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 # edc-listboard
 Listboard class for edc
```

### Comparing `edc-listboard-0.1.8/edc_listboard.egg-info/SOURCES.txt` & `edc-listboard-0.1.9/edc_listboard.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

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
 edc_listboard/__init__.py
 edc_listboard/apps.py
```

### Comparing `edc-listboard-0.1.8/pyproject.toml` & `edc-listboard-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,36 +32,39 @@
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
     pip install -U pip coverage[toml]
     pip --version
     pip freeze
     coverage run -a runtests.py
```

### Comparing `edc-listboard-0.1.8/runtests.py` & `edc-listboard-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.8/setup.cfg` & `edc-listboard-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
-python_requires = >=3.9
+python_requires = >=3.10
 zip_safe = False
 include_package_data = True
 packages = find:
 
 [options.packages.find]
 exclude = 
 	examples*
```

