# Comparing `tmp/is_msgs-1.1.8.tar.gz` & `tmp/is_msgs-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/is_msgs-1.1.8.tar", last modified: Wed Oct 17 13:28:18 2018, max compression
+gzip compressed data, was "dist/is_msgs-1.1.9.tar", last modified: Tue Nov 27 13:02:11 2018, max compression
```

## Comparing `is_msgs-1.1.8.tar` & `is_msgs-1.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 felippe   (1000) felippe   (1000)        0 2018-10-17 13:28:18.000000 is_msgs-1.1.8/
-drwxrwxr-x   0 felippe   (1000) felippe   (1000)        0 2018-10-17 13:28:18.000000 is_msgs-1.1.8/is_msgs/
--rw-rw-r--   0 felippe   (1000) felippe   (1000)     3557 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/camera.proto
--rw-rw-r--   0 felippe   (1000) felippe   (1000)      895 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/tests.proto
--rw-rw-r--   0 felippe   (1000) felippe   (1000)    31367 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/camera_pb2.py
-drwxrwxr-x   0 felippe   (1000) felippe   (1000)        0 2018-10-17 13:28:18.000000 is_msgs-1.1.8/is_msgs/utils/
--rw-rw-r--   0 felippe   (1000) felippe   (1000)        0 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/utils/__init__.py
--rw-rw-r--   0 felippe   (1000) felippe   (1000)     1337 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/utils/build.py
--rw-rw-r--   0 felippe   (1000) felippe   (1000)     9952 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/tests_pb2.py
--rw-rw-r--   0 felippe   (1000) felippe   (1000)     4746 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/image.proto
--rw-rw-r--   0 felippe   (1000) felippe   (1000)    28449 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/image_pb2.py
--rw-rw-r--   0 felippe   (1000) felippe   (1000)    14171 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/robot_pb2.py
--rw-rw-r--   0 felippe   (1000) felippe   (1000)     2266 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/common.proto
--rw-rw-r--   0 felippe   (1000) felippe   (1000)      902 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/power.proto
--rw-rw-r--   0 felippe   (1000) felippe   (1000)        0 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/__init__.py
--rw-rw-r--   0 felippe   (1000) felippe   (1000)     8194 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/power_pb2.py
--rw-rw-r--   0 felippe   (1000) felippe   (1000)    26756 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/validate.proto
--rw-rw-r--   0 felippe   (1000) felippe   (1000)    99271 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/validate_pb2.py
--rw-rw-r--   0 felippe   (1000) felippe   (1000)    24549 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/common_pb2.py
--rw-rw-r--   0 felippe   (1000) felippe   (1000)      940 2018-10-17 13:28:04.000000 is_msgs-1.1.8/is_msgs/robot.proto
--rw-rw-r--   0 felippe   (1000) felippe   (1000)      231 2018-10-17 13:28:18.000000 is_msgs-1.1.8/PKG-INFO
--rw-rw-r--   0 felippe   (1000) felippe   (1000)     2488 2018-10-17 13:20:48.000000 is_msgs-1.1.8/README.md
--rw-rw-r--   0 felippe   (1000) felippe   (1000)       38 2018-10-17 13:28:18.000000 is_msgs-1.1.8/setup.cfg
-drwxrwxr-x   0 felippe   (1000) felippe   (1000)        0 2018-10-17 13:28:18.000000 is_msgs-1.1.8/is_msgs.egg-info/
--rw-rw-r--   0 felippe   (1000) felippe   (1000)        1 2018-10-17 13:28:18.000000 is_msgs-1.1.8/is_msgs.egg-info/not-zip-safe
--rw-rw-r--   0 felippe   (1000) felippe   (1000)      568 2018-10-17 13:28:18.000000 is_msgs-1.1.8/is_msgs.egg-info/SOURCES.txt
--rw-rw-r--   0 felippe   (1000) felippe   (1000)        1 2018-10-17 13:28:18.000000 is_msgs-1.1.8/is_msgs.egg-info/dependency_links.txt
--rw-rw-r--   0 felippe   (1000) felippe   (1000)      231 2018-10-17 13:28:18.000000 is_msgs-1.1.8/is_msgs.egg-info/PKG-INFO
--rw-rw-r--   0 felippe   (1000) felippe   (1000)        8 2018-10-17 13:28:18.000000 is_msgs-1.1.8/is_msgs.egg-info/top_level.txt
--rw-rw-r--   0 felippe   (1000) felippe   (1000)       16 2018-10-17 13:28:18.000000 is_msgs-1.1.8/is_msgs.egg-info/requires.txt
--rw-rw-r--   0 felippe   (1000) felippe   (1000)      371 2018-10-17 13:26:21.000000 is_msgs-1.1.8/setup.py
+drwxrwxr-x   0 felippe   (1000) felippe   (1000)        0 2018-11-27 13:02:11.000000 is_msgs-1.1.9/
+drwxrwxr-x   0 felippe   (1000) felippe   (1000)        0 2018-11-27 13:02:11.000000 is_msgs-1.1.9/is_msgs/
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)     3557 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/camera.proto
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)      895 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/tests.proto
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)    31367 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/camera_pb2.py
+drwxrwxr-x   0 felippe   (1000) felippe   (1000)        0 2018-11-27 13:02:11.000000 is_msgs-1.1.9/is_msgs/utils/
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)        0 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/utils/__init__.py
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)     1337 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/utils/build.py
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)     9952 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/tests_pb2.py
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)     4715 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/image.proto
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)    28325 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/image_pb2.py
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)    16838 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/robot_pb2.py
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)     2266 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/common.proto
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)      902 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/power.proto
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)        0 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/__init__.py
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)     8194 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/power_pb2.py
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)    26756 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/validate.proto
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)    99271 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/validate_pb2.py
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)    24549 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/common_pb2.py
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)     1598 2018-11-27 13:02:02.000000 is_msgs-1.1.9/is_msgs/robot.proto
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)      231 2018-11-27 13:02:11.000000 is_msgs-1.1.9/PKG-INFO
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)     2488 2018-10-17 13:20:48.000000 is_msgs-1.1.9/README.md
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)       38 2018-11-27 13:02:11.000000 is_msgs-1.1.9/setup.cfg
+drwxrwxr-x   0 felippe   (1000) felippe   (1000)        0 2018-11-27 13:02:11.000000 is_msgs-1.1.9/is_msgs.egg-info/
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)        1 2018-11-27 13:02:11.000000 is_msgs-1.1.9/is_msgs.egg-info/not-zip-safe
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)      568 2018-11-27 13:02:11.000000 is_msgs-1.1.9/is_msgs.egg-info/SOURCES.txt
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)        1 2018-11-27 13:02:11.000000 is_msgs-1.1.9/is_msgs.egg-info/dependency_links.txt
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)      231 2018-11-27 13:02:11.000000 is_msgs-1.1.9/is_msgs.egg-info/PKG-INFO
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)        8 2018-11-27 13:02:11.000000 is_msgs-1.1.9/is_msgs.egg-info/top_level.txt
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)       16 2018-11-27 13:02:11.000000 is_msgs-1.1.9/is_msgs.egg-info/requires.txt
+-rw-rw-r--   0 felippe   (1000) felippe   (1000)      372 2018-11-27 13:01:29.000000 is_msgs-1.1.9/setup.py
```

### Comparing `is_msgs-1.1.8/is_msgs/camera.proto` & `is_msgs-1.1.9/is_msgs/camera.proto`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/is_msgs/tests.proto` & `is_msgs-1.1.9/is_msgs/tests.proto`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/is_msgs/camera_pb2.py` & `is_msgs-1.1.9/is_msgs/camera_pb2.py`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/is_msgs/utils/build.py` & `is_msgs-1.1.9/is_msgs/utils/build.py`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/is_msgs/tests_pb2.py` & `is_msgs-1.1.9/is_msgs/tests_pb2.py`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/is_msgs/image.proto` & `is_msgs-1.1.9/is_msgs/image.proto`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 package is.vision;
 
 option java_package = "com.is.vision";
 option java_multiple_files = true;
 
 import "google/protobuf/wrappers.proto";
-import "is_msgs/common.proto";
 import "is_msgs/validate.proto";
 
 /* Message representing an Image. The image content can be either sent embedded on this message
 or referenced as an external resource. */
 message Image {
   oneof content {
     /* Image content, represented as a stream of bytes in well known image
```

### Comparing `is_msgs-1.1.8/is_msgs/image_pb2.py` & `is_msgs-1.1.9/is_msgs/image_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,25 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
-from is_msgs import common_pb2 as is__msgs_dot_common__pb2
 from is_msgs import validate_pb2 as is__msgs_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='is_msgs/image.proto',
   package='is.vision',
   syntax='proto3',
   serialized_options=_b('\n\rcom.is.visionP\001'),
-  serialized_pb=_b('\n\x13is_msgs/image.proto\x12\tis.vision\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x14is_msgs/common.proto\x1a\x16is_msgs/validate.proto\"1\n\x05Image\x12\x0e\n\x04\x64\x61ta\x18\x01 \x01(\x0cH\x00\x12\r\n\x03uri\x18\x02 \x01(\tH\x00\x42\t\n\x07\x63ontent\"h\n\x0bImageFormat\x12\'\n\x06\x66ormat\x18\x01 \x01(\x0e\x32\x17.is.vision.ImageFormats\x12\x30\n\x0b\x63ompression\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\")\n\x06Vertex\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\t\n\x01z\x18\x03 \x01(\x02\"3\n\x0c\x42oundingPoly\x12#\n\x08vertices\x18\x01 \x03(\x0b\x32\x11.is.vision.Vertex\"+\n\nResolution\x12\x0e\n\x06height\x18\x01 \x01(\r\x12\r\n\x05width\x18\x02 \x01(\r\"3\n\nColorSpace\x12%\n\x05value\x18\x01 \x01(\x0e\x32\x16.is.vision.ColorSpaces\"\xb7\x01\n\rImageSettings\x12)\n\nresolution\x18\x01 \x01(\x0b\x32\x15.is.vision.Resolution\x12&\n\x06\x66ormat\x18\x02 \x01(\x0b\x32\x16.is.vision.ImageFormat\x12*\n\x0b\x63olor_space\x18\x03 \x01(\x0b\x32\x15.is.vision.ColorSpace\x12\'\n\x06region\x18\x04 \x01(\x0b\x32\x17.is.vision.BoundingPoly\"d\n\x0fPointAnnotation\x12\n\n\x02id\x18\x01 \x01(\x03\x12 \n\x05score\x18\x02 \x01(\x02\x42\x11\xba\xe9\xc0\x03\x0c\n\n\x1d\x00\x00\x80?-\x00\x00\x00\x00\x12#\n\x08position\x18\x03 \x01(\x0b\x32\x11.is.vision.Vertex\"\xa7\x01\n\x10ObjectAnnotation\x12\r\n\x05label\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\x12 \n\x05score\x18\x03 \x01(\x02\x42\x11\xba\xe9\xc0\x03\x0c\n\n\x1d\x00\x00\x80?-\x00\x00\x00\x00\x12\'\n\x06region\x18\x04 \x01(\x0b\x32\x17.is.vision.BoundingPoly\x12-\n\tkeypoints\x18\x05 \x03(\x0b\x32\x1a.is.vision.PointAnnotation\"~\n\x11ObjectAnnotations\x12,\n\x07objects\x18\x01 \x03(\x0b\x32\x1b.is.vision.ObjectAnnotation\x12)\n\nresolution\x18\x02 \x01(\x0b\x32\x15.is.vision.Resolution\x12\x10\n\x08\x66rame_id\x18\x03 \x01(\x03*+\n\x0cImageFormats\x12\x07\n\x03PNG\x10\x00\x12\x08\n\x04JPEG\x10\x01\x12\x08\n\x04WebP\x10\x02*4\n\x0b\x43olorSpaces\x12\x07\n\x03RGB\x10\x00\x12\x08\n\x04GRAY\x10\x01\x12\t\n\x05YCbCr\x10\x02\x12\x07\n\x03HSV\x10\x03*\xd5\x02\n\x0eHumanKeypoints\x12\x1a\n\x16UNKNOWN_HUMAN_KEYPOINT\x10\x00\x12\x08\n\x04HEAD\x10\x01\x12\x08\n\x04NOSE\x10\x02\x12\x08\n\x04NECK\x10\x03\x12\x12\n\x0eRIGHT_SHOULDER\x10\x04\x12\x0f\n\x0bRIGHT_ELBOW\x10\x05\x12\x0f\n\x0bRIGHT_WRIST\x10\x06\x12\x11\n\rLEFT_SHOULDER\x10\x07\x12\x0e\n\nLEFT_ELBOW\x10\x08\x12\x0e\n\nLEFT_WRIST\x10\t\x12\r\n\tRIGHT_HIP\x10\n\x12\x0e\n\nRIGHT_KNEE\x10\x0b\x12\x0f\n\x0bRIGHT_ANKLE\x10\x0c\x12\x0c\n\x08LEFT_HIP\x10\r\x12\r\n\tLEFT_KNEE\x10\x0e\x12\x0e\n\nLEFT_ANKLE\x10\x0f\x12\r\n\tRIGHT_EYE\x10\x10\x12\x0c\n\x08LEFT_EYE\x10\x11\x12\r\n\tRIGHT_EAR\x10\x12\x12\x0c\n\x08LEFT_EAR\x10\x13\x12\t\n\x05\x43HEST\x10\x14*6\n\x0cObjectLabels\x12\x12\n\x0eUNKNOWN_OBJECT\x10\x00\x12\x12\n\x0eHUMAN_SKELETON\x10\x01\x42\x11\n\rcom.is.visionP\x01\x62\x06proto3')
+  serialized_pb=_b('\n\x13is_msgs/image.proto\x12\tis.vision\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x16is_msgs/validate.proto\"1\n\x05Image\x12\x0e\n\x04\x64\x61ta\x18\x01 \x01(\x0cH\x00\x12\r\n\x03uri\x18\x02 \x01(\tH\x00\x42\t\n\x07\x63ontent\"h\n\x0bImageFormat\x12\'\n\x06\x66ormat\x18\x01 \x01(\x0e\x32\x17.is.vision.ImageFormats\x12\x30\n\x0b\x63ompression\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\")\n\x06Vertex\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\t\n\x01z\x18\x03 \x01(\x02\"3\n\x0c\x42oundingPoly\x12#\n\x08vertices\x18\x01 \x03(\x0b\x32\x11.is.vision.Vertex\"+\n\nResolution\x12\x0e\n\x06height\x18\x01 \x01(\r\x12\r\n\x05width\x18\x02 \x01(\r\"3\n\nColorSpace\x12%\n\x05value\x18\x01 \x01(\x0e\x32\x16.is.vision.ColorSpaces\"\xb7\x01\n\rImageSettings\x12)\n\nresolution\x18\x01 \x01(\x0b\x32\x15.is.vision.Resolution\x12&\n\x06\x66ormat\x18\x02 \x01(\x0b\x32\x16.is.vision.ImageFormat\x12*\n\x0b\x63olor_space\x18\x03 \x01(\x0b\x32\x15.is.vision.ColorSpace\x12\'\n\x06region\x18\x04 \x01(\x0b\x32\x17.is.vision.BoundingPoly\"d\n\x0fPointAnnotation\x12\n\n\x02id\x18\x01 \x01(\x03\x12 \n\x05score\x18\x02 \x01(\x02\x42\x11\xba\xe9\xc0\x03\x0c\n\n\x1d\x00\x00\x80?-\x00\x00\x00\x00\x12#\n\x08position\x18\x03 \x01(\x0b\x32\x11.is.vision.Vertex\"\xa7\x01\n\x10ObjectAnnotation\x12\r\n\x05label\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\x12 \n\x05score\x18\x03 \x01(\x02\x42\x11\xba\xe9\xc0\x03\x0c\n\n\x1d\x00\x00\x80?-\x00\x00\x00\x00\x12\'\n\x06region\x18\x04 \x01(\x0b\x32\x17.is.vision.BoundingPoly\x12-\n\tkeypoints\x18\x05 \x03(\x0b\x32\x1a.is.vision.PointAnnotation\"~\n\x11ObjectAnnotations\x12,\n\x07objects\x18\x01 \x03(\x0b\x32\x1b.is.vision.ObjectAnnotation\x12)\n\nresolution\x18\x02 \x01(\x0b\x32\x15.is.vision.Resolution\x12\x10\n\x08\x66rame_id\x18\x03 \x01(\x03*+\n\x0cImageFormats\x12\x07\n\x03PNG\x10\x00\x12\x08\n\x04JPEG\x10\x01\x12\x08\n\x04WebP\x10\x02*4\n\x0b\x43olorSpaces\x12\x07\n\x03RGB\x10\x00\x12\x08\n\x04GRAY\x10\x01\x12\t\n\x05YCbCr\x10\x02\x12\x07\n\x03HSV\x10\x03*\xd5\x02\n\x0eHumanKeypoints\x12\x1a\n\x16UNKNOWN_HUMAN_KEYPOINT\x10\x00\x12\x08\n\x04HEAD\x10\x01\x12\x08\n\x04NOSE\x10\x02\x12\x08\n\x04NECK\x10\x03\x12\x12\n\x0eRIGHT_SHOULDER\x10\x04\x12\x0f\n\x0bRIGHT_ELBOW\x10\x05\x12\x0f\n\x0bRIGHT_WRIST\x10\x06\x12\x11\n\rLEFT_SHOULDER\x10\x07\x12\x0e\n\nLEFT_ELBOW\x10\x08\x12\x0e\n\nLEFT_WRIST\x10\t\x12\r\n\tRIGHT_HIP\x10\n\x12\x0e\n\nRIGHT_KNEE\x10\x0b\x12\x0f\n\x0bRIGHT_ANKLE\x10\x0c\x12\x0c\n\x08LEFT_HIP\x10\r\x12\r\n\tLEFT_KNEE\x10\x0e\x12\x0e\n\nLEFT_ANKLE\x10\x0f\x12\r\n\tRIGHT_EYE\x10\x10\x12\x0c\n\x08LEFT_EYE\x10\x11\x12\r\n\tRIGHT_EAR\x10\x12\x12\x0c\n\x08LEFT_EAR\x10\x13\x12\t\n\x05\x43HEST\x10\x14*6\n\x0cObjectLabels\x12\x12\n\x0eUNKNOWN_OBJECT\x10\x00\x12\x12\n\x0eHUMAN_SKELETON\x10\x01\x42\x11\n\rcom.is.visionP\x01\x62\x06proto3')
   ,
-  dependencies=[google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,is__msgs_dot_common__pb2.DESCRIPTOR,is__msgs_dot_validate__pb2.DESCRIPTOR,])
+  dependencies=[google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,is__msgs_dot_validate__pb2.DESCRIPTOR,])
 
 _IMAGEFORMATS = _descriptor.EnumDescriptor(
   name='ImageFormats',
   full_name='is.vision.ImageFormats',
   filename=None,
   file=DESCRIPTOR,
   values=[
@@ -44,16 +43,16 @@
     _descriptor.EnumValueDescriptor(
       name='WebP', index=2, number=2,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1049,
-  serialized_end=1092,
+  serialized_start=1027,
+  serialized_end=1070,
 )
 _sym_db.RegisterEnumDescriptor(_IMAGEFORMATS)
 
 ImageFormats = enum_type_wrapper.EnumTypeWrapper(_IMAGEFORMATS)
 _COLORSPACES = _descriptor.EnumDescriptor(
   name='ColorSpaces',
   full_name='is.vision.ColorSpaces',
@@ -75,16 +74,16 @@
     _descriptor.EnumValueDescriptor(
       name='HSV', index=3, number=3,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1094,
-  serialized_end=1146,
+  serialized_start=1072,
+  serialized_end=1124,
 )
 _sym_db.RegisterEnumDescriptor(_COLORSPACES)
 
 ColorSpaces = enum_type_wrapper.EnumTypeWrapper(_COLORSPACES)
 _HUMANKEYPOINTS = _descriptor.EnumDescriptor(
   name='HumanKeypoints',
   full_name='is.vision.HumanKeypoints',
@@ -174,16 +173,16 @@
     _descriptor.EnumValueDescriptor(
       name='CHEST', index=20, number=20,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1149,
-  serialized_end=1490,
+  serialized_start=1127,
+  serialized_end=1468,
 )
 _sym_db.RegisterEnumDescriptor(_HUMANKEYPOINTS)
 
 HumanKeypoints = enum_type_wrapper.EnumTypeWrapper(_HUMANKEYPOINTS)
 _OBJECTLABELS = _descriptor.EnumDescriptor(
   name='ObjectLabels',
   full_name='is.vision.ObjectLabels',
@@ -197,16 +196,16 @@
     _descriptor.EnumValueDescriptor(
       name='HUMAN_SKELETON', index=1, number=1,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1492,
-  serialized_end=1546,
+  serialized_start=1470,
+  serialized_end=1524,
 )
 _sym_db.RegisterEnumDescriptor(_OBJECTLABELS)
 
 ObjectLabels = enum_type_wrapper.EnumTypeWrapper(_OBJECTLABELS)
 PNG = 0
 JPEG = 1
 WebP = 2
@@ -272,16 +271,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='content', full_name='is.vision.Image.content',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=112,
-  serialized_end=161,
+  serialized_start=90,
+  serialized_end=139,
 )
 
 
 _IMAGEFORMAT = _descriptor.Descriptor(
   name='ImageFormat',
   full_name='is.vision.ImageFormat',
   filename=None,
@@ -310,16 +309,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=163,
-  serialized_end=267,
+  serialized_start=141,
+  serialized_end=245,
 )
 
 
 _VERTEX = _descriptor.Descriptor(
   name='Vertex',
   full_name='is.vision.Vertex',
   filename=None,
@@ -355,16 +354,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=269,
-  serialized_end=310,
+  serialized_start=247,
+  serialized_end=288,
 )
 
 
 _BOUNDINGPOLY = _descriptor.Descriptor(
   name='BoundingPoly',
   full_name='is.vision.BoundingPoly',
   filename=None,
@@ -386,16 +385,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=312,
-  serialized_end=363,
+  serialized_start=290,
+  serialized_end=341,
 )
 
 
 _RESOLUTION = _descriptor.Descriptor(
   name='Resolution',
   full_name='is.vision.Resolution',
   filename=None,
@@ -424,16 +423,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=365,
-  serialized_end=408,
+  serialized_start=343,
+  serialized_end=386,
 )
 
 
 _COLORSPACE = _descriptor.Descriptor(
   name='ColorSpace',
   full_name='is.vision.ColorSpace',
   filename=None,
@@ -455,16 +454,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=410,
-  serialized_end=461,
+  serialized_start=388,
+  serialized_end=439,
 )
 
 
 _IMAGESETTINGS = _descriptor.Descriptor(
   name='ImageSettings',
   full_name='is.vision.ImageSettings',
   filename=None,
@@ -507,16 +506,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=464,
-  serialized_end=647,
+  serialized_start=442,
+  serialized_end=625,
 )
 
 
 _POINTANNOTATION = _descriptor.Descriptor(
   name='PointAnnotation',
   full_name='is.vision.PointAnnotation',
   filename=None,
@@ -552,16 +551,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=649,
-  serialized_end=749,
+  serialized_start=627,
+  serialized_end=727,
 )
 
 
 _OBJECTANNOTATION = _descriptor.Descriptor(
   name='ObjectAnnotation',
   full_name='is.vision.ObjectAnnotation',
   filename=None,
@@ -611,16 +610,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=752,
-  serialized_end=919,
+  serialized_start=730,
+  serialized_end=897,
 )
 
 
 _OBJECTANNOTATIONS = _descriptor.Descriptor(
   name='ObjectAnnotations',
   full_name='is.vision.ObjectAnnotations',
   filename=None,
@@ -656,16 +655,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=921,
-  serialized_end=1047,
+  serialized_start=899,
+  serialized_end=1025,
 )
 
 _IMAGE.oneofs_by_name['content'].fields.append(
   _IMAGE.fields_by_name['data'])
 _IMAGE.fields_by_name['data'].containing_oneof = _IMAGE.oneofs_by_name['content']
 _IMAGE.oneofs_by_name['content'].fields.append(
   _IMAGE.fields_by_name['uri'])
```

### Comparing `is_msgs-1.1.8/is_msgs/robot_pb2.py` & `is_msgs-1.1.9/is_msgs/robot_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from is_msgs import common_pb2 as is__msgs_dot_common__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='is_msgs/robot.proto',
   package='is.robot',
   syntax='proto3',
   serialized_options=_b('\n\014com.is.robotP\001'),
-  serialized_pb=_b('\n\x13is_msgs/robot.proto\x12\x08is.robot\x1a\x14is_msgs/common.proto\".\n\x0bRobotConfig\x12\x1f\n\x05speed\x18\x01 \x01(\x0b\x32\x10.is.common.Speed\".\n\rFinalPoseTask\x12\x1d\n\x04goal\x18\x01 \x01(\x0b\x32\x0f.is.common.Pose\"2\n\x08PathTask\x12&\n\tpositions\x18\x01 \x03(\x0b\x32\x13.is.common.Position\"Z\n\x0eTrajectoryTask\x12&\n\tpositions\x18\x01 \x03(\x0b\x32\x13.is.common.Position\x12 \n\x06speeds\x18\x02 \x03(\x0b\x32\x10.is.common.Speed\"\xd6\x01\n\tRobotTask\x12\'\n\x04pose\x18\x01 \x01(\x0b\x32\x17.is.robot.FinalPoseTaskH\x00\x12\"\n\x04path\x18\x02 \x01(\x0b\x32\x12.is.robot.PathTaskH\x00\x12.\n\ntrajectory\x18\x03 \x01(\x0b\x32\x18.is.robot.TrajectoryTaskH\x00\x12\x15\n\rallowed_error\x18\x0e \x01(\x02\x12-\n\x08sampling\x18\x0f \x01(\x0b\x32\x1b.is.common.SamplingSettingsB\x06\n\x04Task\"\xbe\x01\n\x17RobotControllerProgress\x12\'\n\rcurrent_speed\x18\x01 \x01(\x0b\x32\x10.is.common.Speed\x12%\n\x0c\x63urrent_pose\x18\x02 \x01(\x0b\x32\x0f.is.common.Pose\x12%\n\x0c\x64\x65sired_pose\x18\x03 \x01(\x0b\x32\x0f.is.common.Pose\x12\r\n\x05\x65rror\x18\x04 \x01(\x02\x12\x0c\n\x04\x64one\x18\x05 \x01(\x08\x12\x0f\n\x07sources\x18\x06 \x01(\x05\x42\x10\n\x0c\x63om.is.robotP\x01\x62\x06proto3')
+  serialized_pb=_b('\n\x13is_msgs/robot.proto\x12\x08is.robot\x1a\x14is_msgs/common.proto\x1a\x1fgoogle/protobuf/timestamp.proto\".\n\x0bRobotConfig\x12\x1f\n\x05speed\x18\x01 \x01(\x0b\x32\x10.is.common.Speed\".\n\rFinalPoseTask\x12\x1d\n\x04goal\x18\x01 \x01(\x0b\x32\x0f.is.common.Pose\"2\n\x08PathTask\x12&\n\tpositions\x18\x01 \x03(\x0b\x32\x13.is.common.Position\"Z\n\x0eTrajectoryTask\x12&\n\tpositions\x18\x01 \x03(\x0b\x32\x13.is.common.Position\x12 \n\x06speeds\x18\x02 \x03(\x0b\x32\x10.is.common.Speed\"+\n\tRangeScan\x12\x0e\n\x06\x61ngles\x18\x01 \x03(\x02\x12\x0e\n\x06ranges\x18\x02 \x03(\x02\"\xb5\x01\n\tRobotTask\x12\'\n\x04pose\x18\x01 \x01(\x0b\x32\x17.is.robot.FinalPoseTaskH\x00\x12\"\n\x04path\x18\x02 \x01(\x0b\x32\x12.is.robot.PathTaskH\x00\x12.\n\ntrajectory\x18\x03 \x01(\x0b\x32\x18.is.robot.TrajectoryTaskH\x00\x12\x15\n\rallowed_error\x18\x0e \x01(\x02\x12\x0c\n\x04rate\x18\x0f \x01(\x02\x42\x06\n\x04Task\"\x98\x02\n\x17RobotControllerProgress\x12\'\n\rcurrent_speed\x18\x01 \x01(\x0b\x32\x10.is.common.Speed\x12%\n\x0c\x63urrent_pose\x18\x02 \x01(\x0b\x32\x0f.is.common.Pose\x12%\n\x0c\x64\x65sired_pose\x18\x03 \x01(\x0b\x32\x0f.is.common.Pose\x12\r\n\x05\x65rror\x18\x04 \x01(\x02\x12\x12\n\ncompletion\x18\x05 \x01(\x02\x12\x0f\n\x07sources\x18\x06 \x03(\t\x12)\n\x05\x62\x65gin\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x03\x65nd\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x10\n\x0c\x63om.is.robotP\x01\x62\x06proto3')
   ,
-  dependencies=[is__msgs_dot_common__pb2.DESCRIPTOR,])
+  dependencies=[is__msgs_dot_common__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
 
 
 
 
 _ROBOTCONFIG = _descriptor.Descriptor(
   name='RobotConfig',
   full_name='is.robot.RobotConfig',
@@ -49,16 +50,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=55,
-  serialized_end=101,
+  serialized_start=88,
+  serialized_end=134,
 )
 
 
 _FINALPOSETASK = _descriptor.Descriptor(
   name='FinalPoseTask',
   full_name='is.robot.FinalPoseTask',
   filename=None,
@@ -80,16 +81,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=103,
-  serialized_end=149,
+  serialized_start=136,
+  serialized_end=182,
 )
 
 
 _PATHTASK = _descriptor.Descriptor(
   name='PathTask',
   full_name='is.robot.PathTask',
   filename=None,
@@ -111,16 +112,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=151,
-  serialized_end=201,
+  serialized_start=184,
+  serialized_end=234,
 )
 
 
 _TRAJECTORYTASK = _descriptor.Descriptor(
   name='TrajectoryTask',
   full_name='is.robot.TrajectoryTask',
   filename=None,
@@ -149,16 +150,54 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=203,
-  serialized_end=293,
+  serialized_start=236,
+  serialized_end=326,
+)
+
+
+_RANGESCAN = _descriptor.Descriptor(
+  name='RangeScan',
+  full_name='is.robot.RangeScan',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='angles', full_name='is.robot.RangeScan.angles', index=0,
+      number=1, type=2, cpp_type=6, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='ranges', full_name='is.robot.RangeScan.ranges', index=1,
+      number=2, type=2, cpp_type=6, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=328,
+  serialized_end=371,
 )
 
 
 _ROBOTTASK = _descriptor.Descriptor(
   name='RobotTask',
   full_name='is.robot.RobotTask',
   filename=None,
@@ -190,17 +229,17 @@
       name='allowed_error', full_name='is.robot.RobotTask.allowed_error', index=3,
       number=14, type=2, cpp_type=6, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='sampling', full_name='is.robot.RobotTask.sampling', index=4,
-      number=15, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='rate', full_name='is.robot.RobotTask.rate', index=4,
+      number=15, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -211,16 +250,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='Task', full_name='is.robot.RobotTask.Task',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=296,
-  serialized_end=510,
+  serialized_start=374,
+  serialized_end=555,
 )
 
 
 _ROBOTCONTROLLERPROGRESS = _descriptor.Descriptor(
   name='RobotControllerProgress',
   full_name='is.robot.RobotControllerProgress',
   filename=None,
@@ -252,24 +291,38 @@
       name='error', full_name='is.robot.RobotControllerProgress.error', index=3,
       number=4, type=2, cpp_type=6, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='done', full_name='is.robot.RobotControllerProgress.done', index=4,
-      number=5, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
+      name='completion', full_name='is.robot.RobotControllerProgress.completion', index=4,
+      number=5, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
       name='sources', full_name='is.robot.RobotControllerProgress.sources', index=5,
-      number=6, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
+      number=6, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='begin', full_name='is.robot.RobotControllerProgress.begin', index=6,
+      number=7, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='end', full_name='is.robot.RobotControllerProgress.end', index=7,
+      number=8, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -277,43 +330,45 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=513,
-  serialized_end=703,
+  serialized_start=558,
+  serialized_end=838,
 )
 
 _ROBOTCONFIG.fields_by_name['speed'].message_type = is__msgs_dot_common__pb2._SPEED
 _FINALPOSETASK.fields_by_name['goal'].message_type = is__msgs_dot_common__pb2._POSE
 _PATHTASK.fields_by_name['positions'].message_type = is__msgs_dot_common__pb2._POSITION
 _TRAJECTORYTASK.fields_by_name['positions'].message_type = is__msgs_dot_common__pb2._POSITION
 _TRAJECTORYTASK.fields_by_name['speeds'].message_type = is__msgs_dot_common__pb2._SPEED
 _ROBOTTASK.fields_by_name['pose'].message_type = _FINALPOSETASK
 _ROBOTTASK.fields_by_name['path'].message_type = _PATHTASK
 _ROBOTTASK.fields_by_name['trajectory'].message_type = _TRAJECTORYTASK
-_ROBOTTASK.fields_by_name['sampling'].message_type = is__msgs_dot_common__pb2._SAMPLINGSETTINGS
 _ROBOTTASK.oneofs_by_name['Task'].fields.append(
   _ROBOTTASK.fields_by_name['pose'])
 _ROBOTTASK.fields_by_name['pose'].containing_oneof = _ROBOTTASK.oneofs_by_name['Task']
 _ROBOTTASK.oneofs_by_name['Task'].fields.append(
   _ROBOTTASK.fields_by_name['path'])
 _ROBOTTASK.fields_by_name['path'].containing_oneof = _ROBOTTASK.oneofs_by_name['Task']
 _ROBOTTASK.oneofs_by_name['Task'].fields.append(
   _ROBOTTASK.fields_by_name['trajectory'])
 _ROBOTTASK.fields_by_name['trajectory'].containing_oneof = _ROBOTTASK.oneofs_by_name['Task']
 _ROBOTCONTROLLERPROGRESS.fields_by_name['current_speed'].message_type = is__msgs_dot_common__pb2._SPEED
 _ROBOTCONTROLLERPROGRESS.fields_by_name['current_pose'].message_type = is__msgs_dot_common__pb2._POSE
 _ROBOTCONTROLLERPROGRESS.fields_by_name['desired_pose'].message_type = is__msgs_dot_common__pb2._POSE
+_ROBOTCONTROLLERPROGRESS.fields_by_name['begin'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
+_ROBOTCONTROLLERPROGRESS.fields_by_name['end'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 DESCRIPTOR.message_types_by_name['RobotConfig'] = _ROBOTCONFIG
 DESCRIPTOR.message_types_by_name['FinalPoseTask'] = _FINALPOSETASK
 DESCRIPTOR.message_types_by_name['PathTask'] = _PATHTASK
 DESCRIPTOR.message_types_by_name['TrajectoryTask'] = _TRAJECTORYTASK
+DESCRIPTOR.message_types_by_name['RangeScan'] = _RANGESCAN
 DESCRIPTOR.message_types_by_name['RobotTask'] = _ROBOTTASK
 DESCRIPTOR.message_types_by_name['RobotControllerProgress'] = _ROBOTCONTROLLERPROGRESS
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 RobotConfig = _reflection.GeneratedProtocolMessageType('RobotConfig', (_message.Message,), dict(
   DESCRIPTOR = _ROBOTCONFIG,
   __module__ = 'is_msgs.robot_pb2'
@@ -338,14 +393,21 @@
 TrajectoryTask = _reflection.GeneratedProtocolMessageType('TrajectoryTask', (_message.Message,), dict(
   DESCRIPTOR = _TRAJECTORYTASK,
   __module__ = 'is_msgs.robot_pb2'
   # @@protoc_insertion_point(class_scope:is.robot.TrajectoryTask)
   ))
 _sym_db.RegisterMessage(TrajectoryTask)
 
+RangeScan = _reflection.GeneratedProtocolMessageType('RangeScan', (_message.Message,), dict(
+  DESCRIPTOR = _RANGESCAN,
+  __module__ = 'is_msgs.robot_pb2'
+  # @@protoc_insertion_point(class_scope:is.robot.RangeScan)
+  ))
+_sym_db.RegisterMessage(RangeScan)
+
 RobotTask = _reflection.GeneratedProtocolMessageType('RobotTask', (_message.Message,), dict(
   DESCRIPTOR = _ROBOTTASK,
   __module__ = 'is_msgs.robot_pb2'
   # @@protoc_insertion_point(class_scope:is.robot.RobotTask)
   ))
 _sym_db.RegisterMessage(RobotTask)
```

### Comparing `is_msgs-1.1.8/is_msgs/common.proto` & `is_msgs-1.1.9/is_msgs/common.proto`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/is_msgs/power.proto` & `is_msgs-1.1.9/is_msgs/power.proto`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/is_msgs/power_pb2.py` & `is_msgs-1.1.9/is_msgs/power_pb2.py`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/is_msgs/validate.proto` & `is_msgs-1.1.9/is_msgs/validate.proto`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/is_msgs/validate_pb2.py` & `is_msgs-1.1.9/is_msgs/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/is_msgs/common_pb2.py` & `is_msgs-1.1.9/is_msgs/common_pb2.py`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/README.md` & `is_msgs-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `is_msgs-1.1.8/is_msgs.egg-info/SOURCES.txt` & `is_msgs-1.1.9/is_msgs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

