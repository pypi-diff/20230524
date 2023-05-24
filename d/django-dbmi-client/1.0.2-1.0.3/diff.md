# Comparing `tmp/django-dbmi-client-1.0.2.tar.gz` & `tmp/django-dbmi-client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-dbmi-client-1.0.2.tar", last modified: Wed Nov 30 00:48:04 2022, max compression
+gzip compressed data, was "django-dbmi-client-1.0.3.tar", last modified: Wed Feb  8 03:36:47 2023, max compression
```

## Comparing `django-dbmi-client-1.0.2.tar` & `django-dbmi-client-1.0.3.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1979 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     7933 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      116 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/django_dbmi_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/django_dbmi_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/django_dbmi_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3261 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/django_dbmi_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/django_dbmi_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      199 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/django_dbmi_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      313 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)       52 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      166 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/views.py
--rw-r--r--   0 runner    (1001) docker     (122)    16351 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/fileservice.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3902 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1539 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/tests/runtests.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12566 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/tests/test_authz.py
--rw-r--r--   0 runner    (1001) docker     (122)     8399 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)    13718 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/support.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/
--rw-r--r--   0 runner    (1001) docker     (122)    46860 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/android-chrome-256x256.png
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    11147 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (122)    10114 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/mstile-70x70.png
--rw-r--r--   0 runner    (1001) docker     (122)    24472 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (122)    16132 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/mstile-310x150.png
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (122)    17280 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (122)    16968 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/mstile-144x144.png
--rw-r--r--   0 runner    (1001) docker     (122)     2394 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)    15308 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (122)    13934 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (122)    19348 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (122)     5386 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (122)     4043 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (122)    17280 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (122)    37828 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/mstile-310x310.png
--rw-r--r--   0 runner    (1001) docker     (122)    75102 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (122)     9867 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (122)    19348 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (122)    15726 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (122)     4545 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (122)    14291 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76-precomposed.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1450 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/js/
--rwxr-xr-x   0 runner    (1001) docker     (122)    10661 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/js/clipboard.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/img/
--rw-r--r--   0 runner    (1001) docker     (122)    32930 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/img/hms_dbmi_logo.png
--rw-r--r--   0 runner    (1001) docker     (122)    12324 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/img/hms_shield.png
--rw-r--r--   0 runner    (1001) docker     (122)      255 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      459 2022-11-30 00:48:03.000000 django-dbmi-client-1.0.2/dbmi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    44295 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/authn.py
--rw-r--r--   0 runner    (1001) docker     (122)    13536 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/templates/dbmi_client/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/templates/dbmi_client/login/
--rw-r--r--   0 runner    (1001) docker     (122)      951 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/templates/dbmi_client/login/error.html
--rw-r--r--   0 runner    (1001) docker     (122)     2182 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/templates/dbmi_client/login/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2405 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/templates/dbmi_client/login/token.html
--rw-r--r--   0 runner    (1001) docker     (122)      389 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/templates/dbmi_client/login/logout.html
--rw-r--r--   0 runner    (1001) docker     (122)    19898 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/authz.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/login/
--rw-r--r--   0 runner    (1001) docker     (122)    15271 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/login/views.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/login/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      175 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/login/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4302 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/reg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 00:48:04.000000 django-dbmi-client-1.0.2/dbmi_client/provider/
--rw-r--r--   0 runner    (1001) docker     (122)     3917 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/provider/provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     4714 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7677 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/provider/auth0.py
--rw-r--r--   0 runner    (1001) docker     (122)     6068 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/provider/cognito.py
--rw-r--r--   0 runner    (1001) docker     (122)    11528 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)       29 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/sentry.py
--rw-r--r--   0 runner    (1001) docker     (122)     4101 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     3753 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/environment.py
--rw-r--r--   0 runner    (1001) docker     (122)      129 2022-11-30 00:47:33.000000 django-dbmi-client-1.0.2/dbmi_client/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.182446 django-dbmi-client-1.0.3/dbmi_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-08 03:36:46.000000 django-dbmi-client-1.0.3/dbmi_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44470 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/authz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16351 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/fileservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.182446 django-dbmi-client-1.0.3/dbmi_client/login/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/login/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/login/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/login/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.182446 django-dbmi-client-1.0.3/dbmi_client/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.182446 django-dbmi-client-1.0.3/dbmi_client/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/provider/auth0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/provider/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/provider/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13536 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.178446 django-dbmi-client-1.0.3/dbmi_client/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.178446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.178446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.182446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/
+-rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46860 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75102 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    16968 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-310x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37828 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-70x70.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/safari-pinned-tab.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    32930 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/img/hms_dbmi_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/img/hms_shield.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10661 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/js/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.178446 django-dbmi-client-1.0.3/dbmi_client/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.178446 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/logout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/token.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/dbmi_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/tests/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/tests/test_authz.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-08 03:36:47.000000 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-02-08 03:36:47.000000 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 03:36:47.000000 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-08 03:36:47.000000 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-08 03:36:47.000000 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-08 03:36:47.194446 django-dbmi-client-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-dbmi-client-1.0.2/setup.py` & `django-dbmi-client-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/README.rst` & `django-dbmi-client-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/django_dbmi_client.egg-info/SOURCES.txt` & `django-dbmi-client-1.0.3/django_dbmi_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 README.rst
+pyproject.toml
 requirements-dev.txt
 requirements-test.txt
 requirements.txt
 setup.cfg
 setup.py
 dbmi_client/__init__.py
 dbmi_client/admin.py
```

### Comparing `django-dbmi-client-1.0.2/dbmi_client/fileservice.py` & `django-dbmi-client-1.0.3/dbmi_client/fileservice.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/tests/test_auth.py` & `django-dbmi-client-1.0.3/dbmi_client/tests/test_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import mock
 import re
-import unittest
 import responses
 
+from django.test import TestCase
 from django.http import HttpResponse
 from django.contrib.auth.models import User, AnonymousUser
 from django.test.client import RequestFactory
 from dbmi_client import authz
 from dbmi_client.settings import dbmi_settings
 from dbmi_client import auth
 
 
-class TestAuth(unittest.TestCase):
+class TestAuth(TestCase):
 
     # User JWT
     fake_jwt = "somefakejwtalsdijlaiwjdlijawlidjasdhgashgd"
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `django-dbmi-client-1.0.2/dbmi_client/tests/runtests.py` & `django-dbmi-client-1.0.3/dbmi_client/tests/runtests.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 """
 This script is a trick to setup a fake Django environment, since this reusable
 app will be developed and tested outside any specifiv Django project.
 Via ``settings.configure`` you will be able to set all necessary settings
 for your app and run the tests as if you were calling ``./manage.py test``.
 """
 import sys
-from django_nose import NoseTestSuiteRunner
+import pytest
 from django.conf import settings
 
 EXTERNAL_APPS = [
     "django.contrib.admin",
     "django.contrib.admindocs",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.messages",
     "django.contrib.sessions",
     "django.contrib.staticfiles",
     "django.contrib.sitemaps",
     "django.contrib.sites",
 ]
 INTERNAL_APPS = [
-    "django_nose",
     "dbmi_client",
 ]
 INSTALLED_APPS = EXTERNAL_APPS + INTERNAL_APPS
 
 if not settings.configured:
     settings.configure(
         SECRET_KEY="*4n1!z0%@w-e&u9c-kpyqof=-nxvx^v2m000#gf9vewm3s+_v)",
@@ -41,12 +40,12 @@
             "ENVIRONMENT": "prod",
             "AUTH_CLIENTS": {"someauthclientid":{"JWKS_URL":"https://somejwksurl.com/","PROVIDER":"cognito"}},
         },
     )
 
 
 def main(*test_args):
-    sys.exit(NoseTestSuiteRunner(verbosity=2, interactive=True).run_tests(test_args))
+    sys.exit(pytest.main(["-x"]))
 
 
 if __name__ == "__main__":
     main(*sys.argv[1:])
```

### Comparing `django-dbmi-client-1.0.2/dbmi_client/tests/test_authz.py` & `django-dbmi-client-1.0.3/dbmi_client/tests/test_authz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import mock
 import re
-import unittest
+from django.test import TestCase
 import responses
 from django.contrib.auth.models import User
 from django.test.client import RequestFactory
 from dbmi_client import authz
 from dbmi_client.settings import dbmi_settings
 
 
-class TestAuthz(unittest.TestCase):
+class TestAuthz(TestCase):
 
     # User JWT
     fake_jwt = "somefakejwtalsdijlaiwjdlijawlidjasdhgashgd"
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `django-dbmi-client-1.0.2/dbmi_client/auth.py` & `django-dbmi-client-1.0.3/dbmi_client/auth.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/support.py` & `django-dbmi-client-1.0.3/dbmi_client/support.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/android-chrome-256x256.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-256x256.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/favicon.ico` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120-precomposed.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/mstile-70x70.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/android-chrome-192x192.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/mstile-310x150.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/favicon-16x16.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/mstile-144x144.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/favicon-32x32.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/mstile-150x150.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180-precomposed.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/mstile-310x310.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/android-chrome-512x512.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-precomposed.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152-precomposed.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60-precomposed.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/safari-pinned-tab.svg` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76-precomposed.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/css/style.css` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/css/style.css`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/js/clipboard.min.js` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/js/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/img/hms_dbmi_logo.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/img/hms_dbmi_logo.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/static/dbmi_client/login/img/hms_shield.png` & `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/img/hms_shield.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/authn.py` & `django-dbmi-client-1.0.3/dbmi_client/authn.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,14 +464,19 @@
 
     # Get the payload
     payload = get_jwt_payload(request, verify=False)
 
     # Get client ID
     client_id = get_jwt_client_id(request, verify=False)
 
+    # Ensure client ID is valid
+    if client_id not in dbmi_settings.AUTH_CLIENTS:
+        logger.warning(f"Client ID in token is invalid: {client_id}")
+        return None
+
     # Fetch key based off algorithm
     algorithm = get_jwt_algorithm(request)
     if algorithm == "RS256":
 
         # Match the client ID to an authentication provider
         url = dbmi_settings.AUTH_CLIENTS[client_id]["JWKS_URL"]
         jwks_client = PyJWKClient(
```

### Comparing `django-dbmi-client-1.0.2/dbmi_client/settings.py` & `django-dbmi-client-1.0.3/dbmi_client/settings.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/templates/dbmi_client/login/error.html` & `django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/error.html`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/templates/dbmi_client/login/base.html` & `django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/base.html`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/templates/dbmi_client/login/token.html` & `django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/token.html`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/authz.py` & `django-dbmi-client-1.0.3/dbmi_client/authz.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/login/views.py` & `django-dbmi-client-1.0.3/dbmi_client/login/views.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/reg.py` & `django-dbmi-client-1.0.3/dbmi_client/reg.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/provider/provider.py` & `django-dbmi-client-1.0.3/dbmi_client/provider/provider.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/provider/__init__.py` & `django-dbmi-client-1.0.3/dbmi_client/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/provider/auth0.py` & `django-dbmi-client-1.0.3/dbmi_client/provider/auth0.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/provider/cognito.py` & `django-dbmi-client-1.0.3/dbmi_client/provider/cognito.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/middleware.py` & `django-dbmi-client-1.0.3/dbmi_client/middleware.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/sentry.py` & `django-dbmi-client-1.0.3/dbmi_client/sentry.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/logging.py` & `django-dbmi-client-1.0.3/dbmi_client/logging.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.2/dbmi_client/environment.py` & `django-dbmi-client-1.0.3/dbmi_client/environment.py`

 * *Files identical despite different names*

