# Comparing `tmp/tigrisdb-1.0.0b2.tar.gz` & `tmp/tigrisdb-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigrisdb-1.0.0b2.tar", max compression
+gzip compressed data, was "tigrisdb-1.0.0b3.tar", max compression
```

## Comparing `tigrisdb-1.0.0b2.tar` & `tigrisdb-1.0.0b3.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0    11357 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/LICENSE
--rw-r--r--   0        0        0      935 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/README.md
--rw-r--r--   0        0        0     1583 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      313 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     1897 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/field_behavior_pb2.py
--rw-r--r--   0        0        0      685 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/field_behavior_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/field_behavior_pb2_grpc.py
--rw-r--r--   0        0        0     2125 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/http_pb2.py
--rw-r--r--   0        0        0     2272 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0     1507 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/httpbody_pb2.py
--rw-r--r--   0        0        0      882 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/httpbody_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/httpbody_pb2_grpc.py
--rw-r--r--   0        0        0    27129 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/OpenAPIv3_pb2.py
--rw-r--r--   0        0        0    49576 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/OpenAPIv3_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/OpenAPIv3_pb2_grpc.py
--rw-r--r--   0        0        0     2102 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/annotations_pb2.py
--rw-r--r--   0        0        0      555 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/annotations_pb2_grpc.py
--rw-r--r--   0        0        0    44365 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2.py
--rw-r--r--   0        0        0    37886 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2.pyi
--rw-r--r--   0        0        0    51527 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2_grpc.py
--rw-r--r--   0        0        0     7946 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2.py
--rw-r--r--   0        0        0     6220 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2.pyi
--rw-r--r--   0        0        0    11198 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2_grpc.py
--rw-r--r--   0        0        0     9308 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2.py
--rw-r--r--   0        0        0     8458 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2.pyi
--rw-r--r--   0        0        0     7981 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2_grpc.py
--rw-r--r--   0        0        0    14625 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2.py
--rw-r--r--   0        0        0    11907 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2.pyi
--rw-r--r--   0        0        0    23238 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2_grpc.py
--rw-r--r--   0        0        0     1147 2023-05-22 16:31:06.181302 tigrisdb-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/__init__.py
--rw-r--r--   0        0        0     2799 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/auth.py
--rw-r--r--   0        0        0     2333 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/client.py
--rw-r--r--   0        0        0     1968 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/collection.py
--rw-r--r--   0        0        0     1986 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/database.py
--rw-r--r--   0        0        0      484 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/errors.py
--rw-r--r--   0        0        0     1720 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/search.py
--rw-r--r--   0        0        0     4587 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/search_index.py
--rw-r--r--   0        0        0      497 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/types/__init__.py
--rw-r--r--   0        0        0     8746 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/types/search.py
--rw-r--r--   0        0        0      527 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/types/sort.py
--rw-r--r--   0        0        0      760 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/utils.py
--rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 tigrisdb-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/LICENSE
+-rw-r--r--   0        0        0      935 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/README.md
+-rw-r--r--   0        0        0     1583 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      313 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     1897 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/field_behavior_pb2.py
+-rw-r--r--   0        0        0      685 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/field_behavior_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/field_behavior_pb2_grpc.py
+-rw-r--r--   0        0        0     2125 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/http_pb2.py
+-rw-r--r--   0        0        0     2272 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0     1507 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/httpbody_pb2.py
+-rw-r--r--   0        0        0      882 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/httpbody_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/httpbody_pb2_grpc.py
+-rw-r--r--   0        0        0    27129 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/OpenAPIv3_pb2.py
+-rw-r--r--   0        0        0    49576 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/OpenAPIv3_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/OpenAPIv3_pb2_grpc.py
+-rw-r--r--   0        0        0     2102 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/annotations_pb2.py
+-rw-r--r--   0        0        0      555 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0    44365 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2.py
+-rw-r--r--   0        0        0    37886 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2.pyi
+-rw-r--r--   0        0        0    51527 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2_grpc.py
+-rw-r--r--   0        0        0     7946 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2.py
+-rw-r--r--   0        0        0     6220 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2.pyi
+-rw-r--r--   0        0        0    11198 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2_grpc.py
+-rw-r--r--   0        0        0     9308 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2.py
+-rw-r--r--   0        0        0     8458 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2.pyi
+-rw-r--r--   0        0        0     7981 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2_grpc.py
+-rw-r--r--   0        0        0    14625 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2.py
+-rw-r--r--   0        0        0    11907 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2.pyi
+-rw-r--r--   0        0        0    23238 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2_grpc.py
+-rw-r--r--   0        0        0     1147 2023-05-24 01:28:43.288538 tigrisdb-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/__init__.py
+-rw-r--r--   0        0        0     2799 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/auth.py
+-rw-r--r--   0        0        0     2333 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/client.py
+-rw-r--r--   0        0        0     1968 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/collection.py
+-rw-r--r--   0        0        0     1986 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/database.py
+-rw-r--r--   0        0        0      484 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/errors.py
+-rw-r--r--   0        0        0     1860 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/search.py
+-rw-r--r--   0        0        0     4587 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/search_index.py
+-rw-r--r--   0        0        0      554 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/types/__init__.py
+-rw-r--r--   0        0        0      267 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/types/filters/__init__.py
+-rw-r--r--   0        0        0      704 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/types/filters/logical.py
+-rw-r--r--   0        0        0     1132 2023-05-24 01:28:02.696903 tigrisdb-1.0.0b3/tigrisdb/types/filters/selector.py
+-rw-r--r--   0        0        0     8903 2023-05-24 01:28:02.696903 tigrisdb-1.0.0b3/tigrisdb/types/search.py
+-rw-r--r--   0        0        0      487 2023-05-24 01:28:02.696903 tigrisdb-1.0.0b3/tigrisdb/types/sort.py
+-rw-r--r--   0        0        0     1092 2023-05-24 01:28:02.696903 tigrisdb-1.0.0b3/tigrisdb/utils.py
+-rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 tigrisdb-1.0.0b3/PKG-INFO
```

### Comparing `tigrisdb-1.0.0b2/LICENSE` & `tigrisdb-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/README.md` & `tigrisdb-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/google/api/annotations_pb2.py` & `tigrisdb-1.0.0b3/api/generated/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/google/api/field_behavior_pb2.py` & `tigrisdb-1.0.0b3/api/generated/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/google/api/field_behavior_pb2.pyi` & `tigrisdb-1.0.0b3/api/generated/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/google/api/http_pb2.py` & `tigrisdb-1.0.0b3/api/generated/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/google/api/http_pb2.pyi` & `tigrisdb-1.0.0b3/api/generated/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/google/api/httpbody_pb2.py` & `tigrisdb-1.0.0b3/api/generated/google/api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/google/api/httpbody_pb2.pyi` & `tigrisdb-1.0.0b3/api/generated/google/api/httpbody_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/openapiv3/OpenAPIv3_pb2.py` & `tigrisdb-1.0.0b3/api/generated/openapiv3/OpenAPIv3_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/openapiv3/OpenAPIv3_pb2.pyi` & `tigrisdb-1.0.0b3/api/generated/openapiv3/OpenAPIv3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/openapiv3/annotations_pb2.py` & `tigrisdb-1.0.0b3/api/generated/openapiv3/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/openapiv3/annotations_pb2.pyi` & `tigrisdb-1.0.0b3/api/generated/openapiv3/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2.py` & `tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2.pyi` & `tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2_grpc.py` & `tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2.py` & `tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2.pyi` & `tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2_grpc.py` & `tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2.py` & `tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2.pyi` & `tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2_grpc.py` & `tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2.py` & `tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2.pyi` & `tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2_grpc.py` & `tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/pyproject.toml` & `tigrisdb-1.0.0b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tigrisdb"
-version = "1.0.0-beta.2"
+version = "1.0.0-beta.3"
 description = "Python SDK for Tigris <http://www.tigrisdata.com>"
 authors = ["Tigris team <support@tigrisdata.com>"]
 repository = "https://www.github.com/tigrisdata/tigris-client-python"
 documentation = "https://www.tigrisdata.com/docs/"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `tigrisdb-1.0.0b2/tigrisdb/auth.py` & `tigrisdb-1.0.0b3/tigrisdb/auth.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/tigrisdb/client.py` & `tigrisdb-1.0.0b3/tigrisdb/client.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/tigrisdb/collection.py` & `tigrisdb-1.0.0b3/tigrisdb/collection.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/tigrisdb/database.py` & `tigrisdb-1.0.0b3/tigrisdb/database.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/tigrisdb/search.py` & `tigrisdb-1.0.0b3/tigrisdb/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,7 +45,10 @@
         req = DeleteIndexRequest(name=name, project=self.project)
         try:
             resp: DeleteIndexResponse = self.__client.DeleteIndex(req)
         except grpc.RpcError as e:
             raise TigrisServerError("failed to delete search index", e)
 
         return resp.status == "deleted"
+
+    def get_index(self, name: str) -> SearchIndex:
+        return SearchIndex(index_name=name, client=self.__client, config=self.__config)
```

### Comparing `tigrisdb-1.0.0b2/tigrisdb/search_index.py` & `tigrisdb-1.0.0b3/tigrisdb/search_index.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b2/tigrisdb/types/search.py` & `tigrisdb-1.0.0b3/tigrisdb/types/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,79 +16,83 @@
     SearchIndexRequest as ProtoSearchIndexRequest,
 )
 from api.generated.server.v1.search_pb2 import (
     SearchIndexResponse as ProtoSearchIndexResponse,
 )
 from tigrisdb.errors import TigrisException
 from tigrisdb.types import Document, Serializable
+from tigrisdb.types.filters import Filter
 from tigrisdb.types.sort import Sort
 from tigrisdb.utils import marshal, unmarshal
 
 dataclass_default_proto_field = field(
     default=None, repr=False, compare=False, hash=False
 )
 
 
 @dataclass
 class FacetSize(Serializable):
     field: str
     size: int = 10
 
-    def as_obj(self):
+    def query(self):
         return {"size": self.size, "type": "value"}
 
 
 FacetField = Union[str, FacetSize]
 
 
 @dataclass
 class VectorField(Serializable):
     field: str
     vector: List[float]
 
-    def as_obj(self):
+    def query(self):
         return {self.field: self.vector}
 
 
 # TODO: add filter, collation
 @dataclass
 class Query:
     q: str = ""
     search_fields: List[str] = field(default_factory=list)
     vector_query: VectorField = None
+    filter_by: Optional[Filter] = None
     facet_by: Union[str, List[FacetField]] = field(default_factory=list)
     sort_by: Union[Sort, List[Sort]] = field(default_factory=list)
     group_by: Union[str, List[str]] = field(default_factory=list)
     include_fields: List[str] = field(default_factory=list)
     exclude_fields: List[str] = field(default_factory=list)
     hits_per_page: int = 20
 
     def __build__(self, req: ProtoSearchIndexRequest):
         req.q = self.q or ""
         if self.search_fields:
             req.search_fields.extend(self.search_fields)
         if self.vector_query:
-            req.vector = marshal(self.vector_query.as_obj())
+            req.vector = marshal(self.vector_query.query())
+        if self.filter_by:
+            req.filter = marshal(self.filter_by.query())
         if self.facet_by:
             f = {}
             if isinstance(self.facet_by, str):
-                f[self.facet_by] = FacetSize(self.facet_by).as_obj()
+                f[self.facet_by] = FacetSize(self.facet_by).query()
             elif isinstance(self.facet_by, list):
                 for facet in self.facet_by:
                     if isinstance(facet, str):
-                        f[facet] = FacetSize(facet).as_obj()
+                        f[facet] = FacetSize(facet).query()
                     elif isinstance(facet, FacetSize):
-                        f[facet.field] = facet.as_obj()
+                        f[facet.field] = facet.query()
             req.facet = marshal(f)
         if self.sort_by:
             order = []
             if isinstance(self.sort_by, Sort):
-                order.append(self.sort_by.as_obj())
+                order.append(self.sort_by.query())
             elif isinstance(self.sort_by, list):
-                order = [s.as_obj() for s in self.sort_by]
+                order = [s.query() for s in self.sort_by]
             req.sort = marshal(order)
         if self.group_by:
             g = [self.group_by] if isinstance(self.group_by, str) else self.group_by
             req.group_by = marshal(g)
         if self.include_fields:
             req.include_fields.extend(self.include_fields)
         if self.exclude_fields:
```

### Comparing `tigrisdb-1.0.0b2/PKG-INFO` & `tigrisdb-1.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigrisdb
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Python SDK for Tigris <http://www.tigrisdata.com>
 Home-page: https://www.github.com/tigrisdata/tigris-client-python
 License: Apache-2.0
 Keywords: database,nosql,vector,search
 Author: Tigris team
 Author-email: support@tigrisdata.com
 Requires-Python: >=3.8,<4.0
```

