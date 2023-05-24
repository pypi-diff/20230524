# Comparing `tmp/edc-lab-dashboard-0.3.8.tar.gz` & `tmp/edc-lab-dashboard-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-lab-dashboard-0.3.8.tar", last modified: Thu Aug 25 03:22:28 2022, max compression
+gzip compressed data, was "edc-lab-dashboard-0.3.9.tar", last modified: Fri Aug 26 01:58:37 2022, max compression
```

## Comparing `edc-lab-dashboard-0.3.8.tar` & `edc-lab-dashboard-0.3.9.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.024453 edc-lab-dashboard-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      110 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:27.998392 edc-lab-dashboard-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.002922 edc-lab-dashboard-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1406 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:27:47.000000 edc-lab-dashboard-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1627 2022-08-25 03:22:28.024585 edc-lab-dashboard-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      633 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.006267 edc-lab-dashboard-0.3.8/edc_lab_dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      406 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1056 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      861 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1495 2021-01-25 00:37:24.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/dashboard_templates.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1918 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/dashboard_urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1332 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/middleware.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.007245 edc-lab-dashboard-0.3.8/edc_lab_dashboard/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     3631 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.008951 edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      862 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/aliquot_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      557 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/base_box_item_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      284 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/box_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      200 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/manage_box_item_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/manifest_item_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/manifest_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      711 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/requisition_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      186 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/result_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      307 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/verify_box_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      287 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2069 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/navbars.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:27.998714 edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.009085 edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)     7990 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/beep-03.mp3
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.009360 edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/css/
--rw-r--r--   0 erikvw     (501) staff       (20)      153 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/css/extra.css
--rw-r--r--   0 erikvw     (501) staff       (20)      395 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/css/print.css
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.009622 edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/images/
--rw-r--r--   0 erikvw     (501) staff       (20)      354 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/images/checked.png
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/images/unchecked.png
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.009753 edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/js/
--rw-r--r--   0 erikvw     (501) staff       (20)     4493 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/js/beep.js
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:27.998980 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:27.999018 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.012445 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/action_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)      603 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/aliquot_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)      514 2021-01-25 00:37:24.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/base.html
--rw-r--r--   0 erikvw     (501) staff       (20)      945 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/base_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1541 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/box_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1403 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/home.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.012582 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.012995 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/aliquot/
--rw-r--r--   0 erikvw     (501) staff       (20)     2381 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/aliquot/columns.html
--rw-r--r--   0 erikvw     (501) staff       (20)      295 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/aliquot/results_body.html
--rw-r--r--   0 erikvw     (501) staff       (20)      176 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/aliquot/results_header.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.013508 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/
--rw-r--r--   0 erikvw     (501) staff       (20)      755 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/box_cell.html
--rw-r--r--   0 erikvw     (501) staff       (20)      737 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/columns.html
--rw-r--r--   0 erikvw     (501) staff       (20)      192 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/results_body.html
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/results_header.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1088 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manage_manifest_listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.013896 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manifest/
--rw-r--r--   0 erikvw     (501) staff       (20)     1632 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manifest/columns.html
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manifest/results_body.html
--rw-r--r--   0 erikvw     (501) staff       (20)      199 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manifest/results_header.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.014284 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/pack/
--rw-r--r--   0 erikvw     (501) staff       (20)     1479 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/pack/columns.html
--rw-r--r--   0 erikvw     (501) staff       (20)      292 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/pack/results_body.html
--rw-r--r--   0 erikvw     (501) staff       (20)      191 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/pack/results_header.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.014679 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/requisition/
--rw-r--r--   0 erikvw     (501) staff       (20)     1529 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/requisition/columns.html
--rw-r--r--   0 erikvw     (501) staff       (20)      295 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/requisition/results_body.html
--rw-r--r--   0 erikvw     (501) staff       (20)      216 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/requisition/results_header.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.015067 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/result/
--rw-r--r--   0 erikvw     (501) staff       (20)      802 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/result/columns.html
--rw-r--r--   0 erikvw     (501) staff       (20)      294 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/result/results_body.html
--rw-r--r--   0 erikvw     (501) staff       (20)      171 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/result/results_header.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.015202 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/tags/
--rw-r--r--   0 erikvw     (501) staff       (20)      321 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/tags/status_column.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2387 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1878 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manage_box_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2878 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manage_manifest_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1213 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manifest_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)      894 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/pack_aliquots_modal.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2412 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/pack_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)      264 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/process_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)      834 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/receive_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)      828 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/requisition_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)      323 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/result_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2239 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/verify_box_listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.015411 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2949 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/templatetags/edc_lab_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.015610 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.016790 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.017690 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3005 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/test_aliquot_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1620 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/test_box_model_wrappers.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3557 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/test_model_wrappers.py
--rw-r--r--   0 erikvw     (501) staff       (20)      654 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/test_templatetags.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6946 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/test_urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      808 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5629 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.018803 edc-lab-dashboard-0.3.8/edc_lab_dashboard/view_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      282 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/view_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4639 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/view_mixins/box_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      494 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/view_mixins/clean_search_term_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1043 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/view_mixins/form_action_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3865 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/view_mixins/manifest_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2533 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/view_mixins/process_requisition_view_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.019065 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      541 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.022004 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/
--rw-r--r--   0 erikvw     (501) staff       (20)      389 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2215 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/action_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1108 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/aliquot_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      172 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/box_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4942 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/manage_box_item_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2544 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/manage_manifest_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3054 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/manifest_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4078 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/pack_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      742 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/process_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1945 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/receive_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2517 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/requisition_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2636 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/verify_box_item_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      390 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/home_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.022586 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_filters/
--rw-r--r--   0 erikvw     (501) staff       (20)      282 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_filters/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      809 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_filters/aliquot_listboard_view_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)      523 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_filters/manifest_listboard_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)      842 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_filters/pack_listboard_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)      895 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_filters/requisition_listboard_view_filters.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.024285 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/
--rw-r--r--   0 erikvw     (501) staff       (20)      597 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      771 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/aliquot_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      476 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/base_box_item_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      467 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/base_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1286 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/manage_box_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1145 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/manage_manifest_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1746 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/manifest_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1364 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/pack_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1404 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/process_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1419 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/receive_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2457 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/requisition_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      622 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/result_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1934 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/verify_box_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      178 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard/wsgi.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:28.007026 edc-lab-dashboard-0.3.8/edc_lab_dashboard.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1627 2022-08-25 03:22:27.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     8168 2022-08-25 03:22:27.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-25 03:22:27.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:27:47.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       18 2022-08-25 03:22:27.000000 edc-lab-dashboard-0.3.8/edc_lab_dashboard.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1736 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2079 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1263 2022-08-25 03:22:28.024925 edc-lab-dashboard-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.835180 edc-lab-dashboard-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      110 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.809835 edc-lab-dashboard-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.814768 edc-lab-dashboard-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1406 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:27:47.000000 edc-lab-dashboard-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1627 2022-08-26 01:58:37.835325 edc-lab-dashboard-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      633 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-26 01:58:30.000000 edc-lab-dashboard-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.817009 edc-lab-dashboard-0.3.9/edc_lab_dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      406 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1056 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      862 2022-08-26 01:58:30.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1495 2021-01-25 00:37:24.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/dashboard_templates.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1918 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/dashboard_urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1332 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/middleware.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.817945 edc-lab-dashboard-0.3.9/edc_lab_dashboard/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     3631 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.819497 edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      862 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/aliquot_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      557 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/base_box_item_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      284 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/box_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      200 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/manage_box_item_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/manifest_item_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/manifest_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      711 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/requisition_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      186 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/result_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      307 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/verify_box_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      287 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2069 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/navbars.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.810167 edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.819627 edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)     7990 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/beep-03.mp3
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.819941 edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/css/
+-rw-r--r--   0 erikvw     (501) staff       (20)      153 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/css/extra.css
+-rw-r--r--   0 erikvw     (501) staff       (20)      395 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/css/print.css
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.820212 edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/images/
+-rw-r--r--   0 erikvw     (501) staff       (20)      354 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/images/checked.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/images/unchecked.png
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.820354 edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/js/
+-rw-r--r--   0 erikvw     (501) staff       (20)     4493 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/js/beep.js
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.810432 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.810471 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.823235 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/action_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      603 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/aliquot_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      514 2021-01-25 00:37:24.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/base.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      945 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/base_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1541 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/box_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1403 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/home.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.823427 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.823923 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/aliquot/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2381 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/aliquot/columns.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      295 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/aliquot/results_body.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      176 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/aliquot/results_header.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.824551 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/
+-rw-r--r--   0 erikvw     (501) staff       (20)      755 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/box_cell.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      737 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/columns.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      192 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/results_body.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/results_header.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1088 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manage_manifest_listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.825047 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manifest/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1632 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manifest/columns.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manifest/results_body.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      199 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manifest/results_header.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.825438 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/pack/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1479 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/pack/columns.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      292 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/pack/results_body.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      191 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/pack/results_header.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.825825 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/requisition/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1529 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/requisition/columns.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      295 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/requisition/results_body.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      216 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/requisition/results_header.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.826205 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/result/
+-rw-r--r--   0 erikvw     (501) staff       (20)      802 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/result/columns.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      294 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/result/results_body.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      171 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/result/results_header.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.826335 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/tags/
+-rw-r--r--   0 erikvw     (501) staff       (20)      321 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/tags/status_column.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2387 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1878 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manage_box_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2878 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manage_manifest_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1213 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manifest_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      894 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/pack_aliquots_modal.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2412 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/pack_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      264 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/process_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      834 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/receive_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      828 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/requisition_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      323 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/result_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2239 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/verify_box_listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.826542 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2949 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/templatetags/edc_lab_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.826753 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.827951 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.828833 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3005 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/test_aliquot_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1620 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/test_box_model_wrappers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3557 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/test_model_wrappers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      654 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/test_templatetags.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6946 2022-06-23 21:07:38.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/test_urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      808 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5629 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.829819 edc-lab-dashboard-0.3.9/edc_lab_dashboard/view_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      282 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/view_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4639 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/view_mixins/box_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      494 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/view_mixins/clean_search_term_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1043 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/view_mixins/form_action_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3865 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/view_mixins/manifest_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2533 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/view_mixins/process_requisition_view_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.830061 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      541 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.831952 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      389 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2215 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/action_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1108 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/aliquot_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      172 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/box_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4942 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/manage_box_item_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2544 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/manage_manifest_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3054 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/manifest_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4078 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/pack_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      742 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/process_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1945 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/receive_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2517 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/requisition_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2636 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/verify_box_item_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      390 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/home_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.832780 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_filters/
+-rw-r--r--   0 erikvw     (501) staff       (20)      282 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_filters/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      809 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_filters/aliquot_listboard_view_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      523 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_filters/manifest_listboard_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      842 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_filters/pack_listboard_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      895 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_filters/requisition_listboard_view_filters.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.834940 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      597 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      771 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/aliquot_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      476 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/base_box_item_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      467 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/base_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1286 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/manage_box_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1145 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/manage_manifest_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1746 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/manifest_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1364 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/pack_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1404 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/process_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1419 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/receive_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2457 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/requisition_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      622 2022-08-25 03:22:19.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/result_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1934 2021-02-08 17:31:26.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/verify_box_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      178 2020-03-04 23:28:35.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard/wsgi.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 01:58:37.817699 edc-lab-dashboard-0.3.9/edc_lab_dashboard.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1627 2022-08-26 01:58:37.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     8168 2022-08-26 01:58:37.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-26 01:58:37.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:27:47.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       18 2022-08-26 01:58:37.000000 edc-lab-dashboard-0.3.9/edc_lab_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1736 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2079 2022-08-10 11:44:04.000000 edc-lab-dashboard-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1263 2022-08-26 01:58:37.835708 edc-lab-dashboard-0.3.9/setup.cfg
```

### Comparing `edc-lab-dashboard-0.3.8/.github/workflows/build.yml` & `edc-lab-dashboard-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/.gitignore` & `edc-lab-dashboard-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/.pre-commit-config.yaml` & `edc-lab-dashboard-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/LICENSE` & `edc-lab-dashboard-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/PKG-INFO` & `edc-lab-dashboard-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-lab-dashboard
-Version: 0.3.8
+Version: 0.3.9
 Summary: Lab dashboard views for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-lab-dashboard
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc lab dashboard,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-lab-dashboard-0.3.8/README.rst` & `edc-lab-dashboard-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/auth_objects.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/auths.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/auths.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     lab_navbar_tuples,
 )
 
 site_auths.add_post_update_func(
     "edc_lab_dashboard", remove_default_model_permissions_from_edc_permissions
 )
 
-site_auths.update_group(*lab_dashboard_codenames, *lab_navbar_codenames, name=LAB)
-site_auths.update_group(*lab_dashboard_codenames, *lab_navbar_codenames, name=LAB_VIEW)
 site_auths.add_custom_permissions_tuples(
-    model="edc_lab_dashboard.edcpermissions", codename_tuples=lab_dashboard_tuples
+    model="edc_lab_dashboard.edcpermissions", codename_tuples=lab_navbar_tuples
 )
 site_auths.add_custom_permissions_tuples(
-    model="edc_lab_dashboard.edcpermissions", codename_tuples=lab_navbar_tuples
+    model="edc_lab_dashboard.edcpermissions", codename_tuples=lab_dashboard_tuples
 )
+
+site_auths.update_group(*lab_dashboard_codenames, *lab_navbar_codenames, name=LAB)
+site_auths.update_group(*lab_dashboard_codenames, *lab_navbar_codenames, name=LAB_VIEW)
```

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/dashboard_templates.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/dashboard_templates.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/dashboard_urls.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/dashboard_urls.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/middleware.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/middleware.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/migrations/0001_initial.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/aliquot_model_wrapper.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/aliquot_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/base_box_item_model_wrapper.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/base_box_item_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/manifest_item_model_wrapper.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/manifest_item_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/model_wrappers/requisition_model_wrapper.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/model_wrappers/requisition_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/navbars.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/navbars.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/beep-03.mp3` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/beep-03.mp3`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/static/edc_lab_dashboard/js/beep.js` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/static/edc_lab_dashboard/js/beep.js`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/action_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/action_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/aliquot_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/aliquot_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/base.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/base.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/base_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/base_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/box_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/box_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/home.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/home.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/aliquot/columns.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/aliquot/columns.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/box_cell.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/box_cell.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/columns.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/box/columns.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manage_manifest_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manage_manifest_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manifest/columns.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/manifest/columns.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/pack/columns.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/pack/columns.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/requisition/columns.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/requisition/columns.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/result/columns.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard/result/columns.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manage_box_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manage_box_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manage_manifest_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manage_manifest_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manifest_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/manifest_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/pack_aliquots_modal.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/pack_aliquots_modal.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/pack_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/pack_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/receive_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/receive_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/requisition_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/requisition_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/verify_box_listboard.html` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templates/edc_lab_dashboard/bootstrap3/verify_box_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/templatetags/edc_lab_extras.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/templatetags/edc_lab_extras.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/etc/user-rsa-local-private.pem` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/etc/user-rsa-restricted-private.pem` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/test_aliquot_wrapper.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/test_aliquot_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/test_box_model_wrappers.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/test_box_model_wrappers.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/test_model_wrappers.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/test_model_wrappers.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/test_templatetags.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/tests/test_urls.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/tests/urls.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/tests/urls.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/urls.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/view_mixins/box_view_mixin.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/view_mixins/box_view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/view_mixins/form_action_view_mixin.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/view_mixins/form_action_view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/view_mixins/manifest_view_mixin.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/view_mixins/manifest_view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/view_mixins/process_requisition_view_mixin.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/view_mixins/process_requisition_view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/__init__.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/action_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/action_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/aliquot_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/aliquot_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/manage_box_item_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/manage_box_item_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/manage_manifest_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/manage_manifest_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/manifest_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/manifest_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/pack_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/pack_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/process_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/process_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/receive_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/receive_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/requisition_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/requisition_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/action_views/verify_box_item_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/action_views/verify_box_item_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_filters/aliquot_listboard_view_filters.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_filters/aliquot_listboard_view_filters.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_filters/manifest_listboard_filters.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_filters/manifest_listboard_filters.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_filters/pack_listboard_filters.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_filters/pack_listboard_filters.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_filters/requisition_listboard_view_filters.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_filters/requisition_listboard_view_filters.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/__init__.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/aliquot_listboard_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/aliquot_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/manage_box_listboard_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/manage_box_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/manage_manifest_listboard_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/manage_manifest_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/manifest_listboard_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/manifest_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/pack_listboard_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/pack_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/process_listboard_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/process_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/receive_listboard_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/receive_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/requisition_listboard_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/requisition_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/result_listboard_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/result_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard/views/listboard_views/verify_box_listboard_view.py` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard/views/listboard_views/verify_box_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard.egg-info/PKG-INFO` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-lab-dashboard
-Version: 0.3.8
+Version: 0.3.9
 Summary: Lab dashboard views for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-lab-dashboard
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc lab dashboard,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-lab-dashboard-0.3.8/edc_lab_dashboard.egg-info/SOURCES.txt` & `edc-lab-dashboard-0.3.9/edc_lab_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/pyproject.toml` & `edc-lab-dashboard-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/runtests.py` & `edc-lab-dashboard-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-lab-dashboard-0.3.8/setup.cfg` & `edc-lab-dashboard-0.3.9/setup.cfg`

 * *Files identical despite different names*

