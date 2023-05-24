# Comparing `tmp/edc-he-0.1.5.tar.gz` & `tmp/edc-he-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-he-0.1.5.tar", last modified: Wed Oct  5 19:09:09 2022, max compression
+gzip compressed data, was "edc-he-0.1.6.tar", last modified: Wed May 24 16:43:36 2023, max compression
```

## Comparing `edc-he-0.1.5.tar` & `edc-he-0.1.6.tar`

### file list

```diff
@@ -1,53 +1,52 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:09:09.914416 edc-he-0.1.5/
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2021-08-23 17:45:53.000000 edc-he-0.1.5/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-23 17:45:53.000000 edc-he-0.1.5/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:09:09.907336 edc-he-0.1.5/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:09:09.910581 edc-he-0.1.5/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 22:46:20.000000 edc-he-0.1.5/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-25 13:21:02.000000 edc-he-0.1.5/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-25 18:36:50.000000 edc-he-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 22:46:20.000000 edc-he-0.1.5/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.5/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.5/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-19 17:21:37.000000 edc-he-0.1.5/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 13:21:02.000000 edc-he-0.1.5/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1610 2022-10-05 19:09:09.914516 edc-he-0.1.5/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      641 2021-08-23 17:45:53.000000 edc-he-0.1.5/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-10-05 19:09:02.000000 edc-he-0.1.5/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-10 22:46:20.000000 edc-he-0.1.5/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:09:09.911861 edc-he-0.1.5/edc_he/
--rw-r--r--   0 erikvw     (501) staff       (20)       66 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      109 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      361 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      725 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2272 2022-05-25 13:21:02.000000 edc-he-0.1.5/edc_he/form_validators.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:09:09.912575 edc-he-0.1.5/edc_he/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2175 2021-09-12 23:29:21.000000 edc-he-0.1.5/edc_he/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:09:09.912826 edc-he-0.1.5/edc_he/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:09:09.913894 edc-he-0.1.5/edc_he/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      677 2022-10-05 19:09:01.000000 edc-he-0.1.5/edc_he/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      227 2022-09-25 18:36:50.000000 edc-he-0.1.5/edc_he/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:09:09.914184 edc-he-0.1.5/edc_he/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4061 2022-09-25 18:36:50.000000 edc-he-0.1.5/edc_he/tests/tests/test_he.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-08-23 17:45:53.000000 edc-he-0.1.5/edc_he/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:09:09.912465 edc-he-0.1.5/edc_he.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1610 2022-10-05 19:09:09.000000 edc-he-0.1.5/edc_he.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1005 2022-10-05 19:09:09.000000 edc-he-0.1.5/edc_he.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-10-05 19:09:09.000000 edc-he-0.1.5/edc_he.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-08-19 17:35:04.000000 edc-he-0.1.5/edc_he.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        7 2022-10-05 19:09:09.000000 edc-he-0.1.5/edc_he.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1714 2022-08-10 22:46:20.000000 edc-he-0.1.5/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2329 2022-05-25 13:21:02.000000 edc-he-0.1.5/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1227 2022-10-05 19:09:09.914925 edc-he-0.1.5/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:43:36.503801 edc-he-0.1.6/
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2021-08-23 17:45:53.000000 edc-he-0.1.6/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-23 17:45:53.000000 edc-he-0.1.6/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:43:36.496036 edc-he-0.1.6/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:43:36.499199 edc-he-0.1.6/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:43:28.000000 edc-he-0.1.6/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-25 13:21:02.000000 edc-he-0.1.6/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:43:28.000000 edc-he-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 22:46:20.000000 edc-he-0.1.6/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.6/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.6/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-19 17:21:37.000000 edc-he-0.1.6/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 13:21:02.000000 edc-he-0.1.6/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1484 2023-05-24 16:43:36.503892 edc-he-0.1.6/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      641 2021-08-23 17:45:53.000000 edc-he-0.1.6/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-10 22:46:20.000000 edc-he-0.1.6/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:43:36.500746 edc-he-0.1.6/edc_he/
+-rw-r--r--   0 erikvw     (501) staff       (20)       66 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      109 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      361 2023-05-24 14:50:19.000000 edc-he-0.1.6/edc_he/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      725 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2272 2022-05-25 13:21:02.000000 edc-he-0.1.6/edc_he/form_validators.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:43:36.501574 edc-he-0.1.6/edc_he/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2175 2023-05-24 14:50:19.000000 edc-he-0.1.6/edc_he/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-05-24 14:50:19.000000 edc-he-0.1.6/edc_he/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:43:36.502070 edc-he-0.1.6/edc_he/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:43:36.503416 edc-he-0.1.6/edc_he/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      677 2022-10-05 19:09:01.000000 edc-he-0.1.6/edc_he/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      227 2022-09-25 18:36:50.000000 edc-he-0.1.6/edc_he/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:43:36.503689 edc-he-0.1.6/edc_he/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4059 2023-05-24 16:43:28.000000 edc-he-0.1.6/edc_he/tests/tests/test_he.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-08-23 17:45:53.000000 edc-he-0.1.6/edc_he/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:43:36.501449 edc-he-0.1.6/edc_he.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1484 2023-05-24 16:43:36.000000 edc-he-0.1.6/edc_he.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      997 2023-05-24 16:43:36.000000 edc-he-0.1.6/edc_he.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 16:43:36.000000 edc-he-0.1.6/edc_he.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-08-19 17:35:04.000000 edc-he-0.1.6/edc_he.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-05-24 16:43:36.000000 edc-he-0.1.6/edc_he.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1758 2023-05-24 16:43:28.000000 edc-he-0.1.6/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2329 2022-05-25 13:21:02.000000 edc-he-0.1.6/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1134 2023-05-24 16:43:36.504191 edc-he-0.1.6/setup.cfg
```

### Comparing `edc-he-0.1.5/.github/workflows/build.yml` & `edc-he-0.1.6/.github/workflows/build.yml`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,20 @@
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
-
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
           - 3306:3306
@@ -28,28 +29,27 @@
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
 
@@ -61,11 +61,11 @@
 
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

### Comparing `edc-he-0.1.5/.gitignore` & `edc-he-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.5/.pre-commit-config.yaml` & `edc-he-0.1.6/.pre-commit-config.yaml`

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

### Comparing `edc-he-0.1.5/LICENSE` & `edc-he-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.5/PKG-INFO` & `edc-he-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-he
-Version: 0.1.5
+Version: 0.1.6
 Summary: Base django classes for health economics
 Home-page: https://github.com/clinicedc/edc-he
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc health economics,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
 
 edc-he
```

### Comparing `edc-he-0.1.5/README.rst` & `edc-he-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.5/edc_he/fieldsets.py` & `edc-he-0.1.6/edc_he/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.5/edc_he/form_validators.py` & `edc-he-0.1.6/edc_he/form_validators.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.5/edc_he/model_mixins.py` & `edc-he-0.1.6/edc_he/model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.5/edc_he/tests/etc/user-rsa-local-private.pem` & `edc-he-0.1.6/edc_he/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.5/edc_he/tests/etc/user-rsa-restricted-private.pem` & `edc-he-0.1.6/edc_he/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.5/edc_he/tests/forms.py` & `edc-he-0.1.6/edc_he/tests/forms.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.5/edc_he/tests/tests/test_he.py` & `edc-he-0.1.6/edc_he/tests/tests/test_he.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,24 +16,22 @@
 
     @property
     def age_in_years(self) -> int:
         return 25
 
 
 class HealthEconomicsForm(BaseHealthEconomicsForm):
-
     form_validator_cls = HealthEconomicsFormValidator
 
     class Meta:
         model = HealthEconomics
         fields = "__all__"
 
 
 class TestHe(FormValidatorTestCaseMixin, TestCase):
-
     form_validator_cls = HealthEconomicsFormValidator
 
     def test_form_validator_education(self):
         # subject_identifier = "1223"
         # appointment = Appointment.objects.create(
         #     subject_identifier=subject_identifier, appt_datetime=get_utcnow()
         # )
```

### Comparing `edc-he-0.1.5/edc_he.egg-info/PKG-INFO` & `edc-he-0.1.6/edc_he.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-he
-Version: 0.1.5
+Version: 0.1.6
 Summary: Base django classes for health economics
 Home-page: https://github.com/clinicedc/edc-he
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc health economics,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
 
 edc-he
```

### Comparing `edc-he-0.1.5/edc_he.egg-info/SOURCES.txt` & `edc-he-0.1.6/edc_he.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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
 edc_he/__init__.py
 edc_he/apps.py
```

### Comparing `edc-he-0.1.5/pyproject.toml` & `edc-he-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

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
-parallel = true
+parallel = false
 branch = true
 source = ["edc_he"]
 
 [tool.coverage.paths]
 source = ["edc_he"]
 
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

### Comparing `edc-he-0.1.5/runtests.py` & `edc-he-0.1.6/runtests.py`

 * *Files identical despite different names*

