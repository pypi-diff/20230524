# Comparing `tmp/utils-flask-sqlalchemy-geo-0.2.7.tar.gz` & `tmp/utils-flask-sqlalchemy-geo-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils-flask-sqlalchemy-geo-0.2.7.tar", last modified: Fri Mar  3 17:34:40 2023, max compression
+gzip compressed data, was "utils-flask-sqlalchemy-geo-0.2.8.tar", last modified: Wed May 24 12:51:09 2023, max compression
```

## Comparing `utils-flask-sqlalchemy-geo-0.2.7.tar` & `utils-flask-sqlalchemy-geo-0.2.8.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:34:40.745751 utils-flask-sqlalchemy-geo-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-03-03 17:34:40.745751 utils-flask-sqlalchemy-geo-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 17:34:40.745751 utils-flask-sqlalchemy-geo-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:34:40.741751 utils-flask-sqlalchemy-geo-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:34:40.745751 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18083 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/utilsgeometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:34:40.745751 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqlalchemy_geo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-03-03 17:34:40.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqlalchemy_geo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-03 17:34:40.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqlalchemy_geo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 17:34:40.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqlalchemy_geo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-03 17:34:40.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqlalchemy_geo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-03 17:34:40.000000 utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqlalchemy_geo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-03 17:34:30.000000 utils-flask-sqlalchemy-geo-0.2.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:51:09.775930 utils-flask-sqlalchemy-geo-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-24 12:51:09.775930 utils-flask-sqlalchemy-geo-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:51:09.775930 utils-flask-sqlalchemy-geo-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:51:09.767930 utils-flask-sqlalchemy-geo-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:51:09.771930 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18083 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/utilsgeometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:51:09.775930 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqlalchemy_geo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-24 12:51:09.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqlalchemy_geo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 12:51:09.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqlalchemy_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:51:09.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqlalchemy_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 12:51:09.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqlalchemy_geo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-24 12:51:09.000000 utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqlalchemy_geo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-24 12:50:52.000000 utils-flask-sqlalchemy-geo-0.2.8/tox.ini
```

### Comparing `utils-flask-sqlalchemy-geo-0.2.7/LICENSE` & `utils-flask-sqlalchemy-geo-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.2.7/PKG-INFO` & `utils-flask-sqlalchemy-geo-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-flask-sqlalchemy-geo
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python lib of tools for Flask and SQLAlchemy (extension geometry)
 Home-page: https://github.com/PnX-SI/Utils-Flask-SQLAlchemy-Geo
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `utils-flask-sqlalchemy-geo-0.2.7/README.md` & `utils-flask-sqlalchemy-geo-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.2.7/setup.py` & `utils-flask-sqlalchemy-geo-0.2.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     url="https://github.com/PnX-SI/Utils-Flask-SQLAlchemy-Geo",
     packages=setuptools.find_packages("src"),
     package_dir={"": "src"},
     install_requires=requirements,
     extras_require={
         "tests": [
             "pytest",
+            "flask-sqlalchemy",
         ],
     },
     setup_requires=["wheel"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Natural Language :: English",
```

### Comparing `utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/generic.py` & `utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/generic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from itertools import chain
+from typing import Union
 from warnings import warn
 
-from geojson import Feature, FeatureCollection
 from geoalchemy2.shape import to_shape
+from geojson import Feature, FeatureCollection
 from utils_flask_sqla.generic import GenericQuery, GenericTable
-from .utilsgeometry import create_shapes_generic, export_geodata_as_file
+from utils_flask_sqla.schema import SmartRelationshipsMixin
+
+from utils_flask_sqla_geo.schema import GeoAlchemyAutoSchema
+from utils_flask_sqla_geo.utilsgeometry import create_shapes_generic, export_geodata_as_file
 
 
 def get_geojson_feature(wkb):
     """retourne une feature geojson à partir d'un WKB"""
     geometry = to_shape(wkb)
     feature = Feature(geometry=geometry, properties={})
     return feature
@@ -150,7 +154,63 @@
         return {
             "total": nb_result_without_filter,
             "total_filtered": nb_results,
             "page": self.offset,
             "limit": self.limit,
             "items": results,
         }
+
+    def get_model(self, pk_name: Union[str, None] = None):
+        """
+        renvoie le modèle associé à la table
+        """
+
+        if pk_name is None:
+            # recherche de pk_name dans les colonnes
+            pk_names = [col.key for col in self.view.tableDef.columns if col.primary_key]
+            if pk_names:
+                pk_name = pk_names[0]
+            else:
+                # sinon on prend la premiere colonne ????
+                # dans l'ideal il aurait fallu fournir la pk_name dans ce cas là
+                pk_name = self.view.tableDef.columns.keys()[0]
+
+        # test si pk_name existe bien
+        if not hasattr(self.view.tableDef.c, pk_name):
+            raise Exception(f"{pk_name} cannot be found in table")
+
+        dict_model = {
+            "__table__": self.view.tableDef,
+            "__mapper_args__": {"primary_key": getattr(self.view.tableDef.c, pk_name)},
+        }
+
+        Model = type("Model", (self.DB.Model,), dict_model)
+
+        return Model
+
+    def get_marshmallow_schema(self, pk_name: Union[str, None] = None):
+        """
+        renvoie un marshmalow schema à partir d'un modèle
+        ce schema hérite des classes GeoAlchemyAutoSchema et SmartRelationshipsMixin
+
+        TODO (à déplacer dans les lib utils sqla)
+        """
+        Meta = type(
+            "Meta",
+            (),
+            {
+                "model": self.get_model(pk_name),
+                "load_instance": True,
+            },
+        )
+        dict_schema = {
+            "Meta": Meta,
+        }
+
+        return type(
+            "Schema",
+            (
+                SmartRelationshipsMixin,
+                GeoAlchemyAutoSchema,
+            ),
+            dict_schema,
+        )
```

### Comparing `utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/schema.py` & `utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,18 @@
     MultiPointSchema,
     PolygonSchema,
     MultiPolygonSchema,
     LineStringSchema,
     MultiLineStringSchema,
 )
 from shapely.geometry import shape
+from shapely import wkt
+from shapely.errors import WKTReadingError
+
+from .utils import JsonifiableGenerator, GeneratorField
 
 
 class GeometrySchema(Schema):
     schema_map = {
         GeometryType.point.value: PointSchema,
         GeometryType.multi_point.value: MultiPointSchema,
         GeometryType.polygon.value: PolygonSchema,
@@ -45,34 +49,52 @@
     # note: geometry validity done by GeometryField deserialization
     geometry = fields.Mapping(required=True, allow_none=True)
     properties = fields.Mapping(required=True)
 
 
 class FeatureCollectionSchema(Schema):
     type = fields.Constant("FeatureCollection", required=True)
-    features = fields.List(fields.Nested(FeatureSchema), required=True)
+    features = GeneratorField(fields.Nested(FeatureSchema), required=True)
 
 
 class GeometryField(fields.Field):
     geometry_schema = GeometrySchema()
 
-    def _serialize(self, value, attr, obj):
+    def _serialize_wkt(self, value, attr, obj):
+        return to_shape(value).wkt if value else None
+
+    def _serialize_geojson(self, value, attr, obj):
         return to_shape(value).__geo_interface__ if value else None
 
-    def _deserialize(self, value, attr, data, **kwargs):
+    def _deserialize_wkt(self, value, attr, data, **kwargs):
+        try:
+            return wkt.loads(value)
+        except WKTReadingError as error:
+            raise ValidationError("Invalid geometry.") from error
+
+    def _deserialize_geojson(self, value, attr, data, **kwargs):
         try:
             geom = shape(self.geometry_schema.load(value))
             if not geom.is_valid:
                 raise ValidationError("Invalid geometry.")
             if geom.has_z:
                 raise ValidationError("Unexpected third dimension.")
             return from_shape(geom, srid=4326)
         except ValueError as error:
             raise ValidationError("Invalid geometry.") from error
 
+    def _bind_to_schema(self, field_name, schema):
+        super()._bind_to_schema
+        if schema.as_geojson:
+            self._serialize = self._serialize_geojson
+            self._deserialize = self._deserialize_geojson
+        else:
+            self._serialize = self._serialize_wkt
+            self._deserialize = self._deserialize_wkt
+
 
 class GeoModelConverter(ModelConverter):
     """Model converter for models with geometric fields."""
 
     SQLA_TYPE_MAPPING = {
         **ModelConverter.SQLA_TYPE_MAPPING,
         Geometry: GeometryField,
@@ -166,24 +188,40 @@
         return feature
 
     def from_feature(self, feature):
         properties = feature["properties"]
         properties[self.opts.feature_geometry] = feature["geometry"]
         return properties
 
+    def _serialize(self, obj, *, many=None):
+        if many:
+            result = map(
+                lambda o: super(GeoAlchemyAutoSchema, self)._serialize(o, many=False), obj
+            )
+            if isinstance(obj, list):
+                return list(result)
+            else:
+                return result
+        else:
+            result = super(GeoAlchemyAutoSchema, self)._serialize(obj, many=False)
+            return result
+
     @post_dump(pass_many=True)
     def to_geojson(self, data, many, **kwargs):
         if self.as_geojson:
             if many:
-                return FeatureCollectionSchema().dump(
-                    {"features": [self.to_feature(props) for props in data]}
-                )
+                features = map(self.to_feature, data)
+                if isinstance(data, list):
+                    features = list(features)
+                return FeatureCollectionSchema().dump({"features": features})
             else:
                 return FeatureSchema().dump(self.to_feature(data))
         else:
+            if many and not isinstance(data, list):
+                data = JsonifiableGenerator(data)
             return data
 
     @pre_load(pass_many=True)
     def from_geojson(self, data, many, **kwargs):
         if not self.as_geojson:
             return data
         if many:
```

### Comparing `utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/serializers.py` & `utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/serializers.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqla_geo/utilsgeometry.py` & `utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqla_geo/utilsgeometry.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqlalchemy_geo.egg-info/PKG-INFO` & `utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqlalchemy_geo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-flask-sqlalchemy-geo
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python lib of tools for Flask and SQLAlchemy (extension geometry)
 Home-page: https://github.com/PnX-SI/Utils-Flask-SQLAlchemy-Geo
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `utils-flask-sqlalchemy-geo-0.2.7/src/utils_flask_sqlalchemy_geo.egg-info/SOURCES.txt` & `utils-flask-sqlalchemy-geo-0.2.8/src/utils_flask_sqlalchemy_geo.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 VERSION
 pyproject.toml
 requirements.in
 setup.py
 tox.ini
 src/utils_flask_sqla_geo/__init__.py
+src/utils_flask_sqla_geo/export.py
 src/utils_flask_sqla_geo/generic.py
 src/utils_flask_sqla_geo/mixins.py
 src/utils_flask_sqla_geo/schema.py
 src/utils_flask_sqla_geo/serializers.py
 src/utils_flask_sqla_geo/utils.py
 src/utils_flask_sqla_geo/utilsgeometry.py
 src/utils_flask_sqlalchemy_geo.egg-info/PKG-INFO
```

