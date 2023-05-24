# Comparing `tmp/django-simple-notes-0.0.1.tar.gz` & `tmp/django-simple-notes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-notes-0.0.1.tar", last modified: Wed May 24 08:24:51 2023, max compression
+gzip compressed data, was "django-simple-notes-0.0.2.tar", last modified: Wed May 24 09:28:54 2023, max compression
```

## Comparing `django-simple-notes-0.0.1.tar` & `django-simple-notes-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 08:24:51.075263 django-simple-notes-0.0.1/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    35150 2023-05-16 09:56:11.000000 django-simple-notes-0.0.1/LICENSE
--rw-r--r--   0 kapt      (1000) kapt      (1000)      374 2023-05-16 09:56:11.000000 django-simple-notes-0.0.1/MANIFEST.in
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6983 2023-05-24 08:24:51.075263 django-simple-notes-0.0.1/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5847 2023-05-24 08:10:45.000000 django-simple-notes-0.0.1/README.md
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 08:24:51.067263 django-simple-notes-0.0.1/django_simple_notes/
--rw-r--r--   0 kapt      (1000) kapt      (1000)       22 2023-05-16 09:56:11.000000 django-simple-notes-0.0.1/django_simple_notes/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3183 2023-05-24 08:21:41.000000 django-simple-notes-0.0.1/django_simple_notes/admin.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      108 2023-05-19 14:57:18.000000 django-simple-notes-0.0.1/django_simple_notes/apps.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4791 2023-05-23 16:16:56.000000 django-simple-notes-0.0.1/django_simple_notes/cms_toolbars.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 08:24:51.071263 django-simple-notes-0.0.1/django_simple_notes/conf/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2023-05-16 09:56:11.000000 django-simple-notes-0.0.1/django_simple_notes/conf/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      636 2023-05-24 08:21:41.000000 django-simple-notes-0.0.1/django_simple_notes/conf/settings.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 08:24:51.063263 django-simple-notes-0.0.1/django_simple_notes/locale/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 08:24:51.063263 django-simple-notes-0.0.1/django_simple_notes/locale/fr/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 08:24:51.071263 django-simple-notes-0.0.1/django_simple_notes/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      655 2023-05-19 14:50:42.000000 django-simple-notes-0.0.1/django_simple_notes/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt      (1000) kapt      (1000)      879 2023-05-19 14:50:33.000000 django-simple-notes-0.0.1/django_simple_notes/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 08:24:51.071263 django-simple-notes-0.0.1/django_simple_notes/migrations/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2720 2023-05-23 16:16:32.000000 django-simple-notes-0.0.1/django_simple_notes/migrations/0001_initial.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2023-05-16 11:42:48.000000 django-simple-notes-0.0.1/django_simple_notes/migrations/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1085 2023-05-23 16:16:32.000000 django-simple-notes-0.0.1/django_simple_notes/models.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)       44 2023-05-19 14:59:18.000000 django-simple-notes-0.0.1/django_simple_notes/urls.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2023-05-19 14:57:15.000000 django-simple-notes-0.0.1/django_simple_notes/views.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 08:24:51.071263 django-simple-notes-0.0.1/django_simple_notes.egg-info/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6983 2023-05-24 08:24:51.000000 django-simple-notes-0.0.1/django_simple_notes.egg-info/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)      757 2023-05-24 08:24:51.000000 django-simple-notes-0.0.1/django_simple_notes.egg-info/SOURCES.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)        1 2023-05-24 08:24:51.000000 django-simple-notes-0.0.1/django_simple_notes.egg-info/dependency_links.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       11 2023-05-24 08:24:51.000000 django-simple-notes-0.0.1/django_simple_notes.egg-info/requires.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       20 2023-05-24 08:24:51.000000 django-simple-notes-0.0.1/django_simple_notes.egg-info/top_level.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)      642 2023-05-23 16:21:10.000000 django-simple-notes-0.0.1/pyproject.toml
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1164 2023-05-24 08:24:51.075263 django-simple-notes-0.0.1/setup.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)       52 2023-05-23 16:22:28.000000 django-simple-notes-0.0.1/setup.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 09:28:54.048838 django-simple-notes-0.0.2/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    35150 2023-05-16 09:56:11.000000 django-simple-notes-0.0.2/LICENSE
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      374 2023-05-16 09:56:11.000000 django-simple-notes-0.0.2/MANIFEST.in
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6983 2023-05-24 09:28:54.048838 django-simple-notes-0.0.2/PKG-INFO
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5847 2023-05-24 08:10:45.000000 django-simple-notes-0.0.2/README.md
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 09:28:54.048838 django-simple-notes-0.0.2/django_simple_notes/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       22 2023-05-16 09:56:11.000000 django-simple-notes-0.0.2/django_simple_notes/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3183 2023-05-24 08:21:41.000000 django-simple-notes-0.0.2/django_simple_notes/admin.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      108 2023-05-19 14:57:18.000000 django-simple-notes-0.0.2/django_simple_notes/apps.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4896 2023-05-24 09:22:35.000000 django-simple-notes-0.0.2/django_simple_notes/cms_toolbars.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 09:28:54.048838 django-simple-notes-0.0.2/django_simple_notes/conf/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2023-05-16 09:56:11.000000 django-simple-notes-0.0.2/django_simple_notes/conf/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      636 2023-05-24 08:21:41.000000 django-simple-notes-0.0.2/django_simple_notes/conf/settings.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 09:28:54.044838 django-simple-notes-0.0.2/django_simple_notes/locale/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 09:28:54.048838 django-simple-notes-0.0.2/django_simple_notes/locale/fr/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 09:28:54.048838 django-simple-notes-0.0.2/django_simple_notes/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      655 2023-05-19 14:50:42.000000 django-simple-notes-0.0.2/django_simple_notes/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      879 2023-05-19 14:50:33.000000 django-simple-notes-0.0.2/django_simple_notes/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 09:28:54.048838 django-simple-notes-0.0.2/django_simple_notes/migrations/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2720 2023-05-23 16:16:32.000000 django-simple-notes-0.0.2/django_simple_notes/migrations/0001_initial.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2023-05-16 11:42:48.000000 django-simple-notes-0.0.2/django_simple_notes/migrations/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1085 2023-05-23 16:16:32.000000 django-simple-notes-0.0.2/django_simple_notes/models.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       44 2023-05-19 14:59:18.000000 django-simple-notes-0.0.2/django_simple_notes/urls.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2023-05-19 14:57:15.000000 django-simple-notes-0.0.2/django_simple_notes/views.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-05-24 09:28:54.048838 django-simple-notes-0.0.2/django_simple_notes.egg-info/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6983 2023-05-24 09:28:54.000000 django-simple-notes-0.0.2/django_simple_notes.egg-info/PKG-INFO
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      757 2023-05-24 09:28:54.000000 django-simple-notes-0.0.2/django_simple_notes.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        1 2023-05-24 09:28:54.000000 django-simple-notes-0.0.2/django_simple_notes.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       11 2023-05-24 09:28:54.000000 django-simple-notes-0.0.2/django_simple_notes.egg-info/requires.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       20 2023-05-24 09:28:54.000000 django-simple-notes-0.0.2/django_simple_notes.egg-info/top_level.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      642 2023-05-23 16:21:10.000000 django-simple-notes-0.0.2/pyproject.toml
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1164 2023-05-24 09:28:54.048838 django-simple-notes-0.0.2/setup.cfg
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       52 2023-05-23 16:22:28.000000 django-simple-notes-0.0.2/setup.py
```

### Comparing `django-simple-notes-0.0.1/LICENSE` & `django-simple-notes-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-notes-0.0.1/PKG-INFO` & `django-simple-notes-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-notes
-Version: 0.0.1
+Version: 0.0.2
 Summary: Store simple notes linked to Django(-cms) pages. Supports apphooks (but not custom apps)!
 Home-page: https://gitlab.com/kapt/open-source/django-simple-notes
 Author: Dev Kapt
 Author-email: dev@kapt.mobi
 Project-URL: Documentation, https://gitlab.com/kapt/open-source/django-simple-notes/-/blob/main/README.md
 Project-URL: Release notes, https://gitlab.com/kapt/open-source/django-simple-notes/-/blob/main/CHANGELOG.rst
 Project-URL: Tracker, https://gitlab.com/kapt/open-source/django-simple-notes/-/issues
```

### Comparing `django-simple-notes-0.0.1/README.md` & `django-simple-notes-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-simple-notes-0.0.1/django_simple_notes/admin.py` & `django-simple-notes-0.0.2/django_simple_notes/admin.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-0.0.1/django_simple_notes/cms_toolbars.py` & `django-simple-notes-0.0.2/django_simple_notes/cms_toolbars.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,29 +24,31 @@
         object_ct, object_id = SIMPLE_NOTES_CUSTOM_CONTENT_TYPE_AND_ID(request)
         if object_ct is not None and object_id is not None:
             found = True
 
     if not found:
         # djangocms blog post (not the homepage of the blog, which should be treated as a regular cms page)
         if (
-            request.resolver_match.app_name == "djangocms_blog"
+            request.resolver_match
+            and request.resolver_match.app_name == "djangocms_blog"
             and "slug" in request.resolver_match.kwargs
         ):
             # Third party
             from djangocms_blog.models import Post
 
             post = Post.objects.get(
                 translations__slug=request.resolver_match.kwargs["slug"]
             )
             object_ct = Post
             object_id = post.id
         # regular cms pages
 
         elif (
-            "slug" in request.resolver_match.kwargs
+            request.resolver_match
+            and "slug" in request.resolver_match.kwargs
             and request.resolver_match.kwargs["slug"] == ""
         ):
             # Third party
             from cms.models import Page
 
             # homepage
             page = Page.objects.get(
@@ -57,15 +59,15 @@
             object_ct = Page
             object_id = page.id
         else:
             # Third party
             from cms.models import Page
 
             # regular page
-            if "slug" in request.resolver_match.kwargs:
+            if request.resolver_match and "slug" in request.resolver_match.kwargs:
                 slug = request.resolver_match.kwargs["slug"].split("/")[-1]
             else:
                 slug = request.resolver_match.route.split("/")
                 if slug[-1] == r"\Z":
                     slug = slug[-2]
                 else:
                     slug = slug[:-1]
```

### Comparing `django-simple-notes-0.0.1/django_simple_notes/conf/settings.py` & `django-simple-notes-0.0.2/django_simple_notes/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-0.0.1/django_simple_notes/locale/fr/LC_MESSAGES/django.mo` & `django-simple-notes-0.0.2/django_simple_notes/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-notes-0.0.1/django_simple_notes/locale/fr/LC_MESSAGES/django.po` & `django-simple-notes-0.0.2/django_simple_notes/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-simple-notes-0.0.1/django_simple_notes/migrations/0001_initial.py` & `django-simple-notes-0.0.2/django_simple_notes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-0.0.1/django_simple_notes/models.py` & `django-simple-notes-0.0.2/django_simple_notes/models.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-0.0.1/django_simple_notes.egg-info/PKG-INFO` & `django-simple-notes-0.0.2/django_simple_notes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-notes
-Version: 0.0.1
+Version: 0.0.2
 Summary: Store simple notes linked to Django(-cms) pages. Supports apphooks (but not custom apps)!
 Home-page: https://gitlab.com/kapt/open-source/django-simple-notes
 Author: Dev Kapt
 Author-email: dev@kapt.mobi
 Project-URL: Documentation, https://gitlab.com/kapt/open-source/django-simple-notes/-/blob/main/README.md
 Project-URL: Release notes, https://gitlab.com/kapt/open-source/django-simple-notes/-/blob/main/CHANGELOG.rst
 Project-URL: Tracker, https://gitlab.com/kapt/open-source/django-simple-notes/-/issues
```

### Comparing `django-simple-notes-0.0.1/django_simple_notes.egg-info/SOURCES.txt` & `django-simple-notes-0.0.2/django_simple_notes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-simple-notes-0.0.1/pyproject.toml` & `django-simple-notes-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-simple-notes-0.0.1/setup.cfg` & `django-simple-notes-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-simple-notes
-version = 0.0.1
+version = 0.0.2
 description = Store simple notes linked to Django(-cms) pages. Supports apphooks (but not custom apps)!
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = django, django-cms
 url = https://gitlab.com/kapt/open-source/django-simple-notes
 project_urls = 
 	Documentation = https://gitlab.com/kapt/open-source/django-simple-notes/-/blob/main/README.md
```

