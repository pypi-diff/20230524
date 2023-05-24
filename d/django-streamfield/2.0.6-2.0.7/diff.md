# Comparing `tmp/django-streamfield-2.0.6.tar.gz` & `tmp/django-streamfield-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-streamfield-2.0.6.tar", last modified: Tue Apr  4 08:08:02 2023, max compression
+gzip compressed data, was "django-streamfield-2.0.7.tar", last modified: Tue Apr  4 11:37:03 2023, max compression
```

## Comparing `django-streamfield-2.0.6.tar` & `django-streamfield-2.0.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.129180 django-streamfield-2.0.6/
--rw-r--r--   0 raagin     (501) staff       (20)     1309 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/LICENSE
--rw-r--r--   0 raagin     (501) staff       (20)      153 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/MANIFEST.in
--rw-r--r--   0 raagin     (501) staff       (20)    17260 2023-04-04 08:08:02.128082 django-streamfield-2.0.6/PKG-INFO
--rw-r--r--   0 raagin     (501) staff       (20)    16089 2023-04-04 08:00:35.000000 django-streamfield-2.0.6/README.md
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.113095 django-streamfield-2.0.6/django_streamfield.egg-info/
--rw-r--r--   0 raagin     (501) staff       (20)    17260 2023-04-04 08:08:02.000000 django-streamfield-2.0.6/django_streamfield.egg-info/PKG-INFO
--rw-r--r--   0 raagin     (501) staff       (20)     1702 2023-04-04 08:08:02.000000 django-streamfield-2.0.6/django_streamfield.egg-info/SOURCES.txt
--rw-r--r--   0 raagin     (501) staff       (20)        1 2023-04-04 08:08:02.000000 django-streamfield-2.0.6/django_streamfield.egg-info/dependency_links.txt
--rw-r--r--   0 raagin     (501) staff       (20)        1 2023-03-29 12:16:43.000000 django-streamfield-2.0.6/django_streamfield.egg-info/not-zip-safe
--rw-r--r--   0 raagin     (501) staff       (20)       12 2023-04-04 08:08:02.000000 django-streamfield-2.0.6/django_streamfield.egg-info/top_level.txt
--rw-r--r--   0 raagin     (501) staff       (20)       38 2023-04-04 08:08:02.129333 django-streamfield-2.0.6/setup.cfg
--rw-r--r--   0 raagin     (501) staff       (20)     1421 2023-04-04 08:00:44.000000 django-streamfield-2.0.6/setup.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.117058 django-streamfield-2.0.6/streamfield/
--rw-r--r--   0 raagin     (501) staff       (20)       38 2023-04-04 08:00:51.000000 django-streamfield-2.0.6/streamfield/__init__.py
--rw-r--r--   0 raagin     (501) staff       (20)     2917 2023-03-29 12:13:38.000000 django-streamfield-2.0.6/streamfield/admin.py
--rw-r--r--   0 raagin     (501) staff       (20)       95 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/apps.py
--rw-r--r--   0 raagin     (501) staff       (20)     8275 2023-04-03 14:01:51.000000 django-streamfield-2.0.6/streamfield/base.py
--rw-r--r--   0 raagin     (501) staff       (20)     3612 2023-04-04 07:54:11.000000 django-streamfield-2.0.6/streamfield/fields.py
--rw-r--r--   0 raagin     (501) staff       (20)      280 2023-03-29 19:42:23.000000 django-streamfield-2.0.6/streamfield/forms.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.108297 django-streamfield-2.0.6/streamfield/locale/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.107977 django-streamfield-2.0.6/streamfield/locale/en/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.117787 django-streamfield-2.0.6/streamfield/locale/en/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)      380 2023-03-27 20:03:39.000000 django-streamfield-2.0.6/streamfield/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     2618 2023-03-27 19:59:52.000000 django-streamfield-2.0.6/streamfield/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.108176 django-streamfield-2.0.6/streamfield/locale/it/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.118674 django-streamfield-2.0.6/streamfield/locale/it/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)     1855 2023-03-27 20:03:39.000000 django-streamfield-2.0.6/streamfield/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     3337 2023-03-27 20:01:41.000000 django-streamfield-2.0.6/streamfield/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.108369 django-streamfield-2.0.6/streamfield/locale/ru/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.119557 django-streamfield-2.0.6/streamfield/locale/ru/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)     2398 2023-03-27 20:03:39.000000 django-streamfield-2.0.6/streamfield/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     4940 2023-03-27 20:02:50.000000 django-streamfield-2.0.6/streamfield/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 raagin     (501) staff       (20)       57 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/models.py
--rw-r--r--   0 raagin     (501) staff       (20)      787 2023-03-30 07:54:45.000000 django-streamfield-2.0.6/streamfield/settings.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.108563 django-streamfield-2.0.6/streamfield/static/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.120818 django-streamfield-2.0.6/streamfield/static/streamfield/
--rw-r--r--   0 raagin     (501) staff       (20)      267 2023-04-04 08:05:59.000000 django-streamfield-2.0.6/streamfield/static/streamfield/admin_popup_response.js
--rw-r--r--   0 raagin     (501) staff       (20)     9523 2023-04-04 08:05:59.000000 django-streamfield-2.0.6/streamfield/static/streamfield/streamfield_widget.css
--rw-r--r--   0 raagin     (501) staff       (20)   302084 2023-04-04 08:05:59.000000 django-streamfield-2.0.6/streamfield/static/streamfield/streamfield_widget.js
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.108767 django-streamfield-2.0.6/streamfield/templates/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.122657 django-streamfield-2.0.6/streamfield/templates/streamfield/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.124380 django-streamfield-2.0.6/streamfield/templates/streamfield/admin/
--rw-r--r--   0 raagin     (501) staff       (20)        6 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/templates/streamfield/admin/abstract_block_template.html
--rw-r--r--   0 raagin     (501) staff       (20)     2306 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/templates/streamfield/admin/change_form.html
--rw-r--r--   0 raagin     (501) staff       (20)      371 2023-03-25 15:18:30.000000 django-streamfield-2.0.6/streamfield/templates/streamfield/admin/change_form_render_template.html
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.126245 django-streamfield-2.0.6/streamfield/templates/streamfield/admin/fields/
--rw-r--r--   0 raagin     (501) staff       (20)       33 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/templates/streamfield/admin/fields/default.html
--rw-r--r--   0 raagin     (501) staff       (20)     1022 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/templates/streamfield/admin/fields/file_browse_widget.html
--rw-r--r--   0 raagin     (501) staff       (20)       15 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/templates/streamfield/admin/fields/select.html
--rw-r--r--   0 raagin     (501) staff       (20)       71 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/templates/streamfield/admin/fields/stream_field_widget.html
--rw-r--r--   0 raagin     (501) staff       (20)      367 2023-03-29 12:13:38.000000 django-streamfield-2.0.6/streamfield/templates/streamfield/admin/streamfield_popup_response.html
--rw-r--r--   0 raagin     (501) staff       (20)      341 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/templates/streamfield/default_block_tmpl.html
--rw-r--r--   0 raagin     (501) staff       (20)      444 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/templates/streamfield/streamfield_admin_help.html
--rw-r--r--   0 raagin     (501) staff       (20)      978 2023-04-01 05:58:20.000000 django-streamfield-2.0.6/streamfield/templates/streamfield/streamfield_widget.html
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 08:08:02.127303 django-streamfield-2.0.6/streamfield/templatetags/
--rw-r--r--   0 raagin     (501) staff       (20)        0 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/templatetags/__init__.py
--rw-r--r--   0 raagin     (501) staff       (20)     1314 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/templatetags/streamfield_tags.py
--rw-r--r--   0 raagin     (501) staff       (20)       60 2023-03-24 20:31:52.000000 django-streamfield-2.0.6/streamfield/tests.py
--rw-r--r--   0 raagin     (501) staff       (20)      996 2023-03-29 12:13:38.000000 django-streamfield-2.0.6/streamfield/urls.py
--rw-r--r--   0 raagin     (501) staff       (20)     1977 2023-03-30 07:55:09.000000 django-streamfield-2.0.6/streamfield/views.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.787025 django-streamfield-2.0.7/
+-rw-r--r--   0 raagin     (501) staff       (20)     1309 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/LICENSE
+-rw-r--r--   0 raagin     (501) staff       (20)      153 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/MANIFEST.in
+-rw-r--r--   0 raagin     (501) staff       (20)    17260 2023-04-04 11:37:03.785745 django-streamfield-2.0.7/PKG-INFO
+-rw-r--r--   0 raagin     (501) staff       (20)    16089 2023-04-04 11:36:35.000000 django-streamfield-2.0.7/README.md
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.762288 django-streamfield-2.0.7/django_streamfield.egg-info/
+-rw-r--r--   0 raagin     (501) staff       (20)    17260 2023-04-04 11:37:03.000000 django-streamfield-2.0.7/django_streamfield.egg-info/PKG-INFO
+-rw-r--r--   0 raagin     (501) staff       (20)     1702 2023-04-04 11:37:03.000000 django-streamfield-2.0.7/django_streamfield.egg-info/SOURCES.txt
+-rw-r--r--   0 raagin     (501) staff       (20)        1 2023-04-04 11:37:03.000000 django-streamfield-2.0.7/django_streamfield.egg-info/dependency_links.txt
+-rw-r--r--   0 raagin     (501) staff       (20)        1 2023-03-29 12:16:43.000000 django-streamfield-2.0.7/django_streamfield.egg-info/not-zip-safe
+-rw-r--r--   0 raagin     (501) staff       (20)       12 2023-04-04 11:37:03.000000 django-streamfield-2.0.7/django_streamfield.egg-info/top_level.txt
+-rw-r--r--   0 raagin     (501) staff       (20)       38 2023-04-04 11:37:03.787533 django-streamfield-2.0.7/setup.cfg
+-rw-r--r--   0 raagin     (501) staff       (20)     1421 2023-04-04 11:36:35.000000 django-streamfield-2.0.7/setup.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.767670 django-streamfield-2.0.7/streamfield/
+-rw-r--r--   0 raagin     (501) staff       (20)       38 2023-04-04 11:36:35.000000 django-streamfield-2.0.7/streamfield/__init__.py
+-rw-r--r--   0 raagin     (501) staff       (20)     2917 2023-03-29 12:13:38.000000 django-streamfield-2.0.7/streamfield/admin.py
+-rw-r--r--   0 raagin     (501) staff       (20)       95 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/apps.py
+-rw-r--r--   0 raagin     (501) staff       (20)     8275 2023-04-03 14:01:51.000000 django-streamfield-2.0.7/streamfield/base.py
+-rw-r--r--   0 raagin     (501) staff       (20)     3612 2023-04-04 07:54:11.000000 django-streamfield-2.0.7/streamfield/fields.py
+-rw-r--r--   0 raagin     (501) staff       (20)      280 2023-03-29 19:42:23.000000 django-streamfield-2.0.7/streamfield/forms.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.757876 django-streamfield-2.0.7/streamfield/locale/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.757507 django-streamfield-2.0.7/streamfield/locale/en/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.770011 django-streamfield-2.0.7/streamfield/locale/en/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)      380 2023-03-27 20:03:39.000000 django-streamfield-2.0.7/streamfield/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     2618 2023-03-27 19:59:52.000000 django-streamfield-2.0.7/streamfield/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.757737 django-streamfield-2.0.7/streamfield/locale/it/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.772027 django-streamfield-2.0.7/streamfield/locale/it/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)     1855 2023-03-27 20:03:39.000000 django-streamfield-2.0.7/streamfield/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     3337 2023-03-27 20:01:41.000000 django-streamfield-2.0.7/streamfield/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.757957 django-streamfield-2.0.7/streamfield/locale/ru/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.773230 django-streamfield-2.0.7/streamfield/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)     2398 2023-03-27 20:03:39.000000 django-streamfield-2.0.7/streamfield/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     4940 2023-03-27 20:02:50.000000 django-streamfield-2.0.7/streamfield/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 raagin     (501) staff       (20)       57 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/models.py
+-rw-r--r--   0 raagin     (501) staff       (20)      787 2023-03-30 07:54:45.000000 django-streamfield-2.0.7/streamfield/settings.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.758185 django-streamfield-2.0.7/streamfield/static/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.775222 django-streamfield-2.0.7/streamfield/static/streamfield/
+-rw-r--r--   0 raagin     (501) staff       (20)      267 2023-04-04 08:05:59.000000 django-streamfield-2.0.7/streamfield/static/streamfield/admin_popup_response.js
+-rw-r--r--   0 raagin     (501) staff       (20)     9523 2023-04-04 08:05:59.000000 django-streamfield-2.0.7/streamfield/static/streamfield/streamfield_widget.css
+-rw-r--r--   0 raagin     (501) staff       (20)   302377 2023-04-04 11:36:35.000000 django-streamfield-2.0.7/streamfield/static/streamfield/streamfield_widget.js
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.758412 django-streamfield-2.0.7/streamfield/templates/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.778395 django-streamfield-2.0.7/streamfield/templates/streamfield/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.781512 django-streamfield-2.0.7/streamfield/templates/streamfield/admin/
+-rw-r--r--   0 raagin     (501) staff       (20)        6 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/templates/streamfield/admin/abstract_block_template.html
+-rw-r--r--   0 raagin     (501) staff       (20)     2306 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/templates/streamfield/admin/change_form.html
+-rw-r--r--   0 raagin     (501) staff       (20)      371 2023-03-25 15:18:30.000000 django-streamfield-2.0.7/streamfield/templates/streamfield/admin/change_form_render_template.html
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.783738 django-streamfield-2.0.7/streamfield/templates/streamfield/admin/fields/
+-rw-r--r--   0 raagin     (501) staff       (20)       33 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/templates/streamfield/admin/fields/default.html
+-rw-r--r--   0 raagin     (501) staff       (20)     1022 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/templates/streamfield/admin/fields/file_browse_widget.html
+-rw-r--r--   0 raagin     (501) staff       (20)       15 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/templates/streamfield/admin/fields/select.html
+-rw-r--r--   0 raagin     (501) staff       (20)       71 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/templates/streamfield/admin/fields/stream_field_widget.html
+-rw-r--r--   0 raagin     (501) staff       (20)      367 2023-03-29 12:13:38.000000 django-streamfield-2.0.7/streamfield/templates/streamfield/admin/streamfield_popup_response.html
+-rw-r--r--   0 raagin     (501) staff       (20)      341 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/templates/streamfield/default_block_tmpl.html
+-rw-r--r--   0 raagin     (501) staff       (20)      444 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/templates/streamfield/streamfield_admin_help.html
+-rw-r--r--   0 raagin     (501) staff       (20)      978 2023-04-01 05:58:20.000000 django-streamfield-2.0.7/streamfield/templates/streamfield/streamfield_widget.html
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2023-04-04 11:37:03.784479 django-streamfield-2.0.7/streamfield/templatetags/
+-rw-r--r--   0 raagin     (501) staff       (20)        0 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/templatetags/__init__.py
+-rw-r--r--   0 raagin     (501) staff       (20)     1314 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/templatetags/streamfield_tags.py
+-rw-r--r--   0 raagin     (501) staff       (20)       60 2023-03-24 20:31:52.000000 django-streamfield-2.0.7/streamfield/tests.py
+-rw-r--r--   0 raagin     (501) staff       (20)      996 2023-03-29 12:13:38.000000 django-streamfield-2.0.7/streamfield/urls.py
+-rw-r--r--   0 raagin     (501) staff       (20)     1977 2023-03-30 07:55:09.000000 django-streamfield-2.0.7/streamfield/views.py
```

### Comparing `django-streamfield-2.0.6/LICENSE` & `django-streamfield-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/PKG-INFO` & `django-streamfield-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-streamfield
-Version: 2.0.6
+Version: 2.0.7
 Summary: StreamField for native Django Admin or with Grappelli
 Home-page: https://github.com/raagin/django-streamfield
 Author: Yury Lapshinov
 Author-email: y.raagin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.0.6
+Stable version: 2.0.7
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.0.6/README.md` & `django-streamfield-2.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.0.6
+Stable version: 2.0.7
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.0.6/django_streamfield.egg-info/PKG-INFO` & `django-streamfield-2.0.7/django_streamfield.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-streamfield
-Version: 2.0.6
+Version: 2.0.7
 Summary: StreamField for native Django Admin or with Grappelli
 Home-page: https://github.com/raagin/django-streamfield
 Author: Yury Lapshinov
 Author-email: y.raagin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.0.6
+Stable version: 2.0.7
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.0.6/django_streamfield.egg-info/SOURCES.txt` & `django-streamfield-2.0.7/django_streamfield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/setup.py` & `django-streamfield-2.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-streamfield",
-    version="2.0.6",
+    version="2.0.7",
     author="Yury Lapshinov",
     author_email="y.raagin@gmail.com",
     description="StreamField for native Django Admin or with Grappelli",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raagin/django-streamfield",
     packages=setuptools.find_packages(exclude=['test_project', 'frontend']),
```

### Comparing `django-streamfield-2.0.6/streamfield/admin.py` & `django-streamfield-2.0.7/streamfield/admin.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/base.py` & `django-streamfield-2.0.7/streamfield/base.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/fields.py` & `django-streamfield-2.0.7/streamfield/fields.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/locale/en/LC_MESSAGES/django.po` & `django-streamfield-2.0.7/streamfield/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/locale/it/LC_MESSAGES/django.mo` & `django-streamfield-2.0.7/streamfield/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/locale/it/LC_MESSAGES/django.po` & `django-streamfield-2.0.7/streamfield/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/locale/ru/LC_MESSAGES/django.mo` & `django-streamfield-2.0.7/streamfield/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/locale/ru/LC_MESSAGES/django.po` & `django-streamfield-2.0.7/streamfield/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/settings.py` & `django-streamfield-2.0.7/streamfield/settings.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/static/streamfield/streamfield_widget.css` & `django-streamfield-2.0.7/streamfield/static/streamfield/streamfield_widget.css`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/static/streamfield/streamfield_widget.js` & `django-streamfield-2.0.7/streamfield/static/streamfield/streamfield_widget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -3621,130 +3621,130 @@
                 n.d(t, {
                     $d: () => c,
                     $y: () => r.$y,
                     Ah: () => We,
                     B: () => r.B,
                     BK: () => r.BK,
                     Bj: () => r.Bj,
-                    Bz: () => dr,
-                    C3: () => kn,
+                    Bz: () => fr,
+                    C3: () => Cn,
                     C_: () => o.normalizeClass,
                     Cn: () => z,
                     EB: () => r.EB,
                     Eo: () => Qt,
-                    F4: () => Dn,
-                    FN: () => Wn,
-                    Fl: () => lr,
-                    G: () => Cr,
+                    F4: () => Mn,
+                    FN: () => Kn,
+                    Fl: () => ur,
+                    G: () => Tr,
                     HX: () => Y,
-                    HY: () => un,
-                    Ho: () => Mn,
+                    HY: () => dn,
+                    Ho: () => In,
                     IU: () => r.IU,
                     JJ: () => ae,
                     Jd: () => Ye,
                     KU: () => a,
                     Ko: () => ct,
                     LL: () => ot,
-                    MW: () => ur,
-                    MX: () => xr,
-                    Mr: () => Er,
+                    MW: () => dr,
+                    MX: () => Or,
+                    Mr: () => xr,
                     Nv: () => lt,
                     OT: () => r.OT,
                     Ob: () => Re,
                     P$: () => _e,
                     PG: () => r.PG,
                     Q2: () => it,
                     Q6: () => ke,
                     RC: () => Ae,
                     Rh: () => ue,
-                    Rr: () => hr,
+                    Rr: () => mr,
                     S3: () => l,
                     SU: () => r.SU,
                     U2: () => we,
-                    Uc: () => Sr,
-                    Uk: () => In,
+                    Uc: () => wr,
+                    Uk: () => jn,
                     Um: () => r.Um,
                     Us: () => Zt,
                     Vh: () => r.Vh,
                     WI: () => ut,
                     WL: () => r.WL,
-                    WY: () => fr,
-                    Wm: () => Nn,
+                    WY: () => pr,
+                    Wm: () => Rn,
                     Wu: () => s,
                     X3: () => r.X3,
                     XI: () => r.XI,
                     Xl: () => r.Xl,
                     Xn: () => qe,
-                    Y1: () => nr,
+                    Y1: () => rr,
                     Y3: () => b,
                     Y8: () => ye,
                     YP: () => pe,
                     YS: () => r.YS,
                     Yq: () => Je,
                     ZK: () => i,
                     ZM: () => r.ZM,
-                    Zq: () => wr,
-                    _: () => Pn,
+                    Zq: () => Er,
+                    _: () => Nn,
                     _A: () => o.camelize,
                     aZ: () => Ce,
-                    b9: () => pr,
+                    b9: () => hr,
                     bT: () => Ge,
                     bv: () => He,
                     cE: () => r.cE,
                     d1: () => Xe,
                     dD: () => q,
-                    dG: () => Vn,
+                    dG: () => $n,
                     dl: () => Me,
                     dq: () => r.dq,
                     ec: () => R,
-                    eq: () => Tr,
+                    eq: () => Ar,
                     f3: () => ce,
-                    h: () => _r,
+                    h: () => Sr,
                     hR: () => o.toHandlerKey,
-                    i8: () => kr,
-                    iD: () => wn,
+                    i8: () => Cr,
+                    iD: () => En,
                     iH: () => r.iH,
                     ic: () => ze,
-                    j4: () => En,
+                    j4: () => xn,
                     j5: () => o.normalizeStyle,
                     kC: () => o.capitalize,
-                    kq: () => Ln,
-                    l1: () => mr,
-                    lA: () => xn,
-                    lR: () => cn,
+                    kq: () => Fn,
+                    l1: () => gr,
+                    lA: () => On,
+                    lR: () => ln,
                     m0: () => le,
                     mW: () => T,
-                    mv: () => br,
+                    mv: () => _r,
                     mx: () => ft,
                     n4: () => te,
                     nK: () => Oe,
-                    nQ: () => Or,
+                    nQ: () => kr,
                     nZ: () => r.nZ,
                     oR: () => r.oR,
-                    of: () => rr,
-                    p1: () => yr,
-                    qG: () => pn,
-                    qZ: () => _n,
+                    of: () => or,
+                    p1: () => br,
+                    qG: () => hn,
+                    qZ: () => Sn,
                     qb: () => w,
                     qj: () => r.qj,
                     qq: () => r.qq,
-                    ry: () => Ar,
+                    ry: () => Pr,
                     sT: () => r.sT,
                     se: () => Ie,
-                    sv: () => fn,
-                    uE: () => jn,
-                    u_: () => vr,
+                    sv: () => pn,
+                    uE: () => Ln,
+                    u_: () => yr,
                     up: () => nt,
                     vl: () => Ke,
                     vs: () => o.normalizeProps,
                     w5: () => W,
                     wF: () => $e,
-                    wg: () => gn,
+                    wg: () => vn,
                     wy: () => Ze,
-                    xv: () => dn,
+                    xv: () => fn,
                     yT: () => r.yT,
                     yX: () => de,
                     zw: () => o.toDisplayString
                 });
                 var r = n(262),
                     o = n(577);
 
@@ -3970,21 +3970,21 @@
                 }
                 const Y = e => W;
 
                 function W(e, t = V, n) {
                     if (!t) return e;
                     if (e._n) return e;
                     const r = (...n) => {
-                        r._d && _n(-1);
+                        r._d && Sn(-1);
                         const o = H(t);
                         let i;
                         try {
                             i = e(...n)
                         } finally {
-                            H(o), r._d && _n(1)
+                            H(o), r._d && Sn(1)
                         }
                         return __VUE_PROD_DEVTOOLS__ && M(t), i
                     };
                     return r._n = !0, r._c = !0, r._d = !0, r
                 }
 
                 function K(e) {
@@ -4006,43 +4006,43 @@
                         inheritAttrs: v
                     } = e;
                     let y, b;
                     const _ = H(e);
                     try {
                         if (4 & n.shapeFlag) {
                             const e = i || r;
-                            y = Fn(f.call(e, e, p, s, m, h, g)), b = u
+                            y = Bn(f.call(e, e, p, s, m, h, g)), b = u
                         } else {
                             const e = t;
-                            0, y = Fn(e.length > 1 ? e(s, {
+                            0, y = Bn(e.length > 1 ? e(s, {
                                 attrs: u,
                                 slots: c,
                                 emit: d
                             }) : e(s, null)), b = t.props ? u : G(u)
                         }
                     } catch (t) {
-                        hn.length = 0, l(t, e, 1), y = Nn(fn)
+                        mn.length = 0, l(t, e, 1), y = Rn(pn)
                     }
                     let S = y;
                     if (b && !1 !== v) {
                         const e = Object.keys(b),
                             {
                                 shapeFlag: t
                             } = S;
-                        e.length && 7 & t && (a && e.some(o.isModelListener) && (b = X(b, a)), S = Mn(S, b))
+                        e.length && 7 & t && (a && e.some(o.isModelListener) && (b = X(b, a)), S = In(S, b))
                     }
-                    return n.dirs && (S = Mn(S), S.dirs = S.dirs ? S.dirs.concat(n.dirs) : n.dirs), n.transition && (S.transition = n.transition), y = S, H(_), y
+                    return n.dirs && (S = In(S), S.dirs = S.dirs ? S.dirs.concat(n.dirs) : n.dirs), n.transition && (S.transition = n.transition), y = S, H(_), y
                 }
 
                 function J(e) {
                     let t;
                     for (let n = 0; n < e.length; n++) {
                         const r = e[n];
-                        if (!xn(r)) return;
-                        if (r.type !== fn || "v-if" === r.children) {
+                        if (!On(r)) return;
+                        if (r.type !== pn || "v-if" === r.children) {
                             if (t) return;
                             t = r
                         }
                     }
                     return t
                 }
                 const G = e => {
@@ -4098,16 +4098,16 @@
                                     p = t.ssFallback,
                                     {
                                         activeBranch: h,
                                         pendingBranch: m,
                                         isInFallback: g,
                                         isHydrating: v
                                     } = d;
-                                if (m) d.pendingBranch = f, On(f, m) ? (c(m, f, d.hiddenContainer, null, o, d, i, s, a), d.deps <= 0 ? d.resolve() : g && (c(h, p, n, r, o, null, i, s, a), se(d, p))) : (d.pendingId++, v ? (d.isHydrating = !1, d.activeBranch = m) : l(m, o, d), d.deps = 0, d.effects.length = 0, d.hiddenContainer = u("div"), g ? (c(null, f, d.hiddenContainer, null, o, d, i, s, a), d.deps <= 0 ? d.resolve() : (c(h, p, n, r, o, null, i, s, a), se(d, p))) : h && On(f, h) ? (c(h, f, n, r, o, d, i, s, a), d.resolve(!0)) : (c(null, f, d.hiddenContainer, null, o, d, i, s, a), d.deps <= 0 && d.resolve()));
-                                else if (h && On(f, h)) c(h, f, n, r, o, d, i, s, a), se(d, f);
+                                if (m) d.pendingBranch = f, kn(f, m) ? (c(m, f, d.hiddenContainer, null, o, d, i, s, a), d.deps <= 0 ? d.resolve() : g && (c(h, p, n, r, o, null, i, s, a), se(d, p))) : (d.pendingId++, v ? (d.isHydrating = !1, d.activeBranch = m) : l(m, o, d), d.deps = 0, d.effects.length = 0, d.hiddenContainer = u("div"), g ? (c(null, f, d.hiddenContainer, null, o, d, i, s, a), d.deps <= 0 ? d.resolve() : (c(h, p, n, r, o, null, i, s, a), se(d, p))) : h && kn(f, h) ? (c(h, f, n, r, o, d, i, s, a), d.resolve(!0)) : (c(null, f, d.hiddenContainer, null, o, d, i, s, a), d.deps <= 0 && d.resolve()));
+                                else if (h && kn(f, h)) c(h, f, n, r, o, d, i, s, a), se(d, f);
                                 else if (ne(t, "onPending"), d.pendingBranch = f, d.pendingId++, c(null, f, d.hiddenContainer, null, o, d, i, s, a), d.deps <= 0) d.resolve();
                                 else {
                                     const {
                                         timeout: e,
                                         pendingId: t
                                     } = d;
                                     e > 0 ? setTimeout((() => {
@@ -4124,15 +4124,15 @@
                         },
                         create: re,
                         normalize: function(e) {
                             const {
                                 shapeFlag: t,
                                 children: n
                             } = e, r = 32 & t;
-                            e.ssContent = oe(r ? n.default : n), e.ssFallback = r ? oe(n.fallback) : Nn(fn)
+                            e.ssContent = oe(r ? n.default : n), e.ssFallback = r ? oe(n.fallback) : Rn(pn)
                         }
                     };
 
                 function ne(e, t) {
                     const n = e.props && e.props[t];
                     (0, o.isFunction)(n) && n()
                 }
@@ -4227,37 +4227,37 @@
                                 l(t, e, 0)
                             })).then((o => {
                                 if (e.isUnmounted || _.isUnmounted || _.pendingId !== e.suspenseId) return;
                                 e.asyncResolved = !0;
                                 const {
                                     vnode: i
                                 } = e;
-                                tr(e, o, !1), r && (i.el = r);
+                                nr(e, o, !1), r && (i.el = r);
                                 const s = !r && e.subTree.el;
                                 t(e, i, v(r || e.subTree.el), r ? null : g(e.subTree), _, a, u), s && y(s), Q(e, i.el), n && 0 == --_.deps && _.resolve()
                             }))
                         },
                         unmount(e, t) {
                             _.isUnmounted = !0, _.activeBranch && m(_.activeBranch, n, e, t), _.pendingBranch && m(_.pendingBranch, n, e, t)
                         }
                     };
                     return _
                 }
 
                 function oe(e) {
                     let t;
                     if ((0, o.isFunction)(e)) {
-                        const n = bn && e._c;
-                        n && (e._d = !1, gn()), e = e(), n && (e._d = !0, t = mn, vn())
+                        const n = _n && e._c;
+                        n && (e._d = !1, vn()), e = e(), n && (e._d = !0, t = gn, yn())
                     }
                     if ((0, o.isArray)(e)) {
                         const t = J(e);
                         0, e = t
                     }
-                    return e = Fn(e), t && !e.dynamicChildren && (e.dynamicChildren = t.filter((t => t !== e))), e
+                    return e = Bn(e), t && !e.dynamicChildren && (e.dynamicChildren = t.filter((t => t !== e))), e
                 }
 
                 function ie(e, t) {
                     t && t.pendingBranch ? (0, o.isArray)(e) ? t.effects.push(...e) : t.effects.push(e) : w(e)
                 }
 
                 function se(e, t) {
@@ -4266,23 +4266,23 @@
                         vnode: n,
                         parentComponent: r
                     } = e, o = n.el = t.el;
                     r && r.subTree === n && (r.vnode.el = o, Q(r, o))
                 }
 
                 function ae(e, t) {
-                    if (Yn) {
-                        let n = Yn.provides;
-                        const r = Yn.parent && Yn.parent.provides;
-                        r === n && (n = Yn.provides = Object.create(r)), n[e] = t
+                    if (Wn) {
+                        let n = Wn.provides;
+                        const r = Wn.parent && Wn.parent.provides;
+                        r === n && (n = Wn.provides = Object.create(r)), n[e] = t
                     } else 0
                 }
 
                 function ce(e, t, n = !1) {
-                    const r = Yn || V;
+                    const r = Wn || V;
                     if (r) {
                         const i = null == r.parent ? r.vnode.appContext && r.vnode.appContext.provides : r.parent.provides;
                         if (i && e in i) return i[e];
                         if (arguments.length > 1) return n && (0, o.isFunction)(t) ? t.call(r.proxy) : t
                     } else 0
                 }
 
@@ -4310,31 +4310,31 @@
                 function he(e, t, {
                     immediate: n,
                     deep: i,
                     flush: s,
                     onTrack: l,
                     onTrigger: u
                 } = o.EMPTY_OBJ) {
-                    const d = (0, r.nZ)() === (null == Yn ? void 0 : Yn.scope) ? Yn : null;
+                    const d = (0, r.nZ)() === (null == Wn ? void 0 : Wn.scope) ? Wn : null;
                     let f, p, h = !1,
                         m = !1;
                     if ((0, r.dq)(e) ? (f = () => e.value, h = (0, r.yT)(e)) : (0, r.PG)(e) ? (f = () => e, i = !0) : (0, o.isArray)(e) ? (m = !0, h = e.some((e => (0, r.PG)(e) || (0, r.yT)(e))), f = () => e.map((e => (0, r.dq)(e) ? e.value : (0, r.PG)(e) ? ve(e) : (0, o.isFunction)(e) ? a(e, d, 2) : void 0))) : f = (0, o.isFunction)(e) ? t ? () => a(e, d, 2) : () => {
                             if (!d || !d.isUnmounted) return p && p(), c(e, d, 3, [v])
                         } : o.NOOP, t && i) {
                         const e = f;
                         f = () => ve(e())
                     }
                     let g, v = e => {
                         p = w.onStop = () => {
                             a(e, d, 4)
                         }
                     };
-                    if (Qn) {
+                    if (er) {
                         if (v = o.NOOP, t ? n && c(t, d, 3, [f(), m ? [] : void 0, v]) : f(), "sync" !== s) return o.NOOP; {
-                            const e = wr();
+                            const e = Er();
                             g = e.__watcherHandles || (e.__watcherHandles = [])
                         }
                     }
                     let y = m ? new Array(e.length).fill(fe) : fe;
                     const b = () => {
                         if (w.active)
                             if (t) {
@@ -4353,18 +4353,18 @@
                 }
 
                 function me(e, t, n) {
                     const r = this.proxy,
                         i = (0, o.isString)(e) ? e.includes(".") ? ge(r, e) : () => r[e] : e.bind(r, r);
                     let s;
                     (0, o.isFunction)(t) ? s = t: (s = t.handler, n = t);
-                    const a = Yn;
-                    Kn(this);
+                    const a = Wn;
+                    Jn(this);
                     const c = he(i, s.bind(r), n);
-                    return a ? Kn(a) : Jn(), c
+                    return a ? Jn(a) : Gn(), c
                 }
 
                 function ge(e, t) {
                     const n = t.split(".");
                     return () => {
                         let t = e;
                         for (let e = 0; e < n.length && t; e++) t = t[n[e]];
@@ -4418,25 +4418,25 @@
                             onAppear: be,
                             onAfterAppear: be,
                             onAppearCancelled: be
                         },
                         setup(e, {
                             slots: t
                         }) {
-                            const n = Wn(),
+                            const n = Kn(),
                                 o = ye();
                             let i;
                             return () => {
                                 const s = t.default && ke(t.default(), !0);
                                 if (!s || !s.length) return;
                                 let a = s[0];
                                 if (s.length > 1) {
                                     let e = !1;
                                     for (const t of s)
-                                        if (t.type !== fn) {
+                                        if (t.type !== pn) {
                                             0,
                                             a = t,
                                             e = !0;
                                             break
                                         }
                                 }
                                 const c = (0, r.IU)(e),
@@ -4454,20 +4454,20 @@
                                 const {
                                     getTransitionKey: m
                                 } = u.type;
                                 if (m) {
                                     const e = m();
                                     void 0 === i ? i = e : e !== i && (i = e, h = !0)
                                 }
-                                if (p && p.type !== fn && (!On(u, p) || h)) {
+                                if (p && p.type !== pn && (!kn(u, p) || h)) {
                                     const e = we(p, c, o, n);
                                     if (Oe(p, e), "out-in" === l) return o.isLeaving = !0, e.afterLeave = () => {
                                         o.isLeaving = !1, !1 !== n.update.active && n.update()
                                     }, Ee(a);
-                                    "in-out" === l && u.type !== fn && (e.delayLeave = (e, t, n) => {
+                                    "in-out" === l && u.type !== pn && (e.delayLeave = (e, t, n) => {
                                         Se(o, p)[String(p.key)] = p, e._leaveCb = () => {
                                             t(), e._leaveCb = void 0, delete d.delayedLeave
                                         }, d.delayedLeave = n
                                     })
                                 }
                                 return a
                             }
@@ -4511,15 +4511,15 @@
                             let r = l;
                             if (!n.isMounted) {
                                 if (!i) return;
                                 r = v || l
                             }
                             t._leaveCb && t._leaveCb(!0);
                             const o = w[S];
-                            o && On(e, o) && o.el._leaveCb && o.el._leaveCb(), E(r, [t])
+                            o && kn(e, o) && o.el._leaveCb && o.el._leaveCb(), E(r, [t])
                         },
                         enter(e) {
                             let t = u,
                                 r = d,
                                 o = f;
                             if (!n.isMounted) {
                                 if (!i) return;
@@ -4543,15 +4543,15 @@
                         },
                         clone: e => we(e, t, n, r)
                     };
                     return O
                 }
 
                 function Ee(e) {
-                    if (Ne(e)) return (e = Mn(e)).children = null, e
+                    if (Ne(e)) return (e = In(e)).children = null, e
                 }
 
                 function xe(e) {
                     return Ne(e) ? e.children ? e.children[0] : void 0 : e
                 }
 
                 function Oe(e, t) {
@@ -4560,15 +4560,15 @@
 
                 function ke(e, t = !1, n) {
                     let r = [],
                         o = 0;
                     for (let i = 0; i < e.length; i++) {
                         let s = e[i];
                         const a = null == n ? s.key : String(n) + String(null != s.key ? s.key : i);
-                        s.type === un ? (128 & s.patchFlag && o++, r = r.concat(ke(s.children, t, a))) : (t || s.type !== fn) && r.push(null != a ? Mn(s, {
+                        s.type === dn ? (128 & s.patchFlag && o++, r = r.concat(ke(s.children, t, a))) : (t || s.type !== pn) && r.push(null != a ? In(s, {
                             key: a
                         }) : s)
                     }
                     if (o > 1)
                         for (let e = 0; e < r.length; e++) r[e].patchFlag = -2;
                     return r
                 }
@@ -4608,20 +4608,20 @@
                     return Ce({
                         name: "AsyncComponentWrapper",
                         __asyncLoader: h,
                         get __asyncResolved() {
                             return d
                         },
                         setup() {
-                            const e = Yn;
+                            const e = Wn;
                             if (d) return () => Pe(d, e);
                             const t = t => {
                                 f = null, l(t, e, 13, !i)
                             };
-                            if (c && e.suspense || Qn) return h().then((t => () => Pe(t, e))).catch((e => (t(e), () => i ? Nn(i, {
+                            if (c && e.suspense || er) return h().then((t => () => Pe(t, e))).catch((e => (t(e), () => i ? Rn(i, {
                                 error: e
                             }) : null)));
                             const o = (0, r.iH)(!1),
                                 u = (0, r.iH)(),
                                 p = (0, r.iH)(!!s);
                             return s && setTimeout((() => {
                                 p.value = !1
@@ -4630,43 +4630,43 @@
                                     const e = new Error(`Async component timed out after ${a}ms.`);
                                     t(e), u.value = e
                                 }
                             }), a), h().then((() => {
                                 o.value = !0, e.parent && Ne(e.parent.vnode) && _(e.parent.update)
                             })).catch((e => {
                                 t(e), u.value = e
-                            })), () => o.value && d ? Pe(d, e) : u.value && i ? Nn(i, {
+                            })), () => o.value && d ? Pe(d, e) : u.value && i ? Rn(i, {
                                 error: u.value
-                            }) : n && !p.value ? Nn(n) : void 0
+                            }) : n && !p.value ? Rn(n) : void 0
                         }
                     })
                 }
 
                 function Pe(e, t) {
                     const {
                         ref: n,
                         props: r,
                         children: o,
                         ce: i
-                    } = t.vnode, s = Nn(e, r, o);
+                    } = t.vnode, s = Rn(e, r, o);
                     return s.ref = n, s.ce = i, delete t.vnode.ce, s
                 }
                 const Ne = e => e.type.__isKeepAlive,
                     Re = {
                         name: "KeepAlive",
                         __isKeepAlive: !0,
                         props: {
                             include: [String, RegExp, Array],
                             exclude: [String, RegExp, Array],
                             max: [String, Number]
                         },
                         setup(e, {
                             slots: t
                         }) {
-                            const n = Wn(),
+                            const n = Kn(),
                                 r = n.ctx;
                             if (!r.renderer) return () => {
                                 const e = t.default && t.default();
                                 return e && 1 === e.length ? e[0] : e
                             };
                             const i = new Map,
                                 s = new Set;
@@ -4687,36 +4687,36 @@
 
                             function h(e) {
                                 Fe(e), d(e, n, c, !0)
                             }
 
                             function m(e) {
                                 i.forEach(((t, n) => {
-                                    const r = ar(t.type);
+                                    const r = cr(t.type);
                                     !r || e && e(r) || g(n)
                                 }))
                             }
 
                             function g(e) {
                                 const t = i.get(e);
-                                a && On(t, a) ? a && Fe(a) : h(t), i.delete(e), s.delete(e)
+                                a && kn(t, a) ? a && Fe(a) : h(t), i.delete(e), s.delete(e)
                             }
                             r.activate = (e, t, n, r, i) => {
                                 const s = e.component;
                                 u(e, t, n, 0, c), l(s.vnode, e, t, n, s, c, r, e.slotScopeIds, i), Xt((() => {
                                     s.isDeactivated = !1, s.a && (0, o.invokeArrayFns)(s.a);
                                     const t = e.props && e.props.onVnodeMounted;
-                                    t && $n(t, s.parent, e)
+                                    t && Hn(t, s.parent, e)
                                 }), c), __VUE_PROD_DEVTOOLS__ && D(s)
                             }, r.deactivate = e => {
                                 const t = e.component;
                                 u(e, p, null, 1, c), Xt((() => {
                                     t.da && (0, o.invokeArrayFns)(t.da);
                                     const n = e.props && e.props.onVnodeUnmounted;
-                                    n && $n(n, t.parent, e), t.isDeactivated = !0
+                                    n && Hn(n, t.parent, e), t.isDeactivated = !0
                                 }), c), __VUE_PROD_DEVTOOLS__ && D(t)
                             }, pe((() => [e.include, e.exclude]), (([e, t]) => {
                                 e && m((t => De(e, t))), t && m((e => !De(t, e)))
                             }), {
                                 flush: "post",
                                 deep: !0
                             });
@@ -4738,27 +4738,27 @@
                                     }
                                 }))
                             })), () => {
                                 if (v = null, !t.default) return null;
                                 const n = t.default(),
                                     r = n[0];
                                 if (n.length > 1) return a = null, n;
-                                if (!(xn(r) && (4 & r.shapeFlag || 128 & r.shapeFlag))) return a = null, r;
+                                if (!(On(r) && (4 & r.shapeFlag || 128 & r.shapeFlag))) return a = null, r;
                                 let o = Be(r);
                                 const c = o.type,
-                                    l = ar(Te(o) ? o.type.__asyncResolved || {} : c),
+                                    l = cr(Te(o) ? o.type.__asyncResolved || {} : c),
                                     {
                                         include: u,
                                         exclude: d,
                                         max: f
                                     } = e;
                                 if (u && (!l || !De(u, l)) || d && l && De(d, l)) return a = o, r;
                                 const p = null == o.key ? c : o.key,
                                     h = i.get(p);
-                                return o.el && (o = Mn(o), 128 & r.shapeFlag && (r.ssContent = o)), v = p, h ? (o.el = h.el, o.component = h.component, o.transition && Oe(o, o.transition), o.shapeFlag |= 512, s.delete(p), s.add(p)) : (s.add(p), f && s.size > parseInt(f, 10) && g(s.values().next().value)), o.shapeFlag |= 256, a = o, ee(r.type) ? r : o
+                                return o.el && (o = In(o), 128 & r.shapeFlag && (r.ssContent = o)), v = p, h ? (o.el = h.el, o.component = h.component, o.transition && Oe(o, o.transition), o.shapeFlag |= 512, s.delete(p), s.add(p)) : (s.add(p), f && s.size > parseInt(f, 10) && g(s.values().next().value)), o.shapeFlag |= 256, a = o, ee(r.type) ? r : o
                             }
                         }
                     };
 
                 function De(e, t) {
                     return (0, o.isArray)(e) ? e.some((e => De(e, t))) : (0, o.isString)(e) ? e.split(",").includes(t) : !!(0, o.isRegExp)(e) && e.test(t)
                 }
@@ -4767,15 +4767,15 @@
                     je(e, "a", t)
                 }
 
                 function Ie(e, t) {
                     je(e, "da", t)
                 }
 
-                function je(e, t, n = Yn) {
+                function je(e, t, n = Wn) {
                     const r = e.__wdc || (e.__wdc = () => {
                         let t = n;
                         for (; t;) {
                             if (t.isDeactivated) return;
                             t = t.parent
                         }
                         return e()
@@ -4797,45 +4797,45 @@
                     e.shapeFlag &= -257, e.shapeFlag &= -513
                 }
 
                 function Be(e) {
                     return 128 & e.shapeFlag ? e.ssContent : e
                 }
 
-                function Ue(e, t, n = Yn, o = !1) {
+                function Ue(e, t, n = Wn, o = !1) {
                     if (n) {
                         const i = n[e] || (n[e] = []),
                             s = t.__weh || (t.__weh = (...o) => {
                                 if (n.isUnmounted) return;
-                                (0, r.Jd)(), Kn(n);
+                                (0, r.Jd)(), Jn(n);
                                 const i = c(t, n, e, o);
-                                return Jn(), (0, r.lk)(), i
+                                return Gn(), (0, r.lk)(), i
                             });
                         return o ? i.unshift(s) : i.push(s), s
                     }
                 }
-                const Ve = e => (t, n = Yn) => (!Qn || "sp" === e) && Ue(e, ((...e) => t(...e)), n),
+                const Ve = e => (t, n = Wn) => (!er || "sp" === e) && Ue(e, ((...e) => t(...e)), n),
                     $e = Ve("bm"),
                     He = Ve("m"),
                     qe = Ve("bu"),
                     ze = Ve("u"),
                     Ye = Ve("bum"),
                     We = Ve("um"),
                     Ke = Ve("sp"),
                     Je = Ve("rtg"),
                     Ge = Ve("rtc");
 
-                function Xe(e, t = Yn) {
+                function Xe(e, t = Wn) {
                     Ue("ec", e, t)
                 }
 
                 function Ze(e, t) {
                     const n = V;
                     if (null === n) return e;
-                    const r = sr(n) || n.proxy,
+                    const r = ar(n) || n.proxy,
                         i = e.dirs || (e.dirs = []);
                     for (let e = 0; e < t.length; e++) {
                         let [n, s, a, c = o.EMPTY_OBJ] = t[e];
                         n && ((0, o.isFunction)(n) && (n = {
                             mounted: n,
                             updated: n
                         }), n.deep && ve(s), i.push({
@@ -4873,19 +4873,19 @@
                 }
 
                 function it(e) {
                     return st(tt, e)
                 }
 
                 function st(e, t, n = !0, r = !1) {
-                    const i = V || Yn;
+                    const i = V || Wn;
                     if (i) {
                         const n = i.type;
                         if (e === et) {
-                            const e = ar(n, !1);
+                            const e = cr(n, !1);
                             if (e && (e === t || e === (0, o.camelize)(t) || e === (0, o.capitalize)((0, o.camelize)(t)))) return n
                         }
                         const s = at(i[e] || n[e], t) || at(i.appContext[e], t);
                         return !s && r ? n : s
                     }
                 }
 
@@ -4928,34 +4928,34 @@
                             return t && (t.key = r.key), t
                         } : r.fn)
                     }
                     return e
                 }
 
                 function ut(e, t, n = {}, r, o) {
-                    if (V.isCE || V.parent && Te(V.parent) && V.parent.isCE) return "default" !== t && (n.name = t), Nn("slot", n, r && r());
+                    if (V.isCE || V.parent && Te(V.parent) && V.parent.isCE) return "default" !== t && (n.name = t), Rn("slot", n, r && r());
                     let i = e[t];
-                    i && i._c && (i._d = !1), gn();
+                    i && i._c && (i._d = !1), vn();
                     const s = i && dt(i(n)),
-                        a = En(un, {
+                        a = xn(dn, {
                             key: n.key || s && s.key || `_${t}`
                         }, s || (r ? r() : []), s && 1 === e._ ? 64 : -2);
                     return !o && a.scopeId && (a.slotScopeIds = [a.scopeId + "-s"]), i && i._c && (i._d = !0), a
                 }
 
                 function dt(e) {
-                    return e.some((e => !xn(e) || e.type !== fn && !(e.type === un && !dt(e.children)))) ? e : null
+                    return e.some((e => !On(e) || e.type !== pn && !(e.type === dn && !dt(e.children)))) ? e : null
                 }
 
                 function ft(e, t) {
                     const n = {};
                     for (const r in e) n[t && /[A-Z]/.test(r) ? `on:${r}` : (0, o.toHandlerKey)(r)] = e[r];
                     return n
                 }
-                const pt = e => e ? Gn(e) ? sr(e) || e.proxy : pt(e.parent) : null,
+                const pt = e => e ? Xn(e) ? ar(e) || e.proxy : pt(e.parent) : null,
                     ht = (0, o.extend)(Object.create(null), {
                         $: e => e,
                         $el: e => e.vnode.el,
                         $data: e => e.data,
                         $props: e => e.props,
                         $attrs: e => e.attrs,
                         $slots: e => e.slots,
@@ -5099,15 +5099,15 @@
                     }
                     if (yt = !0, a)
                         for (const e in a) {
                             const t = a[e],
                                 r = (0, o.isFunction)(t) ? t.bind(n, n) : (0, o.isFunction)(t.get) ? t.get.bind(n, n) : o.NOOP;
                             0;
                             const s = !(0, o.isFunction)(t) && (0, o.isFunction)(t.set) ? t.set.bind(n) : o.NOOP,
-                                c = lr({
+                                c = ur({
                                     get: r,
                                     set: s
                                 });
                             Object.defineProperty(i, e, {
                                 enumerable: !0,
                                 configurable: !0,
                                 get: () => c.value,
@@ -5274,15 +5274,15 @@
                         const e = (0, o.hasOwn)(a, "default");
                         if (e && void 0 === r) {
                             const e = a.default;
                             if (a.type !== Function && (0, o.isFunction)(e)) {
                                 const {
                                     propsDefaults: o
                                 } = i;
-                                n in o ? r = o[n] : (Kn(i), r = o[n] = e.call(null, t), Jn())
+                                n in o ? r = o[n] : (Jn(i), r = o[n] = e.call(null, t), Gn())
                             } else r = e
                         }
                         a[0] && (s && !e ? r = !1 : !a[1] || "" !== r && r !== (0, o.hyphenate)(n) || (r = !0))
                     }
                     return r
                 }
 
@@ -5341,15 +5341,15 @@
                     return Dt(e) === Dt(t)
                 }
 
                 function It(e, t) {
                     return (0, o.isArray)(t) ? t.findIndex((t => Mt(t, e))) : (0, o.isFunction)(t) && Mt(t, e) ? 0 : -1
                 }
                 const jt = e => "_" === e[0] || "$stable" === e,
-                    Lt = e => (0, o.isArray)(e) ? e.map(Fn) : [Fn(e)],
+                    Lt = e => (0, o.isArray)(e) ? e.map(Bn) : [Bn(e)],
                     Ft = (e, t, n) => {
                         if (t._n) return t;
                         const r = W(((...e) => Lt(t(...e))), n);
                         return r._c = !1, r
                     },
                     Bt = (e, t, n) => {
                         const r = e._ctx;
@@ -5369,15 +5369,15 @@
                         e.slots.default = () => n
                     },
                     Vt = (e, t) => {
                         if (32 & e.vnode.shapeFlag) {
                             const n = t._;
                             n ? (e.slots = (0, r.IU)(t), (0, o.def)(t, "_", n)) : Bt(t, e.slots = {})
                         } else e.slots = {}, t && Ut(e, t);
-                        (0, o.def)(e.slots, Cn, 1)
+                        (0, o.def)(e.slots, Tn, 1)
                     },
                     $t = (e, t, n) => {
                         const {
                             vnode: r,
                             slots: i
                         } = e;
                         let s = !0,
@@ -5424,37 +5424,37 @@
                         const c = i.app = {
                             _uid: qt++,
                             _component: n,
                             _props: r,
                             _container: null,
                             _context: i,
                             _instance: null,
-                            version: kr,
+                            version: Cr,
                             get config() {
                                 return i.config
                             },
                             set config(e) {
                                 0
                             },
                             use: (e, ...t) => (s.has(e) || (e && (0, o.isFunction)(e.install) ? (s.add(e), e.install(c, ...t)) : (0, o.isFunction)(e) && (s.add(e), e(c, ...t))), c),
                             mixin: e => (__VUE_OPTIONS_API__ && (i.mixins.includes(e) || i.mixins.push(e)), c),
                             component: (e, t) => t ? (i.components[e] = t, c) : i.components[e],
                             directive: (e, t) => t ? (i.directives[e] = t, c) : i.directives[e],
                             mount(o, s, l) {
                                 if (!a) {
                                     0;
-                                    const u = Nn(n, r);
+                                    const u = Rn(n, r);
                                     return u.appContext = i, s && t ? t(u, o) : e(u, o, l), a = !0, c._container = o, o.__vue_app__ = c, __VUE_PROD_DEVTOOLS__ && (c._instance = u.component, function(e, t) {
                                         N("app:init", e, t, {
-                                            Fragment: un,
-                                            Text: dn,
-                                            Comment: fn,
-                                            Static: pn
+                                            Fragment: dn,
+                                            Text: fn,
+                                            Comment: pn,
+                                            Static: hn
                                         })
-                                    }(c, kr)), sr(u.component) || u.component.proxy
+                                    }(c, Cr)), ar(u.component) || u.component.proxy
                                 }
                             },
                             unmount() {
                                 a && (e(null, c._container), __VUE_PROD_DEVTOOLS__ && (c._instance = null, function(e) {
                                     N("app:unmount", e)
                                 }(c)), delete c._container.__vue_app__)
                             },
@@ -5463,15 +5463,15 @@
                         return c
                     }
                 }
 
                 function Yt(e, t, n, i, s = !1) {
                     if ((0, o.isArray)(e)) return void e.forEach(((e, r) => Yt(e, t && ((0, o.isArray)(t) ? t[r] : t), n, i, s)));
                     if (Te(i) && !s) return;
-                    const c = 4 & i.shapeFlag ? sr(i.component) || i.component.proxy : i.el,
+                    const c = 4 & i.shapeFlag ? ar(i.component) || i.component.proxy : i.el,
                         l = s ? null : c,
                         {
                             i: u,
                             r: d
                         } = e;
                     const f = t && t.r,
                         p = u.refs === o.EMPTY_OBJ ? u.refs = {} : u.refs,
@@ -5517,40 +5517,40 @@
                                 shapeFlag: w,
                                 patchFlag: E
                             } = r;
                         let x = n.nodeType;
                         r.el = n, -2 === E && (v = !1, r.dynamicChildren = null);
                         let O = null;
                         switch (_) {
-                            case dn:
+                            case fn:
                                 3 !== x ? "" === r.children ? (l(r.el = i(""), a(n), n), O = n) : O = b() : (n.data !== r.children && (Wt = !0, n.data = r.children), O = s(n));
                                 break;
-                            case fn:
+                            case pn:
                                 O = 8 !== x || y ? b() : s(n);
                                 break;
-                            case pn:
+                            case hn:
                                 if (y && (x = (n = s(n)).nodeType), 1 === x || 3 === x) {
                                     O = n;
                                     const e = !r.children.length;
                                     for (let t = 0; t < r.staticCount; t++) e && (r.children += 1 === O.nodeType ? O.outerHTML : O.data), t === r.staticCount - 1 && (r.anchor = O), O = s(O);
                                     return y ? s(O) : O
                                 }
                                 b();
                                 break;
-                            case un:
+                            case dn:
                                 O = y ? h(n, r, o, c, u, v) : b();
                                 break;
                             default:
                                 if (1 & w) O = 1 !== x || r.type.toLowerCase() !== n.tagName.toLowerCase() ? b() : f(n, r, o, c, u, v);
                                 else if (6 & w) {
                                     r.slotScopeIds = u;
                                     const e = a(n);
                                     if (t(r, e, null, o, c, Kt(e), v), O = y ? g(n) : s(n), O && Jt(O) && "teleport end" === O.data && (O = s(O)), Te(r)) {
                                         let t;
-                                        y ? (t = Nn(un), t.anchor = O ? O.previousSibling : e.lastChild) : t = 3 === n.nodeType ? In("") : Nn("div"), t.el = n, r.component.subTree = t
+                                        y ? (t = Rn(dn), t.anchor = O ? O.previousSibling : e.lastChild) : t = 3 === n.nodeType ? jn("") : Rn("div"), t.el = n, r.component.subTree = t
                                     }
                                 } else 64 & w ? O = 8 !== x ? b() : r.type.hydrate(n, r, o, c, u, v, e, p) : 128 & w && (O = r.type.hydrate(n, r, o, c, Kt(a(n)), u, v, e, d))
                         }
                         return null != S && Yt(S, null, c, r), O
                     }, f = (e, t, n, i, s, a) => {
                         a = a || !!t.dynamicChildren;
                         const {
@@ -5562,16 +5562,16 @@
                         } = t, m = "input" === l && h || "option" === l;
                         if (m || -1 !== d) {
                             if (h && Qe(t, null, n, "created"), u)
                                 if (m || !a || 48 & d)
                                     for (const t in u)(m && t.endsWith("value") || (0, o.isOn)(t) && !(0, o.isReservedProp)(t)) && r(e, t, null, u[t], !1, void 0, n);
                                 else u.onClick && r(e, "onClick", null, u.onClick, !1, void 0, n);
                             let l;
-                            if ((l = u && u.onVnodeBeforeMount) && $n(l, n, t), h && Qe(t, null, n, "beforeMount"), ((l = u && u.onVnodeMounted) || h) && ie((() => {
-                                    l && $n(l, n, t), h && Qe(t, null, n, "mounted")
+                            if ((l = u && u.onVnodeBeforeMount) && Hn(l, n, t), h && Qe(t, null, n, "beforeMount"), ((l = u && u.onVnodeMounted) || h) && ie((() => {
+                                    l && Hn(l, n, t), h && Qe(t, null, n, "mounted")
                                 }), i), 16 & f && (!u || !u.innerHTML && !u.textContent)) {
                                 let r = p(e.firstChild, t, e, n, i, s, a);
                                 for (; r;) {
                                     Wt = !0;
                                     const e = r;
                                     r = r.nextSibling, c(e)
                                 }
@@ -5579,18 +5579,18 @@
                         }
                         return e.nextSibling
                     }, p = (e, t, r, o, i, s, a) => {
                         a = a || !!t.dynamicChildren;
                         const c = t.children,
                             l = c.length;
                         for (let t = 0; t < l; t++) {
-                            const l = a ? c[t] : c[t] = Fn(c[t]);
+                            const l = a ? c[t] : c[t] = Bn(c[t]);
                             if (e) e = d(e, l, o, i, s, a);
                             else {
-                                if (l.type === dn && !l.children) continue;
+                                if (l.type === fn && !l.children) continue;
                                 Wt = !0, n(null, l, r, null, o, i, Kt(r), s)
                             }
                         }
                         return e
                     }, h = (e, t, n, r, o, i) => {
                         const {
                             slotScopeIds: c
@@ -5649,31 +5649,31 @@
                         setElementText: h,
                         parentNode: m,
                         nextSibling: g,
                         setScopeId: v = o.NOOP,
                         insertStaticContent: y
                     } = e, b = (e, t, n, r = null, o = null, i = null, s = !1, a = null, c = !!t.dynamicChildren) => {
                         if (e === t) return;
-                        e && !On(e, t) && (r = re(e), G(e, o, i, !0), e = null), -2 === t.patchFlag && (c = !1, t.dynamicChildren = null);
+                        e && !kn(e, t) && (r = re(e), G(e, o, i, !0), e = null), -2 === t.patchFlag && (c = !1, t.dynamicChildren = null);
                         const {
                             type: l,
                             ref: u,
                             shapeFlag: d
                         } = t;
                         switch (l) {
-                            case dn:
+                            case fn:
                                 S(e, t, n, r);
                                 break;
-                            case fn:
+                            case pn:
                                 w(e, t, n, r);
                                 break;
-                            case pn:
+                            case hn:
                                 null == e && O(t, n, r, s);
                                 break;
-                            case un:
+                            case dn:
                                 F(e, t, n, r, o, i, s, a, c);
                                 break;
                             default:
                                 1 & d ? C(e, t, n, r, o, i, s, a, c) : 6 & d ? B(e, t, n, r, o, i, s, a, c) : (64 & d || 128 & d) && l.process(e, t, n, r, o, i, s, a, c, ie)
                         }
                         null != u && o && Yt(u, e && e.ref, i, t || e, !t)
                     }, S = (e, t, n, r) => {
@@ -5702,53 +5702,53 @@
                             props: g,
                             shapeFlag: v,
                             transition: y,
                             dirs: b
                         } = e;
                         if (f = e.el = c(e.type, l, g && g.is, g), 8 & v ? h(f, e.children) : 16 & v && P(e.children, f, null, r, s, l && "foreignObject" !== m, u, d), b && Qe(e, null, r, "created"), A(f, e, e.scopeId, u, r), g) {
                             for (const t in g) "value" === t || (0, o.isReservedProp)(t) || a(f, t, null, g[t], l, e.children, r, s, ne);
-                            "value" in g && a(f, "value", null, g.value), (p = g.onVnodeBeforeMount) && $n(p, r, e)
+                            "value" in g && a(f, "value", null, g.value), (p = g.onVnodeBeforeMount) && Hn(p, r, e)
                         }
                         __VUE_PROD_DEVTOOLS__ && (Object.defineProperty(f, "__vnode", {
                             value: e,
                             enumerable: !1
                         }), Object.defineProperty(f, "__vueParentComponent", {
                             value: r,
                             enumerable: !1
                         })), b && Qe(e, null, r, "beforeMount");
                         const _ = (!s || s && !s.pendingBranch) && y && !y.persisted;
                         _ && y.beforeEnter(f), i(f, t, n), ((p = g && g.onVnodeMounted) || _ || b) && Xt((() => {
-                            p && $n(p, r, e), _ && y.enter(f), b && Qe(e, null, r, "mounted")
+                            p && Hn(p, r, e), _ && y.enter(f), b && Qe(e, null, r, "mounted")
                         }), s)
                     }, A = (e, t, n, r, o) => {
                         if (n && v(e, n), r)
                             for (let t = 0; t < r.length; t++) v(e, r[t]);
                         if (o) {
                             if (t === o.subTree) {
                                 const t = o.vnode;
                                 A(e, t, t.scopeId, t.slotScopeIds, o.parent)
                             }
                         }
                     }, P = (e, t, n, r, o, i, s, a, c = 0) => {
                         for (let l = c; l < e.length; l++) {
-                            const c = e[l] = a ? Bn(e[l]) : Fn(e[l]);
+                            const c = e[l] = a ? Un(e[l]) : Bn(e[l]);
                             b(null, c, t, n, r, o, i, s, a)
                         }
                     }, N = (e, t, n, r, i, s, c) => {
                         const l = t.el = e.el;
                         let {
                             patchFlag: u,
                             dynamicChildren: d,
                             dirs: f
                         } = t;
                         u |= 16 & e.patchFlag;
                         const p = e.props || o.EMPTY_OBJ,
                             m = t.props || o.EMPTY_OBJ;
                         let g;
-                        n && tn(n, !1), (g = m.onVnodeBeforeUpdate) && $n(g, n, t, e), f && Qe(t, e, n, "beforeUpdate"), n && tn(n, !0);
+                        n && tn(n, !1), (g = m.onVnodeBeforeUpdate) && Hn(g, n, t, e), f && Qe(t, e, n, "beforeUpdate"), n && tn(n, !0);
                         const v = i && "foreignObject" !== t.type;
                         if (d ? I(e.dynamicChildren, d, l, n, r, v, s) : c || z(e, t, l, null, n, r, v, s, !1), u > 0) {
                             if (16 & u) L(l, t, p, m, n, r, i);
                             else if (2 & u && p.class !== m.class && a(l, "class", null, m.class, i), 4 & u && a(l, "style", p.style, m.style, i), 8 & u) {
                                 const o = t.dynamicProps;
                                 for (let t = 0; t < o.length; t++) {
                                     const s = o[t],
@@ -5756,21 +5756,21 @@
                                         u = m[s];
                                     u === c && "value" !== s || a(l, s, c, u, i, e.children, n, r, ne)
                                 }
                             }
                             1 & u && e.children !== t.children && h(l, t.children)
                         } else c || null != d || L(l, t, p, m, n, r, i);
                         ((g = m.onVnodeUpdated) || f) && Xt((() => {
-                            g && $n(g, n, t, e), f && Qe(t, e, n, "updated")
+                            g && Hn(g, n, t, e), f && Qe(t, e, n, "updated")
                         }), r)
                     }, I = (e, t, n, r, o, i, s) => {
                         for (let a = 0; a < t.length; a++) {
                             const c = e[a],
                                 l = t[a],
-                                u = c.el && (c.type === un || !On(c, l) || 70 & c.shapeFlag) ? m(c.el) : n;
+                                u = c.el && (c.type === dn || !kn(c, l) || 70 & c.shapeFlag) ? m(c.el) : n;
                             b(c, l, u, null, r, o, i, s, !0)
                         }
                     }, L = (e, t, n, r, i, s, c) => {
                         if (n !== r) {
                             if (n !== o.EMPTY_OBJ)
                                 for (const l in n)(0, o.isReservedProp)(l) || l in r || a(e, l, n[l], null, c, t.children, i, s, ne);
                             for (const l in r) {
@@ -5789,18 +5789,18 @@
                             dynamicChildren: h,
                             slotScopeIds: m
                         } = t;
                         m && (c = c ? c.concat(m) : m), null == e ? (i(d, n, r), i(f, n, r), P(t.children, n, f, o, s, a, c, u)) : p > 0 && 64 & p && h && e.dynamicChildren ? (I(e.dynamicChildren, h, n, o, s, a, c), (null != t.key || o && t === o.subTree) && nn(e, t, !0)) : z(e, t, n, f, o, s, a, c, u)
                     }, B = (e, t, n, r, o, i, s, a, c) => {
                         t.slotScopeIds = a, null == e ? 512 & t.shapeFlag ? o.ctx.activate(t, n, r, s, c) : V(t, n, r, o, i, s, c) : $(e, t, c)
                     }, V = (e, t, n, r, o, i, s) => {
-                        const a = e.component = zn(e, r, o);
-                        if (Ne(e) && (a.ctx.renderer = ie), er(a), a.asyncDep) {
+                        const a = e.component = Yn(e, r, o);
+                        if (Ne(e) && (a.ctx.renderer = ie), tr(a), a.asyncDep) {
                             if (o && o.registerDep(a, H), !e.el) {
-                                const e = a.subTree = Nn(fn);
+                                const e = a.subTree = Rn(pn);
                                 w(null, e, t, n)
                             }
                         } else H(a, e, t, n, o, i, s)
                     }, $ = (e, t, n) => {
                         const r = t.component = e.component;
                         if (function(e, t, n) {
                                 const {
@@ -5839,42 +5839,42 @@
                                             next: n,
                                             bu: r,
                                             u: i,
                                             parent: l,
                                             vnode: u
                                         } = e,
                                         d = n;
-                                    0, tn(e, !1), n ? (n.el = u.el, q(e, n, c)) : n = u, r && (0, o.invokeArrayFns)(r), (t = n.props && n.props.onVnodeBeforeUpdate) && $n(t, l, n, u), tn(e, !0);
+                                    0, tn(e, !1), n ? (n.el = u.el, q(e, n, c)) : n = u, r && (0, o.invokeArrayFns)(r), (t = n.props && n.props.onVnodeBeforeUpdate) && Hn(t, l, n, u), tn(e, !0);
                                     const f = K(e);
                                     0;
                                     const p = e.subTree;
-                                    e.subTree = f, b(p, f, m(p.el), re(p), e, s, a), n.el = f.el, null === d && Q(e, f.el), i && Xt(i, s), (t = n.props && n.props.onVnodeUpdated) && Xt((() => $n(t, l, n, u)), s), __VUE_PROD_DEVTOOLS__ && M(e)
+                                    e.subTree = f, b(p, f, m(p.el), re(p), e, s, a), n.el = f.el, null === d && Q(e, f.el), i && Xt(i, s), (t = n.props && n.props.onVnodeUpdated) && Xt((() => Hn(t, l, n, u)), s), __VUE_PROD_DEVTOOLS__ && M(e)
                                 } else {
                                     let r;
                                     const {
                                         el: c,
                                         props: l
                                     } = t, {
                                         bm: u,
                                         m: d,
                                         parent: f
                                     } = e, p = Te(t);
-                                    if (tn(e, !1), u && (0, o.invokeArrayFns)(u), !p && (r = l && l.onVnodeBeforeMount) && $n(r, f, t), tn(e, !0), c && ae) {
+                                    if (tn(e, !1), u && (0, o.invokeArrayFns)(u), !p && (r = l && l.onVnodeBeforeMount) && Hn(r, f, t), tn(e, !0), c && ae) {
                                         const n = () => {
                                             e.subTree = K(e), ae(c, e.subTree, e, s, null)
                                         };
                                         p ? t.type.__asyncLoader().then((() => !e.isUnmounted && n())) : n()
                                     } else {
                                         0;
                                         const r = e.subTree = K(e);
                                         0, b(null, r, n, i, e, s, a), t.el = r.el
                                     }
                                     if (d && Xt(d, s), !p && (r = l && l.onVnodeMounted)) {
                                         const e = t;
-                                        Xt((() => $n(r, f, e)), s)
+                                        Xt((() => Hn(r, f, e)), s)
                                     }(256 & t.shapeFlag || f && Te(f.vnode) && 256 & f.vnode.shapeFlag) && e.a && Xt(e.a, s), e.isMounted = !0, __VUE_PROD_DEVTOOLS__ && D(e), t = n = i = null
                                 }
                             }), (() => _(u)), e.scope),
                             u = e.update = () => l.run();
                         u.id = e.uid, tn(e, !0), u()
                     }, q = (e, t, n) => {
                         t.component = e;
@@ -5928,49 +5928,49 @@
                     }, Y = (e, t, n, r, i, s, a, c, l) => {
                         e = e || o.EMPTY_ARR, t = t || o.EMPTY_ARR;
                         const u = e.length,
                             d = t.length,
                             f = Math.min(u, d);
                         let p;
                         for (p = 0; p < f; p++) {
-                            const r = t[p] = l ? Bn(t[p]) : Fn(t[p]);
+                            const r = t[p] = l ? Un(t[p]) : Bn(t[p]);
                             b(e[p], r, n, null, i, s, a, c, l)
                         }
                         u > d ? ne(e, i, s, !0, !1, f) : P(t, n, r, i, s, a, c, l, f)
                     }, W = (e, t, n, r, i, s, a, c, l) => {
                         let u = 0;
                         const d = t.length;
                         let f = e.length - 1,
                             p = d - 1;
                         for (; u <= f && u <= p;) {
                             const r = e[u],
-                                o = t[u] = l ? Bn(t[u]) : Fn(t[u]);
-                            if (!On(r, o)) break;
+                                o = t[u] = l ? Un(t[u]) : Bn(t[u]);
+                            if (!kn(r, o)) break;
                             b(r, o, n, null, i, s, a, c, l), u++
                         }
                         for (; u <= f && u <= p;) {
                             const r = e[f],
-                                o = t[p] = l ? Bn(t[p]) : Fn(t[p]);
-                            if (!On(r, o)) break;
+                                o = t[p] = l ? Un(t[p]) : Bn(t[p]);
+                            if (!kn(r, o)) break;
                             b(r, o, n, null, i, s, a, c, l), f--, p--
                         }
                         if (u > f) {
                             if (u <= p) {
                                 const e = p + 1,
                                     o = e < d ? t[e].el : r;
-                                for (; u <= p;) b(null, t[u] = l ? Bn(t[u]) : Fn(t[u]), n, o, i, s, a, c, l), u++
+                                for (; u <= p;) b(null, t[u] = l ? Un(t[u]) : Bn(t[u]), n, o, i, s, a, c, l), u++
                             }
                         } else if (u > p)
                             for (; u <= f;) G(e[u], i, s, !0), u++;
                         else {
                             const h = u,
                                 m = u,
                                 g = new Map;
                             for (u = m; u <= p; u++) {
-                                const e = t[u] = l ? Bn(t[u]) : Fn(t[u]);
+                                const e = t[u] = l ? Un(t[u]) : Bn(t[u]);
                                 null != e.key && g.set(e.key, u)
                             }
                             let v, y = 0;
                             const _ = p - m + 1;
                             let S = !1,
                                 w = 0;
                             const E = new Array(_);
@@ -5981,15 +5981,15 @@
                                     G(r, i, s, !0);
                                     continue
                                 }
                                 let o;
                                 if (null != r.key) o = g.get(r.key);
                                 else
                                     for (v = m; v <= p; v++)
-                                        if (0 === E[v - m] && On(r, t[v])) {
+                                        if (0 === E[v - m] && kn(r, t[v])) {
                                             o = v;
                                             break
                                         } void 0 === o ? G(r, i, s, !0) : (E[o - m] = u + 1, o >= w ? w = o : S = !0, b(r, t[o], n, null, i, s, a, c, l), y++)
                             }
                             const x = S ? function(e) {
                                 const t = e.slice(),
                                     n = [0];
@@ -6024,20 +6024,20 @@
                             transition: c,
                             children: l,
                             shapeFlag: u
                         } = e;
                         if (6 & u) return void J(e.component.subTree, t, n, r);
                         if (128 & u) return void e.suspense.move(t, n, r);
                         if (64 & u) return void a.move(e, t, n, ie);
-                        if (a === un) {
+                        if (a === dn) {
                             i(s, t, n);
                             for (let e = 0; e < l.length; e++) J(l[e], t, n, r);
                             return void i(e.anchor, t, n)
                         }
-                        if (a === pn) return void(({
+                        if (a === hn) return void(({
                             el: e,
                             anchor: t
                         }, n, r) => {
                             let o;
                             for (; e && e !== t;) o = g(e), i(e, n, r), e = o;
                             i(t, n, r)
                         })(e, t, n);
@@ -6067,30 +6067,30 @@
                             patchFlag: d,
                             dirs: f
                         } = e;
                         if (null != a && Yt(a, null, n, e, !0), 256 & u) return void t.ctx.deactivate(e);
                         const p = 1 & u && f,
                             h = !Te(e);
                         let m;
-                        if (h && (m = s && s.onVnodeBeforeUnmount) && $n(m, t, e), 6 & u) te(e.component, n, r);
+                        if (h && (m = s && s.onVnodeBeforeUnmount) && Hn(m, t, e), 6 & u) te(e.component, n, r);
                         else {
                             if (128 & u) return void e.suspense.unmount(n, r);
-                            p && Qe(e, null, t, "beforeUnmount"), 64 & u ? e.type.remove(e, t, n, o, ie, r) : l && (i !== un || d > 0 && 64 & d) ? ne(l, t, n, !1, !0) : (i === un && 384 & d || !o && 16 & u) && ne(c, t, n), r && X(e)
+                            p && Qe(e, null, t, "beforeUnmount"), 64 & u ? e.type.remove(e, t, n, o, ie, r) : l && (i !== dn || d > 0 && 64 & d) ? ne(l, t, n, !1, !0) : (i === dn && 384 & d || !o && 16 & u) && ne(c, t, n), r && X(e)
                         }(h && (m = s && s.onVnodeUnmounted) || p) && Xt((() => {
-                            m && $n(m, t, e), p && Qe(e, null, t, "unmounted")
+                            m && Hn(m, t, e), p && Qe(e, null, t, "unmounted")
                         }), n)
                     }, X = e => {
                         const {
                             type: t,
                             el: n,
                             anchor: r,
                             transition: o
                         } = e;
-                        if (t === un) return void ee(n, r);
-                        if (t === pn) return void k(e);
+                        if (t === dn) return void ee(n, r);
+                        if (t === hn) return void k(e);
                         const i = () => {
                             s(n), o && !o.persisted && o.afterLeave && o.afterLeave()
                         };
                         if (1 & e.shapeFlag && o && !o.persisted) {
                             const {
                                 leave: t,
                                 delayLeave: r
@@ -6146,94 +6146,95 @@
                 function nn(e, t, n = !1) {
                     const r = e.children,
                         i = t.children;
                     if ((0, o.isArray)(r) && (0, o.isArray)(i))
                         for (let e = 0; e < r.length; e++) {
                             const t = r[e];
                             let o = i[e];
-                            1 & o.shapeFlag && !o.dynamicChildren && ((o.patchFlag <= 0 || 32 === o.patchFlag) && (o = i[e] = Bn(i[e]), o.el = t.el), n || nn(t, o)), o.type === dn && (o.el = t.el)
+                            1 & o.shapeFlag && !o.dynamicChildren && ((o.patchFlag <= 0 || 32 === o.patchFlag) && (o = i[e] = Un(i[e]), o.el = t.el), n || nn(t, o)), o.type === fn && (o.el = t.el)
                         }
                 }
-                const rn = e => e && (e.disabled || "" === e.disabled),
-                    on = e => "undefined" != typeof SVGElement && e instanceof SVGElement,
-                    sn = (e, t) => {
+                const rn = e => e.__isTeleport,
+                    on = e => e && (e.disabled || "" === e.disabled),
+                    sn = e => "undefined" != typeof SVGElement && e instanceof SVGElement,
+                    an = (e, t) => {
                         const n = e && e.to;
                         if ((0, o.isString)(n)) {
                             if (t) {
                                 const e = t(n);
                                 return e
                             }
                             return null
                         }
                         return n
                     };
 
-                function an(e, t, n, {
+                function cn(e, t, n, {
                     o: {
                         insert: r
                     },
                     m: o
                 }, i = 2) {
                     0 === i && r(e.targetAnchor, t, n);
                     const {
                         el: s,
                         anchor: a,
                         shapeFlag: c,
                         children: l,
                         props: u
                     } = e, d = 2 === i;
-                    if (d && r(s, t, n), (!d || rn(u)) && 16 & c)
+                    if (d && r(s, t, n), (!d || on(u)) && 16 & c)
                         for (let e = 0; e < l.length; e++) o(l[e], t, n, 2);
                     d && r(a, t, n)
                 }
-                const cn = {
+                const ln = {
                     __isTeleport: !0,
                     process(e, t, n, r, o, i, s, a, c, l) {
                         const {
                             mc: u,
                             pc: d,
                             pbc: f,
                             o: {
                                 insert: p,
                                 querySelector: h,
                                 createText: m,
                                 createComment: g
                             }
-                        } = l, v = rn(t.props);
+                        } = l, v = on(t.props);
                         let {
                             shapeFlag: y,
                             children: b,
                             dynamicChildren: _
                         } = t;
                         if (null == e) {
                             const e = t.el = m(""),
                                 l = t.anchor = m("");
                             p(e, n, r), p(l, n, r);
-                            const d = t.target = sn(t.props, h),
+                            const d = t.target = an(t.props, h),
                                 f = t.targetAnchor = m("");
-                            d && (p(f, d), s = s || on(d));
+                            d && (p(f, d), s = s || sn(d));
                             const g = (e, t) => {
                                 16 & y && u(b, e, t, o, i, s, a, c)
                             };
                             v ? g(n, l) : d && g(d, f)
                         } else {
                             t.el = e.el;
                             const r = t.anchor = e.anchor,
                                 u = t.target = e.target,
                                 p = t.targetAnchor = e.targetAnchor,
-                                m = rn(e.props),
+                                m = on(e.props),
                                 g = m ? n : u,
                                 y = m ? r : p;
-                            if (s = s || on(u), _ ? (f(e.dynamicChildren, _, g, o, i, s, a), nn(e, t, !0)) : c || d(e, t, g, y, o, i, s, a, !1), v) m || an(t, n, r, l, 1);
+                            if (s = s || sn(u), _ ? (f(e.dynamicChildren, _, g, o, i, s, a), nn(e, t, !0)) : c || d(e, t, g, y, o, i, s, a, !1), v) m || cn(t, n, r, l, 1);
                             else if ((t.props && t.props.to) !== (e.props && e.props.to)) {
-                                const e = t.target = sn(t.props, h);
-                                e && an(t, e, null, l, 0)
-                            } else m && an(t, u, p, l, 1)
+                                const e = t.target = an(t.props, h);
+                                e && cn(t, e, null, l, 0)
+                            } else m && cn(t, u, p, l, 1)
                         }
-                        ln(t)
+                        un(t)
                     },
                     remove(e, t, n, r, {
                         um: o,
                         o: {
                             remove: i
                         }
                     }, s) {
@@ -6241,121 +6242,121 @@
                             shapeFlag: a,
                             children: c,
                             anchor: l,
                             targetAnchor: u,
                             target: d,
                             props: f
                         } = e;
-                        if (d && i(u), (s || !rn(f)) && (i(l), 16 & a))
+                        if (d && i(u), (s || !on(f)) && (i(l), 16 & a))
                             for (let e = 0; e < c.length; e++) {
                                 const r = c[e];
                                 o(r, t, n, !0, !!r.dynamicChildren)
                             }
                     },
-                    move: an,
+                    move: cn,
                     hydrate: function(e, t, n, r, o, i, {
                         o: {
                             nextSibling: s,
                             parentNode: a,
                             querySelector: c
                         }
                     }, l) {
-                        const u = t.target = sn(t.props, c);
+                        const u = t.target = an(t.props, c);
                         if (u) {
                             const c = u._lpa || u.firstChild;
                             if (16 & t.shapeFlag)
-                                if (rn(t.props)) t.anchor = l(s(e), t, a(e), n, r, o, i), t.targetAnchor = c;
+                                if (on(t.props)) t.anchor = l(s(e), t, a(e), n, r, o, i), t.targetAnchor = c;
                                 else {
                                     t.anchor = s(e);
                                     let a = c;
                                     for (; a;)
                                         if (a = s(a), a && 8 === a.nodeType && "teleport anchor" === a.data) {
                                             t.targetAnchor = a, u._lpa = t.targetAnchor && s(t.targetAnchor);
                                             break
                                         } l(c, t, u, n, r, o, i)
-                                } ln(t)
+                                } un(t)
                         }
                         return t.anchor && s(t.anchor)
                     }
                 };
 
-                function ln(e) {
+                function un(e) {
                     const t = e.ctx;
                     if (t && t.ut) {
                         let n = e.children[0].el;
                         for (; n !== e.targetAnchor;) 1 === n.nodeType && n.setAttribute("data-v-owner", t.uid), n = n.nextSibling;
                         t.ut()
                     }
                 }
-                const un = Symbol(void 0),
-                    dn = Symbol(void 0),
+                const dn = Symbol(void 0),
                     fn = Symbol(void 0),
                     pn = Symbol(void 0),
-                    hn = [];
-                let mn = null;
+                    hn = Symbol(void 0),
+                    mn = [];
+                let gn = null;
 
-                function gn(e = !1) {
-                    hn.push(mn = e ? null : [])
+                function vn(e = !1) {
+                    mn.push(gn = e ? null : [])
                 }
 
-                function vn() {
-                    hn.pop(), mn = hn[hn.length - 1] || null
+                function yn() {
+                    mn.pop(), gn = mn[mn.length - 1] || null
                 }
-                let yn, bn = 1;
+                let bn, _n = 1;
 
-                function _n(e) {
-                    bn += e
+                function Sn(e) {
+                    _n += e
                 }
 
-                function Sn(e) {
-                    return e.dynamicChildren = bn > 0 ? mn || o.EMPTY_ARR : null, vn(), bn > 0 && mn && mn.push(e), e
+                function wn(e) {
+                    return e.dynamicChildren = _n > 0 ? gn || o.EMPTY_ARR : null, yn(), _n > 0 && gn && gn.push(e), e
                 }
 
-                function wn(e, t, n, r, o, i) {
-                    return Sn(Pn(e, t, n, r, o, i, !0))
+                function En(e, t, n, r, o, i) {
+                    return wn(Nn(e, t, n, r, o, i, !0))
                 }
 
-                function En(e, t, n, r, o) {
-                    return Sn(Nn(e, t, n, r, o, !0))
+                function xn(e, t, n, r, o) {
+                    return wn(Rn(e, t, n, r, o, !0))
                 }
 
-                function xn(e) {
+                function On(e) {
                     return !!e && !0 === e.__v_isVNode
                 }
 
-                function On(e, t) {
+                function kn(e, t) {
                     return e.type === t.type && e.key === t.key
                 }
 
-                function kn(e) {
-                    yn = e
+                function Cn(e) {
+                    bn = e
                 }
-                const Cn = "__vInternal",
-                    Tn = ({
+                const Tn = "__vInternal",
+                    An = ({
                         key: e
                     }) => null != e ? e : null,
-                    An = ({
+                    Pn = ({
                         ref: e,
                         ref_key: t,
                         ref_for: n
                     }) => null != e ? (0, o.isString)(e) || (0, r.dq)(e) || (0, o.isFunction)(e) ? {
                         i: V,
                         r: e,
                         k: t,
                         f: !!n
                     } : e : null;
 
-                function Pn(e, t = null, n = null, r = 0, i = null, s = (e === un ? 0 : 1), a = !1, c = !1) {
+                function Nn(e, t = null, n = null, r = 0, i = null, s = (e === dn ? 0 : 1), a = !1, c = !1) {
                     const l = {
                         __v_isVNode: !0,
                         __v_skip: !0,
                         type: e,
                         props: t,
-                        key: t && Tn(t),
-                        ref: t && An(t),
+                        key: t && An(t),
+                        ref: t && Pn(t),
                         scopeId: $,
                         slotScopeIds: null,
                         children: n,
                         component: null,
                         suspense: null,
                         ssContent: null,
                         ssFallback: null,
@@ -6369,121 +6370,121 @@
                         shapeFlag: s,
                         patchFlag: r,
                         dynamicProps: i,
                         dynamicChildren: null,
                         appContext: null,
                         ctx: V
                     };
-                    return c ? (Un(l, n), 128 & s && e.normalize(l)) : n && (l.shapeFlag |= (0, o.isString)(n) ? 8 : 16), bn > 0 && !a && mn && (l.patchFlag > 0 || 6 & s) && 32 !== l.patchFlag && mn.push(l), l
+                    return c ? (Vn(l, n), 128 & s && e.normalize(l)) : n && (l.shapeFlag |= (0, o.isString)(n) ? 8 : 16), _n > 0 && !a && gn && (l.patchFlag > 0 || 6 & s) && 32 !== l.patchFlag && gn.push(l), l
                 }
-                const Nn = Rn;
+                const Rn = Dn;
 
-                function Rn(e, t = null, n = null, i = 0, s = null, a = !1) {
-                    if (e && e !== rt || (e = fn), xn(e)) {
-                        const r = Mn(e, t, !0);
-                        return n && Un(r, n), bn > 0 && !a && mn && (6 & r.shapeFlag ? mn[mn.indexOf(e)] = r : mn.push(r)), r.patchFlag |= -2, r
+                function Dn(e, t = null, n = null, i = 0, s = null, a = !1) {
+                    if (e && e !== rt || (e = pn), On(e)) {
+                        const r = In(e, t, !0);
+                        return n && Vn(r, n), _n > 0 && !a && gn && (6 & r.shapeFlag ? gn[gn.indexOf(e)] = r : gn.push(r)), r.patchFlag |= -2, r
                     }
-                    if (cr(e) && (e = e.__vccOpts), t) {
-                        t = Dn(t);
+                    if (lr(e) && (e = e.__vccOpts), t) {
+                        t = Mn(t);
                         let {
                             class: e,
                             style: n
                         } = t;
                         e && !(0, o.isString)(e) && (t.class = (0, o.normalizeClass)(e)), (0, o.isObject)(n) && ((0, r.X3)(n) && !(0, o.isArray)(n) && (n = (0, o.extend)({}, n)), t.style = (0, o.normalizeStyle)(n))
                     }
-                    return Pn(e, t, n, i, s, (0, o.isString)(e) ? 1 : ee(e) ? 128 : (e => e.__isTeleport)(e) ? 64 : (0, o.isObject)(e) ? 4 : (0, o.isFunction)(e) ? 2 : 0, a, !0)
+                    return Nn(e, t, n, i, s, (0, o.isString)(e) ? 1 : ee(e) ? 128 : rn(e) ? 64 : (0, o.isObject)(e) ? 4 : (0, o.isFunction)(e) ? 2 : 0, a, !0)
                 }
 
-                function Dn(e) {
-                    return e ? (0, r.X3)(e) || Cn in e ? (0, o.extend)({}, e) : e : null
+                function Mn(e) {
+                    return e ? (0, r.X3)(e) || Tn in e ? (0, o.extend)({}, e) : e : null
                 }
 
-                function Mn(e, t, n = !1) {
+                function In(e, t, n = !1) {
                     const {
                         props: r,
                         ref: i,
                         patchFlag: s,
                         children: a
-                    } = e, c = t ? Vn(r || {}, t) : r;
+                    } = e, c = t ? $n(r || {}, t) : r;
                     return {
                         __v_isVNode: !0,
                         __v_skip: !0,
                         type: e.type,
                         props: c,
-                        key: c && Tn(c),
-                        ref: t && t.ref ? n && i ? (0, o.isArray)(i) ? i.concat(An(t)) : [i, An(t)] : An(t) : i,
+                        key: c && An(c),
+                        ref: t && t.ref ? n && i ? (0, o.isArray)(i) ? i.concat(Pn(t)) : [i, Pn(t)] : Pn(t) : i,
                         scopeId: e.scopeId,
                         slotScopeIds: e.slotScopeIds,
                         children: a,
                         target: e.target,
                         targetAnchor: e.targetAnchor,
                         staticCount: e.staticCount,
                         shapeFlag: e.shapeFlag,
-                        patchFlag: t && e.type !== un ? -1 === s ? 16 : 16 | s : s,
+                        patchFlag: t && e.type !== dn ? -1 === s ? 16 : 16 | s : s,
                         dynamicProps: e.dynamicProps,
                         dynamicChildren: e.dynamicChildren,
                         appContext: e.appContext,
                         dirs: e.dirs,
                         transition: e.transition,
                         component: e.component,
                         suspense: e.suspense,
-                        ssContent: e.ssContent && Mn(e.ssContent),
-                        ssFallback: e.ssFallback && Mn(e.ssFallback),
+                        ssContent: e.ssContent && In(e.ssContent),
+                        ssFallback: e.ssFallback && In(e.ssFallback),
                         el: e.el,
                         anchor: e.anchor,
                         ctx: e.ctx,
                         ce: e.ce
                     }
                 }
 
-                function In(e = " ", t = 0) {
-                    return Nn(dn, null, e, t)
+                function jn(e = " ", t = 0) {
+                    return Rn(fn, null, e, t)
                 }
 
-                function jn(e, t) {
-                    const n = Nn(pn, null, e);
+                function Ln(e, t) {
+                    const n = Rn(hn, null, e);
                     return n.staticCount = t, n
                 }
 
-                function Ln(e = "", t = !1) {
-                    return t ? (gn(), En(fn, null, e)) : Nn(fn, null, e)
+                function Fn(e = "", t = !1) {
+                    return t ? (vn(), xn(pn, null, e)) : Rn(pn, null, e)
                 }
 
-                function Fn(e) {
-                    return null == e || "boolean" == typeof e ? Nn(fn) : (0, o.isArray)(e) ? Nn(un, null, e.slice()) : "object" == typeof e ? Bn(e) : Nn(dn, null, String(e))
+                function Bn(e) {
+                    return null == e || "boolean" == typeof e ? Rn(pn) : (0, o.isArray)(e) ? Rn(dn, null, e.slice()) : "object" == typeof e ? Un(e) : Rn(fn, null, String(e))
                 }
 
-                function Bn(e) {
-                    return null === e.el && -1 !== e.patchFlag || e.memo ? e : Mn(e)
+                function Un(e) {
+                    return null === e.el && -1 !== e.patchFlag || e.memo ? e : In(e)
                 }
 
-                function Un(e, t) {
+                function Vn(e, t) {
                     let n = 0;
                     const {
                         shapeFlag: r
                     } = e;
                     if (null == t) t = null;
                     else if ((0, o.isArray)(t)) n = 16;
                     else if ("object" == typeof t) {
                         if (65 & r) {
                             const n = t.default;
-                            return void(n && (n._c && (n._d = !1), Un(e, n()), n._c && (n._d = !0)))
+                            return void(n && (n._c && (n._d = !1), Vn(e, n()), n._c && (n._d = !0)))
                         } {
                             n = 32;
                             const r = t._;
-                            r || Cn in t ? 3 === r && V && (1 === V.slots._ ? t._ = 1 : (t._ = 2, e.patchFlag |= 1024)) : t._ctx = V
+                            r || Tn in t ? 3 === r && V && (1 === V.slots._ ? t._ = 1 : (t._ = 2, e.patchFlag |= 1024)) : t._ctx = V
                         }
                     } else(0, o.isFunction)(t) ? (t = {
                         default: t,
                         _ctx: V
-                    }, n = 32) : (t = String(t), 64 & r ? (n = 16, t = [In(t)]) : n = 8);
+                    }, n = 32) : (t = String(t), 64 & r ? (n = 16, t = [jn(t)]) : n = 8);
                     e.children = t, e.shapeFlag |= n
                 }
 
-                function Vn(...e) {
+                function $n(...e) {
                     const t = {};
                     for (let n = 0; n < e.length; n++) {
                         const r = e[n];
                         for (const e in r)
                             if ("class" === e) t.class !== r.class && (t.class = (0, o.normalizeClass)([t.class, r.class]));
                             else if ("style" === e) t.style = (0, o.normalizeStyle)([t.style, r.style]);
                         else if ((0, o.isOn)(e)) {
@@ -6491,25 +6492,25 @@
                                 i = r[e];
                             !i || n === i || (0, o.isArray)(n) && n.includes(i) || (t[e] = n ? [].concat(n, i) : i)
                         } else "" !== e && (t[e] = r[e])
                     }
                     return t
                 }
 
-                function $n(e, t, n, r = null) {
+                function Hn(e, t, n, r = null) {
                     c(e, t, 7, [n, r])
                 }
-                const Hn = Ht();
-                let qn = 0;
+                const qn = Ht();
+                let zn = 0;
 
-                function zn(e, t, n) {
+                function Yn(e, t, n) {
                     const i = e.type,
-                        s = (t ? t.appContext : e.appContext) || Hn,
+                        s = (t ? t.appContext : e.appContext) || qn,
                         a = {
-                            uid: qn++,
+                            uid: zn++,
                             vnode: e,
                             type: i,
                             parent: t,
                             appContext: s,
                             root: null,
                             next: null,
                             subTree: null,
@@ -6562,102 +6563,102 @@
                             ec: null,
                             sp: null
                         };
                     return a.ctx = {
                         _: a
                     }, a.root = t ? t.root : a, a.emit = F.bind(null, a), e.ce && e.ce(a), a
                 }
-                let Yn = null;
-                const Wn = () => Yn || V,
-                    Kn = e => {
-                        Yn = e, e.scope.on()
+                let Wn = null;
+                const Kn = () => Wn || V,
+                    Jn = e => {
+                        Wn = e, e.scope.on()
                     },
-                    Jn = () => {
-                        Yn && Yn.scope.off(), Yn = null
+                    Gn = () => {
+                        Wn && Wn.scope.off(), Wn = null
                     };
 
-                function Gn(e) {
+                function Xn(e) {
                     return 4 & e.vnode.shapeFlag
                 }
-                let Xn, Zn, Qn = !1;
+                let Zn, Qn, er = !1;
 
-                function er(e, t = !1) {
-                    Qn = t;
+                function tr(e, t = !1) {
+                    er = t;
                     const {
                         props: n,
                         children: i
-                    } = e.vnode, s = Gn(e);
+                    } = e.vnode, s = Xn(e);
                     ! function(e, t, n, i = !1) {
                         const s = {},
                             a = {};
-                        (0, o.def)(a, Cn, 1), e.propsDefaults = Object.create(null), At(e, t, s, a);
+                        (0, o.def)(a, Tn, 1), e.propsDefaults = Object.create(null), At(e, t, s, a);
                         for (const t in e.propsOptions[0]) t in s || (s[t] = void 0);
                         n ? e.props = i ? s : (0, r.Um)(s) : e.type.props ? e.props = s : e.props = a, e.attrs = a
                     }(e, n, s, t), Vt(e, i);
                     const c = s ? function(e, t) {
                         const n = e.type;
                         0;
                         e.accessCache = Object.create(null), e.proxy = (0, r.Xl)(new Proxy(e.ctx, gt)), !1;
                         const {
                             setup: i
                         } = n;
                         if (i) {
-                            const n = e.setupContext = i.length > 1 ? ir(e) : null;
-                            Kn(e), (0, r.Jd)();
+                            const n = e.setupContext = i.length > 1 ? sr(e) : null;
+                            Jn(e), (0, r.Jd)();
                             const s = a(i, e, 0, [e.props, n]);
-                            if ((0, r.lk)(), Jn(), (0, o.isPromise)(s)) {
-                                if (s.then(Jn, Jn), t) return s.then((n => {
-                                    tr(e, n, t)
+                            if ((0, r.lk)(), Gn(), (0, o.isPromise)(s)) {
+                                if (s.then(Gn, Gn), t) return s.then((n => {
+                                    nr(e, n, t)
                                 })).catch((t => {
                                     l(t, e, 0)
                                 }));
                                 e.asyncDep = s
-                            } else tr(e, s, t)
-                        } else or(e, t)
+                            } else nr(e, s, t)
+                        } else ir(e, t)
                     }(e, t) : void 0;
-                    return Qn = !1, c
+                    return er = !1, c
                 }
 
-                function tr(e, t, n) {
-                    (0, o.isFunction)(t) ? e.type.__ssrInlineRender ? e.ssrRender = t : e.render = t: (0, o.isObject)(t) && (__VUE_PROD_DEVTOOLS__ && (e.devtoolsRawSetupState = t), e.setupState = (0, r.WL)(t)), or(e, n)
+                function nr(e, t, n) {
+                    (0, o.isFunction)(t) ? e.type.__ssrInlineRender ? e.ssrRender = t : e.render = t: (0, o.isObject)(t) && (__VUE_PROD_DEVTOOLS__ && (e.devtoolsRawSetupState = t), e.setupState = (0, r.WL)(t)), ir(e, n)
                 }
 
-                function nr(e) {
-                    Xn = e, Zn = e => {
+                function rr(e) {
+                    Zn = e, Qn = e => {
                         e.render._rc && (e.withProxy = new Proxy(e.ctx, vt))
                     }
                 }
-                const rr = () => !Xn;
+                const or = () => !Zn;
 
-                function or(e, t, n) {
+                function ir(e, t, n) {
                     const i = e.type;
                     if (!e.render) {
-                        if (!t && Xn && !i.render) {
+                        if (!t && Zn && !i.render) {
                             const t = i.template || wt(e).template;
                             if (t) {
                                 0;
                                 const {
                                     isCustomElement: n,
                                     compilerOptions: r
                                 } = e.appContext.config, {
                                     delimiters: s,
                                     compilerOptions: a
                                 } = i, c = (0, o.extend)((0, o.extend)({
                                     isCustomElement: n,
                                     delimiters: s
                                 }, r), a);
-                                i.render = Xn(t, c)
+                                i.render = Zn(t, c)
                             }
                         }
-                        e.render = i.render || o.NOOP, Zn && Zn(e)
+                        e.render = i.render || o.NOOP, Qn && Qn(e)
                     }
-                    __VUE_OPTIONS_API__ && (Kn(e), (0, r.Jd)(), bt(e), (0, r.lk)(), Jn())
+                    __VUE_OPTIONS_API__ && (Jn(e), (0, r.Jd)(), bt(e), (0, r.lk)(), Gn())
                 }
 
-                function ir(e) {
+                function sr(e) {
                     const t = t => {
                         e.exposed = t || {}
                     };
                     let n;
                     return {
                         get attrs() {
                             return n || (n = function(e) {
@@ -6668,131 +6669,131 @@
                         },
                         slots: e.slots,
                         emit: e.emit,
                         expose: t
                     }
                 }
 
-                function sr(e) {
+                function ar(e) {
                     if (e.exposed) return e.exposeProxy || (e.exposeProxy = new Proxy((0, r.WL)((0, r.Xl)(e.exposed)), {
                         get: (t, n) => n in t ? t[n] : n in ht ? ht[n](e) : void 0,
                         has: (e, t) => t in e || t in ht
                     }))
                 }
 
-                function ar(e, t = !0) {
+                function cr(e, t = !0) {
                     return (0, o.isFunction)(e) ? e.displayName || e.name : e.name || t && e.__name
                 }
 
-                function cr(e) {
+                function lr(e) {
                     return (0, o.isFunction)(e) && "__vccOpts" in e
                 }
-                const lr = (e, t) => (0, r.Fl)(e, t, Qn);
+                const ur = (e, t) => (0, r.Fl)(e, t, er);
 
-                function ur() {
+                function dr() {
                     return null
                 }
 
-                function dr() {
+                function fr() {
                     return null
                 }
 
-                function fr(e) {
+                function pr(e) {
                     0
                 }
 
-                function pr(e, t) {
+                function hr(e, t) {
                     return null
                 }
 
-                function hr() {
-                    return gr().slots
-                }
-
                 function mr() {
-                    return gr().attrs
+                    return vr().slots
                 }
 
                 function gr() {
-                    const e = Wn();
-                    return e.setupContext || (e.setupContext = ir(e))
+                    return vr().attrs
+                }
+
+                function vr() {
+                    const e = Kn();
+                    return e.setupContext || (e.setupContext = sr(e))
                 }
 
-                function vr(e, t) {
+                function yr(e, t) {
                     const n = (0, o.isArray)(e) ? e.reduce(((e, t) => (e[t] = {}, e)), {}) : e;
                     for (const e in t) {
                         const r = n[e];
                         r ? (0, o.isArray)(r) || (0, o.isFunction)(r) ? n[e] = {
                             type: r,
                             default: t[e]
                         } : r.default = t[e] : null === r && (n[e] = {
                             default: t[e]
                         })
                     }
                     return n
                 }
 
-                function yr(e, t) {
+                function br(e, t) {
                     const n = {};
                     for (const r in e) t.includes(r) || Object.defineProperty(n, r, {
                         enumerable: !0,
                         get: () => e[r]
                     });
                     return n
                 }
 
-                function br(e) {
-                    const t = Wn();
+                function _r(e) {
+                    const t = Kn();
                     let n = e();
-                    return Jn(), (0, o.isPromise)(n) && (n = n.catch((e => {
-                        throw Kn(t), e
-                    }))), [n, () => Kn(t)]
+                    return Gn(), (0, o.isPromise)(n) && (n = n.catch((e => {
+                        throw Jn(t), e
+                    }))), [n, () => Jn(t)]
                 }
 
-                function _r(e, t, n) {
+                function Sr(e, t, n) {
                     const r = arguments.length;
-                    return 2 === r ? (0, o.isObject)(t) && !(0, o.isArray)(t) ? xn(t) ? Nn(e, null, [t]) : Nn(e, t) : Nn(e, null, t) : (r > 3 ? n = Array.prototype.slice.call(arguments, 2) : 3 === r && xn(n) && (n = [n]), Nn(e, t, n))
+                    return 2 === r ? (0, o.isObject)(t) && !(0, o.isArray)(t) ? On(t) ? Rn(e, null, [t]) : Rn(e, t) : Rn(e, null, t) : (r > 3 ? n = Array.prototype.slice.call(arguments, 2) : 3 === r && On(n) && (n = [n]), Rn(e, t, n))
                 }
-                const Sr = Symbol(""),
-                    wr = () => {
+                const wr = Symbol(""),
+                    Er = () => {
                         {
-                            const e = ce(Sr);
+                            const e = ce(wr);
                             return e
                         }
                     };
 
-                function Er() {
+                function xr() {
                     return void 0
                 }
 
-                function xr(e, t, n, r) {
+                function Or(e, t, n, r) {
                     const o = n[r];
-                    if (o && Or(o, e)) return o;
+                    if (o && kr(o, e)) return o;
                     const i = t();
                     return i.memo = e.slice(), n[r] = i
                 }
 
-                function Or(e, t) {
+                function kr(e, t) {
                     const n = e.memo;
                     if (n.length != t.length) return !1;
                     for (let e = 0; e < n.length; e++)
                         if ((0, o.hasChanged)(n[e], t[e])) return !1;
-                    return bn > 0 && mn && mn.push(e), !0
+                    return _n > 0 && gn && gn.push(e), !0
                 }
-                const kr = "3.2.47",
-                    Cr = {
-                        createComponentInstance: zn,
-                        setupComponent: er,
+                const Cr = "3.2.47",
+                    Tr = {
+                        createComponentInstance: Yn,
+                        setupComponent: tr,
                         renderComponentRoot: K,
                         setCurrentRenderingInstance: H,
-                        isVNode: xn,
-                        normalizeVNode: Fn
+                        isVNode: On,
+                        normalizeVNode: Bn
                     },
-                    Tr = null,
-                    Ar = null
+                    Ar = null,
+                    Pr = null
             },
             963: (e, t, n) => {
                 "use strict";
                 n.r(t), n.d(t, {
                     BaseTransition: () => o.P$,
                     Comment: () => o.sv,
                     EffectScope: () => o.Bj,
@@ -13816,36 +13817,39 @@
                     })
                 } catch (e) {}
                 Object.defineProperty(e, "adapterName", {
                     value: t
                 })
             }
         }));
-        const we = e => {
-            e = M.isArray(e) ? e : [e];
-            const {
-                length: t
-            } = e;
-            let n, r;
-            for (let o = 0; o < t && (n = e[o], !(r = M.isString(n) ? Se[n.toLowerCase()] : n)); o++);
-            if (!r) {
-                if (!1 === r) throw new F(`Adapter ${n} is not supported by the environment`, "ERR_NOT_SUPPORT");
-                throw new Error(M.hasOwnProp(Se, n) ? `Adapter '${n}' is not available in the build` : `Unknown adapter '${n}'`)
-            }
-            if (!M.isFunction(r)) throw new TypeError("adapter is not a function");
-            return r
+        const we = {
+            getAdapter: e => {
+                e = M.isArray(e) ? e : [e];
+                const {
+                    length: t
+                } = e;
+                let n, r;
+                for (let o = 0; o < t && (n = e[o], !(r = M.isString(n) ? Se[n.toLowerCase()] : n)); o++);
+                if (!r) {
+                    if (!1 === r) throw new F(`Adapter ${n} is not supported by the environment`, "ERR_NOT_SUPPORT");
+                    throw new Error(M.hasOwnProp(Se, n) ? `Adapter '${n}' is not available in the build` : `Unknown adapter '${n}'`)
+                }
+                if (!M.isFunction(r)) throw new TypeError("adapter is not a function");
+                return r
+            },
+            adapters: Se
         };
 
         function Ee(e) {
             if (e.cancelToken && e.cancelToken.throwIfRequested(), e.signal && e.signal.aborted) throw new he(null, e)
         }
 
         function xe(e) {
             Ee(e), e.headers = ue.from(e.headers), e.data = de.call(e, e.transformRequest), -1 !== ["post", "put", "patch"].indexOf(e.method) && e.headers.setContentType("application/x-www-form-urlencoded", !1);
-            return we(e.adapter || re.adapter)(e).then((function(t) {
+            return we.getAdapter(e.adapter || re.adapter)(e).then((function(t) {
                 return Ee(e), t.data = de.call(e, e.transformResponse, t), t.headers = ue.from(t.headers), t
             }), (function(t) {
                 return fe(t) || (Ee(e), t && t.response && (t.response.data = de.call(e, e.transformResponse, t.response), t.response.headers = ue.from(t.response.headers))), Promise.reject(t)
             }))
         }
         const Oe = e => e instanceof ue ? e.toJSON() : e;
 
@@ -14639,36 +14643,38 @@
                     }, null, 8, zt)], 2), (0, qe.Wm)(a, {
                         block: n.block
                     }, null, 8, ["block"])]), (0, qe.Wm)(c, {
                         block: n.block
                     }, null, 8, ["block"])], 2)
                 }]
             ]);
-        let Kt, Jt, Gt;
-        const Xt = {
+        const Kt = {
                 props: ["app_node"],
                 components: {
                     draggable: ot(),
                     StreamBlock: Ht,
                     AbstractBlock: Wt
                 },
                 data: () => ({
                     blocks: {},
                     show_help: !1,
                     show_add_block: !1,
                     will_removed: [],
                     stream: [],
                     model_info: {},
                     base_admin_url: "",
-                    stream_texts: window.stream_texts
+                    stream_texts: window.stream_texts,
+                    text_area: null,
+                    delete_blocks_from_db: null,
+                    popup_size: null
                 }),
                 beforeMount: function() {
-                    if (Kt = this.app_node.querySelector("textarea"), Jt = Boolean(Kt.hasAttribute("delete_blocks_from_db")), Gt = Kt.dataset.popup_size ? JSON.parse(Kt.dataset.popup_size) : [1e3, 500], this.base_admin_url = Kt.getAttribute("base_admin_url"), this.stream = JSON.parse(Kt.innerHTML), this.model_info = JSON.parse(Kt.getAttribute("model_list_info")), this.stream.length && !this.stream[0].hasOwnProperty("collapsed") && this.setAllCollapsed(!1), Jt) {
+                    if (this.text_area = this.app_node.querySelector("textarea"), this.delete_blocks_from_db = Boolean(this.text_area.hasAttribute("delete_blocks_from_db")), this.popup_size = this.text_area.dataset.popup_size ? JSON.parse(this.text_area.dataset.popup_size) : [1e3, 500], this.base_admin_url = this.text_area.getAttribute("base_admin_url"), this.stream = JSON.parse(this.text_area.innerHTML), this.model_info = JSON.parse(this.text_area.getAttribute("model_list_info")), this.stream.length && !this.stream[0].hasOwnProperty("collapsed") && this.setAllCollapsed(!1), this.delete_blocks_from_db) {
                         let e = this;
-                        django.jQuery('input[type="submit"]', Kt.closest("form")).on("click", (function(t) {
+                        django.jQuery('input[type="submit"]', this.text_area.closest("form")).on("click", (function(t) {
                             if (e.will_removed.length) {
                                 t.preventDefault();
                                 for (var n = [], r = e.will_removed.length - 1; r >= 0; r--)
                                     if (-1 != e.will_removed[r].id)
                                         if (it(e.will_removed[r].id))
                                             for (var o = e.will_removed[r].id, i = o.length - 1; i >= 0; i--) n.push(e.deleteAction(e.will_removed[r], o[i], r));
                                         else n.push(e.deleteAction(e.will_removed[r], e.will_removed[r].id, r));
@@ -14732,35 +14738,35 @@
                             collapsed: !1
                         }, e.abstract || (r.id = e.as_list ? [] : -1), n ? this.stream.splice(n, 0, r) : this.stream.push(r), this.show_add_block = !1
                     },
                     openPopup: function(e) {
                         let t = e.target,
                             n = t.id.replace(/^(change|add|delete)_/, "").replace(/\./g, "__dot__").replace(/\-/g, "__dash__");
                         let r = t.href;
-                        return window.open(r, n, "height=" + Gt[1] + ",width=" + Gt[0] + ",resizable=yes,scrollbars=yes").focus(), !1
+                        return window.open(r, n, "height=" + this.popup_size[1] + ",width=" + this.popup_size[0] + ",resizable=yes,scrollbars=yes").focus(), !1
                     }
                 },
                 watch: {
                     stream: {
                         handler(e) {
-                            Kt.innerHTML = JSON.stringify(e.map((function(e) {
+                            this.text_area.innerHTML = JSON.stringify(e.map((function(e) {
                                 return {
                                     unique_id: e.unique_id,
                                     model_name: e.model_name,
                                     id: e.id,
                                     options: e.options,
                                     collapsed: e.collapsed
                                 }
                             })))
                         },
                         deep: !0
                     }
                 }
             },
-            Zt = (0, Ot.Z)(Xt, [
+            Jt = (0, Ot.Z)(Kt, [
                 ["render", function(e, t, n, r, o, i) {
                     const s = (0, qe.up)("StreamBlock"),
                         a = (0, qe.up)("AbstractBlock"),
                         c = (0, qe.up)("draggable");
                     return (0, qe.wg)(), (0, qe.iD)("div", null, [o.stream_texts.help_text ? ((0, qe.wg)(), (0, qe.iD)("div", Ye, [(0, qe._)("div", {
                         class: "stream-help-text__title",
                         onClick: t[0] || (t[0] = e => o.show_help = !o.show_help),
@@ -14779,15 +14785,15 @@
                         href: "javascript:;",
                         onClick: t[2] || (t[2] = e => i.setAllCollapsed(!0)),
                         innerHTML: o.stream_texts["Collapse all"] + " −",
                         class: "collapse-handler"
                     }, null, 8, Xe)])) : (0, qe.kq)("v-if", !0), (0, qe._)("div", Ze, [(0, qe.Wm)(c, {
                         modelValue: o.stream,
                         "onUpdate:modelValue": t[3] || (t[3] = e => o.stream = e),
-                        group: "stream",
+                        group: n.app_node.id,
                         handle: ".block-move",
                         "item-key": "unique_id"
                     }, {
                         item: (0, qe.w5)((e => {
                             let {
                                 element: t
                             } = e;
@@ -14798,15 +14804,15 @@
                             }, null, 8, ["block"])) : ((0, qe.wg)(), (0, qe.j4)(s, {
                                 key: 0,
                                 block: t,
                                 ref: t.unique_id
                             }, null, 8, ["block"]))]
                         })),
                         _: 1
-                    }, 8, ["modelValue"]), (0, qe._)("div", Qe, [(0, qe._)("div", {
+                    }, 8, ["modelValue", "group"]), (0, qe._)("div", Qe, [(0, qe._)("div", {
                         class: "add-new-block-button",
                         onClick: t[4] || (t[4] = e => o.show_add_block = !o.show_add_block),
                         textContent: (0, ze.toDisplayString)(o.stream_texts.AddNewBlock)
                     }, null, 8, et), o.show_add_block ? ((0, qe.wg)(), (0, qe.iD)("div", tt, [(0, qe._)("ul", null, [((0, qe.wg)(!0), (0, qe.iD)(qe.HY, null, (0, qe.Ko)(o.model_info, ((e, t) => ((0, qe.wg)(), (0, qe.iD)("li", null, [(0, qe._)("a", {
                         class: "stream-btn",
                         href: "#",
                         textContent: (0, ze.toDisplayString)("+ " + e.model_doc),
@@ -14820,15 +14826,15 @@
                 window.ax = Be.create({
                     headers: {
                         "X-CSRFToken": $e.get("csrftoken")
                     }
                 }), window.streamapps = {};
                 for (let t = 0; t < e.length; t++) {
                     let n = e[t],
-                        r = (0, He.createApp)(Zt, {
+                        r = (0, He.createApp)(Jt, {
                             app_node: n
                         }).mount(n.querySelector(".mount-node"));
                     window.streamapps[e[t].id] = r
                 }
             }()
         }))
     })()
```

### Comparing `django-streamfield-2.0.6/streamfield/templates/streamfield/admin/change_form.html` & `django-streamfield-2.0.7/streamfield/templates/streamfield/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/templates/streamfield/admin/fields/file_browse_widget.html` & `django-streamfield-2.0.7/streamfield/templates/streamfield/admin/fields/file_browse_widget.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/templates/streamfield/streamfield_widget.html` & `django-streamfield-2.0.7/streamfield/templates/streamfield/streamfield_widget.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/templatetags/streamfield_tags.py` & `django-streamfield-2.0.7/streamfield/templatetags/streamfield_tags.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/urls.py` & `django-streamfield-2.0.7/streamfield/urls.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.0.6/streamfield/views.py` & `django-streamfield-2.0.7/streamfield/views.py`

 * *Files identical despite different names*

