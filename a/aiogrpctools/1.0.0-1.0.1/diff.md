# Comparing `tmp/aiogrpctools-1.0.0-py3-none-any.whl.zip` & `tmp/aiogrpctools-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2473 bytes, number of entries: 5
--rw-r--r--  2.0 unx      202 b- defN 22-Oct-25 09:23 __init__.py
--rw-r--r--  2.0 unx     4772 b- defN 23-May-24 12:29 base.py
-?rw-------  2.0 unx       91 b- defN 23-May-24 12:30 aiogrpctools-1.0.0.dist-info/WHEEL
-?rw-------  2.0 unx      425 b- defN 23-May-24 12:30 aiogrpctools-1.0.0.dist-info/METADATA
-?rw-------  2.0 unx      351 b- defN 23-May-24 12:30 aiogrpctools-1.0.0.dist-info/RECORD
-5 files, 5841 bytes uncompressed, 1823 bytes compressed:  68.8%
+Zip file size: 2526 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      202 b- defN 22-Oct-25 09:23 aiogrpctools/__init__.py
+-rw-r--r--  2.0 unx     4780 b- defN 23-May-24 12:37 aiogrpctools/base.py
+?rw-------  2.0 unx       91 b- defN 23-May-24 12:37 aiogrpctools-1.0.1.dist-info/WHEEL
+?rw-------  2.0 unx      425 b- defN 23-May-24 12:37 aiogrpctools-1.0.1.dist-info/METADATA
+?rw-------  2.0 unx      377 b- defN 23-May-24 12:37 aiogrpctools-1.0.1.dist-info/RECORD
+5 files, 5875 bytes uncompressed, 1824 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: __init__.py
+Filename: aiogrpctools/__init__.py
 Comment: 
 
-Filename: base.py
+Filename: aiogrpctools/base.py
 Comment: 
 
-Filename: aiogrpctools-1.0.0.dist-info/WHEEL
+Filename: aiogrpctools-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: aiogrpctools-1.0.0.dist-info/METADATA
+Filename: aiogrpctools-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: aiogrpctools-1.0.0.dist-info/RECORD
+Filename: aiogrpctools-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `base.py` & `aiogrpctools/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import yaml
 from aiokit import (
     AioRootThing,
     AioThing,
 )
 from google.protobuf.json_format import MessageToDict
 from grpc import aio
+from izihawa_loglib import error_log
 from izihawa_utils.text import camel_to_snake
-from loglib import error_log
 
 
 class AioGrpcServer(AioRootThing):
     def __init__(self, address, port, max_message_length: int = 1024 * 1024 * 1024, termination_timeout: float = 1.0):
         super().__init__()
         self.address = address
         self.port = port
```

