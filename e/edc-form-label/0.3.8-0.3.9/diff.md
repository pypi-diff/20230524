# Comparing `tmp/edc-form-label-0.3.8.tar.gz` & `tmp/edc-form-label-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-form-label-0.3.8.tar", last modified: Wed Oct 26 14:33:06 2022, max compression
+gzip compressed data, was "edc-form-label-0.3.9.tar", last modified: Wed May 24 17:15:14 2023, max compression
```

## Comparing `edc-form-label-0.3.8.tar` & `edc-form-label-0.3.9.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 14:33:06.197247 edc-form-label-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 18:21:41.000000 edc-form-label-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 14:33:06.188727 edc-form-label-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 14:33:06.192233 edc-form-label-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-09-08 15:10:50.000000 edc-form-label-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1142 2022-05-25 12:17:58.000000 edc-form-label-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-21 17:09:22.000000 edc-form-label-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-09-08 15:10:50.000000 edc-form-label-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 12:17:58.000000 edc-form-label-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 12:17:58.000000 edc-form-label-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-04 23:36:03.000000 edc-form-label-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       51 2020-03-04 23:36:03.000000 edc-form-label-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     3051 2022-10-26 14:33:06.197353 edc-form-label-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2177 2021-02-04 18:21:41.000000 edc-form-label-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-21 17:09:22.000000 edc-form-label-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-09-08 15:10:50.000000 edc-form-label-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 14:33:06.193545 edc-form-label-0.3.8/edc_form_label/
--rw-r--r--   0 erikvw     (501) staff       (20)      179 2021-02-04 18:21:41.000000 edc-form-label-0.3.8/edc_form_label/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      117 2020-03-04 23:36:03.000000 edc-form-label-0.3.8/edc_form_label/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2361 2022-09-21 17:09:22.000000 edc-form-label-0.3.8/edc_form_label/custom_label_condition.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1668 2022-09-08 15:10:50.000000 edc-form-label-0.3.8/edc_form_label/form_label.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1037 2022-09-08 15:10:50.000000 edc-form-label-0.3.8/edc_form_label/form_label_modeladmin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 12:17:58.000000 edc-form-label-0.3.8/edc_form_label/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 14:33:06.195437 edc-form-label-0.3.8/edc_form_label/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:36:03.000000 edc-form-label-0.3.8/edc_form_label/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1048 2021-02-04 18:21:41.000000 edc-form-label-0.3.8/edc_form_label/tests/admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 14:33:06.196779 edc-form-label-0.3.8/edc_form_label/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-13 03:05:40.000000 edc-form-label-0.3.8/edc_form_label/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-13 03:05:40.000000 edc-form-label-0.3.8/edc_form_label/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-13 03:05:40.000000 edc-form-label-0.3.8/edc_form_label/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-13 03:05:40.000000 edc-form-label-0.3.8/edc_form_label/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-13 03:05:40.000000 edc-form-label-0.3.8/edc_form_label/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-13 03:05:40.000000 edc-form-label-0.3.8/edc_form_label/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-13 03:05:40.000000 edc-form-label-0.3.8/edc_form_label/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-13 03:05:40.000000 edc-form-label-0.3.8/edc_form_label/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2020-03-04 23:36:03.000000 edc-form-label-0.3.8/edc_form_label/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1895 2022-05-25 12:17:58.000000 edc-form-label-0.3.8/edc_form_label/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     1307 2022-10-26 14:32:58.000000 edc-form-label-0.3.8/edc_form_label/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 14:33:06.196997 edc-form-label-0.3.8/edc_form_label/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-13 03:05:40.000000 edc-form-label-0.3.8/edc_form_label/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6387 2022-09-08 00:27:32.000000 edc-form-label-0.3.8/edc_form_label/tests/tests/test_form_label.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1178 2022-05-25 12:17:58.000000 edc-form-label-0.3.8/edc_form_label/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-04 23:36:03.000000 edc-form-label-0.3.8/edc_form_label/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 14:33:06.194290 edc-form-label-0.3.8/edc_form_label.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     3051 2022-10-26 14:33:06.000000 edc-form-label-0.3.8/edc_form_label.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1279 2022-10-26 14:33:06.000000 edc-form-label-0.3.8/edc_form_label.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-10-26 14:33:06.000000 edc-form-label-0.3.8/edc_form_label.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:36:03.000000 edc-form-label-0.3.8/edc_form_label.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       15 2022-10-26 14:33:06.000000 edc-form-label-0.3.8/edc_form_label.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1731 2022-09-08 15:10:50.000000 edc-form-label-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2284 2022-10-26 14:32:58.000000 edc-form-label-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1171 2022-10-26 14:33:06.197777 edc-form-label-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:15:14.381626 edc-form-label-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 18:21:41.000000 edc-form-label-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:15:14.374324 edc-form-label-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:15:14.377317 edc-form-label-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 17:15:05.000000 edc-form-label-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1142 2022-05-25 12:17:58.000000 edc-form-label-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 17:15:05.000000 edc-form-label-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-09-08 15:10:50.000000 edc-form-label-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 12:17:58.000000 edc-form-label-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 12:17:58.000000 edc-form-label-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-04 23:36:03.000000 edc-form-label-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       51 2020-03-04 23:36:03.000000 edc-form-label-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     3054 2023-05-24 17:15:14.381718 edc-form-label-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2177 2021-02-04 18:21:41.000000 edc-form-label-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-09-08 15:10:50.000000 edc-form-label-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:15:14.378322 edc-form-label-0.3.9/edc_form_label/
+-rw-r--r--   0 erikvw     (501) staff       (20)      179 2021-02-04 18:21:41.000000 edc-form-label-0.3.9/edc_form_label/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      117 2020-03-04 23:36:03.000000 edc-form-label-0.3.9/edc_form_label/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2360 2023-05-24 17:15:05.000000 edc-form-label-0.3.9/edc_form_label/custom_label_condition.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1668 2022-09-08 15:10:50.000000 edc-form-label-0.3.9/edc_form_label/form_label.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1037 2022-09-08 15:10:50.000000 edc-form-label-0.3.9/edc_form_label/form_label_modeladmin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 12:17:58.000000 edc-form-label-0.3.9/edc_form_label/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:15:14.379914 edc-form-label-0.3.9/edc_form_label/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:36:03.000000 edc-form-label-0.3.9/edc_form_label/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1048 2021-02-04 18:21:41.000000 edc-form-label-0.3.9/edc_form_label/tests/admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:15:14.381262 edc-form-label-0.3.9/edc_form_label/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-13 03:05:40.000000 edc-form-label-0.3.9/edc_form_label/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-13 03:05:40.000000 edc-form-label-0.3.9/edc_form_label/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-13 03:05:40.000000 edc-form-label-0.3.9/edc_form_label/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-13 03:05:40.000000 edc-form-label-0.3.9/edc_form_label/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-13 03:05:40.000000 edc-form-label-0.3.9/edc_form_label/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-13 03:05:40.000000 edc-form-label-0.3.9/edc_form_label/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-13 03:05:40.000000 edc-form-label-0.3.9/edc_form_label/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-13 03:05:40.000000 edc-form-label-0.3.9/edc_form_label/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2020-03-04 23:36:03.000000 edc-form-label-0.3.9/edc_form_label/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1895 2022-05-25 12:17:58.000000 edc-form-label-0.3.9/edc_form_label/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     1305 2023-05-24 17:15:05.000000 edc-form-label-0.3.9/edc_form_label/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:15:14.381500 edc-form-label-0.3.9/edc_form_label/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-13 03:05:40.000000 edc-form-label-0.3.9/edc_form_label/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6384 2023-05-24 17:15:05.000000 edc-form-label-0.3.9/edc_form_label/tests/tests/test_form_label.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1178 2022-05-25 12:17:58.000000 edc-form-label-0.3.9/edc_form_label/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-04 23:36:03.000000 edc-form-label-0.3.9/edc_form_label/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:15:14.379055 edc-form-label-0.3.9/edc_form_label.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     3054 2023-05-24 17:15:14.000000 edc-form-label-0.3.9/edc_form_label.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1271 2023-05-24 17:15:14.000000 edc-form-label-0.3.9/edc_form_label.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 17:15:14.000000 edc-form-label-0.3.9/edc_form_label.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:36:03.000000 edc-form-label-0.3.9/edc_form_label.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-05-24 17:15:14.000000 edc-form-label-0.3.9/edc_form_label.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1774 2023-05-24 17:15:05.000000 edc-form-label-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2284 2022-10-26 14:32:58.000000 edc-form-label-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1174 2023-05-24 17:15:14.382006 edc-form-label-0.3.9/setup.cfg
```

### Comparing `edc-form-label-0.3.8/.github/workflows/build.yml` & `edc-form-label-0.3.9/.github/workflows/build.yml`

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

### Comparing `edc-form-label-0.3.8/.gitignore` & `edc-form-label-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-form-label-0.3.8/.pre-commit-config.yaml` & `edc-form-label-0.3.9/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 ---
 exclude: tests/etc/user-*
 
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
-        language_version: python3.9
+        language_version: python3.10
 
   - repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: requirements-txt-fixer
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.27.1
+    rev: v1.31.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-form-label-0.3.8/LICENSE` & `edc-form-label-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-form-label-0.3.8/PKG-INFO` & `edc-form-label-0.3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-form-label
-Version: 0.3.8
+Version: 0.3.9
 Summary: Customize Django form label in realtime in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-form-label
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc modelform,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |coverage|
 
 edc-form-label
```

### Comparing `edc-form-label-0.3.8/README.rst` & `edc-form-label-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-form-label-0.3.8/edc_form_label/custom_label_condition.py` & `edc-form-label-0.3.9/edc_form_label/custom_label_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 
 class CustomFormLabelError(Exception):
     pass
 
 
 class CustomLabelCondition:
-
     appointment_model = "edc_appointment.appointment"
 
     def __init__(self, request=None, obj=None, model=None):
         self.request = request
         self.obj = obj
         self.model = model
```

### Comparing `edc-form-label-0.3.8/edc_form_label/form_label.py` & `edc-form-label-0.3.9/edc_form_label/form_label.py`

 * *Files identical despite different names*

### Comparing `edc-form-label-0.3.8/edc_form_label/form_label_modeladmin_mixin.py` & `edc-form-label-0.3.9/edc_form_label/form_label_modeladmin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-form-label-0.3.8/edc_form_label/tests/admin.py` & `edc-form-label-0.3.9/edc_form_label/tests/admin.py`

 * *Files identical despite different names*

### Comparing `edc-form-label-0.3.8/edc_form_label/tests/etc/user-rsa-local-private.pem` & `edc-form-label-0.3.9/edc_form_label/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-form-label-0.3.8/edc_form_label/tests/etc/user-rsa-restricted-private.pem` & `edc-form-label-0.3.9/edc_form_label/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-form-label-0.3.8/edc_form_label/tests/holidays.csv` & `edc-form-label-0.3.9/edc_form_label/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-form-label-0.3.8/edc_form_label/tests/models.py` & `edc-form-label-0.3.9/edc_form_label/tests/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 from edc_sites.models import SiteModelMixin
 from edc_utils import get_utcnow
 from edc_visit_schedule.model_mixins import OffScheduleModelMixin, OnScheduleModelMixin
 from edc_visit_tracking.model_mixins import VisitModelMixin
 
 
 class SubjectVisit(SiteModelMixin, VisitModelMixin, BaseUuidModel):
-
     subject_identifier = models.CharField(max_length=25)
 
     report_datetime = models.DateTimeField(default=get_utcnow)
 
     appointment = models.OneToOneField(Appointment, on_delete=PROTECT)
 
 
 class MyModel(CrfModelMixin, BaseUuidModel):
-
     subject_visit = models.OneToOneField(SubjectVisit, on_delete=PROTECT)
 
     report_datetime = models.DateTimeField(default=get_utcnow)
 
     circumcised = models.CharField(
         verbose_name="Are you circumcised?", max_length=10, choices=YES_NO
     )
```

### Comparing `edc-form-label-0.3.8/edc_form_label/tests/tests/test_form_label.py` & `edc-form-label-0.3.9/edc_form_label/tests/tests/test_form_label.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
         for field in MyModel._meta.get_fields():
             if field.name == "circumcised":
                 self.default_label = field.verbose_name
                 break
 
     def test_init(self):
-
         form_label = FormLabel(
             field="circumcised",
             custom_label="New label",
             condition_cls=CustomLabelCondition,
         )
 
         rf = RequestFactory()
@@ -136,29 +135,27 @@
             "The appointment is 2000.0. "
             "The previous appointment is 1000.0. "
             "The previous obj is None. "
             "The previous visit is 1234 1000.0.",
         )
 
     def test_custom_form_labels_default(self):
-
         for model, model_admin in admin.site._registry.items():
             if model == MyModel:
                 my_model_admin = model_admin.admin_site._registry.get(MyModel)
                 rf = RequestFactory()
                 request = rf.get(f"/?appointment={str(self.appointment_one.id)}")
                 request.user = self.user
                 rendered_change_form = my_model_admin.changeform_view(
                     request, None, "", {"subject_visit": self.subject_visit_one}
                 )
                 self.assertIn("Are you circumcised", rendered_change_form.rendered_content)
 
     @skip
     def test_custom_form_labels_2(self):
-
         MyModel.objects.create(subject_visit=self.subject_visit_one, circumcised=NO)
 
         for model, model_admin in admin.site._registry.items():
             if model == MyModel:
                 my_model_admin = model_admin.admin_site._registry.get(MyModel)
                 rf = RequestFactory()
                 request = rf.get(f"/?appointment={str(self.appointment_two.id)}")
```

### Comparing `edc-form-label-0.3.8/edc_form_label/tests/visit_schedule.py` & `edc-form-label-0.3.9/edc_form_label/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-form-label-0.3.8/edc_form_label.egg-info/PKG-INFO` & `edc-form-label-0.3.9/edc_form_label.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-form-label
-Version: 0.3.8
+Version: 0.3.9
 Summary: Customize Django form label in realtime in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-form-label
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc modelform,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |coverage|
 
 edc-form-label
```

### Comparing `edc-form-label-0.3.8/edc_form_label.egg-info/SOURCES.txt` & `edc-form-label-0.3.9/edc_form_label.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
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
 edc_form_label/__init__.py
 edc_form_label/apps.py
```

### Comparing `edc-form-label-0.3.8/pyproject.toml` & `edc-form-label-0.3.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,70 +3,72 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "_version.py"
 
 [tool.black]
 line-length = 95
-target-version = ["py39"]
+target-version = ["py310"]
 extend-exclude = '''^(.*\/)*\b(migrations)\b($|\/.*$)'''
 
 [tool.isort]
 profile = "black"
-py_version = "39"
+py_version = "310"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
 parallel = false
 branch = true
 source = ["edc_form_label"]
 
 [tool.coverage.paths]
 source = ["edc_form_label"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 omit = ["requirements.txt"]
+exclude_lines = [
+  "pragma: no cover",
+  "if TYPE_CHECKING:",
+]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{38,39,310}-dj{32,40,41,dev},
+    py{310}-dj{41,42},
+    py{311}-dj{41,42,dev},
     lint
 
 isolated_build = true
 
 [gh-actions]
 python =
-    3.8: py38
-    3.9: py39, lint
     3.10: py310
+    3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
-    3.2: dj32, lint
-    4.0: dj40
     4.1: dj41
+    4.2: dj42, lint
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
-    dj32: Django>=3.2,<3.3
-    dj40: Django>=4.0,<4.1
     dj41: Django>=4.1,<4.2
+    dj42: Django>=4.2,<5.0
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

### Comparing `edc-form-label-0.3.8/runtests.py` & `edc-form-label-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-form-label-0.3.8/setup.cfg` & `edc-form-label-0.3.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 description = Customize Django form label in realtime in clinicedc/edc projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django Edc modelform, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 3.2
+	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
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

