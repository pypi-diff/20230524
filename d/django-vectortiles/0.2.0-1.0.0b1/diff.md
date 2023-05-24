# Comparing `tmp/django-vectortiles-0.2.0.tar.gz` & `tmp/django-vectortiles-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-vectortiles-0.2.0.tar", last modified: Mon Oct 17 10:04:24 2022, max compression
+gzip compressed data, was "dist/django-vectortiles-1.0.0b1.tar", last modified: Wed May 24 07:35:52 2023, max compression
```

## Comparing `django-vectortiles-0.2.0.tar` & `django-vectortiles-1.0.0b1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 10:04:24.000000 django-vectortiles-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     4255 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-17 10:04:24.000000 django-vectortiles-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6533 2022-10-17 10:04:24.000000 django-vectortiles-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 10:04:24.000000 django-vectortiles-0.2.0/django_vectortiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-10-17 10:04:23.000000 django-vectortiles-0.2.0/django_vectortiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-17 10:04:23.000000 django-vectortiles-0.2.0/django_vectortiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6533 2022-10-17 10:04:23.000000 django-vectortiles-0.2.0/django_vectortiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-10-17 10:04:23.000000 django-vectortiles-0.2.0/django_vectortiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 10:04:23.000000 django-vectortiles-0.2.0/django_vectortiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/CHANGES.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 10:04:24.000000 django-vectortiles-0.2.0/vectortiles/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/vectortiles/VERSION.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 10:04:24.000000 django-vectortiles-0.2.0/vectortiles/mapbox/
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/vectortiles/mapbox/views.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/vectortiles/mapbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/vectortiles/mapbox/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 10:04:24.000000 django-vectortiles-0.2.0/vectortiles/postgis/
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/vectortiles/postgis/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/vectortiles/postgis/views.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/vectortiles/postgis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2193 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/vectortiles/postgis/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/vectortiles/views.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/vectortiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5927 2022-10-17 10:04:10.000000 django-vectortiles-0.2.0/vectortiles/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/vectortiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      976 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/vectortiles/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/rest_framework/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5070 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/vectortiles/backends/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/vectortiles/backends/python/
+-rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/backends/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/vectortiles/backends/postgis/
+-rw-r--r--   0 runner    (1001) docker     (122)      891 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/backends/postgis/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/backends/postgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/VERSION.md
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/vectortiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4581 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/django_vectortiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-05-24 07:35:42.000000 django-vectortiles-1.0.0b1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4581 2023-05-24 07:35:52.000000 django-vectortiles-1.0.0b1/PKG-INFO
```

### Comparing `django-vectortiles-0.2.0/README.md` & `django-vectortiles-1.0.0b1/django_vectortiles.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: django-vectortiles
+Version: 1.0.0b1
+Summary: Django vector tile generation
+Home-page: https://github.com/submarcos/django-vectortiles.git
+Author: Jean-Etienne Castagnede
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: python
+Provides-Extra: mapbox
+
 ![Tests](https://github.com/submarcos/django-vectortiles/workflows/Python%20/%20Django%20matrix%20test/badge.svg)
 [![Coverage](https://codecov.io/gh/submarcos/django-vectortiles/branch/master/graph/badge.svg)](https://codecov.io/gh/submarcos/django-vectortiles)
 
 ![Python Version](https://img.shields.io/badge/python-%3E%3D%203.6-blue.svg)
 ![Django Version](https://img.shields.io/badge/django-%3E%3D%202.2-blue.svg)
 
 # Generate MapBox VectorTiles from GeoDjango models
@@ -13,151 +43,139 @@
 ### Installation
 
 #### Basic
 ```bash
 pip install django-vectortiles
 ```
 
-* Without any other option, use only vectortiles.postgis
+* By default, postgis backend is enabled.
 * Ensure you have psycopg2 set and installed
 
-#### If you don't want to use Postgis
+#### If you don't want to use Postgis and / or PostgreSQL
 ```bash
-pip install django-vectortiles[mapbox]
+pip install django-vectortiles[python]
 ```
 * This will incude mapbox_vector_tiles package and its dependencies
-* Use only vectortiles.mapbox
+* Set VECTOR_TILES_BACKEND to "vectortiles.backends.python"
 
 ### Examples
 
-* assuming you have django.contrib.gis in your INSTALLED_APPS and a gis compatible database backend
+* assuming you have ```django.contrib.gis``` in your ```INSTALLED_APPS``` and a gis compatible database backend
 
 ```python
 # in your app models.py
 
 from django.contrib.gis.db import models
 
 
-class Layer(models.Model):
-    name = models.CharField(max_length=250)
-
-
 class Feature(models.Model):
     geom = models.GeometryField(srid=4326)
     name = models.CharField(max_length=250)
-    layer = models.ForeignKey(Layer, on_delete=models.CASCADE, related_name='features')
 ```
 
 
-#### Simple model:
+#### Simple Example:
 
 ```python
-# in your view file
-
-from django.views.generic import ListView
-from vectortiles.postgis.views import MVTView
 from yourapp.models import Feature
 
+# in a vector_layers.py file
+from vectortiles import VectorLayer
+
 
-class FeatureTileView(MVTView, ListView):
+class FeatureVectorLayer(VectorLayer):
     model = Feature
     vector_tile_layer_name = "features"
-    vector_tile_fields = ('other_field_to_include', )
+    vector_tile_fields = ("name",)
+
+# in your view file
+
+from yourapp.vector_layers import FeatureVectorLayer
+
+from vectortiles.views import MVTView
+
+
+class FeatureTileView(MVTView):
+    layers = [FeatureVectorLayer()]
 
 
 # in your urls file
 from django.urls import path
 from yourapp import views
 
-
 urlpatterns = [
     ...
     path('tiles/<int:z>/<int:x>/<int:y>', views.FeatureTileView.as_view(), name="feature-tile"),
     ...
 ]
 ```
 
-#### Related model:
+#### Use TileJSON and multiple domains:
 
 ```python
 # in your view file
 
-from django.views.generic import DetailView
-from vectortiles.mixins import BaseVectorTileView
-from vectortiles.postgis.views import MVTView
-from yourapp.models import Layer
+from django.urls import reverse
 
+from vectortiles.views import TileJSONView
 
-class LayerTileView(MVTView, DetailView):
-    model = Layer
-    vector_tile_fields = ('other_field_to_include', )
 
-    def get_vector_tile_layer_name(self):
-        return self.get_object().name
+class FeatureTileJSONView(TileJSONView):
+    """Simple model TileJSON View"""
 
-    def get_vector_tile_queryset(self):
-        return self.get_object().features.all()
+    name = "My features dataset"
+    attribution = "@JEC Data"
+    description = "My dataset"
 
-    def get(self, request, *args, **kwargs):
-        self.object = self.get_object()
-        return BaseVectorTileView.get(self,request=request, z=kwargs.get('z'), x=kwargs.get('x'), y=kwargs.get('y'))
+    def get_tile_url(self):
+        """ Base MVTView Url used to generates urls in TileJSON in a.tiles.xxxx/{z}/{x}/{y} format """
+        return str(reverse("feature-tile", args=(0, 0, 0))).replace("0/0/0", "{z}/{x}/{y}")
 
 
 # in your urls file
 from django.urls import path
 from yourapp import views
 
-
 urlpatterns = [
     ...
-    path('layer/<int:pk>/tile/<int:z>/<int:x>/<int:y>', views.LayerTileView.as_view(), name="layer-tile"),
+    path('tiles/<int:z>/<int:x>/<int:y>', views.FeatureTileView.as_view(), name="feature-tile"),
+    path("feature/tiles.json", views.FeatureTileJSONView.as_view(), name="feature-tilejson"),
     ...
 ]
-```
-
-#### Usage without PostgreSQL / PostGIS
 
-Just import and use vectortiles.mapbox.view.MVTView instead of vectortiles.postgis.view.MVTView
-
-#### Usage with DRF
-
-django-vectortiles can be used with DRF if `renderer_classes` of the view is overridden (see [DRF docs](https://www.django-rest-framework.org/api-guide/renderers/#custom-renderers)). Simply use the right BaseMixin and action on viewsets, or directly a GET method in an APIView, i.e.:
-
-```python
-from rest_framework import renderers, views
-from vectortiles.postgis.views import MVTView
-
-
-class MVTRenderer(renderers.BaseRenderer):
-    media_type = "application/vnd.mapbox-vector-tile"
-    format = "pbf"
-
-    def render(self, data, accepted_media_type=None, renderer_context=None):
-        return data
-
-
-class TileServerView(MVTView, views.APIView):
-    renderer_classes = [MVTRenderer]
+# in your settings file
+ALLOWED_HOSTS = [
+    "a.tiles.xxxx",
+    "b.tiles.xxxx",
+    "c.tiles.xxxx",
+    ...
+]
 
-    def get(...): ...
-```
+VECTOR_TILES_URLS = [
+    "https://a.tiles.xxxx",
+    "https://b.tiles.xxxx",
+    "https://c.tiles.xxxx",
+    ...
+]
 
 #### Development
 
 ##### With docker and docker-compose
 
 ```bash
-docker pull makinacorpus/geodjango:bionic-3.6
-docker-compose build
+docker compose build
 # docker-compose up
-docker-compose run /code/venv/bin/python ./manage.py test
+docker compose run /code/venv/bin/python ./manage.py test
 ```
 
 ##### Local
 
 * Install python and django requirements (python 3.6+, django 2.2+)
 * Install geodjango requirements
 * Have a postgresql / postgis 2.4+ enabled database
 * Use a virtualenv
+
 ```bash
 pip install .[dev] -U
 ```
+
+
```

### Comparing `django-vectortiles-0.2.0/setup.py` & `django-vectortiles-1.0.0b1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 #!/usr/bin/env python
 
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 README = open(os.path.join(HERE, 'README.md')).read()
-CHANGES = open(os.path.join(HERE, 'CHANGES.md')).read()
 
 test_require = [
     'factory-boy',
     'flake8',
+    'isort',
+    'black',
     'coverage',
+    'djangorestframework',
     'psycopg2-binary'  # for dev and test only. in production, use psycopg2
 ]
 
-mapbox = [
+python = [
     'mapbox_vector_tile',
     'protobuf<4.21.0',  # https://github.com/tilezen/mapbox-vector-tile/issues/113
 ]
 
 setup(
     name='django-vectortiles',
     version=open(os.path.join(HERE, 'vectortiles', 'VERSION.md')).read().strip(),
     include_package_data=True,
     author="Jean-Etienne Castagnede",
     description='Django vector tile generation',
-    long_description=README + '\n\n' + CHANGES,
+    long_description=README,
     description_content_type="text/markdown",
     long_description_content_type="text/markdown",
     packages=find_packages(),
     url='https://github.com/submarcos/django-vectortiles.git',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
+        'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10'
     ],
@@ -51,13 +55,14 @@
     install_requires=[
         'django',
         'mercantile'
     ],
     tests_require=test_require,
     extras_require={
         'test': test_require,
-        'dev': test_require + mapbox + [
+        'dev': test_require + python + [
             'django-debug-toolbar', 'sphinx-rtd-theme'
         ],
-        'mapbox': mapbox,
+        'python': python,
+        'mapbox': python
     }
 )
```

### Comparing `django-vectortiles-0.2.0/vectortiles/mapbox/mixins.py` & `django-vectortiles-1.0.0b1/vectortiles/backends/python/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 import math
 
 import mapbox_vector_tile
 from django.contrib.gis.db.models.functions import Intersection, Transform
 from django.contrib.gis.geos import Polygon
 from django.db.models import F
 
-from vectortiles.mixins import BaseVectorTileMixin
+from vectortiles.backends import BaseVectorLayerMixin
 
 
-class MapboxBaseVectorTile(BaseVectorTileMixin):
-    vector_tile_generation = "mapbox"
-
+class VectorLayer(BaseVectorLayerMixin):
     def pixel_length(self, zoom, size):
         radius = 6378137
         circum = 2 * math.pi * radius
         return circum / size / 2 ** int(zoom)
 
     def get_tile(self, x, y, z):
+        if not self.check_in_zoom_levels(z):
+            return b""
+
+        features = self.get_vector_tile_queryset(z, x, y)
+
         # get tile coordinates from x, y and z
         west, south, east, north = self.get_bounds(x, y, z)
-        features = self.get_vector_tile_queryset()
-
         bbox = Polygon.from_bbox((west, south, east, north))
         bbox.srid = 3857
 
-        filters = {
-            f"{self.vector_tile_geom_name}__intersects": bbox
-        }
+        filters = {f"{self.geom_field}__intersects": bbox}
         features = features.filter(**filters)
         # limit feature number if limit provided
-        limit = self.get_vector_tile_queryset_limit()
+        limit = self.get_queryset_limit()
         if limit:
             features = features[:limit]
-        features = features.annotate(clipped=Intersection(Transform(self.vector_tile_geom_name, 3857),
-                                                          bbox.buffer(self.pixel_length(z, self.vector_tile_buffer))) if self.vector_tile_clip_geom else F('geom'))
+        features = features.annotate(
+            clipped=Intersection(
+                Transform(self.geom_field, 3857),
+                bbox.buffer(self.pixel_length(z, self.tile_buffer)),
+            )
+            if self.clip_geom
+            else F("geom")
+        )
         if features:
             tile = {
-                "name": self.get_vector_tile_layer_name(),
+                "name": self.get_id(),
                 "features": [
                     {
                         "geometry": feature.clipped.wkb.tobytes(),
                         "properties": {
-                            key: getattr(feature, key) for key in self.vector_tile_fields if
-                            self.vector_tile_fields
-                        }
+                            key: getattr(feature, key)
+                            for key in self.tile_fields
+                            if self.tile_fields
+                        },
                     }
                     for feature in features
                 ],
             }
-            return mapbox_vector_tile.encode(tile,
-                                             quantize_bounds=(west, south, east, north),
-                                             extents=self.vector_tile_extent)
+            return mapbox_vector_tile.encode(
+                tile,
+                quantize_bounds=(west, south, east, north),
+                extents=self.tile_extent,
+            )
```

### Comparing `django-vectortiles-0.2.0/vectortiles/postgis/functions.py` & `django-vectortiles-1.0.0b1/vectortiles/backends/postgis/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,17 @@
         return sql, params
 
 
 class MakeEnvelope(Func):
     function = "ST_MAKEENVELOPE"
 
     def __init__(self, *expressions, output_field=None, **extra):
-        super().__init__(*expressions, output_field=None, **extra)
-        self.output_field = GeometryField(srid=expressions[4])
+        super().__init__(
+            *expressions, output_field=GeometryField(srid=expressions[4]), **extra
+        )
 
 
 class AsMVTGeom(GeoFunc):
     function = "ST_ASMVTGEOM"
 
     @cached_property
     def output_field(self):
```

