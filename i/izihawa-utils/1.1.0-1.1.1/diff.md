# Comparing `tmp/izihawa_utils-1.1.0-py3-none-any.whl.zip` & `tmp/izihawa_utils-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 14867 bytes, number of entries: 17
+Zip file size: 14835 bytes, number of entries: 17
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-25 09:23 izihawa_utils/__init__.py
 -rw-r--r--  2.0 unx     1490 b- defN 22-Oct-25 09:23 izihawa_utils/coding.py
 -rw-r--r--  2.0 unx     2895 b- defN 22-Oct-25 09:23 izihawa_utils/common.py
 -rw-r--r--  2.0 unx      248 b- defN 22-Oct-25 09:23 izihawa_utils/env.py
 -rw-r--r--  2.0 unx     1244 b- defN 22-Nov-03 12:40 izihawa_utils/exceptions.py
 -rw-r--r--  2.0 unx     2023 b- defN 22-Oct-25 09:23 izihawa_utils/file.py
 -rw-r--r--  2.0 unx      661 b- defN 22-Oct-25 09:23 izihawa_utils/importlib.py
 -rw-r--r--  2.0 unx      394 b- defN 22-Oct-25 09:23 izihawa_utils/itertools.py
 -rw-r--r--  2.0 unx     2913 b- defN 22-Oct-25 09:23 izihawa_utils/json.py
--rw-r--r--  2.0 unx    30755 b- defN 22-Oct-25 09:23 izihawa_utils/pb_to_json.py
+-rw-r--r--  2.0 unx    30683 b- defN 23-May-24 13:51 izihawa_utils/pb_to_json.py
 -rw-r--r--  2.0 unx      678 b- defN 22-Oct-25 09:23 izihawa_utils/podolsky_encoding.py
 -rw-r--r--  2.0 unx      218 b- defN 22-Oct-25 09:23 izihawa_utils/random.py
 -rw-r--r--  2.0 unx      340 b- defN 22-Oct-25 09:23 izihawa_utils/text.py
 -rw-r--r--  2.0 unx      984 b- defN 22-Oct-25 09:23 izihawa_utils/tskv.py
-?rw-------  2.0 unx       91 b- defN 22-Dec-03 22:51 izihawa_utils-1.1.0.dist-info/WHEEL
-?rw-------  2.0 unx      326 b- defN 22-Dec-03 22:51 izihawa_utils-1.1.0.dist-info/METADATA
-?rw-------  2.0 unx     1350 b- defN 22-Dec-03 22:51 izihawa_utils-1.1.0.dist-info/RECORD
-17 files, 46610 bytes uncompressed, 12659 bytes compressed:  72.8%
+?rw-------  2.0 unx       91 b- defN 23-May-24 13:51 izihawa_utils-1.1.1.dist-info/WHEEL
+?rw-------  2.0 unx      326 b- defN 23-May-24 13:51 izihawa_utils-1.1.1.dist-info/METADATA
+?rw-------  2.0 unx     1350 b- defN 23-May-24 13:51 izihawa_utils-1.1.1.dist-info/RECORD
+17 files, 46538 bytes uncompressed, 12627 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -36,17 +36,17 @@
 
 Filename: izihawa_utils/text.py
 Comment: 
 
 Filename: izihawa_utils/tskv.py
 Comment: 
 
-Filename: izihawa_utils-1.1.0.dist-info/WHEEL
+Filename: izihawa_utils-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: izihawa_utils-1.1.0.dist-info/METADATA
+Filename: izihawa_utils-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: izihawa_utils-1.1.0.dist-info/RECORD
+Filename: izihawa_utils-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## izihawa_utils/pb_to_json.py

```diff
@@ -1,15 +1,14 @@
 import base64
 import json
 import math
 import re
 from collections import OrderedDict
 from operator import methodcaller
 
-import six
 from google.protobuf import (
     descriptor,
     symbol_database,
 )
 from google.protobuf.internal import type_checkers
 
 _TIMESTAMPFOMAT = '%Y-%m-%dT%H:%M:%S'
@@ -19,17 +18,17 @@
                         descriptor.FieldDescriptor.CPPTYPE_UINT64])
 _FLOAT_TYPES = frozenset([descriptor.FieldDescriptor.CPPTYPE_FLOAT,
                           descriptor.FieldDescriptor.CPPTYPE_DOUBLE])
 _INFINITY = 'Infinity'
 _NEG_INFINITY = '-Infinity'
 _NAN = 'NaN'
 
-_UNPAIRED_SURROGATE_PATTERN = re.compile(six.u(
+_UNPAIRED_SURROGATE_PATTERN = re.compile(
     r'[\ud800-\udbff](?![\udc00-\udfff])|(?<![\ud800-\udbff])[\udc00-\udfff]'
-))
+)
 
 _VALID_EXTENSION_NAME = re.compile(r'\[[a-zA-Z0-9\._]*\]$')
 
 
 class Error(Exception):
   """Top-level module error for json_format."""
 
@@ -374,15 +373,15 @@
 
   Returns:
     The same message passed as argument.
 
   Raises::
     ParseError: On JSON parsing problems.
   """
-  if not isinstance(text, six.text_type): text = text.decode('utf-8')
+  if not isinstance(text, str): text = text.decode('utf-8')
   try:
     js = json.loads(text, object_pairs_hook=_DuplicateChecker)
   except ValueError as e:
     raise ParseError('Failed to load JSON: {0}.'.format(str(e)))
   return ParseDict(js, message, ignore_unknown_fields, descriptor_pool)
 
 
@@ -403,15 +402,15 @@
     The same message passed as argument.
   """
   parser = _Parser(ignore_unknown_fields, descriptor_pool)
   parser.ConvertMessage(js_dict, message)
   return message
 
 
-_INT_OR_FLOAT = six.integer_types + (float,)
+_INT_OR_FLOAT = (int,) + (float,)
 
 
 class _Parser(object):
   """JSON format parser for protocol message."""
 
   def __init__(self, ignore_unknown_fields, descriptor_pool):
     self.ignore_unknown_fields = ignore_unknown_fields
@@ -594,15 +593,15 @@
       self._ConvertStructMessage(value, message.struct_value)
     elif isinstance(value, list):
       self. _ConvertListValueMessage(value, message.list_value)
     elif value is None:
       message.null_value = 0
     elif isinstance(value, bool):
       message.bool_value = value
-    elif isinstance(value, six.string_types):
+    elif isinstance(value, str):
       message.string_value = value
     elif isinstance(value, _INT_OR_FLOAT):
       message.number_value = value
     else:
       raise ParseError('Value {0} has unexpected type {1}.'.format(
           value, type(value)))
 
@@ -677,15 +676,15 @@
     return _ConvertInteger(value)
   elif field.cpp_type in _FLOAT_TYPES:
     return _ConvertFloat(value, field)
   elif field.cpp_type == descriptor.FieldDescriptor.CPPTYPE_BOOL:
     return _ConvertBool(value, require_str)
   elif field.cpp_type == descriptor.FieldDescriptor.CPPTYPE_STRING:
     if field.type == descriptor.FieldDescriptor.TYPE_BYTES:
-      if isinstance(value, six.text_type):
+      if isinstance(value, str):
         encoded = value.encode('utf-8')
       else:
         encoded = value
       # Add extra padding '='
       padded_value = encoded + b'=' * (4 - len(encoded) % 4)
       return base64.urlsafe_b64decode(padded_value)
     else:
@@ -724,15 +723,15 @@
 
   Raises:
     ParseError: If an integer couldn't be consumed.
   """
   if isinstance(value, float) and not value.is_integer():
     raise ParseError('Couldn\'t parse integer: {0}.'.format(value))
 
-  if isinstance(value, six.text_type) and value.find(' ') != -1:
+  if isinstance(value, str) and value.find(' ') != -1:
     raise ParseError('Couldn\'t parse integer: "{0}".'.format(value))
 
   if isinstance(value, bool):
     raise ParseError('Bool value {0} is not acceptable for '
                      'integer field.'.format(value))
 
   return int(value)
```

## Comparing `izihawa_utils-1.1.0.dist-info/RECORD` & `izihawa_utils-1.1.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-izihawa_utils-1.1.0.dist-info/METADATA,sha256=qZk3vlxeEyMAvvySbEjsgXY9eQUY8uciAHGPfJK34AE,326
-izihawa_utils-1.1.0.dist-info/RECORD,,
-izihawa_utils-1.1.0.dist-info/WHEEL,sha256=sobxWSyDDkdg_rinUth-jxhXHqoNqlmNMJY3aTZn2Us,91
+izihawa_utils-1.1.1.dist-info/METADATA,sha256=4HXq6j4UNFQOGjKZ9nR96pAHyIt27vUzNm2AtcOEVtc,326
+izihawa_utils-1.1.1.dist-info/RECORD,,
+izihawa_utils-1.1.1.dist-info/WHEEL,sha256=sobxWSyDDkdg_rinUth-jxhXHqoNqlmNMJY3aTZn2Us,91
 izihawa_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 izihawa_utils/coding.py,sha256=zAisgY-vgSttj7yOX29vPz-0iZgcD8YVdduwhVHZ7fQ,1490
 izihawa_utils/common.py,sha256=4-9tdCDj-UhGxs93rAx7otH5IVppIHMCdOqvULRp9uQ,2895
 izihawa_utils/env.py,sha256=3LmDAB9PR8hxBRVaUqnf-eVx5LR8TjHIhJtVB303-xc,248
 izihawa_utils/exceptions.py,sha256=1HdD_3du33zPDCZwKR1PvXa4d4RVMd6LxIuDuTjhaOM,1244
 izihawa_utils/file.py,sha256=RYjl8v7zyqktIOEWPLjfxKLp6o-cwDXisomiZ96Vjyg,2023
 izihawa_utils/importlib.py,sha256=D9WDh4SkaNy57fjxaAQh--1WOfhqW3zJU_vO4EARKHk,661
 izihawa_utils/itertools.py,sha256=veoYhCeRPD_yyeLQ1B7Ri4IJOBkntsHeyNr_2h5PuOE,394
 izihawa_utils/json.py,sha256=FFfLszhUcb-SzD9o7mXE-cuwtABPAdgK_76w5oBjo_M,2913
-izihawa_utils/pb_to_json.py,sha256=3EecfqekL5fOP_kWZuehbUxwplx0t51R9OVrJ45wJWY,30755
+izihawa_utils/pb_to_json.py,sha256=3AKrKjJ2gqb2j30bJNQXH8UFuvUTLZt94HvmAjqfXeg,30683
 izihawa_utils/podolsky_encoding.py,sha256=TSwYtX8DoVRJfnKse6GaH0XfQMXCoNIxNTlIgvzhb4I,678
 izihawa_utils/random.py,sha256=OFKTbncBCdVvJbimVa_eEMaGj5l0aH3rKJmdrf0jnKM,218
 izihawa_utils/text.py,sha256=KvlbYkx23vk88ocfg9XLYLWhqo0BUSzO7QcSqHzic-8,340
 izihawa_utils/tskv.py,sha256=Pn020gz2so-5gL6Kyns7snuMbPEhj8fwx90iMRuwIPg,984
```

