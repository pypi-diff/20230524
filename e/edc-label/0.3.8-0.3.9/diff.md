# Comparing `tmp/edc-label-0.3.8.tar.gz` & `tmp/edc-label-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-label-0.3.8.tar", last modified: Wed May 25 18:35:05 2022, max compression
+gzip compressed data, was "edc-label-0.3.9.tar", last modified: Wed May 25 19:04:28 2022, max compression
```

## Comparing `edc-label-0.3.8.tar` & `edc-label-0.3.9.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.857888 edc-label-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      107 2020-03-04 23:38:10.000000 edc-label-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 17:34:32.000000 edc-label-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.846070 edc-label-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.849496 edc-label-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-19 02:12:43.000000 edc-label-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1407 2022-05-25 13:58:13.000000 edc-label-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:58:13.000000 edc-label-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:58:13.000000 edc-label-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:37:31.000000 edc-label-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2022-05-25 13:58:13.000000 edc-label-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     3470 2022-05-25 18:35:05.858039 edc-label-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2663 2021-02-08 17:34:32.000000 edc-label-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-05-25 18:34:57.000000 edc-label-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-08 17:34:32.000000 edc-label-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.852552 edc-label-0.3.8/edc_label/
--rw-r--r--   0 erikvw     (501) staff       (20)      254 2021-02-08 17:34:32.000000 edc-label-0.3.8/edc_label/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      444 2021-10-12 04:37:08.000000 edc-label-0.3.8/edc_label/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2021-10-12 04:37:08.000000 edc-label-0.3.8/edc_label/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-25 13:58:13.000000 edc-label-0.3.8/edc_label/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      482 2021-10-12 04:37:08.000000 edc-label-0.3.8/edc_label/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      156 2021-10-12 04:37:08.000000 edc-label-0.3.8/edc_label/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      273 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1220 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/job_result.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1548 2021-02-08 17:34:32.000000 edc-label-0.3.8/edc_label/lab_printers_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1506 2021-10-26 13:17:33.000000 edc-label-0.3.8/edc_label/label.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1926 2021-10-26 13:17:33.000000 edc-label-0.3.8/edc_label/label_template.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.853635 edc-label-0.3.8/edc_label/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     2644 2021-10-12 04:37:08.000000 edc-label-0.3.8/edc_label/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-10-12 04:37:08.000000 edc-label-0.3.8/edc_label/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      395 2021-10-12 04:37:08.000000 edc-label-0.3.8/edc_label/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      316 2021-02-08 17:34:32.000000 edc-label-0.3.8/edc_label/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2844 2021-02-08 17:34:32.000000 edc-label-0.3.8/edc_label/printer.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3802 2021-02-08 17:34:32.000000 edc-label-0.3.8/edc_label/printers_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.846337 edc-label-0.3.8/edc_label/static/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.853719 edc-label-0.3.8/edc_label/static/edc_label/
--rw-r--r--   0 erikvw     (501) staff       (20)     8196 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/static/edc_label/.DS_Store
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.853993 edc-label-0.3.8/edc_label/static/edc_label/js/
--rw-r--r--   0 erikvw     (501) staff       (20)     6972 2021-10-12 03:30:55.000000 edc-label-0.3.8/edc_label/static/edc_label/js/BrowserPrint-3.0.216.min.js
--rw-r--r--   0 erikvw     (501) staff       (20)     3932 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/static/edc_label/js/edc_label.js
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.854510 edc-label-0.3.8/edc_label/static/edc_label/label_templates/
--rw-r--r--   0 erikvw     (501) staff       (20)      406 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/static/edc_label/label_templates/aliquot.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      297 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/static/edc_label/label_templates/box.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      294 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/static/edc_label/label_templates/manifest.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      410 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/static/edc_label/label_templates/requisition.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)     1579 2021-10-26 13:17:33.000000 edc-label-0.3.8/edc_label/subject_label.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.846632 edc-label-0.3.8/edc_label/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.854728 edc-label-0.3.8/edc_label/templates/edc_label/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.855248 edc-label-0.3.8/edc_label/templates/edc_label/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      951 2021-10-12 04:37:08.000000 edc-label-0.3.8/edc_label/templates/edc_label/bootstrap3/home.html
--rw-r--r--   0 erikvw     (501) staff       (20)      509 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/templates/edc_label/bootstrap3/print_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2523 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/templates/edc_label/bootstrap3/printer_config.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1601 2021-10-12 04:37:08.000000 edc-label-0.3.8/edc_label/templates/edc_label/bootstrap3/printer_setup.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1426 2021-10-13 01:46:55.000000 edc-label-0.3.8/edc_label/templates/edc_label/browser_print_labels.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.855449 edc-label-0.3.8/edc_label/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      764 2021-02-08 17:34:32.000000 edc-label-0.3.8/edc_label/templatetags/edc_label_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.855662 edc-label-0.3.8/edc_label/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:38:10.000000 edc-label-0.3.8/edc_label/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.855831 edc-label-0.3.8/edc_label/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-08 17:34:32.000000 edc-label-0.3.8/edc_label/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1150 2022-05-25 13:58:13.000000 edc-label-0.3.8/edc_label/tests/tests/test_label.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1646 2022-05-25 13:58:13.000000 edc-label-0.3.8/edc_label/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1301 2021-02-08 17:34:32.000000 edc-label-0.3.8/edc_label/view_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.856947 edc-label-0.3.8/edc_label/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      190 2021-10-12 03:30:55.000000 edc-label-0.3.8/edc_label/views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      698 2022-05-25 13:58:13.000000 edc-label-0.3.8/edc_label/views/browser_print_labels_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1817 2021-02-08 17:34:32.000000 edc-label-0.3.8/edc_label/views/change_printer_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      745 2022-05-25 13:58:13.000000 edc-label-0.3.8/edc_label/views/home_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1360 2021-02-08 17:34:32.000000 edc-label-0.3.8/edc_label/views/print_label_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1022 2021-10-12 04:37:08.000000 edc-label-0.3.8/edc_label/views/print_setup_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.853401 edc-label-0.3.8/edc_label.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     3470 2022-05-25 18:35:05.000000 edc-label-0.3.8/edc_label.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1964 2022-05-25 18:35:05.000000 edc-label-0.3.8/edc_label.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-25 18:35:05.000000 edc-label-0.3.8/edc_label.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-25 14:03:58.000000 edc-label-0.3.8/edc_label.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       10 2022-05-25 18:35:05.000000 edc-label-0.3.8/edc_label.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:35:05.857765 edc-label-0.3.8/label_templates/
--rw-r--r--   0 erikvw     (501) staff       (20)      406 2020-03-04 23:38:10.000000 edc-label-0.3.8/label_templates/aliquot.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      297 2020-03-04 23:38:10.000000 edc-label-0.3.8/label_templates/box.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      294 2020-03-04 23:38:10.000000 edc-label-0.3.8/label_templates/manifest.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      387 2020-03-04 23:38:10.000000 edc-label-0.3.8/label_templates/requisition.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)     1579 2022-05-25 13:58:13.000000 edc-label-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1461 2021-09-12 16:58:32.000000 edc-label-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1127 2022-05-25 18:35:05.858435 edc-label-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.343619 edc-label-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      107 2020-03-04 23:38:10.000000 edc-label-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 17:34:32.000000 edc-label-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.331192 edc-label-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.334910 edc-label-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-19 02:12:43.000000 edc-label-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1407 2022-05-25 13:58:13.000000 edc-label-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:58:13.000000 edc-label-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:58:13.000000 edc-label-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:37:31.000000 edc-label-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2022-05-25 13:58:13.000000 edc-label-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     3470 2022-05-25 19:04:28.343732 edc-label-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2663 2021-02-08 17:34:32.000000 edc-label-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-05-25 19:04:17.000000 edc-label-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-08 17:34:32.000000 edc-label-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.337999 edc-label-0.3.9/edc_label/
+-rw-r--r--   0 erikvw     (501) staff       (20)      254 2021-02-08 17:34:32.000000 edc-label-0.3.9/edc_label/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      444 2021-10-12 04:37:08.000000 edc-label-0.3.9/edc_label/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2021-10-12 04:37:08.000000 edc-label-0.3.9/edc_label/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-25 13:58:13.000000 edc-label-0.3.9/edc_label/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      482 2021-10-12 04:37:08.000000 edc-label-0.3.9/edc_label/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      156 2021-10-12 04:37:08.000000 edc-label-0.3.9/edc_label/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      273 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1220 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/job_result.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1548 2021-02-08 17:34:32.000000 edc-label-0.3.9/edc_label/lab_printers_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1506 2021-10-26 13:17:33.000000 edc-label-0.3.9/edc_label/label.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1926 2021-10-26 13:17:33.000000 edc-label-0.3.9/edc_label/label_template.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.339044 edc-label-0.3.9/edc_label/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2644 2021-10-12 04:37:08.000000 edc-label-0.3.9/edc_label/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-10-12 04:37:08.000000 edc-label-0.3.9/edc_label/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      395 2021-10-12 04:37:08.000000 edc-label-0.3.9/edc_label/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      316 2021-02-08 17:34:32.000000 edc-label-0.3.9/edc_label/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2844 2021-02-08 17:34:32.000000 edc-label-0.3.9/edc_label/printer.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3802 2021-02-08 17:34:32.000000 edc-label-0.3.9/edc_label/printers_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.331474 edc-label-0.3.9/edc_label/static/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.339125 edc-label-0.3.9/edc_label/static/edc_label/
+-rw-r--r--   0 erikvw     (501) staff       (20)     8196 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/static/edc_label/.DS_Store
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.339399 edc-label-0.3.9/edc_label/static/edc_label/js/
+-rw-r--r--   0 erikvw     (501) staff       (20)     6972 2021-10-12 03:30:55.000000 edc-label-0.3.9/edc_label/static/edc_label/js/BrowserPrint-3.0.216.min.js
+-rw-r--r--   0 erikvw     (501) staff       (20)     3932 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/static/edc_label/js/edc_label.js
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.339930 edc-label-0.3.9/edc_label/static/edc_label/label_templates/
+-rw-r--r--   0 erikvw     (501) staff       (20)      406 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/static/edc_label/label_templates/aliquot.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      297 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/static/edc_label/label_templates/box.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      294 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/static/edc_label/label_templates/manifest.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      410 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/static/edc_label/label_templates/requisition.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)     1579 2021-10-26 13:17:33.000000 edc-label-0.3.9/edc_label/subject_label.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.331697 edc-label-0.3.9/edc_label/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.340163 edc-label-0.3.9/edc_label/templates/edc_label/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.340816 edc-label-0.3.9/edc_label/templates/edc_label/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      951 2021-10-12 04:37:08.000000 edc-label-0.3.9/edc_label/templates/edc_label/bootstrap3/home.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      509 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/templates/edc_label/bootstrap3/print_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2523 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/templates/edc_label/bootstrap3/printer_config.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1601 2021-10-12 04:37:08.000000 edc-label-0.3.9/edc_label/templates/edc_label/bootstrap3/printer_setup.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1426 2021-10-13 01:46:55.000000 edc-label-0.3.9/edc_label/templates/edc_label/browser_print_labels.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.341057 edc-label-0.3.9/edc_label/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      764 2021-02-08 17:34:32.000000 edc-label-0.3.9/edc_label/templatetags/edc_label_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.341307 edc-label-0.3.9/edc_label/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:38:10.000000 edc-label-0.3.9/edc_label/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.341491 edc-label-0.3.9/edc_label/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-08 17:34:32.000000 edc-label-0.3.9/edc_label/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1150 2022-05-25 13:58:13.000000 edc-label-0.3.9/edc_label/tests/tests/test_label.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1646 2022-05-25 13:58:13.000000 edc-label-0.3.9/edc_label/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1301 2021-02-08 17:34:32.000000 edc-label-0.3.9/edc_label/view_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.342680 edc-label-0.3.9/edc_label/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      190 2021-10-12 03:30:55.000000 edc-label-0.3.9/edc_label/views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      698 2022-05-25 13:58:13.000000 edc-label-0.3.9/edc_label/views/browser_print_labels_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1817 2021-02-08 17:34:32.000000 edc-label-0.3.9/edc_label/views/change_printer_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      745 2022-05-25 13:58:13.000000 edc-label-0.3.9/edc_label/views/home_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1360 2021-02-08 17:34:32.000000 edc-label-0.3.9/edc_label/views/print_label_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1022 2021-10-12 04:37:08.000000 edc-label-0.3.9/edc_label/views/print_setup_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.338823 edc-label-0.3.9/edc_label.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     3470 2022-05-25 19:04:28.000000 edc-label-0.3.9/edc_label.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1996 2022-05-25 19:04:28.000000 edc-label-0.3.9/edc_label.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-25 19:04:28.000000 edc-label-0.3.9/edc_label.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-25 14:03:58.000000 edc-label-0.3.9/edc_label.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        7 2022-05-25 19:04:28.000000 edc-label-0.3.9/edc_label.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       10 2022-05-25 19:04:28.000000 edc-label-0.3.9/edc_label.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 19:04:28.343503 edc-label-0.3.9/label_templates/
+-rw-r--r--   0 erikvw     (501) staff       (20)      406 2020-03-04 23:38:10.000000 edc-label-0.3.9/label_templates/aliquot.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      297 2020-03-04 23:38:10.000000 edc-label-0.3.9/label_templates/box.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      294 2020-03-04 23:38:10.000000 edc-label-0.3.9/label_templates/manifest.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      387 2020-03-04 23:38:10.000000 edc-label-0.3.9/label_templates/requisition.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)     1579 2022-05-25 13:58:13.000000 edc-label-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1461 2021-09-12 16:58:32.000000 edc-label-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1127 2022-05-25 19:04:28.344067 edc-label-0.3.9/setup.cfg
```

### Comparing `edc-label-0.3.8/.github/workflows/build.yml` & `edc-label-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/.gitignore` & `edc-label-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/LICENSE` & `edc-label-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/PKG-INFO` & `edc-label-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-label
-Version: 0.3.8
+Version: 0.3.9
 Summary: Labeling
 Home-page: https://github.com/clinicedc/edc-label
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc labelling,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-label-0.3.8/README.rst` & `edc-label-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/apps.py` & `edc-label-0.3.9/edc_label/apps.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/job_result.py` & `edc-label-0.3.9/edc_label/job_result.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/lab_printers_mixin.py` & `edc-label-0.3.9/edc_label/lab_printers_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/label.py` & `edc-label-0.3.9/edc_label/label.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/label_template.py` & `edc-label-0.3.9/edc_label/label_template.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/migrations/0001_initial.py` & `edc-label-0.3.9/edc_label/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/printer.py` & `edc-label-0.3.9/edc_label/printer.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/printers_mixin.py` & `edc-label-0.3.9/edc_label/printers_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/static/edc_label/.DS_Store` & `edc-label-0.3.9/edc_label/static/edc_label/.DS_Store`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/static/edc_label/js/BrowserPrint-3.0.216.min.js` & `edc-label-0.3.9/edc_label/static/edc_label/js/BrowserPrint-3.0.216.min.js`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/static/edc_label/js/edc_label.js` & `edc-label-0.3.9/edc_label/static/edc_label/js/edc_label.js`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/subject_label.py` & `edc-label-0.3.9/edc_label/subject_label.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/templates/edc_label/bootstrap3/home.html` & `edc-label-0.3.9/edc_label/templates/edc_label/bootstrap3/home.html`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/templates/edc_label/bootstrap3/printer_config.html` & `edc-label-0.3.9/edc_label/templates/edc_label/bootstrap3/printer_config.html`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/templates/edc_label/bootstrap3/printer_setup.html` & `edc-label-0.3.9/edc_label/templates/edc_label/bootstrap3/printer_setup.html`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/templates/edc_label/browser_print_labels.html` & `edc-label-0.3.9/edc_label/templates/edc_label/browser_print_labels.html`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/templatetags/edc_label_extras.py` & `edc-label-0.3.9/edc_label/templatetags/edc_label_extras.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/tests/tests/test_label.py` & `edc-label-0.3.9/edc_label/tests/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/urls.py` & `edc-label-0.3.9/edc_label/urls.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/view_mixins.py` & `edc-label-0.3.9/edc_label/view_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/views/browser_print_labels_view.py` & `edc-label-0.3.9/edc_label/views/browser_print_labels_view.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/views/change_printer_view.py` & `edc-label-0.3.9/edc_label/views/change_printer_view.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/views/home_view.py` & `edc-label-0.3.9/edc_label/views/home_view.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/views/print_label_view.py` & `edc-label-0.3.9/edc_label/views/print_label_view.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label/views/print_setup_view.py` & `edc-label-0.3.9/edc_label/views/print_setup_view.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/edc_label.egg-info/PKG-INFO` & `edc-label-0.3.9/edc_label.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-label
-Version: 0.3.8
+Version: 0.3.9
 Summary: Labeling
 Home-page: https://github.com/clinicedc/edc-label
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc labelling,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-label-0.3.8/edc_label.egg-info/SOURCES.txt` & `edc-label-0.3.9/edc_label.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 edc_label/subject_label.py
 edc_label/urls.py
 edc_label/view_mixins.py
 edc_label.egg-info/PKG-INFO
 edc_label.egg-info/SOURCES.txt
 edc_label.egg-info/dependency_links.txt
 edc_label.egg-info/not-zip-safe
+edc_label.egg-info/requires.txt
 edc_label.egg-info/top_level.txt
 edc_label/migrations/0001_initial.py
 edc_label/migrations/__init__.py
 edc_label/static/edc_label/.DS_Store
 edc_label/static/edc_label/js/BrowserPrint-3.0.216.min.js
 edc_label/static/edc_label/js/edc_label.js
 edc_label/static/edc_label/label_templates/aliquot.lbl
```

### Comparing `edc-label-0.3.8/pyproject.toml` & `edc-label-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/runtests.py` & `edc-label-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-label-0.3.8/setup.cfg` & `edc-label-0.3.9/setup.cfg`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 author_email = ew2789@gmail.com
 url = https://github.com/clinicedc/edc-label
 license = GPL license, see LICENSE
 description = Labeling
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django Edc labelling, clinicedc, clinical trials
-install_requires = 
-	pycups
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
@@ -23,14 +21,16 @@
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
 python_requires = >=3.9
 zip_safe = False
 include_package_data = True
 packages = find:
+install_requires = 
+	pycups
 
 [options.packages.find]
 exclude = 
 	examples*
 	tools*
 	docs*
 	bin*
```

