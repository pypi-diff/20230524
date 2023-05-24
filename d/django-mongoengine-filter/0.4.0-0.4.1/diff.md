# Comparing `tmp/django-mongoengine-filter-0.4.0.tar.gz` & `tmp/django-mongoengine-filter-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mongoengine-filter-0.4.0.tar", last modified: Sun Dec 25 00:00:06 2022, max compression
+gzip compressed data, was "django-mongoengine-filter-0.4.1.tar", last modified: Thu Feb 23 21:32:55 2023, max compression
```

## Comparing `django-mongoengine-filter-0.4.0.tar` & `django-mongoengine-filter-0.4.1.tar`

### file list

```diff
@@ -1,122 +1,120 @@
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.222443 django-mongoengine-filter-0.4.0/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      156 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/.coveragerc
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/.coveralls.yml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/.env
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.198442 django-mongoengine-filter-0.4.0/.github/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.206442 django-mongoengine-filter-0.4.0/.github/workflows/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2865 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/.github/workflows/test.yml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      743 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/.gitignore
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1474 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/.pre-commit-config.yaml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      226 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/.pre-commit-hooks.yaml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1470 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/CHANGELOG.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/CREDITS.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/LICENSE_GPL2.0.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/LICENSE_LGPL_2.1.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      201 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/MANIFEST.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     7297 2022-12-25 00:00:06.222443 django-mongoengine-filter-0.4.0/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5761 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.206442 django-mongoengine-filter-0.4.0/django_mongoengine_filter/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      680 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      559 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter/compat.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1246 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter/fields.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     7819 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter/filters.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    13262 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter/filterset.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.202443 django-mongoengine-filter-0.4.0/django_mongoengine_filter/locale/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.202443 django-mongoengine-filter-0.4.0/django_mongoengine_filter/locale/fr/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.210442 django-mongoengine-filter-0.4.0/django_mongoengine_filter/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3640 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter/views.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3441 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter/widgets.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.206442 django-mongoengine-filter-0.4.0/django_mongoengine_filter.egg-info/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     7297 2022-12-25 00:00:06.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter.egg-info/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2554 2022-12-25 00:00:06.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2022-12-25 00:00:06.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2022-12-24 23:02:49.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter.egg-info/not-zip-safe
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        9 2022-12-25 00:00:06.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter.egg-info/requires.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       32 2022-12-25 00:00:06.000000 django-mongoengine-filter-0.4.0/django_mongoengine_filter.egg-info/top_level.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      333 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docker-compose.yml
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.210442 django-mongoengine-filter-0.4.0/docs/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/Makefile
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/changelog.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    11953 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/conf.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    11953 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/conf.py.distrib
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      215 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/documentation.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/filters.rst.distrib
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4006 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/docs/filters_doc.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/index.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/index.rst.distrib
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/make.bat
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/usage.rst.distrib
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/widgets.rst.distrib
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/docs/widgets_doc.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1737 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/pyproject.toml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      430 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/pytest.ini
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.218443 django-mongoengine-filter-0.4.0/requirements/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       70 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/code_style.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1904 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/code_style.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       18 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/common.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      263 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/common.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       13 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/debug.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      947 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/debug.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       45 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/dev.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4273 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/dev.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_2_2.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1790 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_2_2.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_3_0.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1822 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_3_0.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_3_1.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1822 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_3_1.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_3_2.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1822 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_3_2.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_4_0.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1791 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_4_0.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_4_1.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1791 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/django_4_1.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/docs.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1102 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/docs.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/documentation.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2769 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/documentation.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      103 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/test.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1538 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/test.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/testing.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1541 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements/testing.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       10 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/requirements.txt
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.218443 django-mongoengine-filter-0.4.0/scripts/
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/scripts/black.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      166 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/scripts/build_docs.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      406 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/scripts/clean_up.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      887 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/scripts/compile_requirements.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       37 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/scripts/create_dirs.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       62 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/scripts/install.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       49 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/scripts/isort.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      157 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/scripts/make_release.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/scripts/migrate.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      288 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/scripts/rebuild_docs.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      448 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/scripts/runserver.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      207 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/scripts/uninstall.sh
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       67 2022-12-25 00:00:06.222443 django-mongoengine-filter-0.4.0/setup.cfg
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2210 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/setup.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.218443 django-mongoengine-filter-0.4.0/tests/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/tests/__init__.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.218443 django-mongoengine-filter-0.4.0/tests/dfm_app/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/tests/dfm_app/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      471 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/tests/dfm_app/constants.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      883 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/dfm_app/documents.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      872 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/tests/dfm_app/filters.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.202443 django-mongoengine-filter-0.4.0/tests/dfm_app/templates/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.222443 django-mongoengine-filter-0.4.0/tests/dfm_app/templates/dfm_app/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      126 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.0/tests/dfm_app/templates/dfm_app/person_list.html
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      602 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/dfm_app/views.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.222443 django-mongoengine-filter-0.4.0/tests/factories/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/factories/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      652 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/factories/person.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      826 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/manage.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-25 00:00:06.222443 django-mongoengine-filter-0.4.0/tests/settings/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/settings/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1330 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/settings/base.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1482 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/settings/dev.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      356 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/settings/helpers.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/settings/test.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3331 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/test_filters.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      262 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tests/urls.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      772 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.0/tox.ini
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.268861 django-mongoengine-filter-0.4.1/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      156 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/.coveragerc
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/.coveralls.yml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/.env
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.256861 django-mongoengine-filter-0.4.1/.github/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.260861 django-mongoengine-filter-0.4.1/.github/workflows/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2865 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/.github/workflows/test.yml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      743 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/.gitignore
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1473 2023-02-23 20:49:07.000000 django-mongoengine-filter-0.4.1/.pre-commit-config.yaml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      226 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/.pre-commit-hooks.yaml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1534 2023-02-23 21:32:09.000000 django-mongoengine-filter-0.4.1/CHANGELOG.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/CREDITS.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/LICENSE_GPL2.0.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/LICENSE_LGPL_2.1.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      201 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/MANIFEST.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     7333 2023-02-23 21:32:55.268861 django-mongoengine-filter-0.4.1/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5761 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.260861 django-mongoengine-filter-0.4.1/django_mongoengine_filter/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      680 2023-02-23 21:31:00.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      559 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter/compat.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1246 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter/fields.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     7912 2023-02-23 21:30:39.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter/filters.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    13262 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter/filterset.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.256861 django-mongoengine-filter-0.4.1/django_mongoengine_filter/locale/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.256861 django-mongoengine-filter-0.4.1/django_mongoengine_filter/locale/fr/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.260861 django-mongoengine-filter-0.4.1/django_mongoengine_filter/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3640 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter/views.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3441 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter/widgets.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.260861 django-mongoengine-filter-0.4.1/django_mongoengine_filter.egg-info/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     7333 2023-02-23 21:32:55.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2488 2023-02-23 21:32:55.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2023-02-23 21:32:55.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2022-12-24 23:02:49.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter.egg-info/not-zip-safe
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        9 2023-02-23 21:32:55.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter.egg-info/requires.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       32 2023-02-23 21:32:55.000000 django-mongoengine-filter-0.4.1/django_mongoengine_filter.egg-info/top_level.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      333 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/docker-compose.yml
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.260861 django-mongoengine-filter-0.4.1/docs/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/docs/Makefile
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/docs/changelog.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    10730 2023-02-23 20:13:46.000000 django-mongoengine-filter-0.4.1/docs/conf.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    10730 2023-02-23 20:13:46.000000 django-mongoengine-filter-0.4.1/docs/conf.py.distrib
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      216 2023-02-23 20:13:46.000000 django-mongoengine-filter-0.4.1/docs/documentation.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4004 2023-02-23 20:13:46.000000 django-mongoengine-filter-0.4.1/docs/filters.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/docs/index.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/docs/index.rst.distrib
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/docs/make.bat
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     9031 2023-02-23 20:13:46.000000 django-mongoengine-filter-0.4.1/docs/usage.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      648 2023-02-23 20:13:46.000000 django-mongoengine-filter-0.4.1/docs/widgets.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1737 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/pyproject.toml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      430 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/pytest.ini
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.264861 django-mongoengine-filter-0.4.1/requirements/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       70 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/code_style.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1904 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/code_style.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       18 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/common.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      263 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/common.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       13 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/debug.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      947 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/debug.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       45 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/dev.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4273 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/dev.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_2_2.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1790 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_2_2.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_3_0.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1822 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_3_0.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_3_1.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1822 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_3_1.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_3_2.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1822 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_3_2.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_4_0.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1791 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_4_0.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       42 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_4_1.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1791 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/django_4_1.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/docs.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1102 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/docs.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/documentation.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2769 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/documentation.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      103 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/test.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1538 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/test.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/testing.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1541 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements/testing.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       10 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/requirements.txt
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.268861 django-mongoengine-filter-0.4.1/scripts/
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/scripts/black.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      168 2023-02-23 20:13:46.000000 django-mongoengine-filter-0.4.1/scripts/build_docs.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      406 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.1/scripts/clean_up.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      887 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/scripts/compile_requirements.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       37 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.1/scripts/create_dirs.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       62 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/scripts/install.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       49 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/scripts/isort.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      157 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/scripts/make_release.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.1/scripts/migrate.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      288 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/scripts/rebuild_docs.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      448 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.1/scripts/runserver.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      207 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.1/scripts/uninstall.sh
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       67 2023-02-23 21:32:55.268861 django-mongoengine-filter-0.4.1/setup.cfg
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2253 2023-02-23 21:32:19.000000 django-mongoengine-filter-0.4.1/setup.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.268861 django-mongoengine-filter-0.4.1/tests/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.1/tests/__init__.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.268861 django-mongoengine-filter-0.4.1/tests/dfm_app/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.1/tests/dfm_app/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      471 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.1/tests/dfm_app/constants.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      882 2023-02-23 20:19:50.000000 django-mongoengine-filter-0.4.1/tests/dfm_app/documents.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      871 2023-02-23 20:19:50.000000 django-mongoengine-filter-0.4.1/tests/dfm_app/filters.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.256861 django-mongoengine-filter-0.4.1/tests/dfm_app/templates/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.268861 django-mongoengine-filter-0.4.1/tests/dfm_app/templates/dfm_app/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      126 2022-12-24 22:54:41.000000 django-mongoengine-filter-0.4.1/tests/dfm_app/templates/dfm_app/person_list.html
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      602 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/tests/dfm_app/views.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.268861 django-mongoengine-filter-0.4.1/tests/factories/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/tests/factories/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      651 2023-02-23 20:19:50.000000 django-mongoengine-filter-0.4.1/tests/factories/person.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      826 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/tests/manage.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-02-23 21:32:55.268861 django-mongoengine-filter-0.4.1/tests/settings/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/tests/settings/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1330 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/tests/settings/base.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1482 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/tests/settings/dev.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      356 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/tests/settings/helpers.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/tests/settings/test.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3331 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/tests/test_filters.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      262 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/tests/urls.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      772 2022-12-24 23:56:03.000000 django-mongoengine-filter-0.4.1/tox.ini
```

### Comparing `django-mongoengine-filter-0.4.0/.github/workflows/test.yml` & `django-mongoengine-filter-0.4.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/.gitignore` & `django-mongoengine-filter-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/.pre-commit-config.yaml` & `django-mongoengine-filter-0.4.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -10,43 +10,43 @@
       - id: detect-secrets
         name: Detect secrets
         language: python
         entry: detect-secrets-hook
         args: ['--baseline', '.secrets.baseline']
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
         exclude: "data/"
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-toml
       - id: check-added-large-files
       - id: debug-statements
       - id: check-merge-conflict
 
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.1.0
     hooks:
       - id: black
         name: black
         files: .
         args: [ "--config", "pyproject.toml" ]
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         name: isort
         files: .
         args: [ "--settings-path", "pyproject.toml", "--profile=black" ]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.106
+    rev: v0.0.252
     hooks:
       - id: ruff
         name: lint
         files: .
         args: [ "--config", "pyproject.toml" ]
 
 #  - repo: https://github.com/asottile/pyupgrade
```

### Comparing `django-mongoengine-filter-0.4.0/CHANGELOG.rst` & `django-mongoengine-filter-0.4.1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 - It's always safe to upgrade within the same minor version (for example, from
   0.3 to 0.3.4).
 - Minor version changes might be backwards incompatible. Read the
   release notes carefully before upgrading (for example, when upgrading from
   0.3.4 to 0.4).
 - All backwards incompatible changes are mentioned in this document.
 
+0.4.1
+-----
+2023-02-23
+
+- Fix issue with adding ``help_text``.
+
 0.4.0
 -----
 2022-12-24
 
 - Drop support for Python < 3.7.
 - Drop support for Django < 2.2.
 - Tested against Python 3.9, 3.10 and 3.11.
```

### Comparing `django-mongoengine-filter-0.4.0/PKG-INFO` & `django-mongoengine-filter-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: django-mongoengine-filter
-Version: 0.4.0
+Version: 0.4.1
 Summary: django-mongoengine-filter is a reusable Django application inspired from django-filter for allowing mongoengine users to filter querysets dynamically.
 Home-page: https://github.com/barseghyanartur/django-mongoengine-filter
 Author: Artur Barseghyhan
 Author-email: artur.barseghyan@gmail.com
 License: GPL-2.0-only OR LGPL-2.1-or-later
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/django-mongoengine-filter/issues
 Project-URL: Documentation, https://django-mongoengine-filter.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/django-mongoengine-filter
 Project-URL: Changelog, https://django-mongoengine-filter.readthedocs.io/en/latest/changelog.html
+Keywords: mongoengine,django-filter
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Requires-Python: >=2.7
+Requires-Python: >=3.7
 License-File: LICENSE_GPL2.0.txt
 License-File: LICENSE_LGPL_2.1.txt
 
 =========================
 django-mongoengine-filter
 =========================
 ``django-mongoengine-filter`` is a reusable Django application for allowing
```

### Comparing `django-mongoengine-filter-0.4.0/README.rst` & `django-mongoengine-filter-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/django_mongoengine_filter/__init__.py` & `django-mongoengine-filter-0.4.1/django_mongoengine_filter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .filters import *  # noqa
 from .filterset import FilterSet
 
-VERSION = (0, 4, 0)
+VERSION = (0, 4, 1)
 
 __title__ = "django-mongoengine-filter"
 __version__ = ".".join([str(_i) for _i in VERSION])
 __author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
 __copyright__ = "2019-2022 Artur Barseghyan"
 __license__ = "GPL 2.0/LGPL 2.1"
 __all__ = (  # noqa
```

### Comparing `django-mongoengine-filter-0.4.0/django_mongoengine_filter/compat.py` & `django-mongoengine-filter-0.4.1/django_mongoengine_filter/compat.py`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/django_mongoengine_filter/fields.py` & `django-mongoengine-filter-0.4.1/django_mongoengine_filter/fields.py`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/django_mongoengine_filter/filters.py` & `django-mongoengine-filter-0.4.1/django_mongoengine_filter/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,19 @@
 
         self.creation_counter = Filter.creation_counter
         Filter.creation_counter += 1
 
     @property
     def field(self):
         if not hasattr(self, "_field"):
-            help_text = _("This is an exclusion filter") if self.exclude else ""
+            help_text = (
+                _("This is an exclusion filter")
+                if self.exclude
+                else self.extra.pop("help_text", "")
+            )
             if self.lookup_type is None or isinstance(
                 self.lookup_type, (list, tuple)
             ):
                 if self.lookup_type is None:
                     lookup = [(x, x) for x in LOOKUP_TYPES]
                 else:
                     lookup = [
```

### Comparing `django-mongoengine-filter-0.4.0/django_mongoengine_filter/filterset.py` & `django-mongoengine-filter-0.4.1/django_mongoengine_filter/filterset.py`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/django_mongoengine_filter/views.py` & `django-mongoengine-filter-0.4.1/django_mongoengine_filter/views.py`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/django_mongoengine_filter/widgets.py` & `django-mongoengine-filter-0.4.1/django_mongoengine_filter/widgets.py`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/django_mongoengine_filter.egg-info/PKG-INFO` & `django-mongoengine-filter-0.4.1/django_mongoengine_filter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: django-mongoengine-filter
-Version: 0.4.0
+Version: 0.4.1
 Summary: django-mongoengine-filter is a reusable Django application inspired from django-filter for allowing mongoengine users to filter querysets dynamically.
 Home-page: https://github.com/barseghyanartur/django-mongoengine-filter
 Author: Artur Barseghyhan
 Author-email: artur.barseghyan@gmail.com
 License: GPL-2.0-only OR LGPL-2.1-or-later
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/django-mongoengine-filter/issues
 Project-URL: Documentation, https://django-mongoengine-filter.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/django-mongoengine-filter
 Project-URL: Changelog, https://django-mongoengine-filter.readthedocs.io/en/latest/changelog.html
+Keywords: mongoengine,django-filter
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Requires-Python: >=2.7
+Requires-Python: >=3.7
 License-File: LICENSE_GPL2.0.txt
 License-File: LICENSE_LGPL_2.1.txt
 
 =========================
 django-mongoengine-filter
 =========================
 ``django-mongoengine-filter`` is a reusable Django application for allowing
```

### Comparing `django-mongoengine-filter-0.4.0/django_mongoengine_filter.egg-info/SOURCES.txt` & `django-mongoengine-filter-0.4.1/django_mongoengine_filter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,22 +33,20 @@
 django_mongoengine_filter.egg-info/top_level.txt
 django_mongoengine_filter/locale/fr/LC_MESSAGES/django.po
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
 docs/conf.py.distrib
 docs/documentation.rst
-docs/filters.rst.distrib
-docs/filters_doc.rst
+docs/filters.rst
 docs/index.rst
 docs/index.rst.distrib
 docs/make.bat
-docs/usage.rst.distrib
-docs/widgets.rst.distrib
-docs/widgets_doc.rst
+docs/usage.rst
+docs/widgets.rst
 requirements/code_style.in
 requirements/code_style.txt
 requirements/common.in
 requirements/common.txt
 requirements/debug.in
 requirements/debug.txt
 requirements/dev.in
```

### Comparing `django-mongoengine-filter-0.4.0/docs/conf.py` & `django-mongoengine-filter-0.4.1/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,75 +15,33 @@
 import sys
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # sys.path.insert(0, os.path.abspath('.'))
 
-sys.path.insert(0, os.path.abspath("."))
-sys.path.insert(0, os.path.abspath("./tests"))
+sys.path.insert(0, os.path.abspath(".."))
+sys.path.insert(0, os.path.abspath("../tests"))
 try:
     import django_mongoengine_filter
     from tests import settings as docs_settings
 
     version = django_mongoengine_filter.__version__
     project = django_mongoengine_filter.__title__
     copyright = django_mongoengine_filter.__copyright__
 except Exception:
     version = "0.1"
     project = "django-filter-mongoengine"
     copyright = "2019, Artur Barseghyan <artur.barseghyan@gmail.com>"
 
-    class Settings:
-        pass
-
-    docs_settings = Settings()
-    docs_settings.DATABASES = {
-        "default": {"ENGINE": "django.db.backends.sqlite3", "NAME": ":memory:"}
-    }
-
-    docs_settings.SECRET_KEY = "top-secret"
-
-    docs_settings.INSTALLED_APPS = [
-        "django.contrib.admin",
-        "django.contrib.auth",
-        "django.contrib.contenttypes",
-        "django.contrib.sessions",
-        "django.contrib.messages",
-        "django.contrib.staticfiles",
-        # Third party
-        "dfm_app",
-    ]
-
-    docs_settings.ROOT_URLCONF = "urls"
-
-    docs_settings.TEMPLATES = [
-        {
-            "BACKEND": "django.template.backends.django.DjangoTemplates",
-            "DIRS": [],
-            "APP_DIRS": True,
-            "OPTIONS": {
-                "context_processors": [
-                    "django.template.context_processors.debug",
-                    "django.template.context_processors.request",
-                    "django.contrib.auth.context_processors.auth",
-                    "django.contrib.messages.context_processors.messages",
-                ]
-            },
-        }
-    ]
-
-    docs_settings.ALLOWED_HOSTS = ["*", "127.0.0.1", "localhost"]
-
 # -- Django configuration ------------------------------------------------------
-from django.conf import settings  # noqa
-
-if not settings.configured:
-    settings.configure(**docs_settings.__dict__)
+os.environ["DJANGO_SETTINGS_MODULE"] = "settings.dev"
+import django
 
+django.setup()
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
```

### Comparing `django-mongoengine-filter-0.4.0/docs/conf.py.distrib` & `django-mongoengine-filter-0.4.1/docs/conf.py.distrib`

 * *Files 12% similar despite different names*

```diff
@@ -15,75 +15,33 @@
 import sys
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # sys.path.insert(0, os.path.abspath('.'))
 
-sys.path.insert(0, os.path.abspath("."))
-sys.path.insert(0, os.path.abspath("./tests"))
+sys.path.insert(0, os.path.abspath(".."))
+sys.path.insert(0, os.path.abspath("../tests"))
 try:
     import django_mongoengine_filter
     from tests import settings as docs_settings
 
     version = django_mongoengine_filter.__version__
     project = django_mongoengine_filter.__title__
     copyright = django_mongoengine_filter.__copyright__
 except Exception:
     version = "0.1"
     project = "django-filter-mongoengine"
     copyright = "2019, Artur Barseghyan <artur.barseghyan@gmail.com>"
 
-    class Settings:
-        pass
-
-    docs_settings = Settings()
-    docs_settings.DATABASES = {
-        "default": {"ENGINE": "django.db.backends.sqlite3", "NAME": ":memory:"}
-    }
-
-    docs_settings.SECRET_KEY = "top-secret"
-
-    docs_settings.INSTALLED_APPS = [
-        "django.contrib.admin",
-        "django.contrib.auth",
-        "django.contrib.contenttypes",
-        "django.contrib.sessions",
-        "django.contrib.messages",
-        "django.contrib.staticfiles",
-        # Third party
-        "dfm_app",
-    ]
-
-    docs_settings.ROOT_URLCONF = "urls"
-
-    docs_settings.TEMPLATES = [
-        {
-            "BACKEND": "django.template.backends.django.DjangoTemplates",
-            "DIRS": [],
-            "APP_DIRS": True,
-            "OPTIONS": {
-                "context_processors": [
-                    "django.template.context_processors.debug",
-                    "django.template.context_processors.request",
-                    "django.contrib.auth.context_processors.auth",
-                    "django.contrib.messages.context_processors.messages",
-                ]
-            },
-        }
-    ]
-
-    docs_settings.ALLOWED_HOSTS = ["*", "127.0.0.1", "localhost"]
-
 # -- Django configuration ------------------------------------------------------
-from django.conf import settings  # noqa
-
-if not settings.configured:
-    settings.configure(**docs_settings.__dict__)
+os.environ["DJANGO_SETTINGS_MODULE"] = "settings.dev"
+import django
 
+django.setup()
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
```

### Comparing `django-mongoengine-filter-0.4.0/docs/filters_doc.rst` & `django-mongoengine-filter-0.4.1/docs/filters.rst`

 * *Files 2% similar despite different names*

```diff
@@ -101,45 +101,46 @@
 ~~~~~~~~~~
 
 The django.form Widget class which will represent the ``Filter``.  In addition
 to the widgets that are included with Django that you can use there are
 additional ones that django-filter provides which may be useful:
 
     * ``django_filters.widgets.LinkWidget`` -- this displays the options in a
-      mannner similar to the way the Django Admin does, as a series of links.
+      manner similar to the way the Django Admin does, as a series of links.
       The link for the selected option will have ``class="selected"``.
 
 ``action``
 ~~~~~~~~~~
 
-An optional callable that tells the filter how to handle the queryset.  It
-recieves a ``QuerySet`` and the value to filter on and should return a
+An optional callable that tells the filter how to handle the queryset. It
+receives a ``QuerySet`` and the value to filter on and should return a
 ``Queryset`` that is filtered appropriately.
 
 ``lookup_type``
 ~~~~~~~~~~~~~~~
 
 The type of lookup that should be performed using the Django ORM.  All the
 normal options are allowed, and should be provided as a string.  You can also
 provide either ``None`` or a ``list`` or a ``tuple``.  If ``None`` is provided,
-then the user can select the lookup type from all the ones available in the Django
-ORM.  If a ``list`` or ``tuple`` is provided, then the user can select from those
-options.
+then the user can select the lookup type from all the ones available in the
+Django ORM.  If a ``list`` or ``tuple`` is provided, then the user can select
+from those options.
 
 ``distinct``
 ~~~~~~~~~~~~
 
 A boolean value that specifies whether the Filter will use distinct on the
-queryset. This option can be used to eliminate duplicate results when using filters that span related models. Defaults to ``False``.
+queryset. This option can be used to eliminate duplicate results when using
+filters that span related models. Defaults to ``False``.
 
 ``exclude``
 ~~~~~~~~~~~
 
-A boolean value that specifies whether the Filter should use ``filter`` or ``exclude`` on the queryset.
-Defaults to ``False``.
+A boolean value that specifies whether the Filter should use ``filter``
+or ``exclude`` on the queryset. Defaults to ``False``.
 
 
 ``**kwargs``
 ~~~~~~~~~~~~
 
 Any extra keyword arguments will be provided to the accompanying form Field.
 This can be used to provide arguments like ``choices`` or ``queryset``.
```

### Comparing `django-mongoengine-filter-0.4.0/pyproject.toml` & `django-mongoengine-filter-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/code_style.txt` & `django-mongoengine-filter-0.4.1/requirements/code_style.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/debug.txt` & `django-mongoengine-filter-0.4.1/requirements/debug.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/dev.txt` & `django-mongoengine-filter-0.4.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/django_2_2.txt` & `django-mongoengine-filter-0.4.1/requirements/django_2_2.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/django_3_0.txt` & `django-mongoengine-filter-0.4.1/requirements/django_3_0.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/django_3_1.txt` & `django-mongoengine-filter-0.4.1/requirements/django_3_1.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/django_3_2.txt` & `django-mongoengine-filter-0.4.1/requirements/django_3_2.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/django_4_0.txt` & `django-mongoengine-filter-0.4.1/requirements/django_4_0.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/django_4_1.txt` & `django-mongoengine-filter-0.4.1/requirements/django_4_1.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/docs.txt` & `django-mongoengine-filter-0.4.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/documentation.txt` & `django-mongoengine-filter-0.4.1/requirements/documentation.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/test.txt` & `django-mongoengine-filter-0.4.1/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/requirements/testing.txt` & `django-mongoengine-filter-0.4.1/requirements/testing.txt`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/scripts/compile_requirements.sh` & `django-mongoengine-filter-0.4.1/scripts/compile_requirements.sh`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/setup.py` & `django-mongoengine-filter-0.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,21 +16,22 @@
     "pytest-django",
     "pytest-cov",
     "tox",
 ]
 
 setup(
     name="django-mongoengine-filter",
-    version="0.4.0",
+    version="0.4.1",
     description=(
         "django-mongoengine-filter is a reusable Django application inspired "
         "from django-filter for allowing mongoengine users to filter querysets "
         "dynamically."
     ),
     long_description=readme,
+    keywords="mongoengine, django-filter",
     author="Artur Barseghyhan",
     author_email="artur.barseghyan@gmail.com",
     url="https://github.com/barseghyanartur/django-mongoengine-filter",
     project_urls={
         "Bug Tracker": "https://github.com/barseghyanartur/"
         "django-mongoengine-filter/issues",
         "Documentation": "https://django-mongoengine-filter.readthedocs.io/",
@@ -54,13 +55,13 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Framework :: Django",
     ],
-    python_requires=">=2.7",
+    python_requires=">=3.7",
     install_requires=(install_requires + extras_require),
     tests_require=tests_require,
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `django-mongoengine-filter-0.4.0/tests/dfm_app/documents.py` & `django-mongoengine-filter-0.4.1/tests/dfm_app/documents.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from .constants import GENDER_MALE, GENDERS, PROFILE_TYPE_FREE, PROFILE_TYPES
 
 __all__ = ("Person",)
 
 
 class Person(document.Document):
-
     name = fields.StringField(
         required=True, max_length=255, default="Robot", verbose_name="Name"
     )
     age = fields.IntField(required=True, verbose_name="Age")
     num_fingers = fields.IntField(
         required=False, verbose_name="Number of fingers"
     )
```

### Comparing `django-mongoengine-filter-0.4.0/tests/dfm_app/filters.py` & `django-mongoengine-filter-0.4.1/tests/dfm_app/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from .documents import Person
 
 __all__ = ("PersonFilter",)
 
 
 class PersonFilter(django_mongoengine_filter.FilterSet):
-
     profile_type = django_mongoengine_filter.StringFilter()
     ten_fingers = django_mongoengine_filter.MethodFilter(
         action="ten_fingers_filter"
     )
     # agnostic = django_mongoengine_filter.BooleanFilter()
     # gender = django_mongoengine_filter.StringFilter()
     # contract_type = django_mongoengine_filter.StringFilter()
```

### Comparing `django-mongoengine-filter-0.4.0/tests/dfm_app/views.py` & `django-mongoengine-filter-0.4.1/tests/dfm_app/views.py`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/tests/factories/person.py` & `django-mongoengine-filter-0.4.1/tests/factories/person.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 def build_factory(cls, specified_fields=None):
     return factory.build(
         dict, FACTORY_CLASS=cls, **specified_fields if specified_fields else {}
     )
 
 
 class PersonFactory(factory.mongoengine.MongoEngineFactory):
-
     name = factory.Faker("word")
     age = factory.Faker("pyint")
     num_fingers = factory.Faker("pyint")
     profile_type = factory.fuzzy.FuzzyChoice(choices=PROFILE_TYPES)
     gender = factory.fuzzy.FuzzyChoice(choices=GENDERS)
 
     class Meta:
```

### Comparing `django-mongoengine-filter-0.4.0/tests/manage.py` & `django-mongoengine-filter-0.4.1/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/tests/settings/base.py` & `django-mongoengine-filter-0.4.1/tests/settings/base.py`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/tests/settings/dev.py` & `django-mongoengine-filter-0.4.1/tests/settings/dev.py`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/tests/test_filters.py` & `django-mongoengine-filter-0.4.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-mongoengine-filter-0.4.0/tox.ini` & `django-mongoengine-filter-0.4.1/tox.ini`

 * *Files identical despite different names*

