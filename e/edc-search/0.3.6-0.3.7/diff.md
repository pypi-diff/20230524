# Comparing `tmp/edc-search-0.3.6.tar.gz` & `tmp/edc-search-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-search-0.3.6.tar", last modified: Sun Sep 25 22:22:16 2022, max compression
+gzip compressed data, was "edc-search-0.3.7.tar", last modified: Wed May 24 16:44:33 2023, max compression
```

## Comparing `edc-search-0.3.6.tar` & `edc-search-0.3.7.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:16.533129 edc-search-0.3.6/
--rw-r--r--   0 erikvw     (501) staff       (20)       90 2021-02-07 13:19:55.000000 edc-search-0.3.6/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-06 15:47:52.000000 edc-search-0.3.6/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:16.526713 edc-search-0.3.6/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:16.529938 edc-search-0.3.6/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1832 2022-09-25 22:22:08.000000 edc-search-0.3.6/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1119 2022-06-01 23:57:05.000000 edc-search-0.3.6/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)      127 2022-06-01 23:57:05.000000 edc-search-0.3.6/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-06-01 23:57:05.000000 edc-search-0.3.6/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:12:34.000000 edc-search-0.3.6/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:57:05.000000 edc-search-0.3.6/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2850 2022-09-25 22:22:16.533239 edc-search-0.3.6/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1991 2021-02-06 16:35:53.000000 edc-search-0.3.6/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 22:22:08.000000 edc-search-0.3.6/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-06 15:47:52.000000 edc-search-0.3.6/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:16.531011 edc-search-0.3.6/edc_search/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-search-0.3.6/edc_search/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      113 2020-03-04 23:12:34.000000 edc-search-0.3.6/edc_search/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1284 2021-03-01 04:04:15.000000 edc-search-0.3.6/edc_search/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:57:05.000000 edc-search-0.3.6/edc_search/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      812 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/search_slug.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:16.531739 edc-search-0.3.6/edc_search/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-search-0.3.6/edc_search/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:16.532794 edc-search-0.3.6/edc_search/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1362 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:16.533011 edc-search-0.3.6/edc_search/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2197 2022-06-01 23:57:05.000000 edc-search-0.3.6/edc_search/tests/tests/tests.py
--rw-r--r--   0 erikvw     (501) staff       (20)      583 2021-02-06 15:47:52.000000 edc-search-0.3.6/edc_search/updater.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-01 23:57:05.000000 edc-search-0.3.6/edc_search/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      171 2020-03-04 23:12:34.000000 edc-search-0.3.6/edc_search/wsgi.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:16.531558 edc-search-0.3.6/edc_search.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2850 2022-09-25 22:22:16.000000 edc-search-0.3.6/edc_search.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1008 2022-09-25 22:22:16.000000 edc-search-0.3.6/edc_search.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-25 22:22:16.000000 edc-search-0.3.6/edc_search.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-06 20:43:35.000000 edc-search-0.3.6/edc_search.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-09-25 22:22:16.000000 edc-search-0.3.6/edc_search.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1581 2022-06-01 23:57:05.000000 edc-search-0.3.6/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1620 2022-06-01 23:57:05.000000 edc-search-0.3.6/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1152 2022-09-25 22:22:16.533563 edc-search-0.3.6/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.305156 edc-search-0.3.7/
+-rw-r--r--   0 erikvw     (501) staff       (20)       90 2021-02-07 13:19:55.000000 edc-search-0.3.7/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-06 15:47:52.000000 edc-search-0.3.7/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.298562 edc-search-0.3.7/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.301936 edc-search-0.3.7/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:44:25.000000 edc-search-0.3.7/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1119 2022-06-01 23:57:05.000000 edc-search-0.3.7/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:44:25.000000 edc-search-0.3.7/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      127 2022-06-01 23:57:05.000000 edc-search-0.3.7/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-06-01 23:57:05.000000 edc-search-0.3.7/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:12:34.000000 edc-search-0.3.7/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:57:05.000000 edc-search-0.3.7/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2853 2023-05-24 16:44:33.305246 edc-search-0.3.7/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1991 2021-02-06 16:35:53.000000 edc-search-0.3.7/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 22:22:08.000000 edc-search-0.3.7/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-06 15:47:52.000000 edc-search-0.3.7/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.302991 edc-search-0.3.7/edc_search/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-search-0.3.7/edc_search/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      113 2020-03-04 23:12:34.000000 edc-search-0.3.7/edc_search/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1282 2023-05-24 16:44:25.000000 edc-search-0.3.7/edc_search/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:57:05.000000 edc-search-0.3.7/edc_search/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      812 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/search_slug.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.303767 edc-search-0.3.7/edc_search/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-search-0.3.7/edc_search/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.304817 edc-search-0.3.7/edc_search/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1357 2023-05-24 16:44:25.000000 edc-search-0.3.7/edc_search/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.305035 edc-search-0.3.7/edc_search/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2197 2022-06-01 23:57:05.000000 edc-search-0.3.7/edc_search/tests/tests/tests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      582 2023-05-24 16:44:25.000000 edc-search-0.3.7/edc_search/updater.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-01 23:57:05.000000 edc-search-0.3.7/edc_search/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      171 2020-03-04 23:12:34.000000 edc-search-0.3.7/edc_search/wsgi.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.303580 edc-search-0.3.7/edc_search.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2853 2023-05-24 16:44:33.000000 edc-search-0.3.7/edc_search.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1032 2023-05-24 16:44:33.000000 edc-search-0.3.7/edc_search.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 16:44:33.000000 edc-search-0.3.7/edc_search.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-06 20:43:35.000000 edc-search-0.3.7/edc_search.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2023-05-24 16:44:33.000000 edc-search-0.3.7/edc_search.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1766 2023-05-24 16:44:25.000000 edc-search-0.3.7/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1620 2022-06-01 23:57:05.000000 edc-search-0.3.7/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1155 2023-05-24 16:44:33.305528 edc-search-0.3.7/setup.cfg
```

### Comparing `edc-search-0.3.6/.github/workflows/build.yml` & `edc-search-0.3.7/.github/workflows/build.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,71 @@
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
         options: --health-cmd="mysqladmin ping" --health-interval=10s --health-timeout=5s --health-retries=3
 
     steps:
-    - name: Install pycups and words dependency
-      run: |
-        sudo sed -i 's/azure\.//' /etc/apt/sources.list
-        sudo apt-get -y update
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
+      - uses: actions/checkout@v3
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Get pip cache dir
+        id: pip-cache
+        run: |
+          echo "dir=$(pip cache dir)" >>$GITHUB_OUTPUT
+
+      - name: Cache
+        uses: actions/cache@v3
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
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v3
+        with:
+          name: Python ${{ matrix.python-version }}
```

### Comparing `edc-search-0.3.6/.gitignore` & `edc-search-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.6/LICENSE` & `edc-search-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.6/PKG-INFO` & `edc-search-0.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-search
-Version: 0.3.6
+Version: 0.3.7
 Summary: Simple edc-search forms and view mixins for the clinicedc/edc
 Home-page: https://github.com/clinicedc/edc-search
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc search,clinicedc,clinical trials
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
 
 edc-search
```

### Comparing `edc-search-0.3.6/README.rst` & `edc-search-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.6/edc_search/model_mixins.py` & `edc-search-0.3.7/edc_search/model_mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 
 from django.db import models
 
 from .updater import SearchSlugUpdater
 
 
 class SearchSlugManager(models.Manager):
-
     search_slug_updater_cls = SearchSlugUpdater
     search_slug_field_name = "slug"
 
     def update_search_slugs(self) -> None:
         for obj in self.all():
             updater = self.search_slug_updater_cls(
                 fields=obj.get_search_slug_fields(), model_obj=obj
             )
             setattr(obj, self.search_slug_field_name, updater.slug)
             obj.save_base(update_fields=[self.search_slug_field_name])
 
 
 class SearchSlugModelMixin(models.Model):
-
     search_slug_warning = None
     search_slug_updater_cls = SearchSlugUpdater
 
     def get_search_slug_fields(self) -> List[str]:
         return []
 
     slug = models.CharField(
```

### Comparing `edc-search-0.3.6/edc_search/search_slug.py` & `edc-search-0.3.7/edc_search/search_slug.py`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.6/edc_search/tests/etc/user-rsa-local-private.pem` & `edc-search-0.3.7/edc_search/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.6/edc_search/tests/etc/user-rsa-restricted-private.pem` & `edc-search-0.3.7/edc_search/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.6/edc_search/tests/models.py` & `edc-search-0.3.7/edc_search/tests/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 from django.db import models
 
 from ..model_mixins import SearchSlugManager, SearchSlugModelMixin
 
 
 class Dummy:
-
     attr = "dummy_attr"
 
     def __str__(self):
         return "Dummy"
 
 
 class TestModelMixin(SearchSlugModelMixin, models.Model):
-
     f1 = models.CharField(max_length=25, null=True)
 
     f2 = models.DateTimeField(null=True)
 
     f3 = models.IntegerField(null=True)
 
     objects = SearchSlugManager()
@@ -37,29 +35,26 @@
         return fields
 
     class Meta:
         abstract = True
 
 
 class TestModel(TestModelMixin, models.Model):
-
     pass
 
 
 class TestModelExtra(TestModelMixin, models.Model):
-
     f4 = models.CharField(max_length=25, null=True)
 
     def get_search_slug_fields(self):
         fields = super().get_search_slug_fields()
         fields.append("f4")
         return fields
 
 
 class TestModelDuplicate(TestModelMixin, models.Model):
-
     f4 = models.CharField(max_length=25, null=True)
 
     def get_search_slug_fields(self):
         fields = super().get_search_slug_fields()
         fields.extend(["f1", "f4"])
         return fields
```

### Comparing `edc-search-0.3.6/edc_search/tests/tests/tests.py` & `edc-search-0.3.7/edc_search/tests/tests/tests.py`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.6/edc_search/updater.py` & `edc-search-0.3.7/edc_search/updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 
 class SearchSlugDuplicateFields(Exception):
     pass
 
 
 class SearchSlugUpdater:
-
     search_slug_cls = SearchSlug
     sep = "|"
 
     def __init__(self, fields, model_obj=None):
         if len(fields) > len(list(set(fields))):
             raise SearchSlugDuplicateFields(
                 f"Duplicate search slug fields detected. Got {fields}. " f"See {repr(self)}"
```

### Comparing `edc-search-0.3.6/edc_search.egg-info/PKG-INFO` & `edc-search-0.3.7/edc_search.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-search
-Version: 0.3.6
+Version: 0.3.7
 Summary: Simple edc-search forms and view mixins for the clinicedc/edc
 Home-page: https://github.com/clinicedc/edc-search
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc search,clinicedc,clinical trials
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
 
 edc-search
```

### Comparing `edc-search-0.3.6/edc_search.egg-info/SOURCES.txt` & `edc-search-0.3.7/edc_search.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .coveragerc
 .editorconfig
 .gitignore
+.pre-commit-config.yaml
 AUTHORS
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
 VERSION
 codecov.yml
```

### Comparing `edc-search-0.3.6/pyproject.toml` & `edc-search-0.3.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -3,64 +3,74 @@
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
 source = ["edc_search"]
 
 [tool.coverage.paths]
 source = ["edc_search"]
 
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
-    py{39}-dj{32,dev},
+    py{310}-dj{41,42},
+    py{311}-dj{41,42,dev},
     lint
+
 isolated_build = true
 
 [gh-actions]
 python =
-    3.9: py39, lint
+    3.10: py310
+    3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
-    3.2: dj32, lint
+    4.1: dj41
+    4.2: dj42, lint
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
-    dj32: Django>=3.2,<3.3
+    dj41: Django>=4.1,<4.2
+    dj42: Django>=4.2,<5.0
     djdev: https://github.com/django/django/tarball/main
 
 commands =
-    pip install -U pip
+    pip install -U pip coverage[toml]
     pip --version
+    pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
 commands =
     isort --profile=black --check --diff .
```

### Comparing `edc-search-0.3.6/runtests.py` & `edc-search-0.3.7/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.6/setup.cfg` & `edc-search-0.3.7/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 description = Simple edc-search forms and view mixins for the clinicedc/edc
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django Edc search, clinicedc, clinical trials
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

