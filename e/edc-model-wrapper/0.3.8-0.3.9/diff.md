# Comparing `tmp/edc-model-wrapper-0.3.8.tar.gz` & `tmp/edc-model-wrapper-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-model-wrapper-0.3.8.tar", last modified: Thu Sep  8 15:11:53 2022, max compression
+gzip compressed data, was "edc-model-wrapper-0.3.9.tar", last modified: Sun Sep 25 19:34:28 2022, max compression
```

## Comparing `edc-model-wrapper-0.3.8.tar` & `edc-model-wrapper-0.3.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 15:11:53.015007 edc-model-wrapper-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      110 2020-03-04 23:12:47.000000 edc-model-wrapper-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 15:11:53.006254 edc-model-wrapper-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 15:11:53.010144 edc-model-wrapper-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-22 01:57:42.000000 edc-model-wrapper-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1203 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1075 2022-09-08 11:34:35.000000 edc-model-wrapper-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-09-08 11:34:35.000000 edc-model-wrapper-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       88 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2022-09-08 15:11:53.015123 edc-model-wrapper-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2620 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-08 15:11:43.000000 edc-model-wrapper-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-09-08 11:34:35.000000 edc-model-wrapper-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 15:11:53.011049 edc-model-wrapper-0.3.8/edc_model_wrapper/
--rw-r--r--   0 erikvw     (501) staff       (20)      181 2021-03-01 03:53:01.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      120 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 15:11:53.012241 edc-model-wrapper-0.3.8/edc_model_wrapper/parsers/
--rw-r--r--   0 erikvw     (501) staff       (20)       88 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/parsers/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1545 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/parsers/keywords.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2407 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/parsers/next_url_parser.py
--rw-r--r--   0 erikvw     (501) staff       (20)      968 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/permissions_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      525 2021-03-01 03:53:01.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/stubs.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 15:11:53.013103 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)      105 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1108 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1732 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/model_wrapper_test_helper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2245 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 15:11:53.014306 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3448 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_example_wrappers.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4978 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_example_wrappers2.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1482 2021-03-01 03:53:01.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_fields.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2461 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_keywords.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5378 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_next_url.py
--rw-r--r--   0 erikvw     (501) staff       (20)      639 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 15:11:53.014788 edc-model-wrapper-0.3.8/edc_model_wrapper/wrappers/
--rw-r--r--   0 erikvw     (501) staff       (20)      200 2021-03-01 03:53:01.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/wrappers/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1940 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/wrappers/fields.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8701 2022-09-08 11:34:35.000000 edc-model-wrapper-0.3.8/edc_model_wrapper/wrappers/model_wrapper.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 15:11:53.011745 edc-model-wrapper-0.3.8/edc_model_wrapper.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2022-09-08 15:11:52.000000 edc-model-wrapper-0.3.8/edc_model_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1346 2022-09-08 15:11:53.000000 edc-model-wrapper-0.3.8/edc_model_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-08 15:11:52.000000 edc-model-wrapper-0.3.8/edc_model_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:12:49.000000 edc-model-wrapper-0.3.8/edc_model_wrapper.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       18 2022-09-08 15:11:52.000000 edc-model-wrapper-0.3.8/edc_model_wrapper.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1736 2022-09-08 15:11:43.000000 edc-model-wrapper-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.8/requirements.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1684 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1293 2022-09-08 15:11:53.015452 edc-model-wrapper-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 19:34:28.576518 edc-model-wrapper-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      110 2020-03-04 23:12:47.000000 edc-model-wrapper-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 19:34:28.568766 edc-model-wrapper-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 19:34:28.572060 edc-model-wrapper-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-22 01:57:42.000000 edc-model-wrapper-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1203 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1075 2022-09-25 19:34:20.000000 edc-model-wrapper-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-09-08 11:34:35.000000 edc-model-wrapper-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       88 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2022-09-25 19:34:28.576654 edc-model-wrapper-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2620 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 19:34:20.000000 edc-model-wrapper-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-09-08 11:34:35.000000 edc-model-wrapper-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 19:34:28.572808 edc-model-wrapper-0.3.9/edc_model_wrapper/
+-rw-r--r--   0 erikvw     (501) staff       (20)      207 2022-09-25 19:34:20.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      120 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 19:34:28.574040 edc-model-wrapper-0.3.9/edc_model_wrapper/parsers/
+-rw-r--r--   0 erikvw     (501) staff       (20)       88 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/parsers/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1545 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/parsers/keywords.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2407 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/parsers/next_url_parser.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      976 2022-09-25 19:34:20.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/permissions_model_wrapper_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      525 2021-03-01 03:53:01.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/stubs.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 19:34:28.574868 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)      105 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1108 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1732 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/model_wrapper_test_helper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2245 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 19:34:28.576006 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3448 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_example_wrappers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4978 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_example_wrappers2.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1482 2021-03-01 03:53:01.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_fields.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2461 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_keywords.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5378 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_next_url.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      639 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 19:34:28.576427 edc-model-wrapper-0.3.9/edc_model_wrapper/wrappers/
+-rw-r--r--   0 erikvw     (501) staff       (20)      200 2021-03-01 03:53:01.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/wrappers/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1940 2022-05-03 02:58:58.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/wrappers/fields.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9535 2022-09-25 19:34:20.000000 edc-model-wrapper-0.3.9/edc_model_wrapper/wrappers/model_wrapper.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 19:34:28.573473 edc-model-wrapper-0.3.9/edc_model_wrapper.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2022-09-25 19:34:28.000000 edc-model-wrapper-0.3.9/edc_model_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1360 2022-09-25 19:34:28.000000 edc-model-wrapper-0.3.9/edc_model_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-25 19:34:28.000000 edc-model-wrapper-0.3.9/edc_model_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:12:49.000000 edc-model-wrapper-0.3.9/edc_model_wrapper.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       18 2022-09-25 19:34:28.000000 edc-model-wrapper-0.3.9/edc_model_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1736 2022-09-08 15:11:43.000000 edc-model-wrapper-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-model-wrapper-0.3.9/requirements.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1684 2021-02-08 16:46:44.000000 edc-model-wrapper-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1293 2022-09-25 19:34:28.576968 edc-model-wrapper-0.3.9/setup.cfg
```

### Comparing `edc-model-wrapper-0.3.8/.github/workflows/build.yml` & `edc-model-wrapper-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/.gitignore` & `edc-model-wrapper-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/.pre-commit-config.yaml` & `edc-model-wrapper-0.3.9/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
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

### Comparing `edc-model-wrapper-0.3.8/LICENSE` & `edc-model-wrapper-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/PKG-INFO` & `edc-model-wrapper-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-model-wrapper
-Version: 0.3.8
+Version: 0.3.9
 Summary: Model wrappers that add dashboard methods for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-model-wrapper
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django model wrapper dashboard edc clinicedc clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-model-wrapper-0.3.8/README.rst` & `edc-model-wrapper-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/parsers/keywords.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/parsers/keywords.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/parsers/next_url_parser.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/parsers/next_url_parser.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/permissions_mixin.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/permissions_model_wrapper_mixin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from typing import Any, Optional
+from __future__ import annotations
 
+from typing import Any
 
-class PermissionsMixin:
-    def __init__(self, request: Optional[Any] = None, **kwargs):
+
+class PermissionsModelWrapperMixin:
+    def __init__(self, request: Any = None, **kwargs):
         super().__init__(**kwargs)
         self.request = request
 
     @property
-    def has_add_permission(self: Any) -> bool:
+    def has_add_permission(self) -> bool:
         app_label, model_name = self.model.split(".")
         return self.request.user.has_perm(f"{app_label}.add_{model_name}")
 
     @property
-    def has_change_permission(self: Any) -> bool:
+    def has_change_permission(self) -> bool:
         app_label, model_name = self.model.split(".")
         return self.request.user.has_perm(f"{app_label}.change_{model_name}")
 
     @property
-    def has_delete_permission(self: Any) -> bool:
+    def has_delete_permission(self) -> bool:
         app_label, model_name = self.model.split(".")
         return self.request.user.has_perm(f"{app_label}.delete_{model_name}")
 
     @property
-    def has_view_permission(self: Any) -> bool:
+    def has_view_permission(self) -> bool:
         app_label, model_name = self.model.split(".")
         return self.request.user.has_perm(f"{app_label}.view_{model_name}")
```

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/stubs.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/stubs.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/tests/admin.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/tests/admin.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/tests/model_wrapper_test_helper.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/tests/model_wrapper_test_helper.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/tests/models.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_example_wrappers.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_example_wrappers.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_example_wrappers2.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_example_wrappers2.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_fields.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_keywords.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_keywords.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_model_wrapper.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/tests/tests/test_next_url.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/tests/tests/test_next_url.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/tests/urls.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/tests/urls.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/wrappers/fields.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/wrappers/fields.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper/wrappers/model_wrapper.py` & `edc-model-wrapper-0.3.9/edc_model_wrapper/wrappers/model_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from __future__ import annotations
 
-from typing import Any, Iterator
+from typing import TYPE_CHECKING, Any, Iterator
 from urllib import parse
 
 from django.db.models import ForeignKey, ManyToManyField, OneToOneField
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from django.urls.base import reverse
 from edc_dashboard import url_names
 from edc_model.stubs import ModelMetaStub
 
 from ..parsers import Keywords, NextUrlParser
-from ..stubs import ModelStub
+
+if TYPE_CHECKING:
+    from edc_appointment.models import Appointment
+    from edc_crf.model_mixins import CrfModelMixin
+    from edc_lab.model_mixins import RequisitionModelMixin
+    from edc_model.models import BaseModel, BaseUuidModel
+    from edc_visit_tracking.model_mixins import VisitModelMixin
 
 
 class ModelWrapperError(Exception):
     pass
 
 
 class ModelWrapperModelError(Exception):
@@ -86,20 +92,41 @@
         querystring_attrs: list[str] | None = None,
         force_wrap: bool | None = None,
         **kwargs,
     ):
 
         self._querystring_attrs = querystring_attrs or self.querystring_attrs
         self.kwargs = kwargs
-        self.object: ModelStub = model_obj
+        self.object: (
+            Appointment
+            | VisitModelMixin
+            | CrfModelMixin
+            | RequisitionModelMixin
+            | BaseUuidModel
+            | BaseModel
+        ) = model_obj
         if not force_wrap:
             self._raise_if_model_obj_is_wrapped()
-        self.model_cls = model_cls or self.model_cls or self.object.__class__
-        self.model_name = self.model_cls._meta.object_name.lower().replace(" ", "_")
-        self.model = model or self.model or self.model_cls._meta.label_lower
+        self.model_cls: (
+            Appointment
+            | VisitModelMixin
+            | CrfModelMixin
+            | RequisitionModelMixin
+            | BaseUuidModel
+            | BaseModel
+        ) = (model_cls or self.model_cls or self.object.__class__)
+        self.model_name: str = self.model_cls._meta.object_name.lower().replace(" ", "_")
+        self.model: (
+            Appointment
+            | VisitModelMixin
+            | CrfModelMixin
+            | RequisitionModelMixin
+            | BaseUuidModel
+            | BaseModel
+        ) = (model or self.model or self.model_cls._meta.label_lower)
         if not isinstance(self.object, self.model_cls):
             raise ModelWrapperModelError(
                 f"Expected an instance of {self.model}. " f"Got model_obj={repr(self.object)}"
             )
         if self.model != self.model_cls._meta.label_lower:
             raise ModelWrapperModelError(
                 f"Wrapper is for model {self.model}. "
```

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper.egg-info/PKG-INFO` & `edc-model-wrapper-0.3.9/edc_model_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-model-wrapper
-Version: 0.3.8
+Version: 0.3.9
 Summary: Model wrappers that add dashboard methods for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-model-wrapper
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django model wrapper dashboard edc clinicedc clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-model-wrapper-0.3.8/edc_model_wrapper.egg-info/SOURCES.txt` & `edc-model-wrapper-0.3.9/edc_model_wrapper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 requirements.txt
 runtests.py
 setup.cfg
 .github/workflows/build.yml
 edc_model_wrapper/__init__.py
 edc_model_wrapper/apps.py
 edc_model_wrapper/models.py
-edc_model_wrapper/permissions_mixin.py
+edc_model_wrapper/permissions_model_wrapper_mixin.py
 edc_model_wrapper/stubs.py
 edc_model_wrapper.egg-info/PKG-INFO
 edc_model_wrapper.egg-info/SOURCES.txt
 edc_model_wrapper.egg-info/dependency_links.txt
 edc_model_wrapper.egg-info/not-zip-safe
 edc_model_wrapper.egg-info/top_level.txt
 edc_model_wrapper/parsers/__init__.py
```

### Comparing `edc-model-wrapper-0.3.8/pyproject.toml` & `edc-model-wrapper-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/runtests.py` & `edc-model-wrapper-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-model-wrapper-0.3.8/setup.cfg` & `edc-model-wrapper-0.3.9/setup.cfg`

 * *Files identical despite different names*

