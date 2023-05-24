# Comparing `tmp/django-vectortiles-1.0.0b1.tar.gz` & `tmp/django-vectortiles-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-vectortiles-1.0.0b1.tar", last modified: Wed May 24 07:35:52 2023, max compression
+gzip compressed data, was "dist/django-vectortiles-1.0.0b2.tar", last modified: Wed May 24 08:38:55 2023, max compression
```

## Comparing `django-vectortiles-1.0.0b1.tar` & `django-vectortiles-1.0.0b2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/vectortiles/
--rw-r--r--   0 runner    (1001) docker     (122)      976 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/vectortiles/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/rest_framework/views.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5070 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/vectortiles/backends/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/vectortiles/backends/python/
--rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/backends/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/vectortiles/backends/postgis/
--rw-r--r--   0 runner    (1001) docker     (122)      891 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/backends/postgis/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/backends/postgis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/VERSION.md
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      348 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4581 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     4581 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/vectortiles/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/VERSION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/vectortiles/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/vectortiles/backends/postgis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/backends/postgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/backends/postgis/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/vectortiles/backends/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/backends/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/vectortiles/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/rest_framework/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/views.py
```

### Comparing `django-vectortiles-1.0.0b1/vectortiles/views.py` & `django-vectortiles-1.0.0b2/vectortiles/views.py`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b1/vectortiles/mixins.py` & `django-vectortiles-1.0.0b2/vectortiles/mixins.py`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b1/vectortiles/backends/python/__init__.py` & `django-vectortiles-1.0.0b2/vectortiles/backends/python/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b1/vectortiles/backends/postgis/functions.py` & `django-vectortiles-1.0.0b2/vectortiles/backends/postgis/functions.py`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b1/vectortiles/backends/postgis/__init__.py` & `django-vectortiles-1.0.0b2/vectortiles/backends/postgis/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b1/vectortiles/backends/__init__.py` & `django-vectortiles-1.0.0b2/vectortiles/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b1/README.md` & `django-vectortiles-1.0.0b2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![Tests](https://github.com/submarcos/django-vectortiles/workflows/Python%20/%20Django%20matrix%20test/badge.svg)
 [![Coverage](https://codecov.io/gh/submarcos/django-vectortiles/branch/master/graph/badge.svg)](https://codecov.io/gh/submarcos/django-vectortiles)
 
-![Python Version](https://img.shields.io/badge/python-%3E%3D%203.6-blue.svg)
-![Django Version](https://img.shields.io/badge/django-%3E%3D%202.2-blue.svg)
+![Python Version](https://img.shields.io/badge/python-%3E%3D%203.7-blue.svg)
+![Django Version](https://img.shields.io/badge/django-%3E%3D%203.2-blue.svg)
 
 # Generate MapBox VectorTiles from GeoDjango models
 
 ## Directly with PostgreSQL/PostGIS 2.4+ or python native mapbox_vector_tile
 
 ## [Read full documentation](https://django-vectortiles.readthedocs.io/)
 
@@ -106,39 +106,48 @@
 from yourapp import views
 
 urlpatterns = [
     ...
     path('tiles/<int:z>/<int:x>/<int:y>', views.FeatureTileView.as_view(), name="feature-tile"),
     path("feature/tiles.json", views.FeatureTileJSONView.as_view(), name="feature-tilejson"),
     ...
-]
 
-# in your settings file
-ALLOWED_HOSTS = [
+    # in your settings file
+    ALLOWED_HOSTS = [
     "a.tiles.xxxx",
     "b.tiles.xxxx",
     "c.tiles.xxxx",
     ...
 ]
 
 VECTOR_TILES_URLS = [
     "https://a.tiles.xxxx",
     "https://b.tiles.xxxx",
     "https://c.tiles.xxxx",
     ...
 ]
 
+```
+
+#### Usage without PostgreSQL / PostGIS
+
+Just import and use vectortiles.mapbox.view.MVTView instead of vectortiles.postgis.view.MVTView
+
+#### Usage with Django Rest Framework
+
+django-vectortiles can be used with DRF if `renderer_classes` of the view is overridden (see [DRF docs](https://www.django-rest-framework.org/api-guide/renderers/#custom-renderers)). Simply use the right BaseMixin and action on viewsets, or directly a GET method in an APIView. See [documentation](https://django-vectortiles.readthedocs.io/en/latest/usage.html#django-rest-framework) for more details.
+
 #### Development
 
 ##### With docker and docker-compose
 
 ```bash
-docker compose build
+docker-compose build
 # docker-compose up
-docker compose run /code/venv/bin/python ./manage.py test
+docker-compose run /code/venv/bin/python ./manage.py test
 ```
 
 ##### Local
 
 * Install python and django requirements (python 3.6+, django 2.2+)
 * Install geodjango requirements
 * Have a postgresql / postgis 2.4+ enabled database
```

### Comparing `django-vectortiles-1.0.0b1/django_vectortiles.egg-info/PKG-INFO` & `django-vectortiles-1.0.0b2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: django-vectortiles
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Django vector tile generation
 Home-page: https://github.com/submarcos/django-vectortiles.git
 Author: Jean-Etienne Castagnede
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: python
 Provides-Extra: mapbox
+License-File: LICENSE
 
 ![Tests](https://github.com/submarcos/django-vectortiles/workflows/Python%20/%20Django%20matrix%20test/badge.svg)
 [![Coverage](https://codecov.io/gh/submarcos/django-vectortiles/branch/master/graph/badge.svg)](https://codecov.io/gh/submarcos/django-vectortiles)
 
-![Python Version](https://img.shields.io/badge/python-%3E%3D%203.6-blue.svg)
-![Django Version](https://img.shields.io/badge/django-%3E%3D%202.2-blue.svg)
+![Python Version](https://img.shields.io/badge/python-%3E%3D%203.7-blue.svg)
+![Django Version](https://img.shields.io/badge/django-%3E%3D%203.2-blue.svg)
 
 # Generate MapBox VectorTiles from GeoDjango models
 
 ## Directly with PostgreSQL/PostGIS 2.4+ or python native mapbox_vector_tile
 
 ## [Read full documentation](https://django-vectortiles.readthedocs.io/)
 
@@ -136,46 +135,53 @@
 from yourapp import views
 
 urlpatterns = [
     ...
     path('tiles/<int:z>/<int:x>/<int:y>', views.FeatureTileView.as_view(), name="feature-tile"),
     path("feature/tiles.json", views.FeatureTileJSONView.as_view(), name="feature-tilejson"),
     ...
-]
 
-# in your settings file
-ALLOWED_HOSTS = [
+    # in your settings file
+    ALLOWED_HOSTS = [
     "a.tiles.xxxx",
     "b.tiles.xxxx",
     "c.tiles.xxxx",
     ...
 ]
 
 VECTOR_TILES_URLS = [
     "https://a.tiles.xxxx",
     "https://b.tiles.xxxx",
     "https://c.tiles.xxxx",
     ...
 ]
 
+```
+
+#### Usage without PostgreSQL / PostGIS
+
+Just import and use vectortiles.mapbox.view.MVTView instead of vectortiles.postgis.view.MVTView
+
+#### Usage with Django Rest Framework
+
+django-vectortiles can be used with DRF if `renderer_classes` of the view is overridden (see [DRF docs](https://www.django-rest-framework.org/api-guide/renderers/#custom-renderers)). Simply use the right BaseMixin and action on viewsets, or directly a GET method in an APIView. See [documentation](https://django-vectortiles.readthedocs.io/en/latest/usage.html#django-rest-framework) for more details.
+
 #### Development
 
 ##### With docker and docker-compose
 
 ```bash
-docker compose build
+docker-compose build
 # docker-compose up
-docker compose run /code/venv/bin/python ./manage.py test
+docker-compose run /code/venv/bin/python ./manage.py test
 ```
 
 ##### Local
 
 * Install python and django requirements (python 3.6+, django 2.2+)
 * Install geodjango requirements
 * Have a postgresql / postgis 2.4+ enabled database
 * Use a virtualenv
 
 ```bash
 pip install .[dev] -U
 ```
-
-
```

### Comparing `django-vectortiles-1.0.0b1/django_vectortiles.egg-info/SOURCES.txt` & `django-vectortiles-1.0.0b2/django_vectortiles.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 django_vectortiles.egg-info/PKG-INFO
 django_vectortiles.egg-info/SOURCES.txt
 django_vectortiles.egg-info/dependency_links.txt
```

### Comparing `django-vectortiles-1.0.0b1/setup.py` & `django-vectortiles-1.0.0b2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,19 +41,19 @@
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
     python_requires='>=3.6',
     install_requires=[
         'django',
         'mercantile'
     ],
     tests_require=test_require,
```

### Comparing `django-vectortiles-1.0.0b1/PKG-INFO` & `django-vectortiles-1.0.0b2/django_vectortiles.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: django-vectortiles
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Django vector tile generation
 Home-page: https://github.com/submarcos/django-vectortiles.git
 Author: Jean-Etienne Castagnede
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: python
 Provides-Extra: mapbox
+License-File: LICENSE
 
 ![Tests](https://github.com/submarcos/django-vectortiles/workflows/Python%20/%20Django%20matrix%20test/badge.svg)
 [![Coverage](https://codecov.io/gh/submarcos/django-vectortiles/branch/master/graph/badge.svg)](https://codecov.io/gh/submarcos/django-vectortiles)
 
-![Python Version](https://img.shields.io/badge/python-%3E%3D%203.6-blue.svg)
-![Django Version](https://img.shields.io/badge/django-%3E%3D%202.2-blue.svg)
+![Python Version](https://img.shields.io/badge/python-%3E%3D%203.7-blue.svg)
+![Django Version](https://img.shields.io/badge/django-%3E%3D%203.2-blue.svg)
 
 # Generate MapBox VectorTiles from GeoDjango models
 
 ## Directly with PostgreSQL/PostGIS 2.4+ or python native mapbox_vector_tile
 
 ## [Read full documentation](https://django-vectortiles.readthedocs.io/)
 
@@ -136,46 +135,53 @@
 from yourapp import views
 
 urlpatterns = [
     ...
     path('tiles/<int:z>/<int:x>/<int:y>', views.FeatureTileView.as_view(), name="feature-tile"),
     path("feature/tiles.json", views.FeatureTileJSONView.as_view(), name="feature-tilejson"),
     ...
-]
 
-# in your settings file
-ALLOWED_HOSTS = [
+    # in your settings file
+    ALLOWED_HOSTS = [
     "a.tiles.xxxx",
     "b.tiles.xxxx",
     "c.tiles.xxxx",
     ...
 ]
 
 VECTOR_TILES_URLS = [
     "https://a.tiles.xxxx",
     "https://b.tiles.xxxx",
     "https://c.tiles.xxxx",
     ...
 ]
 
+```
+
+#### Usage without PostgreSQL / PostGIS
+
+Just import and use vectortiles.mapbox.view.MVTView instead of vectortiles.postgis.view.MVTView
+
+#### Usage with Django Rest Framework
+
+django-vectortiles can be used with DRF if `renderer_classes` of the view is overridden (see [DRF docs](https://www.django-rest-framework.org/api-guide/renderers/#custom-renderers)). Simply use the right BaseMixin and action on viewsets, or directly a GET method in an APIView. See [documentation](https://django-vectortiles.readthedocs.io/en/latest/usage.html#django-rest-framework) for more details.
+
 #### Development
 
 ##### With docker and docker-compose
 
 ```bash
-docker compose build
+docker-compose build
 # docker-compose up
-docker compose run /code/venv/bin/python ./manage.py test
+docker-compose run /code/venv/bin/python ./manage.py test
 ```
 
 ##### Local
 
 * Install python and django requirements (python 3.6+, django 2.2+)
 * Install geodjango requirements
 * Have a postgresql / postgis 2.4+ enabled database
 * Use a virtualenv
 
 ```bash
 pip install .[dev] -U
 ```
-
-
```

