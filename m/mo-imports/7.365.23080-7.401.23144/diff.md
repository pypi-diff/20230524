# Comparing `tmp/mo_imports-7.365.23080-py2.py3-none-any.whl.zip` & `tmp/mo_imports-7.401.23144-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11166 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     9758 b- defN 23-Mar-21 00:02 mo_imports/__init__.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Mar-21 00:02 mo_imports-7.365.23080.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4945 b- defN 23-Mar-21 00:02 mo_imports-7.365.23080.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Mar-21 00:02 mo_imports-7.365.23080.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Mar-21 00:02 mo_imports-7.365.23080.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      512 b- defN 23-Mar-21 00:02 mo_imports-7.365.23080.dist-info/RECORD
-6 files, 32061 bytes uncompressed, 10236 bytes compressed:  68.1%
+Zip file size: 11130 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     9696 b- defN 23-May-24 02:37 mo_imports/__init__.py
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-May-24 02:37 mo_imports-7.401.23144.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4945 b- defN 23-May-24 02:37 mo_imports-7.401.23144.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-24 02:37 mo_imports-7.401.23144.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-24 02:37 mo_imports-7.401.23144.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      512 b- defN 23-May-24 02:37 mo_imports-7.401.23144.dist-info/RECORD
+6 files, 31999 bytes uncompressed, 10200 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: mo_imports/__init__.py
 Comment: 
 
-Filename: mo_imports-7.365.23080.dist-info/LICENSE
+Filename: mo_imports-7.401.23144.dist-info/LICENSE
 Comment: 
 
-Filename: mo_imports-7.365.23080.dist-info/METADATA
+Filename: mo_imports-7.401.23144.dist-info/METADATA
 Comment: 
 
-Filename: mo_imports-7.365.23080.dist-info/WHEEL
+Filename: mo_imports-7.401.23144.dist-info/WHEEL
 Comment: 
 
-Filename: mo_imports-7.365.23080.dist-info/top_level.txt
+Filename: mo_imports-7.401.23144.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_imports-7.365.23080.dist-info/RECORD
+Filename: mo_imports-7.401.23144.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_imports/__init__.py

```diff
@@ -3,25 +3,25 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
-from __future__ import absolute_import, division, unicode_literals
+
 
 import importlib
 import sys
 from threading import Thread, Event
 from time import time
 
 from mo_future import text, allocate_lock
 
 DEBUG = False
-WAIT_FOR_EXPORT = 10  # SECONDS TO WAIT FROM MOST RECENT expect() TO LAST export()
+WAIT_FOR_EXPORT = 10_000  # SECONDS TO WAIT FROM MOST RECENT expect() TO LAST export()
 
 _locker = allocate_lock()
 _expectations = []
 _expiry = None
 _monitor = None
 _nothing = object()
 _set = object.__setattr__
```

## Comparing `mo_imports-7.365.23080.dist-info/LICENSE` & `mo_imports-7.401.23144.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_imports-7.365.23080.dist-info/METADATA` & `mo_imports-7.401.23144.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mo-imports
-Version: 7.365.23080
+Version: 7.401.23144
 Summary: More Imports! - Delayed importing
 Home-page: https://github.com/klahnakoski/mo-imports
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-future (==7.340.23006)
+Requires-Dist: mo-future (==7.401.23144)
 Provides-Extra: tests
 Requires-Dist: mo-logs ; extra == 'tests'
 
 # More Imports! - Delayed importing 
 
 A couple of methods to make late importing cleaner
```

