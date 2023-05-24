# Comparing `tmp/graphene-federation-3.1.3.tar.gz` & `tmp/graphene-federation-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-federation-3.1.3.tar", last modified: Tue Mar 28 08:37:56 2023, max compression
+gzip compressed data, was "graphene-federation-3.1.4.tar", last modified: Wed May 24 01:38:51 2023, max compression
```

## Comparing `graphene-federation-3.1.3.tar` & `graphene-federation-3.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:37:56.960943 graphene-federation-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-03-28 08:37:56.960943 graphene-federation-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:37:56.960943 graphene-federation-3.1.3/graphene_federation/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/inaccessible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/override.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/provides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/shareable.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:37:56.960943 graphene-federation-3.1.3/graphene_federation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_annotation_corner_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_annotation_corner_cases_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_custom_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_extend_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_inaccessible.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_key_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_provides.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_provides_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_requires_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_schema_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_schema_annotation_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/tests/test_shareable.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/graphene_federation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:37:56.960943 graphene-federation-3.1.3/graphene_federation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-03-28 08:37:56.000000 graphene-federation-3.1.3/graphene_federation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-28 08:37:56.000000 graphene-federation-3.1.3/graphene_federation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 08:37:56.000000 graphene-federation-3.1.3/graphene_federation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-28 08:37:56.000000 graphene-federation-3.1.3/graphene_federation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-28 08:37:56.000000 graphene-federation-3.1.3/graphene_federation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-28 08:37:56.960943 graphene-federation-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-28 08:37:52.000000 graphene-federation-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:51.947281 graphene-federation-3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-24 01:38:51.947281 graphene-federation-3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:51.943281 graphene-federation-3.1.4/graphene_federation/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/inaccessible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/provides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/shareable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:51.947281 graphene-federation-3.1.4/graphene_federation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_annotation_corner_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_annotation_corner_cases_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_custom_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_extend_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_inaccessible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_key_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_provides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_provides_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_requires_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_schema_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_schema_annotation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/tests/test_shareable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/graphene_federation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:51.943281 graphene-federation-3.1.4/graphene_federation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-24 01:38:51.000000 graphene-federation-3.1.4/graphene_federation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-24 01:38:51.000000 graphene-federation-3.1.4/graphene_federation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 01:38:51.000000 graphene-federation-3.1.4/graphene_federation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-24 01:38:51.000000 graphene-federation-3.1.4/graphene_federation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 01:38:51.000000 graphene-federation-3.1.4/graphene_federation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 01:38:51.947281 graphene-federation-3.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-24 01:38:49.000000 graphene-federation-3.1.4/setup.py
```

### Comparing `graphene-federation-3.1.3/LICENSE.txt` & `graphene-federation-3.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/PKG-INFO` & `graphene-federation-3.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphene-federation
-Version: 3.1.3
+Version: 3.1.4
 Summary: Federation implementation for graphene
 Home-page: https://github.com/graphql-python/graphene-federation
-Download-URL: https://github.com/graphql-python/graphene-federation/archive/3.1.3.tar.gz
+Download-URL: https://github.com/graphql-python/graphene-federation/archive/3.1.4.tar.gz
 Author: Igor Kasianov
 Author-email: super.hang.glider@gmail.com
 License: MIT
 Keywords: graphene,graphql,gql,federation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `graphene-federation-3.1.3/README.md` & `graphene-federation-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/entity.py` & `graphene-federation-3.1.4/graphene_federation/entity.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/extend.py` & `graphene-federation-3.1.4/graphene_federation/extend.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Any, Callable
+from typing import Any, Callable, Dict
 
 from graphene import Schema
 
 from graphene_federation.utils import check_fields_exist_on_type, is_valid_compound_key
 
 
-def get_extended_types(schema: Schema) -> dict[str, Any]:
+def get_extended_types(schema: Schema) -> Dict[str, Any]:
     """
     Find all the extended types from the schema.
     They can be easily distinguished from the other type as
     the `@extend` decorator adds a `_extended` attribute to them.
     """
     extended_types = {}
     for type_name, type_ in schema.graphql_schema.type_map.items():
```

### Comparing `graphene-federation-3.1.3/graphene_federation/external.py` & `graphene-federation-3.1.4/graphene_federation/external.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/inaccessible.py` & `graphene-federation-3.1.4/graphene_federation/inaccessible.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Any, Optional
+from typing import Any, Dict, Optional
 
 from graphene import Schema
 
 from graphene_federation.utils import get_attributed_fields
 
 
-def get_inaccessible_types(schema: Schema) -> dict[str, Any]:
+def get_inaccessible_types(schema: Schema) -> Dict[str, Any]:
     """
     Find all the inaccessible types from the schema.
     They can be easily distinguished from the other type as
     the `@inaccessible` decorator adds a `_inaccessible` attribute to them.
     """
     inaccessible_types = {}
     for type_name, type_ in schema.graphql_schema.type_map.items():
```

### Comparing `graphene-federation-3.1.3/graphene_federation/main.py` & `graphene-federation-3.1.4/graphene_federation/main.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/override.py` & `graphene-federation-3.1.4/graphene_federation/override.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/provides.py` & `graphene-federation-3.1.4/graphene_federation/provides.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/requires.py` & `graphene-federation-3.1.4/graphene_federation/requires.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Union
+from typing import List, Union
 
 from graphene import Schema
 
 from graphene_federation.utils import get_attributed_fields
 
 
-def requires(field, fields: Union[str, list[str]]):
+def requires(field, fields: Union[str, List[str]]):
     """
     Mark the required fields for a given field.
     The input `fields` can be either a string or a list.
     When it is a string we split at spaces to get the list of fields.
     """
     # TODO: We should validate the `fields` input to check it is actually existing fields but we
     # don't have access here to the parent graphene type.
```

### Comparing `graphene-federation-3.1.3/graphene_federation/service.py` & `graphene-federation-3.1.4/graphene_federation/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from typing import List
 
 from graphene.types.interface import InterfaceOptions
 from graphene.types.union import UnionOptions
 from graphql import GraphQLInterfaceType, GraphQLObjectType
 
 from .external import get_external_fields
 from .inaccessible import get_inaccessible_types, get_inaccessible_fields
@@ -27,15 +28,15 @@
     string definition, we need to define an object that has a `.fields` attribute.
     """
 
     def __init__(self, name, field):
         self.fields = {name: field}
 
 
-def convert_fields(schema: Schema, fields: list[str]) -> str:
+def convert_fields(schema: Schema, fields: List[str]) -> str:
     get_field_name = type_attribute_to_field_name(schema)
     return " ".join([get_field_name(field) for field in fields])
 
 
 DECORATORS = {
     "_external": lambda schema, fields: "@external",
     "_requires": lambda schema, fields: f'@requires(fields: "{convert_fields(schema, fields)}")',
```

### Comparing `graphene-federation-3.1.3/graphene_federation/shareable.py` & `graphene-federation-3.1.4/graphene_federation/shareable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Any, Optional
+from typing import Any, Dict, Optional
 
 from graphene import Schema
 from graphene.types.interface import InterfaceOptions
 
 from graphene_federation.utils import get_attributed_fields
 
 
-def get_shareable_types(schema: Schema) -> dict[str, Any]:
+def get_shareable_types(schema: Schema) -> Dict[str, Any]:
     """
     Find all the extended types from the schema.
     They can be easily distinguished from the other type as
     the `@shareable` decorator adds a `_shareable` attribute to them.
     """
     shareable_types = {}
     for type_name, type_ in schema.graphql_schema.type_map.items():
```

### Comparing `graphene-federation-3.1.3/graphene_federation/tag.py` & `graphene-federation-3.1.4/graphene_federation/tag.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_annotation_corner_cases.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_annotation_corner_cases.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_annotation_corner_cases_v1.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_annotation_corner_cases_v1.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_custom_enum.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_custom_enum.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_extend.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_extend.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_extend_v1.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_extend_v1.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_inaccessible.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_inaccessible.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_key.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_key_v1.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_key_v1.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_provides.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_provides.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_provides_v1.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_provides_v1.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_requires.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_requires.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_requires_v1.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_requires_v1.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_scalar.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_scalar.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_schema_annotation.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_schema_annotation.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_schema_annotation_v1.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_schema_annotation_v1.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/tests/test_shareable.py` & `graphene-federation-3.1.4/graphene_federation/tests/test_shareable.py`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/graphene_federation/utils.py` & `graphene-federation-3.1.4/graphene_federation/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable
+from typing import Any, Callable, List, Tuple
 
 import graphene
 from graphene import Schema, ObjectType
 from graphene.types.definitions import GrapheneObjectType
 from graphene.types.enum import EnumOptions
 from graphene.types.scalars import ScalarOptions
 from graphene.types.union import UnionOptions
@@ -39,15 +39,15 @@
     return fields.issubset(set(type_._meta.fields))
 
 
 def is_valid_compound_key(type_name: str, key: str, schema: Schema):
     key_document = parse(f"{{{key}}}")
 
     # List storing tuples of nodes in the key document with its parent types
-    key_nodes: list[tuple[Any, GrapheneObjectType]] = [
+    key_nodes: List[Tuple[Any, GrapheneObjectType]] = [
         (key_document.definitions[0], schema.graphql_schema.type_map[type_name])
     ]
 
     while key_nodes:
         selection_node, parent_object_type = key_nodes[0]
         if isinstance(parent_object_type, GraphQLNonNull):
             parent_type_fields = parent_object_type.of_type.fields
```

### Comparing `graphene-federation-3.1.3/graphene_federation.egg-info/PKG-INFO` & `graphene-federation-3.1.4/graphene_federation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphene-federation
-Version: 3.1.3
+Version: 3.1.4
 Summary: Federation implementation for graphene
 Home-page: https://github.com/graphql-python/graphene-federation
-Download-URL: https://github.com/graphql-python/graphene-federation/archive/3.1.3.tar.gz
+Download-URL: https://github.com/graphql-python/graphene-federation/archive/3.1.4.tar.gz
 Author: Igor Kasianov
 Author-email: super.hang.glider@gmail.com
 License: MIT
 Keywords: graphene,graphql,gql,federation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `graphene-federation-3.1.3/graphene_federation.egg-info/SOURCES.txt` & `graphene-federation-3.1.4/graphene_federation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphene-federation-3.1.3/setup.py` & `graphene-federation-3.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 
 def read(*rnames):
   return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
-version = '3.1.3'
+version = '3.1.4'
 
 tests_require = [
     "pytest==7.1.2",
     "pytest-cov",
 ]
 
 dev_require = [
```

