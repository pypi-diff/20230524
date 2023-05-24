# Comparing `tmp/facets_overview-1.1.0-py2.py3-none-any.whl.zip` & `tmp/facets_overview-1.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 22359 bytes, number of entries: 12
+Zip file size: 22363 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      677 b- defN 20-Jun-18 23:34 facets_overview/__init__.py
 -rw-r--r--  2.0 unx     9498 b- defN 20-Jun-18 23:34 facets_overview/base_feature_statistics_generator.py
--rw-r--r--  2.0 unx    13759 b- defN 23-Feb-06 13:39 facets_overview/base_generic_feature_statistics_generator.py
+-rw-r--r--  2.0 unx    13756 b- defN 23-May-24 15:55 facets_overview/base_generic_feature_statistics_generator.py
 -rw-r--r--  2.0 unx     1290 b- defN 20-Jun-18 23:34 facets_overview/feature_statistics_generator.py
 -rw-r--r--  2.0 unx    22511 b- defN 20-Jun-18 23:34 facets_overview/feature_statistics_generator_test.py
--rw-r--r--  2.0 unx     9368 b- defN 23-Feb-18 14:11 facets_overview/feature_statistics_pb2.py
+-rw-r--r--  2.0 unx     9368 b- defN 23-May-24 15:55 facets_overview/feature_statistics_pb2.py
 -rw-r--r--  2.0 unx     1277 b- defN 20-Jun-18 23:34 facets_overview/generic_feature_statistics_generator.py
--rw-r--r--  2.0 unx     8410 b- defN 20-Jun-18 23:34 facets_overview/generic_feature_statistics_generator_test.py
--rw-r--r--  2.0 unx    10403 b- defN 23-Feb-18 14:14 facets_overview-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Feb-18 14:14 facets_overview-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Feb-18 14:14 facets_overview-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1183 b- defN 23-Feb-18 14:14 facets_overview-1.1.0.dist-info/RECORD
-12 files, 78502 bytes uncompressed, 20317 bytes compressed:  74.1%
+-rw-r--r--  2.0 unx     8404 b- defN 23-May-24 15:55 facets_overview/generic_feature_statistics_generator_test.py
+-rw-r--r--  2.0 unx    10403 b- defN 23-May-24 15:56 facets_overview-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-24 15:56 facets_overview-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-24 15:56 facets_overview-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1183 b- defN 23-May-24 15:56 facets_overview-1.1.1.dist-info/RECORD
+12 files, 78493 bytes uncompressed, 20321 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: facets_overview/generic_feature_statistics_generator.py
 Comment: 
 
 Filename: facets_overview/generic_feature_statistics_generator_test.py
 Comment: 
 
-Filename: facets_overview-1.1.0.dist-info/METADATA
+Filename: facets_overview-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: facets_overview-1.1.0.dist-info/WHEEL
+Filename: facets_overview-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: facets_overview-1.1.0.dist-info/top_level.txt
+Filename: facets_overview-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: facets_overview-1.1.0.dist-info/RECORD
+Filename: facets_overview-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## facets_overview/base_generic_feature_statistics_generator.py

```diff
@@ -61,15 +61,15 @@
       datasets,
       histogram_categorical_levels_count=histogram_categorical_levels_count)
 
   def DtypeToType(self, dtype):
     """Converts a Numpy dtype to the FeatureNameStatistics.Type proto enum."""
     if dtype.char in np.typecodes['AllFloat']:
       return self.fs_proto.FLOAT
-    elif (dtype.char in np.typecodes['AllInteger'] or dtype == np.bool or
+    elif (dtype.char in np.typecodes['AllInteger'] or dtype == bool or
           np.issubdtype(dtype, np.datetime64) or
           np.issubdtype(dtype, np.timedelta64)):
       return self.fs_proto.INT
     else:
       return self.fs_proto.STRING
 
   def DtypeToNumberConverter(self, dtype):
```

## facets_overview/generic_feature_statistics_generator_test.py

```diff
@@ -75,23 +75,23 @@
     self.assertEqual([31622400000000000], entry['vals'])
 
   def testDTypeToType(self):
     self.assertEqual(self.gfsg.fs_proto.INT,
                      self.gfsg.DtypeToType(np.dtype(np.int32)))
     # Boolean and time types treated as int
     self.assertEqual(self.gfsg.fs_proto.INT,
-                     self.gfsg.DtypeToType(np.dtype(np.bool)))
+                     self.gfsg.DtypeToType(np.dtype(bool)))
     self.assertEqual(self.gfsg.fs_proto.INT,
                      self.gfsg.DtypeToType(np.dtype(np.datetime64)))
     self.assertEqual(self.gfsg.fs_proto.INT,
                      self.gfsg.DtypeToType(np.dtype(np.timedelta64)))
     self.assertEqual(self.gfsg.fs_proto.FLOAT,
                      self.gfsg.DtypeToType(np.dtype(np.float32)))
     self.assertEqual(self.gfsg.fs_proto.STRING,
-                     self.gfsg.DtypeToType(np.dtype(np.str)))
+                     self.gfsg.DtypeToType(np.dtype(str)))
     # Unsupported types treated as string for now
     self.assertEqual(self.gfsg.fs_proto.STRING,
                      self.gfsg.DtypeToType(np.dtype(np.void)))
 
   def testGetDatasetsProtoFromEntriesLists(self):
     entries = {}
     entries['testFeature'] = {
```

## Comparing `facets_overview-1.1.0.dist-info/METADATA` & `facets_overview-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facets-overview
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python code to support the Facets Overview visualization
 Home-page: http://github.com/pair-code/facets
 Author: Google Inc.
 Author-email: opensource@google.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy (>=1.16.0)
```

## Comparing `facets_overview-1.1.0.dist-info/RECORD` & `facets_overview-1.1.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 facets_overview/__init__.py,sha256=nWmGON3eif2EL-oD8rIcHWdLxZwGOGTG7yzhTDW92ns,677
 facets_overview/base_feature_statistics_generator.py,sha256=iRwJ8EOmpcSTdDW7F668XtpCVsKC13ddee0liZlcpkE,9498
-facets_overview/base_generic_feature_statistics_generator.py,sha256=xg3sAOwNMemRNb_rShpsedbIZ2vEMYiRY-BhIrLLrk0,13759
+facets_overview/base_generic_feature_statistics_generator.py,sha256=e9A3DX2shELqK11IQOt0Y2E7368rLllz7pLdD8CYJvI,13756
 facets_overview/feature_statistics_generator.py,sha256=tslfICNmK5ZTNje1srBH6c8AUaekOEsBr0882ybvgCc,1290
 facets_overview/feature_statistics_generator_test.py,sha256=sRFvnS_z3LTBtKTlPg0yzqRDweXQT1YMi2YEHjI3g8s,22511
 facets_overview/feature_statistics_pb2.py,sha256=0iK6bHKhMckJr16Ta_Ibe-exPpVL0u6TVy5ZQUuRbPw,9368
 facets_overview/generic_feature_statistics_generator.py,sha256=P4-RIhAcoCuxvItbKTPfzCfOFTQ_s61Ex8WCccPoJRQ,1277
-facets_overview/generic_feature_statistics_generator_test.py,sha256=SCdqFP8_qAik04JPFIDDLC8qNWT5xUQAzrhtTz__p00,8410
-facets_overview-1.1.0.dist-info/METADATA,sha256=czYEpX4J5m-Sx4VfZqt2GVm2fYr0yYJRtnkaD9BO94Y,10403
-facets_overview-1.1.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-facets_overview-1.1.0.dist-info/top_level.txt,sha256=g7m0lYu84oPwUAIu4McWqpQAmWu9Afanjn9yQhYqlF0,16
-facets_overview-1.1.0.dist-info/RECORD,,
+facets_overview/generic_feature_statistics_generator_test.py,sha256=XH-pHufKgnnq_CpUlCvRqTYKMJXXlRwa2TLeUFoKp38,8404
+facets_overview-1.1.1.dist-info/METADATA,sha256=ysoIIxLDAhGnOIJa_ywrZbDPfzsLDlbRJBSPVSreNJs,10403
+facets_overview-1.1.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+facets_overview-1.1.1.dist-info/top_level.txt,sha256=g7m0lYu84oPwUAIu4McWqpQAmWu9Afanjn9yQhYqlF0,16
+facets_overview-1.1.1.dist-info/RECORD,,
```

