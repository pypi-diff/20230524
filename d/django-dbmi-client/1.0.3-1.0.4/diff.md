# Comparing `tmp/django-dbmi-client-1.0.3.tar.gz` & `tmp/django-dbmi-client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dbmi-client-1.0.3.tar", last modified: Wed Feb  8 03:36:47 2023, max compression
+gzip compressed data, was "django-dbmi-client-1.0.4.tar", last modified: Wed May 24 16:21:40 2023, max compression
```

## Comparing `django-dbmi-client-1.0.3.tar` & `django-dbmi-client-1.0.4.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.182446 django-dbmi-client-1.0.3/dbmi_client/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-08 03:36:46.000000 django-dbmi-client-1.0.3/dbmi_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    44470 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/authn.py
--rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/authz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16351 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/fileservice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.182446 django-dbmi-client-1.0.3/dbmi_client/login/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/login/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/login/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/login/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.182446 django-dbmi-client-1.0.3/dbmi_client/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.182446 django-dbmi-client-1.0.3/dbmi_client/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/provider/auth0.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/provider/cognito.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/provider/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/reg.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13536 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.178446 django-dbmi-client-1.0.3/dbmi_client/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.178446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.178446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.182446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/
--rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    46860 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-256x256.png
--rw-r--r--   0 runner    (1001) docker     (123)    75102 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    16968 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-144x144.png
--rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-310x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    37828 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-310x310.png
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-70x70.png
--rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/safari-pinned-tab.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/img/
--rw-r--r--   0 runner    (1001) docker     (123)    32930 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/img/hms_dbmi_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/img/hms_shield.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10661 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/js/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.178446 django-dbmi-client-1.0.3/dbmi_client/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.178446 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/error.html
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/logout.html
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/token.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/dbmi_client/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/tests/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/tests/test_authz.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/dbmi_client/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:36:47.190446 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-08 03:36:47.000000 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-02-08 03:36:47.000000 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 03:36:47.000000 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-08 03:36:47.000000 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-08 03:36:47.000000 django-dbmi-client-1.0.3/django_dbmi_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-08 03:36:47.194446 django-dbmi-client-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-02-08 03:36:24.000000 django-dbmi-client-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.406357 django-dbmi-client-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-24 16:21:40.406357 django-dbmi-client-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.394357 django-dbmi-client-1.0.4/dbmi_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-24 16:21:38.000000 django-dbmi-client-1.0.4/dbmi_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44470 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/authz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16351 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/fileservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.398357 django-dbmi-client-1.0.4/dbmi_client/login/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/login/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/login/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/login/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.398357 django-dbmi-client-1.0.4/dbmi_client/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.398357 django-dbmi-client-1.0.4/dbmi_client/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/provider/auth0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/provider/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/provider/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13536 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.394357 django-dbmi-client-1.0.4/dbmi_client/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.394357 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.394357 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.398357 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.402357 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/
+-rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46860 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/android-chrome-256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75102 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    16968 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/mstile-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/mstile-310x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37828 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/mstile-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/mstile-70x70.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/safari-pinned-tab.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.402357 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    32930 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/img/hms_dbmi_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/img/hms_shield.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.402357 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10661 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/js/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.394357 django-dbmi-client-1.0.4/dbmi_client/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.394357 django-dbmi-client-1.0.4/dbmi_client/templates/dbmi_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.406357 django-dbmi-client-1.0.4/dbmi_client/templates/dbmi_client/login/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/templates/dbmi_client/login/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/templates/dbmi_client/login/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/templates/dbmi_client/login/logout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/templates/dbmi_client/login/token.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.406357 django-dbmi-client-1.0.4/dbmi_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/tests/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/tests/test_authz.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/dbmi_client/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:21:40.406357 django-dbmi-client-1.0.4/django_dbmi_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-24 16:21:40.000000 django-dbmi-client-1.0.4/django_dbmi_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-24 16:21:40.000000 django-dbmi-client-1.0.4/django_dbmi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:21:40.000000 django-dbmi-client-1.0.4/django_dbmi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 16:21:40.000000 django-dbmi-client-1.0.4/django_dbmi_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 16:21:40.000000 django-dbmi-client-1.0.4/django_dbmi_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-24 16:21:40.406357 django-dbmi-client-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-24 16:21:13.000000 django-dbmi-client-1.0.4/setup.py
```

### Comparing `django-dbmi-client-1.0.3/PKG-INFO` & `django-dbmi-client-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dbmi-client
-Version: 1.0.3
+Version: 1.0.4
 Home-page: https://github.com/hms-dbmi/django-dbmi-client
 Author: HMS DBMI Tech-core
 Author-email: dbmi-tech-core@hms.harvard.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

### Comparing `django-dbmi-client-1.0.3/README.rst` & `django-dbmi-client-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/auth.py` & `django-dbmi-client-1.0.4/dbmi_client/auth.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/authn.py` & `django-dbmi-client-1.0.4/dbmi_client/authn.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/authz.py` & `django-dbmi-client-1.0.4/dbmi_client/authz.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/environment.py` & `django-dbmi-client-1.0.4/dbmi_client/environment.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/fileservice.py` & `django-dbmi-client-1.0.4/dbmi_client/fileservice.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/logging.py` & `django-dbmi-client-1.0.4/dbmi_client/logging.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/login/views.py` & `django-dbmi-client-1.0.4/dbmi_client/login/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,21 @@
     :type request: HttpRequest
     :returns: Whether the state matches or not, the state object
     :rtype: bool, dict
     """
     # Fetch some of the request parameters
     state = None
     try:
+        # Check for state in request (not used for refreshes or impersonations)
+        if not request.get("state"):
+
+            # Nothing to compare, let it pass
+            logger.warning(f"No 'state' found in request, allowing login")
+            return True, None
+
         # Get query from state in returning call
         return_state = QueryDict(base64.urlsafe_b64decode(request.GET["state"].encode('utf-8')).decode('utf-8'))
 
         # Get encrypted state in cookies
         state_enc = request.COOKIES.get(DBMI_AUTH_STATE_COOKIE_NAME)
 
         # Decrypt the state cookie
```

### Comparing `django-dbmi-client-1.0.3/dbmi_client/middleware.py` & `django-dbmi-client-1.0.4/dbmi_client/middleware.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/provider/__init__.py` & `django-dbmi-client-1.0.4/dbmi_client/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/provider/auth0.py` & `django-dbmi-client-1.0.4/dbmi_client/provider/auth0.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/provider/cognito.py` & `django-dbmi-client-1.0.4/dbmi_client/provider/cognito.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/provider/provider.py` & `django-dbmi-client-1.0.4/dbmi_client/provider/provider.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/reg.py` & `django-dbmi-client-1.0.4/dbmi_client/reg.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/sentry.py` & `django-dbmi-client-1.0.4/dbmi_client/sentry.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/settings.py` & `django-dbmi-client-1.0.4/dbmi_client/settings.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/css/style.css` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/css/style.css`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-192x192.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-256x256.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/android-chrome-256x256.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/android-chrome-512x512.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120-precomposed.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152-precomposed.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180-precomposed.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60-precomposed.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76-precomposed.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-precomposed.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon-16x16.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon-32x32.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/favicon.ico` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-144x144.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-150x150.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-310x150.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-310x310.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/mstile-70x70.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/favicon/safari-pinned-tab.svg` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/favicon/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/img/hms_dbmi_logo.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/img/hms_dbmi_logo.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/img/hms_shield.png` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/img/hms_shield.png`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/static/dbmi_client/login/js/clipboard.min.js` & `django-dbmi-client-1.0.4/dbmi_client/static/dbmi_client/login/js/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/support.py` & `django-dbmi-client-1.0.4/dbmi_client/support.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/base.html` & `django-dbmi-client-1.0.4/dbmi_client/templates/dbmi_client/login/base.html`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/error.html` & `django-dbmi-client-1.0.4/dbmi_client/templates/dbmi_client/login/error.html`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/templates/dbmi_client/login/token.html` & `django-dbmi-client-1.0.4/dbmi_client/templates/dbmi_client/login/token.html`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/tests/runtests.py` & `django-dbmi-client-1.0.4/dbmi_client/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/tests/test_auth.py` & `django-dbmi-client-1.0.4/dbmi_client/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/dbmi_client/tests/test_authz.py` & `django-dbmi-client-1.0.4/dbmi_client/tests/test_authz.py`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/django_dbmi_client.egg-info/PKG-INFO` & `django-dbmi-client-1.0.4/django_dbmi_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dbmi-client
-Version: 1.0.3
+Version: 1.0.4
 Home-page: https://github.com/hms-dbmi/django-dbmi-client
 Author: HMS DBMI Tech-core
 Author-email: dbmi-tech-core@hms.harvard.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

### Comparing `django-dbmi-client-1.0.3/django_dbmi_client.egg-info/SOURCES.txt` & `django-dbmi-client-1.0.4/django_dbmi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/pyproject.toml` & `django-dbmi-client-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-dbmi-client-1.0.3/setup.py` & `django-dbmi-client-1.0.4/setup.py`

 * *Files identical despite different names*

