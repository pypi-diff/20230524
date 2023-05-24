# Comparing `tmp/prefixed_aiostatsd-1.1-py3-none-any.whl.zip` & `tmp/prefixed_aiostatsd-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3164 bytes, number of entries: 6
--rw-r--r--  2.0 unx     3276 b- defN 23-May-22 19:03 prefixed_aiostatsd/__init__.py
--rw-r--r--  2.0 unx     1067 b- defN 23-May-22 19:05 prefixed_aiostatsd-1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      677 b- defN 23-May-22 19:05 prefixed_aiostatsd-1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 19:05 prefixed_aiostatsd-1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 19:05 prefixed_aiostatsd-1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      517 b- defN 23-May-22 19:05 prefixed_aiostatsd-1.1.dist-info/RECORD
-6 files, 5648 bytes uncompressed, 2218 bytes compressed:  60.7%
+Zip file size: 3152 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     3249 b- defN 23-May-24 14:05 prefixed_aiostatsd/__init__.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-May-24 14:06 prefixed_aiostatsd-1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      677 b- defN 23-May-24 14:06 prefixed_aiostatsd-1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 14:06 prefixed_aiostatsd-1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-May-24 14:06 prefixed_aiostatsd-1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      517 b- defN 23-May-24 14:06 prefixed_aiostatsd-1.2.dist-info/RECORD
+6 files, 5621 bytes uncompressed, 2206 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: prefixed_aiostatsd/__init__.py
 Comment: 
 
-Filename: prefixed_aiostatsd-1.1.dist-info/LICENSE
+Filename: prefixed_aiostatsd-1.2.dist-info/LICENSE
 Comment: 
 
-Filename: prefixed_aiostatsd-1.1.dist-info/METADATA
+Filename: prefixed_aiostatsd-1.2.dist-info/METADATA
 Comment: 
 
-Filename: prefixed_aiostatsd-1.1.dist-info/WHEEL
+Filename: prefixed_aiostatsd-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: prefixed_aiostatsd-1.1.dist-info/top_level.txt
+Filename: prefixed_aiostatsd-1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: prefixed_aiostatsd-1.1.dist-info/RECORD
+Filename: prefixed_aiostatsd-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## prefixed_aiostatsd/__init__.py

```diff
@@ -1,12 +1,11 @@
 import abc
 import contextlib
 import time
-from collections.abc import Iterator
-from typing import Any
+from typing import Any, Iterator
 
 from aiostatsd.client import StatsdClient as StatsdClientBase
 
 
 class IStatsdClient(StatsdClientBase, metaclass=abc.ABCMeta):
     def __init__(self) -> None:
         pass  # Override parent initializer. We don't want implementation inheritance.
```

## Comparing `prefixed_aiostatsd-1.1.dist-info/LICENSE` & `prefixed_aiostatsd-1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `prefixed_aiostatsd-1.1.dist-info/METADATA` & `prefixed_aiostatsd-1.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefixed-aiostatsd
-Version: 1.1
+Version: 1.2
 Summary: Prefixed AioStatsD
 Home-page: https://github.com/DomainsBot/prefixed-aiostatsd
 Author: Domainsbot
 Author-email: tech@domainsbot.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

