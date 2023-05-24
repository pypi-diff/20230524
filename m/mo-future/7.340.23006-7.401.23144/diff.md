# Comparing `tmp/mo_future-7.340.23006-py2.py3-none-any.whl.zip` & `tmp/mo_future-7.401.23144-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10802 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     4164 b- defN 22-Dec-15 04:31 mo_future/__init__.py
--rw-rw-rw-  2.0 fat     4308 b- defN 22-Dec-04 23:23 mo_future/cache.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Jan-06 04:03 mo_future-7.340.23006.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1965 b- defN 23-Jan-06 04:03 mo_future-7.340.23006.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jan-06 04:03 mo_future-7.340.23006.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jan-06 04:03 mo_future-7.340.23006.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      581 b- defN 23-Jan-06 04:03 mo_future-7.340.23006.dist-info/RECORD
-7 files, 27863 bytes uncompressed, 9772 bytes compressed:  64.9%
+Zip file size: 10737 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     4098 b- defN 23-May-24 02:37 mo_future/__init__.py
+-rw-rw-rw-  2.0 fat     4242 b- defN 23-May-24 02:37 mo_future/cache.py
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-May-24 02:37 mo_future-7.401.23144.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1965 b- defN 23-May-24 02:37 mo_future-7.401.23144.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-24 02:37 mo_future-7.401.23144.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-24 02:37 mo_future-7.401.23144.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      581 b- defN 23-May-24 02:37 mo_future-7.401.23144.dist-info/RECORD
+7 files, 27731 bytes uncompressed, 9707 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: mo_future/__init__.py
 Comment: 
 
 Filename: mo_future/cache.py
 Comment: 
 
-Filename: mo_future-7.340.23006.dist-info/LICENSE
+Filename: mo_future-7.401.23144.dist-info/LICENSE
 Comment: 
 
-Filename: mo_future-7.340.23006.dist-info/METADATA
+Filename: mo_future-7.401.23144.dist-info/METADATA
 Comment: 
 
-Filename: mo_future-7.340.23006.dist-info/WHEEL
+Filename: mo_future-7.401.23144.dist-info/WHEEL
 Comment: 
 
-Filename: mo_future-7.340.23006.dist-info/top_level.txt
+Filename: mo_future-7.401.23144.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_future-7.340.23006.dist-info/RECORD
+Filename: mo_future-7.401.23144.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_future/__init__.py

```diff
@@ -3,15 +3,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
-from __future__ import absolute_import, division, unicode_literals
+
 
 import json
 import sys
 
 from collections import OrderedDict, UserDict
 from collections.abc import Callable, Iterable, Mapping, Set, MutableMapping
 from functools import cmp_to_key, reduce, update_wrapper
```

## mo_future/cache.py

```diff
@@ -3,15 +3,15 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from __future__ import absolute_import, division, unicode_literals
+
 
 from collections import namedtuple
 from functools import update_wrapper
 from types import FunctionType
 
 from mo_dots import Null
 from mo_future import get_function_arguments, get_function_name, get_function_defaults
```

## Comparing `mo_future-7.340.23006.dist-info/LICENSE` & `mo_future-7.401.23144.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_future-7.340.23006.dist-info/METADATA` & `mo_future-7.401.23144.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-future
-Version: 7.340.23006
+Version: 7.401.23144
 Summary: More future! Make Python 2/3 compatibility a bit easier
 Home-page: https://github.com/klahnakoski/mo-future
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

## Comparing `mo_future-7.340.23006.dist-info/RECORD` & `mo_future-7.401.23144.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-mo_future/__init__.py,sha256=PgTeJGw-AiSJaWNrwytwORKsc-cBEjLhsWAxn7b5yjI,4164
-mo_future/cache.py,sha256=nhdrZl08VV7v3-KG8ePQmYJjx_xHzZ5Zyq-llTkYjUc,4308
-mo_future-7.340.23006.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_future-7.340.23006.dist-info/METADATA,sha256=fNAyVciEfj4ZRh843bwm_O_ai3zkwc90rwLeACn6XpI,1965
-mo_future-7.340.23006.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_future-7.340.23006.dist-info/top_level.txt,sha256=HFDr53Or48gARE_hYcBfZUdD2p2g7xZWSK2He4LZhJs,10
-mo_future-7.340.23006.dist-info/RECORD,,
+mo_future/__init__.py,sha256=GNxfVmAy5ZiCUF-n8skDaAQtZBfx-1rsgHTKbxuZXRk,4098
+mo_future/cache.py,sha256=fZSqvEuz3DyWP-80AmHHMeRbFYqqqosNRq5pAgbQZb4,4242
+mo_future-7.401.23144.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_future-7.401.23144.dist-info/METADATA,sha256=_VxakHGV8_OxXiY8rt4_ObyRl7mBvxFg0JGpHAmeAgo,1965
+mo_future-7.401.23144.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_future-7.401.23144.dist-info/top_level.txt,sha256=HFDr53Or48gARE_hYcBfZUdD2p2g7xZWSK2He4LZhJs,10
+mo_future-7.401.23144.dist-info/RECORD,,
```

