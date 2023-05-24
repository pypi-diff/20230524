# Comparing `tmp/edc-document-status-0.1.3.tar.gz` & `tmp/edc-document-status-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-document-status-0.1.3.tar", last modified: Wed Oct 26 02:33:27 2022, max compression
+gzip compressed data, was "edc-document-status-0.1.4.tar", last modified: Wed May 24 16:44:05 2023, max compression
```

## Comparing `edc-document-status-0.1.3.tar` & `edc-document-status-0.1.4.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 02:33:27.828230 edc-document-status-0.1.3/
--rw-r--r--   0 erikvw     (501) staff       (20)      145 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 02:33:27.820584 edc-document-status-0.1.3/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 02:33:27.824486 edc-document-status-0.1.3/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-09 18:44:34.000000 edc-document-status-0.1.3/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1844 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1039 2022-10-26 02:33:20.000000 edc-document-status-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-09 18:44:34.000000 edc-document-status-0.1.3/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-05-19 19:51:05.000000 edc-document-status-0.1.3/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1718 2022-10-26 02:33:27.828354 edc-document-status-0.1.3/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      711 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-10 00:25:02.000000 edc-document-status-0.1.3/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-09 18:44:34.000000 edc-document-status-0.1.3/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 02:33:27.825457 edc-document-status-0.1.3/edc_document_status/
--rw-r--r--   0 erikvw     (501) staff       (20)       85 2022-10-26 02:33:20.000000 edc-document-status-0.1.3/edc_document_status/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      241 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      196 2022-08-09 18:44:34.000000 edc-document-status-0.1.3/edc_document_status/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1366 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      275 2022-08-09 18:44:34.000000 edc-document-status-0.1.3/edc_document_status/modeladmin_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 02:33:27.826521 edc-document-status-0.1.3/edc_document_status/models/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1318 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/models/signals.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 02:33:27.826747 edc-document-status-0.1.3/edc_document_status/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 02:33:27.828003 edc-document-status-0.1.3/edc_document_status/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 02:33:27.828134 edc-document-status-0.1.3/edc_document_status/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      213 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/edc_document_status/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-26 02:33:27.826287 edc-document-status-0.1.3/edc_document_status.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1718 2022-10-26 02:33:27.000000 edc-document-status-0.1.3/edc_document_status.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1217 2022-10-26 02:33:27.000000 edc-document-status-0.1.3/edc_document_status.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-10-26 02:33:27.000000 edc-document-status-0.1.3/edc_document_status.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-19 20:39:30.000000 edc-document-status-0.1.3/edc_document_status.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       20 2022-10-26 02:33:27.000000 edc-document-status-0.1.3/edc_document_status.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1740 2022-08-09 18:44:34.000000 edc-document-status-0.1.3/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2225 2022-05-25 03:00:32.000000 edc-document-status-0.1.3/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1279 2022-10-26 02:33:27.828779 edc-document-status-0.1.3/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.220845 edc-document-status-0.1.4/
+-rw-r--r--   0 erikvw     (501) staff       (20)      145 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.214041 edc-document-status-0.1.4/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.217356 edc-document-status-0.1.4/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:43:56.000000 edc-document-status-0.1.4/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1844 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:43:56.000000 edc-document-status-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-09 18:44:34.000000 edc-document-status-0.1.4/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-05-19 19:51:05.000000 edc-document-status-0.1.4/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1592 2023-05-24 16:44:05.220937 edc-document-status-0.1.4/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      711 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-09 18:44:34.000000 edc-document-status-0.1.4/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.218437 edc-document-status-0.1.4/edc_document_status/
+-rw-r--r--   0 erikvw     (501) staff       (20)       85 2022-10-26 02:33:20.000000 edc-document-status-0.1.4/edc_document_status/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      241 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      196 2022-08-09 18:44:34.000000 edc-document-status-0.1.4/edc_document_status/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1365 2023-05-24 16:43:56.000000 edc-document-status-0.1.4/edc_document_status/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      275 2022-08-09 18:44:34.000000 edc-document-status-0.1.4/edc_document_status/modeladmin_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.219396 edc-document-status-0.1.4/edc_document_status/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1318 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/models/signals.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.219537 edc-document-status-0.1.4/edc_document_status/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.220619 edc-document-status-0.1.4/edc_document_status/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.220757 edc-document-status-0.1.4/edc_document_status/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      213 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.219183 edc-document-status-0.1.4/edc_document_status.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1592 2023-05-24 16:44:05.000000 edc-document-status-0.1.4/edc_document_status.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1209 2023-05-24 16:44:05.000000 edc-document-status-0.1.4/edc_document_status.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 16:44:05.000000 edc-document-status-0.1.4/edc_document_status.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-19 20:39:30.000000 edc-document-status-0.1.4/edc_document_status.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       20 2023-05-24 16:44:05.000000 edc-document-status-0.1.4/edc_document_status.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1784 2023-05-24 16:43:56.000000 edc-document-status-0.1.4/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2225 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1186 2023-05-24 16:44:05.221222 edc-document-status-0.1.4/setup.cfg
```

### Comparing `edc-document-status-0.1.3/.github/workflows/build.yml` & `edc-document-status-0.1.4/.github/workflows/build.yml`

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

### Comparing `edc-document-status-0.1.3/.gitignore` & `edc-document-status-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.3/.pre-commit-config.yaml` & `edc-document-status-0.1.4/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 ---
 exclude: tests/etc/user-*
+
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

### Comparing `edc-document-status-0.1.3/LICENSE` & `edc-document-status-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.3/PKG-INFO` & `edc-document-status-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-document-status
-Version: 0.1.3
+Version: 0.1.4
 Summary: Base classes for CRFs in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-document-status
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc case report forms,CRF,clinicedc,clinical trials
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
 
 edc_document_status
```

### Comparing `edc-document-status-0.1.3/README.rst` & `edc-document-status-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.3/edc_document_status/model_mixins.py` & `edc-document-status-0.1.4/edc_document_status/model_mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.db import models
 from edc_constants.choices import DOCUMENT_STATUS
 from edc_constants.constants import COMPLETE
 
 
 class DocumentStatusModelMixin(models.Model):
-
     document_status = models.CharField(
         verbose_name="Document status",
         max_length=25,
         choices=DOCUMENT_STATUS,
         default=COMPLETE,
         help_text="If some data is still pending, flag as incomplete",
     )
```

### Comparing `edc-document-status-0.1.3/edc_document_status/models/signals.py` & `edc-document-status-0.1.4/edc_document_status/models/signals.py`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.3/edc_document_status/tests/etc/user-rsa-local-private.pem` & `edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.3/edc_document_status/tests/etc/user-rsa-restricted-private.pem` & `edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.3/edc_document_status.egg-info/PKG-INFO` & `edc-document-status-0.1.4/edc_document_status.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-document-status
-Version: 0.1.3
+Version: 0.1.4
 Summary: Base classes for CRFs in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-document-status
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc case report forms,CRF,clinicedc,clinical trials
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
 
 edc_document_status
```

### Comparing `edc-document-status-0.1.3/edc_document_status.egg-info/SOURCES.txt` & `edc-document-status-0.1.4/edc_document_status.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

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
 edc_document_status/__init__.py
 edc_document_status/apps.py
```

### Comparing `edc-document-status-0.1.3/pyproject.toml` & `edc-document-status-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

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
 source = ["edc_document_status"]
 
 [tool.coverage.paths]
 source = ["edc_document_status"]
 
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

### Comparing `edc-document-status-0.1.3/runtests.py` & `edc-document-status-0.1.4/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.3/setup.cfg` & `edc-document-status-0.1.4/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -8,27 +8,24 @@
 description = Base classes for CRFs in clinicedc/edc projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django Edc case report forms, CRF, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
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

