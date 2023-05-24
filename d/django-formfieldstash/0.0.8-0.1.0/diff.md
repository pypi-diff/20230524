# Comparing `tmp/django-formfieldstash-0.0.8.tar.gz` & `tmp/django-formfieldstash-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-formfieldstash-0.0.8.tar", last modified: Thu Dec  5 13:48:02 2019, max compression
+gzip compressed data, was "django-formfieldstash-0.1.0.tar", last modified: Wed May 24 14:45:25 2023, max compression
```

## Comparing `django-formfieldstash-0.0.8.tar` & `django-formfieldstash-0.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 benzkji   (1000) benzkji   (1000)        0 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     1077 2019-11-27 10:49:46.000000 django-formfieldstash-0.0.8/LICENSES
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      223 2019-01-14 15:50:52.000000 django-formfieldstash-0.0.8/MANIFEST.in
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     1336 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/PKG-INFO
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      694 2019-11-15 08:39:29.000000 django-formfieldstash-0.0.8/PYPI.rst
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     4710 2019-11-15 08:39:29.000000 django-formfieldstash-0.0.8/README.rst
-drwxrwxr-x   0 benzkji   (1000) benzkji   (1000)        0 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/django_formfieldstash.egg-info/
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     1336 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/django_formfieldstash.egg-info/PKG-INFO
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     1460 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/django_formfieldstash.egg-info/SOURCES.txt
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)        1 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/django_formfieldstash.egg-info/dependency_links.txt
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)        1 2019-01-14 15:51:41.000000 django-formfieldstash-0.0.8/django_formfieldstash.egg-info/not-zip-safe
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)       12 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/django_formfieldstash.egg-info/requires.txt
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)       15 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/django_formfieldstash.egg-info/top_level.txt
-drwxrwxr-x   0 benzkji   (1000) benzkji   (1000)        0 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/formfieldstash/
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)       45 2019-12-05 13:47:36.000000 django-formfieldstash-0.0.8/formfieldstash/__init__.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     1814 2019-11-27 10:49:46.000000 django-formfieldstash-0.0.8/formfieldstash/admin.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      662 2019-11-27 10:39:08.000000 django-formfieldstash-0.0.8/formfieldstash/helpers.py
-drwxrwxr-x   0 benzkji   (1000) benzkji   (1000)        0 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/formfieldstash/static/
-drwxrwxr-x   0 benzkji   (1000) benzkji   (1000)        0 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/formfieldstash/static/formfield_stash/
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     4083 2019-12-05 13:47:28.000000 django-formfieldstash-0.0.8/formfieldstash/static/formfield_stash/formfield_stash.js
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      389 2019-11-27 10:49:46.000000 django-formfieldstash-0.0.8/formfieldstash/static/formfield_stash/zzz_adjust-divers.css
-drwxrwxr-x   0 benzkji   (1000) benzkji   (1000)        0 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/formfieldstash/tests/
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)       23 2019-01-14 15:27:29.000000 django-formfieldstash-0.0.8/formfieldstash/tests/__init__.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     2935 2019-01-14 15:50:52.000000 django-formfieldstash-0.0.8/formfieldstash/tests/settings.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)       59 2019-01-14 15:50:52.000000 django-formfieldstash-0.0.8/formfieldstash/tests/settings_no_headless.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     5957 2019-11-15 08:39:29.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_admin.py
-drwxrwxr-x   0 benzkji   (1000) benzkji   (1000)        0 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)        0 2019-01-14 15:27:29.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/__init__.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     2117 2019-11-27 10:39:08.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/admin.py
-drwxrwxr-x   0 benzkji   (1000) benzkji   (1000)        0 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      830 2019-01-14 15:27:29.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0001_initial.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     3385 2019-01-14 15:50:52.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0002_auto_20160714_0808.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     1348 2019-11-15 08:39:29.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0003_auto_20191114_1039.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      937 2019-11-15 08:39:29.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0004_testmodelsingle2.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      775 2019-11-27 10:39:08.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0005_auto_20191119_0327.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      461 2019-12-05 13:47:28.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0006_auto_20191205_0657.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      486 2019-12-05 13:47:28.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0007_auto_20191205_0658.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)        0 2019-01-14 15:27:29.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/__init__.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     3396 2019-12-05 13:47:28.000000 django-formfieldstash-0.0.8/formfieldstash/tests/test_app/models.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      378 2019-01-14 15:50:52.000000 django-formfieldstash-0.0.8/formfieldstash/tests/urls.py
-drwxrwxr-x   0 benzkji   (1000) benzkji   (1000)        0 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/formfieldstash/tests/utils/
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)       23 2019-01-14 15:27:29.000000 django-formfieldstash-0.0.8/formfieldstash/tests/utils/__init__.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      265 2019-01-14 15:27:29.000000 django-formfieldstash-0.0.8/formfieldstash/tests/utils/django_utils.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)     2419 2019-01-14 15:50:52.000000 django-formfieldstash-0.0.8/formfieldstash/tests/utils/selenium_utils.py
--rw-rw-r--   0 benzkji   (1000) benzkji   (1000)      150 2019-12-05 13:48:02.000000 django-formfieldstash-0.0.8/setup.cfg
--rwxrwxr-x   0 benzkji   (1000) benzkji   (1000)     1164 2019-11-27 10:49:46.000000 django-formfieldstash-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:45:25.231727 django-formfieldstash-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/LICENSES
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-24 14:45:25.231727 django-formfieldstash-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:45:25.227727 django-formfieldstash-0.1.0/django_formfieldstash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-24 14:45:25.000000 django-formfieldstash-0.1.0/django_formfieldstash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-24 14:45:25.000000 django-formfieldstash-0.1.0/django_formfieldstash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:45:25.000000 django-formfieldstash-0.1.0/django_formfieldstash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:45:25.000000 django-formfieldstash-0.1.0/django_formfieldstash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 14:45:25.000000 django-formfieldstash-0.1.0/django_formfieldstash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 14:45:25.000000 django-formfieldstash-0.1.0/django_formfieldstash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:45:25.227727 django-formfieldstash-0.1.0/formfieldstash/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:45:25.227727 django-formfieldstash-0.1.0/formfieldstash/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:45:25.227727 django-formfieldstash-0.1.0/formfieldstash/static/formfield_stash/
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/static/formfield_stash/formfield_stash.js
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/static/formfield_stash/zzz_adjust-divers.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:45:25.231727 django-formfieldstash-0.1.0/formfieldstash/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/settings_no_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:45:25.231727 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:45:25.231727 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0002_auto_20160714_0808.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0003_auto_20191114_1039.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0004_testmodelsingle2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0005_auto_20191119_0327.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0006_auto_20191205_0657.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0007_auto_20191205_0658.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/test_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:45:25.231727 django-formfieldstash-0.1.0/formfieldstash/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/utils/django_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/formfieldstash/tests/utils/selenium_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 14:45:25.231727 django-formfieldstash-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-05-24 14:45:14.000000 django-formfieldstash-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-formfieldstash-0.0.8/LICENSES` & `django-formfieldstash-0.1.0/LICENSES`

 * *Files identical despite different names*

### Comparing `django-formfieldstash-0.0.8/README.rst` & `django-formfieldstash-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 django-formfieldstash
 *****************
 
-.. image:: https://travis-ci.org/bnzk/django-formfieldstash.svg
-    :target: https://travis-ci.org/bnzk/django-formfieldstash
-.. image:: https://img.shields.io/pypi/v/django-formfieldstash.svg
-    :target: https://pypi.python.org/pypi/django-formfieldstash/
-.. image:: https://img.shields.io/pypi/l/django-formfieldstash.svg
-    :target: https://pypi.python.org/pypi/django-formfieldstash/
+[![CI](https://img.shields.io/github/actions/workflow/status/bnzk/django-formfieldstash/ci.yml?style=flat-square&logo=github "CI")](https://github.com/bnzk/django-formfieldstash/actions/workflows/ci.yml)
+[![Version](https://img.shields.io/pypi/v/django-formfieldstash.svg?style=flat-square "Version")](https://pypi.python.org/pypi/django-formfieldstash/)
+[![Licence](https://img.shields.io/github/license/bnzk/django-formfieldstash.svg?style=flat-square "Licence")](https://pypi.python.org/pypi/django-formfieldstash/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/django-formfieldstash?style=flat-square "PyPi Downloads")](https://pypistats.org/packages/django-formfieldstash)
 
 
 show/hide modelform fields, depending on current value of a dropdown in the form. without page reload.
 this is a pure javascript solution, using a modeladminmixin approach.
 
+Example, using the included test app (see code for how it's done):
+
+![CI](https://raw.githubusercontent.com/bnzk/django-formfieldstash/main/docs/formfieldstash.gif "Demo GIF")
+ 
+
 Installation
 ------------
 
 To get the latest stable release from PyPi
 
 .. code-block:: bash
```

### Comparing `django-formfieldstash-0.0.8/django_formfieldstash.egg-info/SOURCES.txt` & `django-formfieldstash-0.1.0/django_formfieldstash.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSES
 MANIFEST.in
-PYPI.rst
-README.rst
+PYPI.md
+README.md
 setup.cfg
 setup.py
 django_formfieldstash.egg-info/PKG-INFO
 django_formfieldstash.egg-info/SOURCES.txt
 django_formfieldstash.egg-info/dependency_links.txt
 django_formfieldstash.egg-info/not-zip-safe
 django_formfieldstash.egg-info/requires.txt
```

### Comparing `django-formfieldstash-0.0.8/formfieldstash/admin.py` & `django-formfieldstash-0.1.0/formfieldstash/admin.py`

 * *Files identical despite different names*

### Comparing `django-formfieldstash-0.0.8/formfieldstash/helpers.py` & `django-formfieldstash-0.1.0/formfieldstash/helpers.py`

 * *Files identical despite different names*

### Comparing `django-formfieldstash-0.0.8/formfieldstash/static/formfield_stash/formfield_stash.js` & `django-formfieldstash-0.1.0/formfieldstash/static/formfield_stash/formfield_stash.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -83,22 +83,26 @@
     }
 })(django.jQuery);
 
 
 // init, including add row for inlines
 django.jQuery(document).ready(function($) {
 
-    $('.inline-group').each(function(index, inline) {
-        if ($(inline).find("fieldset select[data-formfield-stash=true]").length) {
-            $(inline).find(".add-row").click(add_row_handler);
-        };
-    });
-
-    function add_row_handler(event) {
-        // depends on html structure, bad. but...
-        var $inline = $(event.currentTarget).parent();
-        var $to_enhance = $inline.find(".last-related:not(.empty-form ) select[data-formfield-stash=true]");
+    // https://docs.djangoproject.com/en/4.2/ref/contrib/admin/javascript/
+    $(document).on('formset:added', (event, $row, formsetName) => {
+        if (event.detail && event.detail.formsetName) {
+            // Django >= 4.1
+            handleFormsetAdded(event.target, event.detail.formsetName)
+        } else {
+            // Django < 4.1, use $row and formsetName
+            handleFormsetAdded($row.get(0), formsetName)
+        }
+    })
+
+    function handleFormsetAdded(row, formsetName) {
+        var $to_enhance = $(row).find('select[data-formfield-stash="true"]')
         $to_enhance.formfield_stash();
     }
 
     $('form select[data-formfield-stash=true]').not("[name*=__prefix__]").formfield_stash();
+
 });
```

### Comparing `django-formfieldstash-0.0.8/formfieldstash/tests/settings.py` & `django-formfieldstash-0.1.0/formfieldstash/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-formfieldstash-0.0.8/formfieldstash/tests/test_admin.py` & `django-formfieldstash-0.1.0/formfieldstash/tests/test_admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.advanced2 = TestModelAdvanced2(**{'set': 'set1', })
         self.advanced2.save()
         self.superuser = create_superuser()
         # Instantiating the WebDriver will load your browser
         options = Options()
         if settings.HEADLESS_TESTING:
             options.add_argument("--headless")
-        self.webdriver = CustomWebDriver(firefox_options=options, )
+        self.webdriver = CustomWebDriver(options=options, )
 
     def tearDown(self):
         self.webdriver.quit()
 
     def test_app_index_get(self):
         self.login()
         self.open(reverse('admin:index'))
```

### Comparing `django-formfieldstash-0.0.8/formfieldstash/tests/test_app/admin.py` & `django-formfieldstash-0.1.0/formfieldstash/tests/test_app/admin.py`

 * *Files identical despite different names*

### Comparing `django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0001_initial.py` & `django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0002_auto_20160714_0808.py` & `django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0002_auto_20160714_0808.py`

 * *Files identical despite different names*

### Comparing `django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0003_auto_20191114_1039.py` & `django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0003_auto_20191114_1039.py`

 * *Files identical despite different names*

### Comparing `django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0004_testmodelsingle2.py` & `django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0004_testmodelsingle2.py`

 * *Files identical despite different names*

### Comparing `django-formfieldstash-0.0.8/formfieldstash/tests/test_app/migrations/0005_auto_20191119_0327.py` & `django-formfieldstash-0.1.0/formfieldstash/tests/test_app/migrations/0005_auto_20191119_0327.py`

 * *Files identical despite different names*

### Comparing `django-formfieldstash-0.0.8/formfieldstash/tests/test_app/models.py` & `django-formfieldstash-0.1.0/formfieldstash/tests/test_app/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,96 +1,85 @@
-from __future__ import unicode_literals
-
-from django.utils.encoding import python_2_unicode_compatible
 from django.db import models
 
 
 SELECTION_CHOICES = (
     ('', 'Empty'),
     ('horse', 'Horse'),
     ('bear', 'Bear'),
     ('octopus', 'Octopus'),
 )
 
-
 SET_CHOICES = (
     ('', 'Empty'),
     ('set1', '1'),
     ('set2', '2'),
     ('set3_1', '3'),
 )
 
 
-@python_2_unicode_compatible
 class TestModelSingle(models.Model):
     selection = models.CharField('Selection', max_length=20, blank=True, choices=SELECTION_CHOICES)
     horse = models.CharField(max_length=20, blank=True, )
     bear = models.DateTimeField(blank=True, null=True, default=None)
     octopus = models.CharField(max_length=20, blank=True, )
 
     def __str__(self):
         return "Single Stash Test Model: %s" % self.selection
 
 
-@python_2_unicode_compatible
 class TestModelSingle2(models.Model):
     selection = models.CharField('Selection', max_length=20, blank=True, choices=SELECTION_CHOICES)
     horse = models.CharField(max_length=20, blank=True, )
     bear = models.CharField(max_length=20, blank=True, )
     octopus = models.CharField(max_length=20, blank=True, )
 
     def __str__(self):
         return "Single Stash Test Model 2: %s" % self.selection
 
 
-@python_2_unicode_compatible
 class TestModelAdvanced(models.Model):
     set = models.CharField('Selection', max_length=20, blank=True, choices=SET_CHOICES)
     set1_1 = models.CharField(max_length=20, blank=True, )
     set2_1 = models.CharField(max_length=20, blank=True, )
     set2_2 = models.CharField(max_length=20, blank=True, )
     set2_3 = models.CharField(max_length=20, blank=True, )
     set3_1 = models.CharField(max_length=20, blank=True, )
 
     def __str__(self):
         return "Test Advanced Model: %s" % self.set
 
 
-@python_2_unicode_compatible
 class TestModelAdvanced2(models.Model):
     set = models.CharField('Selection', max_length=20, blank=True, choices=SET_CHOICES)
     set1_1 = models.CharField(max_length=20, blank=True, )
     set2_1 = models.CharField(max_length=20, blank=True, )
     set2_2 = models.CharField(max_length=20, blank=True, )
     set2_3 = models.CharField(max_length=20, blank=True, )
     set3_1 = models.CharField(max_length=20, blank=True, )
 
     def __str__(self):
         return "Test Advanced Model 2: %s" % self.set
 
 
-@python_2_unicode_compatible
 class TestInlineModel(models.Model):
     parent = models.ForeignKey(TestModelAdvanced, on_delete=models.CASCADE)
     parent2 = models.ForeignKey(TestModelAdvanced2, on_delete=models.CASCADE, default=None, null=True)
     title = models.CharField(max_length=20, blank=True, )
 
     def __str__(self):
         return "A Simple Inline Model: %s" % self.title
 
 
-@python_2_unicode_compatible
 class TestModelInInlineModel(models.Model):
     title = models.CharField(max_length=20, blank=True, )
 
     def __str__(self):
         return "Has Stash In Inline Model: %s" % self.title
 
 
-@python_2_unicode_compatible
 class TestInlineModelSingle(models.Model):
     parent = models.ForeignKey(TestModelInInlineModel, on_delete=models.CASCADE)
     selection = models.CharField('Selection', max_length=20, blank=True, choices=SELECTION_CHOICES)
     horse = models.CharField(max_length=20, blank=True, )
     bear = models.CharField(max_length=20, blank=True, )
     octopus = models.CharField(max_length=20, blank=True, )
```

### Comparing `django-formfieldstash-0.0.8/formfieldstash/tests/utils/selenium_utils.py` & `django-formfieldstash-0.1.0/formfieldstash/tests/utils/selenium_utils.py`

 * *Files identical despite different names*

