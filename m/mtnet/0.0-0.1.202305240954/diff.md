# Comparing `tmp/mtnet-0.0-py3-none-any.whl.zip` & `tmp/mtnet-0.1.202305240954-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,14 @@
-Zip file size: 1901 bytes, number of entries: 5
--rw-r--r--  2.0 unx     1070 b- defN 23-Apr-20 05:25 mtnet-0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-20 05:25 mtnet-0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 05:25 mtnet-0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-20 05:25 mtnet-0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      364 b- defN 23-Apr-20 05:25 mtnet-0.0.dist-info/RECORD
-5 files, 1907 bytes uncompressed, 1221 bytes compressed:  36.0%
+Zip file size: 12835 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1156 b- defN 23-May-24 09:53 mt/net/__init__.py
+-rw-r--r--  2.0 unx     2986 b- defN 23-May-24 09:47 mt/net/base.py
+-rw-r--r--  2.0 unx     5102 b- defN 23-May-24 09:47 mt/net/host_port.py
+-rw-r--r--  2.0 unx    10611 b- defN 23-May-24 09:47 mt/net/port_forwarding.py
+-rw-r--r--  2.0 unx     9630 b- defN 23-May-24 09:47 mt/net/port_forwarding_async.py
+-rw-r--r--  2.0 unx     5483 b- defN 23-May-24 09:47 mt/net/ssh_forwarding.py
+-rw-r--r--  2.0 unx      396 b- defN 23-May-24 09:54 mt/net/version.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-24 09:54 mtnet-0.1.202305240954.dist-info/LICENSE
+-rw-r--r--  2.0 unx      472 b- defN 23-May-24 09:54 mtnet-0.1.202305240954.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 09:54 mtnet-0.1.202305240954.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-May-24 09:54 mtnet-0.1.202305240954.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      976 b- defN 23-May-24 09:54 mtnet-0.1.202305240954.dist-info/RECORD
+12 files, 37977 bytes uncompressed, 11197 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -1,16 +1,37 @@
-Filename: mtnet-0.0.dist-info/LICENSE
+Filename: mt/net/__init__.py
 Comment: 
 
-Filename: mtnet-0.0.dist-info/METADATA
+Filename: mt/net/base.py
 Comment: 
 
-Filename: mtnet-0.0.dist-info/WHEEL
+Filename: mt/net/host_port.py
 Comment: 
 
-Filename: mtnet-0.0.dist-info/top_level.txt
+Filename: mt/net/port_forwarding.py
 Comment: 
 
-Filename: mtnet-0.0.dist-info/RECORD
+Filename: mt/net/port_forwarding_async.py
+Comment: 
+
+Filename: mt/net/ssh_forwarding.py
+Comment: 
+
+Filename: mt/net/version.py
+Comment: 
+
+Filename: mtnet-0.1.202305240954.dist-info/LICENSE
+Comment: 
+
+Filename: mtnet-0.1.202305240954.dist-info/METADATA
+Comment: 
+
+Filename: mtnet-0.1.202305240954.dist-info/WHEEL
+Comment: 
+
+Filename: mtnet-0.1.202305240954.dist-info/top_level.txt
+Comment: 
+
+Filename: mtnet-0.1.202305240954.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mtnet-0.0.dist-info/LICENSE` & `mtnet-0.1.202305240954.dist-info/LICENSE`

 * *Files identical despite different names*

