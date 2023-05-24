# Comparing `tmp/django-typomatic-2.3.1.tar.gz` & `tmp/django-typomatic-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-typomatic-2.3.1.tar", last modified: Sat May 20 09:38:49 2023, max compression
+gzip compressed data, was "django-typomatic-2.3.2.tar", last modified: Wed May 24 12:50:40 2023, max compression
```

## Comparing `django-typomatic-2.3.1.tar` & `django-typomatic-2.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:38:49.233048 django-typomatic-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-20 09:38:34.000000 django-typomatic-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-20 09:38:49.233048 django-typomatic-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-20 09:38:34.000000 django-typomatic-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:38:49.233048 django-typomatic-2.3.1/django_typomatic/
--rw-r--r--   0 runner    (1001) docker     (123)    17200 2023-05-20 09:38:34.000000 django-typomatic-2.3.1/django_typomatic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:38:49.233048 django-typomatic-2.3.1/django_typomatic/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 09:38:34.000000 django-typomatic-2.3.1/django_typomatic/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:38:49.233048 django-typomatic-2.3.1/django_typomatic/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 09:38:34.000000 django-typomatic-2.3.1/django_typomatic/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-20 09:38:34.000000 django-typomatic-2.3.1/django_typomatic/management/commands/generate_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-20 09:38:34.000000 django-typomatic-2.3.1/django_typomatic/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-20 09:38:34.000000 django-typomatic-2.3.1/django_typomatic/test__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:38:49.233048 django-typomatic-2.3.1/django_typomatic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-20 09:38:49.000000 django-typomatic-2.3.1/django_typomatic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-20 09:38:49.000000 django-typomatic-2.3.1/django_typomatic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:38:49.000000 django-typomatic-2.3.1/django_typomatic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:38:49.000000 django-typomatic-2.3.1/django_typomatic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 09:38:49.000000 django-typomatic-2.3.1/django_typomatic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-20 09:38:49.000000 django-typomatic-2.3.1/django_typomatic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 09:38:49.233048 django-typomatic-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-20 09:38:34.000000 django-typomatic-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:40.922547 django-typomatic-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 12:50:23.000000 django-typomatic-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-24 12:50:40.922547 django-typomatic-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-24 12:50:23.000000 django-typomatic-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:40.922547 django-typomatic-2.3.2/django_typomatic/
+-rw-r--r--   0 runner    (1001) docker     (123)    17235 2023-05-24 12:50:23.000000 django-typomatic-2.3.2/django_typomatic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:40.922547 django-typomatic-2.3.2/django_typomatic/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:23.000000 django-typomatic-2.3.2/django_typomatic/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:40.922547 django-typomatic-2.3.2/django_typomatic/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:23.000000 django-typomatic-2.3.2/django_typomatic/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-24 12:50:23.000000 django-typomatic-2.3.2/django_typomatic/management/commands/generate_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-24 12:50:23.000000 django-typomatic-2.3.2/django_typomatic/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-24 12:50:23.000000 django-typomatic-2.3.2/django_typomatic/test__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:40.922547 django-typomatic-2.3.2/django_typomatic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-24 12:50:40.000000 django-typomatic-2.3.2/django_typomatic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-24 12:50:40.000000 django-typomatic-2.3.2/django_typomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:50:40.000000 django-typomatic-2.3.2/django_typomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:50:40.000000 django-typomatic-2.3.2/django_typomatic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 12:50:40.000000 django-typomatic-2.3.2/django_typomatic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 12:50:40.000000 django-typomatic-2.3.2/django_typomatic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:50:40.922547 django-typomatic-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-24 12:50:23.000000 django-typomatic-2.3.2/setup.py
```

### Comparing `django-typomatic-2.3.1/LICENSE` & `django-typomatic-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.3.1/PKG-INFO` & `django-typomatic-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-typomatic
-Version: 2.3.1
+Version: 2.3.2
 Summary: A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.
 Home-page: https://github.com/adenh93/django-typomatic
 Author: Aden Herold
 Author-email: aden.herold1@gmail.com
 Keywords: Django,Django Rest Framework,DRF,Typescript,Python
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `django-typomatic-2.3.1/README.md` & `django-typomatic-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.3.1/django_typomatic/__init__.py` & `django-typomatic-2.3.2/django_typomatic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,16 @@
     '''
     if not choices:
         _LOG.warning(f'No choices specified for Serializer Field: {field_type}')
         return 'any'
 
     choices_enum = f"export enum {enum_name} {{\n"
     for key, value in choices.items():
-        value = value.replace("'", "\\'")
+        if type(value) == str:
+            value = value.replace("'", "\\'")
         if type(key) == str:
             choices_enum = choices_enum + f"    {str(key).replace(' ', '_')} = '{value}',\n"
         else:
             "Number enums not need it"
             return None
     choices_enum = choices_enum + "}\n"
```

### Comparing `django-typomatic-2.3.1/django_typomatic/management/commands/generate_ts.py` & `django-typomatic-2.3.2/django_typomatic/management/commands/generate_ts.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     def handle(self, *args, serializers, output, all, **options):
         if all and serializers:
             raise CommandError('Only --all or --serializers must be specified, not together')
 
         if all:
             for app in apps.get_app_configs():
                 # Filter external modules
-                if str(settings.BASE_DIR.parent) not in app.path:
+                if str(settings.BASE_DIR.parent) not in app.path or '.venv' in app.path:
                     continue
 
                 serializers += self._get_app_serializers(app.name)
 
         for serializer in serializers:
             user_input = serializer.split('.')
```

### Comparing `django-typomatic-2.3.1/django_typomatic/mappings.py` & `django-typomatic-2.3.2/django_typomatic/mappings.py`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.3.1/django_typomatic/test__init__.py` & `django-typomatic-2.3.2/django_typomatic/test__init__.py`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.3.1/django_typomatic.egg-info/PKG-INFO` & `django-typomatic-2.3.2/django_typomatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-typomatic
-Version: 2.3.1
+Version: 2.3.2
 Summary: A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.
 Home-page: https://github.com/adenh93/django-typomatic
 Author: Aden Herold
 Author-email: aden.herold1@gmail.com
 Keywords: Django,Django Rest Framework,DRF,Typescript,Python
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `django-typomatic-2.3.1/setup.py` & `django-typomatic-2.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md') as file:
     long_description = file.read()
 
 setuptools.setup(
     name="django-typomatic",
-    version="2.3.1",
+    version="2.3.2",
     url="https://github.com/adenh93/django-typomatic",
 
     author="Aden Herold",
     author_email="aden.herold1@gmail.com",
 
     description="A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.",
     long_description=long_description,
```

