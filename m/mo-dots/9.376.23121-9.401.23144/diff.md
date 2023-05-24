# Comparing `tmp/mo_dots-9.376.23121-py2.py3-none-any.whl.zip` & `tmp/mo_dots-9.401.23144-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 25457 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat    19983 b- defN 23-Apr-02 13:51 mo_dots/__init__.py
--rw-rw-rw-  2.0 fat    14049 b- defN 23-May-01 12:32 mo_dots/datas.py
--rw-rw-rw-  2.0 fat     9899 b- defN 23-Apr-02 13:51 mo_dots/lists.py
--rw-rw-rw-  2.0 fat     6670 b- defN 23-Apr-02 13:51 mo_dots/nones.py
--rw-rw-rw-  2.0 fat     5088 b- defN 23-Apr-02 13:51 mo_dots/objects.py
--rw-rw-rw-  2.0 fat     1490 b- defN 23-Apr-02 13:51 mo_dots/utils.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-May-01 12:32 mo_dots-9.376.23121.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4849 b- defN 23-May-01 12:32 mo_dots-9.376.23121.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-01 12:32 mo_dots-9.376.23121.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-01 12:32 mo_dots-9.376.23121.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      862 b- defN 23-May-01 12:32 mo_dots-9.376.23121.dist-info/RECORD
-11 files, 79733 bytes uncompressed, 24019 bytes compressed:  69.9%
+Zip file size: 25237 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat    19917 b- defN 23-May-24 02:40 mo_dots/__init__.py
+-rw-rw-rw-  2.0 fat    13983 b- defN 23-May-24 02:40 mo_dots/datas.py
+-rw-rw-rw-  2.0 fat     9833 b- defN 23-May-24 02:40 mo_dots/lists.py
+-rw-rw-rw-  2.0 fat     6604 b- defN 23-May-24 02:40 mo_dots/nones.py
+-rw-rw-rw-  2.0 fat     5022 b- defN 23-May-24 02:40 mo_dots/objects.py
+-rw-rw-rw-  2.0 fat     1424 b- defN 23-May-24 02:40 mo_dots/utils.py
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-May-24 02:40 mo_dots-9.401.23144.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4849 b- defN 23-May-24 02:40 mo_dots-9.401.23144.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-24 02:40 mo_dots-9.401.23144.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-24 02:40 mo_dots-9.401.23144.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      862 b- defN 23-May-24 02:40 mo_dots-9.401.23144.dist-info/RECORD
+11 files, 79337 bytes uncompressed, 23799 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mo_dots/objects.py
 Comment: 
 
 Filename: mo_dots/utils.py
 Comment: 
 
-Filename: mo_dots-9.376.23121.dist-info/LICENSE
+Filename: mo_dots-9.401.23144.dist-info/LICENSE
 Comment: 
 
-Filename: mo_dots-9.376.23121.dist-info/METADATA
+Filename: mo_dots-9.401.23144.dist-info/METADATA
 Comment: 
 
-Filename: mo_dots-9.376.23121.dist-info/WHEEL
+Filename: mo_dots-9.401.23144.dist-info/WHEEL
 Comment: 
 
-Filename: mo_dots-9.376.23121.dist-info/top_level.txt
+Filename: mo_dots-9.401.23144.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_dots-9.376.23121.dist-info/RECORD
+Filename: mo_dots-9.401.23144.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_dots/__init__.py

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
 
 import re
 import sys
 
 from mo_dots.datas import Data, data_types, is_data
 from mo_dots.lists import (
     FlatList,
```

## mo_dots/datas.py

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
 
 from copy import copy, deepcopy
 from decimal import Decimal
 
 from mo_future import (
     generator_types,
     iteritems,
```

## mo_dots/lists.py

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
 
 import types
 from copy import deepcopy
 
 from mo_future import generator_types, first
 from mo_imports import expect, delay_import
```

## mo_dots/nones.py

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
 
 from mo_future import text
 from mo_imports import expect, export
 
 from mo_dots.lists import is_sequence
 from mo_dots.utils import CLASS, KEY, SLOT
```

## mo_dots/objects.py

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
 
 from collections import OrderedDict
 from copy import deepcopy
 from datetime import date, datetime
 from decimal import Decimal
 
 from mo_future import (
```

## mo_dots/utils.py

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
 
 import importlib
 
 from mo_future import STDOUT, STDERR
 
 KEY = str("_key")
 SLOT = str("_internal_value")
```

## Comparing `mo_dots-9.376.23121.dist-info/LICENSE` & `mo_dots-9.401.23144.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_dots-9.376.23121.dist-info/METADATA` & `mo_dots-9.401.23144.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.376.23121
+Version: 9.401.23144
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
@@ -12,16 +12,16 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-future (==7.340.23006)
-Requires-Dist: mo-imports (==7.365.23080)
+Requires-Dist: mo-future (==7.401.23144)
+Requires-Dist: mo-imports (==7.401.23144)
 Provides-Extra: tests
 Requires-Dist: mo-logs ; extra == 'tests'
 Requires-Dist: mo-json ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: pyLibrary ; extra == 'tests'
 Requires-Dist: mo-math ; extra == 'tests'
```

