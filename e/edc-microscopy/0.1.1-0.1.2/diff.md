# Comparing `tmp/edc-microscopy-0.1.1.tar.gz` & `tmp/edc-microscopy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-microscopy-0.1.1.tar", last modified: Tue May 16 02:33:22 2023, max compression
+gzip compressed data, was "edc-microscopy-0.1.2.tar", last modified: Wed May 24 17:03:35 2023, max compression
```

## Comparing `edc-microscopy-0.1.1.tar` & `edc-microscopy-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.038676 edc-microscopy-0.1.1/
--rw-r--r--   0 erikvw     (501) staff       (20)      102 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.031700 edc-microscopy-0.1.1/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.034782 edc-microscopy-0.1.1/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-28 22:00:40.000000 edc-microscopy-0.1.1/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-05-16 02:33:22.038751 edc-microscopy-0.1.1/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      712 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.035724 edc-microscopy-0.1.1/edc_microscopy/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      193 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      593 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      366 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      207 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/choices.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.036715 edc-microscopy-0.1.1/edc_microscopy/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)       66 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      427 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/edc_microscopy/form_validators/malaria_test_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.036999 edc-microscopy-0.1.1/edc_microscopy/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       60 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      931 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/edc_microscopy/model_mixins/malaria_test_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.037270 edc-microscopy-0.1.1/edc_microscopy/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       70 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      755 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/edc_microscopy/modeladmin_mixins/malaria_test_modeladmin_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.037386 edc-microscopy-0.1.1/edc_microscopy/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.038537 edc-microscopy-0.1.1/edc_microscopy/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      301 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.036461 edc-microscopy-0.1.1/edc_microscopy.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-05-16 02:33:21.000000 edc-microscopy-0.1.1/edc_microscopy.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1303 2023-05-16 02:33:22.000000 edc-microscopy-0.1.1/edc_microscopy.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-16 02:33:21.000000 edc-microscopy-0.1.1/edc_microscopy.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-28 22:32:02.000000 edc-microscopy-0.1.1/edc_microscopy.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-05-16 02:33:22.000000 edc-microscopy-0.1.1/edc_microscopy.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1695 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1758 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1166 2023-05-16 02:33:22.039060 edc-microscopy-0.1.1/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:03:35.684766 edc-microscopy-0.1.2/
+-rw-r--r--   0 erikvw     (501) staff       (20)      102 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:03:35.677812 edc-microscopy-0.1.2/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:03:35.680742 edc-microscopy-0.1.2/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 17:03:27.000000 edc-microscopy-0.1.2/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 17:03:27.000000 edc-microscopy-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-28 22:00:40.000000 edc-microscopy-0.1.2/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-05-24 17:03:35.684851 edc-microscopy-0.1.2/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      712 2023-05-16 02:33:14.000000 edc-microscopy-0.1.2/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:03:35.681666 edc-microscopy-0.1.2/edc_microscopy/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      193 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      593 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      366 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      207 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/choices.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:03:35.682718 edc-microscopy-0.1.2/edc_microscopy/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)       66 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      427 2023-05-16 02:33:14.000000 edc-microscopy-0.1.2/edc_microscopy/form_validators/malaria_test_form_validator.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:03:35.683112 edc-microscopy-0.1.2/edc_microscopy/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       60 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      931 2023-05-16 02:33:14.000000 edc-microscopy-0.1.2/edc_microscopy/model_mixins/malaria_test_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:03:35.683457 edc-microscopy-0.1.2/edc_microscopy/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       70 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      755 2023-05-16 02:33:14.000000 edc-microscopy-0.1.2/edc_microscopy/modeladmin_mixins/malaria_test_modeladmin_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:03:35.683599 edc-microscopy-0.1.2/edc_microscopy/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:03:35.684641 edc-microscopy-0.1.2/edc_microscopy/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      301 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/edc_microscopy/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:03:35.682447 edc-microscopy-0.1.2/edc_microscopy.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-05-24 17:03:35.000000 edc-microscopy-0.1.2/edc_microscopy.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1303 2023-05-24 17:03:35.000000 edc-microscopy-0.1.2/edc_microscopy.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 17:03:35.000000 edc-microscopy-0.1.2/edc_microscopy.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-28 22:32:02.000000 edc-microscopy-0.1.2/edc_microscopy.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-05-24 17:03:35.000000 edc-microscopy-0.1.2/edc_microscopy.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1774 2023-05-24 17:03:27.000000 edc-microscopy-0.1.2/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1758 2022-11-28 22:31:54.000000 edc-microscopy-0.1.2/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1166 2023-05-24 17:03:35.685137 edc-microscopy-0.1.2/setup.cfg
```

### Comparing `edc-microscopy-0.1.1/.github/workflows/build.yml` & `edc-microscopy-0.1.2/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,27 @@
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.10', '3.11']
-        django-version: ['4.1', 'dev']
+        django-version: ['4.1', '4.2', 'dev']
+        exclude:
+          - python-version: '3.10'
+            django-version: 'dev'
+    services:
+      mysql:
+        image: mysql:latest
+        env:
+          MYSQL_DATABASE: mysql
+          MYSQL_ROOT_PASSWORD: mysql
+        ports:
+          - 3306:3306
+        options: --health-cmd="mysqladmin ping" --health-interval=10s --health-timeout=5s --health-retries=3
 
     steps:
       - name: Install pycups and words dependency
         run: |
           sudo sed -i 's/azure\.//' /etc/apt/sources.list
           sudo apt-get -y update
           sudo apt-get install libcups2-dev wamerican
```

### Comparing `edc-microscopy-0.1.1/.gitignore` & `edc-microscopy-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.1/.pre-commit-config.yaml` & `edc-microscopy-0.1.2/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -37,18 +37,13 @@
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
-  - repo: https://github.com/rstcheck/rstcheck
-    rev: v6.1.2
-    hooks:
-      - id: rstcheck
-
   - repo: https://github.com/adrienverge/yamllint
     rev: v1.31.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-microscopy-0.1.1/LICENSE` & `edc-microscopy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.1/PKG-INFO` & `edc-microscopy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-microscopy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Microscopy model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-microscopy
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc microscopy,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-microscopy-0.1.1/README.rst` & `edc-microscopy-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.1/edc_microscopy/auth_objects.py` & `edc-microscopy-0.1.2/edc_microscopy/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.1/edc_microscopy/model_mixins/malaria_test_model_mixin.py` & `edc-microscopy-0.1.2/edc_microscopy/model_mixins/malaria_test_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.1/edc_microscopy/modeladmin_mixins/malaria_test_modeladmin_mixin.py` & `edc-microscopy-0.1.2/edc_microscopy/modeladmin_mixins/malaria_test_modeladmin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-local-private.pem` & `edc-microscopy-0.1.2/edc_microscopy/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-restricted-private.pem` & `edc-microscopy-0.1.2/edc_microscopy/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.1/edc_microscopy.egg-info/PKG-INFO` & `edc-microscopy-0.1.2/edc_microscopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-microscopy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Microscopy model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-microscopy
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc microscopy,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-microscopy-0.1.1/edc_microscopy.egg-info/SOURCES.txt` & `edc-microscopy-0.1.2/edc_microscopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.1/pyproject.toml` & `edc-microscopy-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 [tool.isort]
 profile = "black"
 py_version = "310"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
-parallel = true
+parallel = false
 branch = true
 source = ["edc_microscopy"]
 
 [tool.coverage.paths]
 source = ["edc_microscopy"]
 
 [tool.coverage.report]
@@ -32,40 +32,43 @@
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
-    pip install -U pip
+    pip install -U pip coverage[toml]
     pip --version
     pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
```

### Comparing `edc-microscopy-0.1.1/runtests.py` & `edc-microscopy-0.1.2/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.1/setup.cfg` & `edc-microscopy-0.1.2/setup.cfg`

 * *Files identical despite different names*

