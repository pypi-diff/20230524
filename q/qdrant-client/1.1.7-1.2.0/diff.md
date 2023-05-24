# Comparing `tmp/qdrant_client-1.1.7.tar.gz` & `tmp/qdrant_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_client-1.1.7.tar", max compression
+gzip compressed data, was "qdrant_client-1.2.0.tar", max compression
```

## Comparing `qdrant_client-1.1.7.tar` & `qdrant_client-1.2.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0    11357 2023-05-09 15:43:22.771894 qdrant_client-1.1.7/LICENSE
--rw-r--r--   0        0        0     6250 2023-05-09 15:43:22.771894 qdrant_client-1.1.7/README.md
--rw-r--r--   0        0        0     1327 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/__init__.py
--rw-r--r--   0        0        0    25845 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/client_base.py
--rw-r--r--   0        0        0     9363 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/connection.py
--rw-r--r--   0        0        0        0 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/conversions/__init__.py
--rw-r--r--   0        0        0     3231 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/conversions/common_types.py
--rw-r--r--   0        0        0    62445 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/conversions/conversion.py
--rw-r--r--   0        0        0      252 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/__init__.py
--rw-r--r--   0        0        0    28633 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/collections_pb2.py
--rw-r--r--   0        0        0      159 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/collections_pb2_grpc.py
--rw-r--r--   0        0        0     1794 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/collections_service_pb2.py
--rw-r--r--   0        0        0    13456 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/collections_service_pb2_grpc.py
--rw-r--r--   0        0        0     3395 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/json_with_int_pb2.py
--rw-r--r--   0        0        0      159 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/json_with_int_pb2_grpc.py
--rw-r--r--   0        0        0    44493 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/points_pb2.py
--rw-r--r--   0        0        0      159 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/points_pb2_grpc.py
--rw-r--r--   0        0        0     2502 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/points_service_pb2.py
--rw-r--r--   0        0        0    23694 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/points_service_pb2_grpc.py
--rw-r--r--   0        0        0     2254 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/qdrant_pb2.py
--rw-r--r--   0        0        0     2411 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/qdrant_pb2_grpc.py
--rw-r--r--   0        0        0     7768 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/snapshots_service_pb2.py
--rw-r--r--   0        0        0    10406 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/snapshots_service_pb2_grpc.py
--rw-r--r--   0        0        0      505 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/http/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/http/api/__init__.py
--rw-r--r--   0        0        0    10437 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api/cluster_api.py
--rw-r--r--   0        0        0    30407 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api/collections_api.py
--rw-r--r--   0        0        0    30820 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api/points_api.py
--rw-r--r--   0        0        0     9499 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api/service_api.py
--rw-r--r--   0        0        0    18850 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api/snapshots_api.py
--rw-r--r--   0        0        0     7577 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api_client.py
--rw-r--r--   0        0        0      233 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/configuration.py
--rw-r--r--   0        0        0     1616 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/exceptions.py
--rw-r--r--   0        0        0       22 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/models/__init__.py
--rw-r--r--   0        0        0    60032 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/models/models.py
--rw-r--r--   0        0        0        0 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/__init__.py
--rw-r--r--   0        0        0     2962 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/distances.py
--rw-r--r--   0        0        0     1446 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/geo.py
--rw-r--r--   0        0        0    21902 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/local_collection.py
--rw-r--r--   0        0        0     5888 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/payload_filters.py
--rw-r--r--   0        0        0     2922 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/payload_value_extractor.py
--rw-r--r--   0        0        0     4388 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/persistence.py
--rw-r--r--   0        0        0    19858 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/qdrant_local.py
--rw-r--r--   0        0        0       40 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/models/__init__.py
--rw-r--r--   0        0        0     7034 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/parallel_processor.py
--rw-r--r--   0        0        0    10979 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/collections.proto
--rw-r--r--   0        0        0     1168 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/collections_service.proto
--rw-r--r--   0        0        0     1936 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/json_with_int.proto
--rw-r--r--   0        0        0    14566 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/points.proto
--rw-r--r--   0        0        0     2196 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/points_service.proto
--rw-r--r--   0        0        0      331 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/qdrant.proto
--rw-r--r--   0        0        0     1895 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/snapshots_service.proto
--rw-r--r--   0        0        0        8 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/py.typed
--rw-r--r--   0        0        0    55103 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/qdrant_client.py
--rw-r--r--   0        0        0    90192 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/qdrant_remote.py
--rw-r--r--   0        0        0        0 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/uploader/__init__.py
--rw-r--r--   0        0        0     2865 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/uploader/grpc_uploader.py
--rw-r--r--   0        0        0     2537 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/uploader/rest_uploader.py
--rw-r--r--   0        0        0     3200 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/uploader/uploader.py
--rw-r--r--   0        0        0      267 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/__init__.py
--rw-r--r--   0        0        0       37 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/api/__init__.py
--rw-r--r--   0        0        0       53 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/api/collections_api.py
--rw-r--r--   0        0        0       48 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/api/points_api.py
--rw-r--r--   0        0        0       44 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/exceptions.py
--rw-r--r--   0        0        0       47 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/models/__init__.py
--rw-r--r--   0        0        0       47 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/models/models.py
--rw-r--r--   0        0        0     7353 1970-01-01 00:00:00.000000 qdrant_client-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 09:08:26.469326 qdrant_client-1.2.0/LICENSE
+-rw-r--r--   0        0        0     6250 2023-05-24 09:08:26.469326 qdrant_client-1.2.0/README.md
+-rw-r--r--   0        0        0     1391 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/__init__.py
+-rw-r--r--   0        0        0     9904 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/client_base.py
+-rw-r--r--   0        0        0     9742 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/connection.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/conversions/__init__.py
+-rw-r--r--   0        0        0     3364 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/conversions/common_types.py
+-rw-r--r--   0        0        0    68611 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/conversions/conversion.py
+-rw-r--r--   0        0        0      252 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/__init__.py
+-rw-r--r--   0        0        0    36463 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/collections_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/collections_pb2_grpc.py
+-rw-r--r--   0        0        0     2063 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/collections_service_pb2.py
+-rw-r--r--   0        0        0    16916 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/collections_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3395 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/json_with_int_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/json_with_int_pb2_grpc.py
+-rw-r--r--   0        0        0    53062 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/points_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/points_pb2_grpc.py
+-rw-r--r--   0        0        0     2907 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/points_service_pb2.py
+-rw-r--r--   0        0        0    30011 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/points_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2254 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/qdrant_pb2.py
+-rw-r--r--   0        0        0     2411 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/qdrant_pb2_grpc.py
+-rw-r--r--   0        0        0     7768 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/snapshots_service_pb2.py
+-rw-r--r--   0        0        0    10406 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/snapshots_service_pb2_grpc.py
+-rw-r--r--   0        0        0      505 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/http/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/__init__.py
+-rw-r--r--   0        0        0    10437 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/cluster_api.py
+-rw-r--r--   0        0        0    30407 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/collections_api.py
+-rw-r--r--   0        0        0    38894 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/points_api.py
+-rw-r--r--   0        0        0     9499 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/service_api.py
+-rw-r--r--   0        0        0    18850 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/snapshots_api.py
+-rw-r--r--   0        0        0     7577 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api_client.py
+-rw-r--r--   0        0        0      233 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/configuration.py
+-rw-r--r--   0        0        0     1616 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/exceptions.py
+-rw-r--r--   0        0        0       22 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/models/__init__.py
+-rw-r--r--   0        0        0    66445 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/models/models.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/__init__.py
+-rw-r--r--   0        0        0     2979 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/distances.py
+-rw-r--r--   0        0        0     1446 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/geo.py
+-rw-r--r--   0        0        0    28665 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/local_collection.py
+-rw-r--r--   0        0        0     6371 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/payload_filters.py
+-rw-r--r--   0        0        0     2922 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/payload_value_extractor.py
+-rw-r--r--   0        0        0     4388 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/persistence.py
+-rw-r--r--   0        0        0    23078 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/qdrant_local.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/tests/__init__.py
+-rw-r--r--   0        0        0     4210 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/tests/test_payload_filters.py
+-rw-r--r--   0        0        0       40 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/models/__init__.py
+-rw-r--r--   0        0        0     7034 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/parallel_processor.py
+-rw-r--r--   0        0        0    13716 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/collections.proto
+-rw-r--r--   0        0        0     1496 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/collections_service.proto
+-rw-r--r--   0        0        0     1936 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/json_with_int.proto
+-rw-r--r--   0        0        0    18788 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/points.proto
+-rw-r--r--   0        0        0     2873 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/points_service.proto
+-rw-r--r--   0        0        0      331 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/qdrant.proto
+-rw-r--r--   0        0        0     1895 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/snapshots_service.proto
+-rw-r--r--   0        0        0        8 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/py.typed
+-rw-r--r--   0        0        0    67758 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/qdrant_client.py
+-rw-r--r--   0        0        0    70630 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/qdrant_remote.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/uploader/__init__.py
+-rw-r--r--   0        0        0     2919 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/uploader/grpc_uploader.py
+-rw-r--r--   0        0        0     2567 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/uploader/rest_uploader.py
+-rw-r--r--   0        0        0     3200 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/uploader/uploader.py
+-rw-r--r--   0        0        0      267 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/api/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/api/collections_api.py
+-rw-r--r--   0        0        0       48 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/api/points_api.py
+-rw-r--r--   0        0        0       44 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/exceptions.py
+-rw-r--r--   0        0        0       47 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/models/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/models/models.py
+-rw-r--r--   0        0        0     7353 1970-01-01 00:00:00.000000 qdrant_client-1.2.0/PKG-INFO
```

### Comparing `qdrant_client-1.1.7/LICENSE` & `qdrant_client-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/README.md` & `qdrant_client-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/pyproject.toml` & `qdrant_client-1.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qdrant-client"
-version = "1.1.7"
+version = "1.2.0"
 description = "Client library for the Qdrant vector search engine"
 authors = ["Andrey Vasnetsov <andrey@qdrant.tech>"]
 packages = [
     {include = "qdrant_client"},
     {include = "qdrant_openapi_client"}
 ]
 readme = "README.md"
@@ -16,15 +16,15 @@
 python = ">=3.7,<3.12"
 httpx = { version = ">=0.14.0", extras = ["http2"] }
 numpy = [
     { version = "<1.21", python = "<3.8" },
     { version = ">=1.21", python = ">=3.8" }
 ]
 pydantic = "^1.8"
-typing-extensions = "^4.0.0"
+typing-extensions = ">=4.0.0,<4.6.0"  # at the moment 4.6.0 breaks support for python3.8,3.9
 grpcio = { version = ">=1.41.0", allow-prereleases = true }
 grpcio-tools = ">=1.41.0"
 urllib3 = "^1.26.14"
 portalocker = "^2.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1"
```

### Comparing `qdrant_client-1.1.7/qdrant_client/connection.py` & `qdrant_client-1.2.0/qdrant_client/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,17 @@
         return postprocess(response_it) if postprocess else response_it
 
 
 def create_generic_client_interceptor(intercept_call: Any) -> _GenericClientInterceptor:
     return _GenericClientInterceptor(intercept_call)
 
 
-def create_generic_async_client_interceptor(intercept_call: Any) -> _GenericAsyncClientInterceptor:
+def create_generic_async_client_interceptor(
+    intercept_call: Any,
+) -> _GenericAsyncClientInterceptor:
     return _GenericAsyncClientInterceptor(intercept_call)
 
 
 # Source:
 # <https://github.com/grpc/grpc/blob/master/examples/python/interceptors/headers/header_manipulator_client_interceptor.py>
 class _ClientCallDetails(
     collections.namedtuple("_ClientCallDetails", ("method", "timeout", "metadata", "credentials")),
@@ -175,14 +177,20 @@
 
     return create_generic_async_client_interceptor(intercept_call)
 
 
 def get_channel(
     host: str, port: int, ssl: bool, metadata: Optional[List[Tuple[str, str]]] = None
 ) -> grpc.Channel:
+    # gRPC client options
+    options = [
+        ("grpc.max_send_message_length", -1),
+        ("grpc.max_receive_message_length", -1),
+    ]
+
     if ssl:
         if metadata:
 
             def metadata_callback(context: Any, callback: Any) -> None:
                 # for more info see grpc docs
                 callback(metadata, None)
 
@@ -195,27 +203,33 @@
             # combine the cert credentials and the macaroon auth credentials
             # such that every call is properly encrypted and authenticated
             creds = grpc.composite_channel_credentials(cert_creds, auth_creds)
         else:
             creds = grpc.ssl_channel_credentials()
 
         # finally pass in the combined credentials when creating a channel
-        return grpc.secure_channel(f"{host}:{port}", creds)
+        return grpc.secure_channel(f"{host}:{port}", creds, options)
     else:
         if metadata:
             metadata_interceptor = header_adder_interceptor(metadata)
-            channel = grpc.insecure_channel(f"{host}:{port}", metadata)
+            channel = grpc.insecure_channel(f"{host}:{port}", metadata, options)
             return grpc.intercept_channel(channel, metadata_interceptor)
         else:
-            return grpc.insecure_channel(f"{host}:{port}")
+            return grpc.insecure_channel(f"{host}:{port}", options)
 
 
 def get_async_channel(
     host: str, port: int, ssl: bool, metadata: Optional[List[Tuple[str, str]]] = None
 ) -> grpc.aio.Channel:
+    # gRPC client options
+    options = [
+        ("grpc.max_send_message_length", -1),
+        ("grpc.max_receive_message_length", -1),
+    ]
+
     if ssl:
         if metadata:
 
             def metadata_callback(context: Any, callback: Any) -> None:
                 # for more info see grpc docs
                 callback(metadata, None)
 
@@ -228,14 +242,16 @@
             # combine the cert credentials and the macaroon auth credentials
             # such that every call is properly encrypted and authenticated
             creds = grpc.composite_channel_credentials(cert_creds, auth_creds)
         else:
             creds = grpc.ssl_channel_credentials()
 
         # finally pass in the combined credentials when creating a channel
-        return grpc.aio.secure_channel(f"{host}:{port}", creds)
+        return grpc.aio.secure_channel(f"{host}:{port}", creds, options)
     else:
         if metadata:
             metadata_interceptor = header_adder_async_interceptor(metadata)
-            return grpc.aio.insecure_channel(f"{host}:{port}", interceptors=[metadata_interceptor])
+            return grpc.aio.insecure_channel(
+                f"{host}:{port}", options, interceptors=[metadata_interceptor]
+            )
         else:
-            return grpc.aio.insecure_channel(f"{host}:{port}")
+            return grpc.aio.insecure_channel(f"{host}:{port}", options)
```

### Comparing `qdrant_client-1.1.7/qdrant_client/conversions/common_types.py` & `qdrant_client-1.2.0/qdrant_client/conversions/common_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,26 +43,30 @@
 UpdateResult: TypeAlias = rest.UpdateResult
 Record: TypeAlias = rest.Record
 CollectionsResponse: TypeAlias = rest.CollectionsResponse
 CollectionInfo: TypeAlias = rest.CollectionInfo
 CountResult: TypeAlias = rest.CountResult
 SnapshotDescription: TypeAlias = rest.SnapshotDescription
 NamedVector: TypeAlias = rest.NamedVector
+PointVectors: TypeAlias = rest.PointVectors
+VectorStruct: TypeAlias = rest.VectorStruct
 VectorParams: TypeAlias = rest.VectorParams
 LocksOption: TypeAlias = rest.LocksOption
 SnapshotPriority: TypeAlias = rest.SnapshotPriority
 CollectionsAliasesResponse: TypeAlias = rest.CollectionsAliasesResponse
 InitFrom: TypeAlias = rest.InitFrom
 
 SearchRequest = Union[rest.SearchRequest, grpc.SearchPoints]
 RecommendRequest = Union[rest.RecommendRequest, grpc.RecommendPoints]
 
 ReadConsistency: TypeAlias = rest.ReadConsistency
 WriteOrdering: TypeAlias = rest.WriteOrdering
 
+GroupsResult: TypeAlias = rest.GroupsResult
+
 # we can't use `nptyping` package due to numpy/python-version incompatibilities
 # thus we need to define precise type annotations while we support python3.7
 _np_numeric = Union[
     np.bool_,  # pylance can't handle np.bool8 alias
     np.int8,
     np.int16,
     np.int32,
```

### Comparing `qdrant_client-1.1.7/qdrant_client/conversions/conversion.py` & `qdrant_client-1.2.0/qdrant_client/conversions/conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,16 @@
             return cls.convert_filter(val)
         if name == "has_id":
             return cls.convert_has_id_condition(val)
         if name == "is_empty":
             return cls.convert_is_empty_condition(val)
         if name == "is_null":
             return cls.convert_is_null_condition(val)
+        if name == "nested":
+            return cls.convert_nested_condition(val)
 
         raise ValueError(f"invalid Condition model: {model}")  # pragma: no cover
 
     @classmethod
     def convert_filter(cls, model: grpc.Filter) -> rest.Filter:
         return rest.Filter(
             must=[cls.convert_condition(condition) for condition in model.must],
@@ -269,15 +271,16 @@
             return rest.CollectionStatus.RED
         else:
             raise ValueError(f"invalid CollectionStatus model: {model}")  # pragma: no cover
 
     @classmethod
     def convert_update_result(cls, model: grpc.UpdateResult) -> rest.UpdateResult:
         return rest.UpdateResult(
-            operation_id=model.operation_id, status=cls.convert_update_status(model.status)
+            operation_id=model.operation_id,
+            status=cls.convert_update_status(model.status),
         )
 
     @classmethod
     def convert_update_status(cls, model: grpc.UpdateStatus) -> rest.UpdateStatus:
         if model == grpc.UpdateStatus.Acknowledged:
             return rest.UpdateStatus.ACKNOWLEDGED
         elif model == grpc.UpdateStatus.Completed:
@@ -314,14 +317,23 @@
         return rest.IsEmptyCondition(is_empty=rest.PayloadField(key=model.key))
 
     @classmethod
     def convert_is_null_condition(cls, model: grpc.IsNullCondition) -> rest.IsNullCondition:
         return rest.IsNullCondition(is_null=rest.PayloadField(key=model.key))
 
     @classmethod
+    def convert_nested_condition(cls, model: grpc.NestedCondition) -> rest.NestedCondition:
+        return rest.NestedCondition(
+            nested=rest.Nested(
+                key=model.key,
+                filter=cls.convert_filter(model.filter),
+            )
+        )
+
+    @classmethod
     def convert_search_params(cls, model: grpc.SearchParams) -> rest.SearchParams:
         return rest.SearchParams(
             hnsw_ef=model.hnsw_ef if model.HasField("hnsw_ef") else None,
             exact=model.exact if model.HasField("exact") else None,
             quantization=cls.convert_quantization_search_params(model.quantization)
             if model.HasField("quantization")
             else None,
@@ -424,14 +436,18 @@
             return rest.MatchValue(value=val)
         if name == "text":
             return rest.MatchText(text=val)
         if name == "keywords":
             return rest.MatchAny(any=list(val.strings))
         if name == "integers":
             return rest.MatchAny(any=list(val.integers))
+        if name == "except_keywords":
+            return rest.MatchExcept(**{"except": list(val.strings)})
+        if name == "except_integers":
+            return rest.MatchExcept(**{"except": list(val.integers)})
         raise ValueError(f"invalid Match model: {model}")  # pragma: no cover
 
     @classmethod
     def convert_wal_config_diff(cls, model: grpc.WalConfigDiff) -> rest.WalConfigDiff:
         return rest.WalConfigDiff(
             wal_capacity_mb=model.wal_capacity_mb if model.HasField("wal_capacity_mb") else None,
             wal_segments_ahead=model.wal_segments_ahead
@@ -583,14 +599,15 @@
             distance=cls.convert_distance(model.distance),
             hnsw_config=cls.convert_hnsw_config_diff(model.hnsw_config)
             if model.HasField("hnsw_config")
             else None,
             quantization_config=cls.convert_quantization_config(model.quantization_config)
             if model.HasField("quantization_config")
             else None,
+            on_disk=model.on_disk if model.HasField("on_disk") else None,
         )
 
     @classmethod
     def convert_vectors_config(cls, model: grpc.VectorsConfig) -> rest.VectorsConfig:
         name = model.WhichOneof("config")
         val = getattr(model, name)
 
@@ -752,32 +769,83 @@
         return rest.ScalarQuantizationConfig(
             type=rest.ScalarType.INT8,
             quantile=model.quantile if model.HasField("quantile") else None,
             always_ram=model.always_ram if model.HasField("always_ram") else None,
         )
 
     @classmethod
+    def convert_product_quantization_config(
+        cls, model: grpc.ProductQuantization
+    ) -> rest.ProductQuantizationConfig:
+        return rest.ProductQuantizationConfig(
+            compression=cls.convert_compression_ratio(model.compression),
+            always_ram=model.always_ram if model.HasField("always_ram") else None,
+        )
+
+    @classmethod
+    def convert_compression_ratio(cls, model: grpc.CompressionRatio) -> rest.CompressionRatio:
+        if model == grpc.x4:
+            return rest.CompressionRatio.X4
+        if model == grpc.x8:
+            return rest.CompressionRatio.X8
+        if model == grpc.x16:
+            return rest.CompressionRatio.X16
+        if model == grpc.x32:
+            return rest.CompressionRatio.X32
+        if model == grpc.x64:
+            return rest.CompressionRatio.X64
+        raise ValueError(f"invalid CompressionRatio model: {model}")  # pragma: no cover
+
+    @classmethod
     def convert_quantization_config(
         cls, model: grpc.QuantizationConfig
     ) -> rest.QuantizationConfig:
         name = model.WhichOneof("quantization")
         val = getattr(model, name)
         if name == "scalar":
             return rest.ScalarQuantization(scalar=cls.convert_scalar_quantization_config(val))
+        if name == "product":
+            return rest.ProductQuantization(product=cls.convert_product_quantization_config(val))
         raise ValueError(f"invalid QuantizationConfig model: {model}")  # pragma: no cover
 
     @classmethod
     def convert_quantization_search_params(
         cls, model: grpc.QuantizationSearchParams
     ) -> rest.QuantizationSearchParams:
         return rest.QuantizationSearchParams(
             ignore=model.ignore if model.HasField("ignore") else None,
             rescore=model.rescore if model.HasField("rescore") else None,
         )
 
+    @classmethod
+    def convert_point_vectors(cls, model: grpc.PointVectors) -> rest.PointVectors:
+        return rest.PointVectors(
+            id=cls.convert_point_id(model.id),
+            vector=cls.convert_vectors(model.vectors),
+        )
+
+    @classmethod
+    def convert_groups_result(cls, model: grpc.GroupsResult) -> rest.GroupsResult:
+        return rest.GroupsResult(
+            groups=[cls.convert_group(group) for group in model.groups],
+        )
+
+    @classmethod
+    def convert_group(cls, model: grpc.PointGroup) -> rest.PointGroup:
+        return rest.PointGroup(
+            id=cls.convert_group_id(model.id),
+            hits=[cls.convert_scored_point(hit) for hit in model.hits],
+        )
+
+    @classmethod
+    def convert_group_id(cls, model: grpc.GroupId) -> rest.GroupId:
+        name = model.WhichOneof("kind")
+        val = getattr(model, name)
+        return val
+
 
 # ----------------------------------------
 #
 # ----------- REST TO gRPC ---------------
 #
 # ----------------------------------------
 
@@ -873,15 +941,16 @@
             return grpc.PayloadSchemaType.Geo
 
         raise ValueError(f"invalid PayloadSchemaType model: {model}")  # pragma: no cover
 
     @classmethod
     def convert_update_result(cls, model: rest.UpdateResult) -> grpc.UpdateResult:
         return grpc.UpdateResult(
-            operation_id=model.operation_id, status=cls.convert_update_stats(model.status)
+            operation_id=model.operation_id,
+            status=cls.convert_update_stats(model.status),
         )
 
     @classmethod
     def convert_update_stats(cls, model: rest.UpdateStatus) -> grpc.UpdateStatus:
         if model == rest.UpdateStatus.COMPLETED:
             return grpc.UpdateStatus.Completed
         if model == rest.UpdateStatus.ACKNOWLEDGED:
@@ -910,14 +979,21 @@
         return grpc.IsEmptyCondition(key=model.is_empty.key)
 
     @classmethod
     def convert_is_null_condition(cls, model: rest.IsNullCondition) -> grpc.IsNullCondition:
         return grpc.IsNullCondition(key=model.is_null.key)
 
     @classmethod
+    def convert_nested_condition(cls, model: rest.NestedCondition) -> grpc.NestedCondition:
+        return grpc.NestedCondition(
+            key=model.nested.key,
+            filter=cls.convert_filter(model.nested.filter),
+        )
+
+    @classmethod
     def convert_search_params(cls, model: rest.SearchParams) -> grpc.SearchParams:
         return grpc.SearchParams(
             hnsw_ef=model.hnsw_ef,
             exact=model.exact,
             quantization=cls.convert_quantization_search_params(model.quantization)
             if model.quantization is not None
             else None,
@@ -1020,15 +1096,16 @@
                 key=model.key, values_count=cls.convert_values_count(model.values_count)
             )
         raise ValueError(f"invalid FieldCondition model: {model}")  # pragma: no cover
 
     @classmethod
     def convert_wal_config_diff(cls, model: rest.WalConfigDiff) -> grpc.WalConfigDiff:
         return grpc.WalConfigDiff(
-            wal_capacity_mb=model.wal_capacity_mb, wal_segments_ahead=model.wal_segments_ahead
+            wal_capacity_mb=model.wal_capacity_mb,
+            wal_segments_ahead=model.wal_segments_ahead,
         )
 
     @classmethod
     def convert_collection_config(cls, model: rest.CollectionConfig) -> grpc.CollectionConfig:
         return grpc.CollectionConfig(
             params=cls.convert_collection_params(model.params),
             hnsw_config=cls.convert_hnsw_config(model.hnsw_config),
@@ -1049,15 +1126,16 @@
             on_disk=model.on_disk,
             payload_m=model.payload_m,
         )
 
     @classmethod
     def convert_wal_config(cls, model: rest.WalConfig) -> grpc.WalConfigDiff:
         return grpc.WalConfigDiff(
-            wal_capacity_mb=model.wal_capacity_mb, wal_segments_ahead=model.wal_segments_ahead
+            wal_capacity_mb=model.wal_capacity_mb,
+            wal_segments_ahead=model.wal_segments_ahead,
         )
 
     @classmethod
     def convert_distance(cls, model: rest.Distance) -> grpc.Distance:
         if model == rest.Distance.DOT:
             return grpc.Distance.Dot
         if model == rest.Distance.COSINE:
@@ -1131,20 +1209,28 @@
                 return grpc.Match(integer=model.value)
             if isinstance(model.value, str):
                 return grpc.Match(keyword=model.value)
         if isinstance(model, rest.MatchText):
             return grpc.Match(text=model.text)
         if isinstance(model, rest.MatchAny):
             if len(model.any) == 0:
-                return grpc.Match(keywords=[])
+                return grpc.Match(keywords=grpc.RepeatedStrings(strings=[]))
             if isinstance(model.any[0], str):
                 return grpc.Match(keywords=grpc.RepeatedStrings(strings=model.any))
             if isinstance(model.any[0], int):
                 return grpc.Match(integers=grpc.RepeatedIntegers(integers=model.any))
             raise ValueError(f"invalid MatchAny model: {model}")  # pragma: no cover
+        if isinstance(model, rest.MatchExcept):
+            if len(model.except_) == 0:
+                return grpc.Match(except_keywords=grpc.RepeatedStrings(strings=[]))
+            if isinstance(model.except_[0], str):
+                return grpc.Match(except_keywords=grpc.RepeatedStrings(strings=model.except_))
+            if isinstance(model.except_[0], int):
+                return grpc.Match(except_integers=grpc.RepeatedIntegers(integers=model.except_))
+            raise ValueError(f"invalid MatchExcept model: {model}")  # pragma: no cover
 
         raise ValueError(f"invalid Match model: {model}")  # pragma: no cover
 
     @classmethod
     def convert_alias_operations(cls, model: rest.AliasOperations) -> grpc.AliasOperations:
         if isinstance(model, rest.CreateAliasOperation):
             return grpc.AliasOperations(create_alias=cls.convert_create_alias(model.create_alias))
@@ -1183,14 +1269,16 @@
             return grpc.Condition(is_empty=cls.convert_is_empty_condition(model))
         if isinstance(model, rest.IsNullCondition):
             return grpc.Condition(is_null=cls.convert_is_null_condition(model))
         if isinstance(model, rest.HasIdCondition):
             return grpc.Condition(has_id=cls.convert_has_id_condition(model))
         if isinstance(model, rest.Filter):
             return grpc.Condition(filter=cls.convert_filter(model))
+        if isinstance(model, rest.NestedCondition):
+            return grpc.Condition(nested=cls.convert_nested_condition(model))
 
         raise ValueError(f"invalid Condition model: {model}")  # pragma: no cover
 
     @classmethod
     def convert_payload_selector(cls, model: rest.PayloadSelector) -> grpc.WithPayloadSelector:
         if isinstance(model, rest.PayloadSelectorInclude):
             return grpc.WithPayloadSelector(
@@ -1262,14 +1350,15 @@
             distance=cls.convert_distance(model.distance),
             hnsw_config=cls.convert_hnsw_config_diff(model.hnsw_config)
             if model.hnsw_config is not None
             else None,
             quantization_config=cls.convert_quantization_config(model.quantization_config)
             if model.quantization_config is not None
             else None,
+            on_disk=model.on_disk,
         )
 
     @classmethod
     def convert_vectors_config(cls, model: rest.VectorsConfig) -> grpc.VectorsConfig:
         if isinstance(model, rest.VectorParams):
             return grpc.VectorsConfig(params=cls.convert_vector_params(model))
         elif isinstance(model, dict):
@@ -1471,25 +1560,91 @@
         return grpc.ScalarQuantization(
             type=grpc.QuantizationType.Int8,
             quantile=model.quantile,
             always_ram=model.always_ram,
         )
 
     @classmethod
+    def convert_product_quantization_config(
+        cls, model: rest.ProductQuantizationConfig
+    ) -> grpc.ProductQuantization:
+        return grpc.ProductQuantization(
+            compression=cls.convert_compression_ratio(model.compression),
+            always_ram=model.always_ram,
+        )
+
+    @classmethod
+    def convert_compression_ratio(cls, model: rest.CompressionRatio) -> grpc.CompressionRatio:
+        if model == rest.CompressionRatio.X4:
+            return grpc.CompressionRatio.x4
+        elif model == rest.CompressionRatio.X8:
+            return grpc.CompressionRatio.x8
+        elif model == rest.CompressionRatio.X16:
+            return grpc.CompressionRatio.x16
+        elif model == rest.CompressionRatio.X32:
+            return grpc.CompressionRatio.x32
+        elif model == rest.CompressionRatio.X64:
+            return grpc.CompressionRatio.x64
+        else:
+            raise ValueError(f"invalid CompressionRatio model: {model}")  # pragma: no cover
+
+    @classmethod
     def convert_quantization_config(
         cls, model: rest.QuantizationConfig
     ) -> grpc.QuantizationConfig:
         if isinstance(model, rest.ScalarQuantization):
             return grpc.QuantizationConfig(
                 scalar=cls.convert_scalar_quantization_config(model.scalar)
             )
+        if isinstance(model, rest.ProductQuantization):
+            return grpc.QuantizationConfig(
+                product=cls.convert_product_quantization_config(model.product)
+            )
         else:
             raise ValueError(f"invalid QuantizationConfig model: {model}")
 
     @classmethod
     def convert_quantization_search_params(
         cls, model: rest.QuantizationSearchParams
     ) -> grpc.QuantizationSearchParams:
         return grpc.QuantizationSearchParams(
             ignore=model.ignore,
             rescore=model.rescore,
         )
+
+    @classmethod
+    def convert_point_vectors(cls, model: rest.PointVectors) -> grpc.PointVectors:
+        return grpc.PointVectors(
+            id=cls.convert_extended_point_id(model.id),
+            vectors=cls.convert_vector_struct(model.vector),
+        )
+
+    @classmethod
+    def convert_groups_result(cls, model: rest.GroupsResult) -> grpc.GroupsResult:
+        return grpc.GroupsResult(
+            groups=[cls.convert_point_group(group) for group in model.groups],
+        )
+
+    @classmethod
+    def convert_point_group(cls, model: rest.PointGroup) -> grpc.PointGroup:
+        return grpc.PointGroup(
+            id=cls.convert_group_id(model.id),
+            hits=[cls.convert_scored_point(point) for point in model.hits],
+        )
+
+    @classmethod
+    def convert_group_id(cls, model: rest.GroupId) -> grpc.GroupId:
+        if isinstance(model, str):
+            return grpc.GroupId(
+                string_value=model,
+            )
+        elif isinstance(model, int):
+            if model >= 0:
+                return grpc.GroupId(
+                    unsigned_value=model,
+                )
+            else:
+                return grpc.GroupId(
+                    integer_value=model,
+                )
+        else:
+            raise ValueError(f"invalid GroupId model: {model}")
```

### Comparing `qdrant_client-1.1.7/qdrant_client/grpc/collections_pb2.py` & `qdrant_client-1.2.0/qdrant_client/grpc/collections_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x63ollections.proto\x12\x06qdrant\"\xd8\x01\n\x0cVectorParams\x12\x0c\n\x04size\x18\x01 \x01(\x04\x12\"\n\x08\x64istance\x18\x02 \x01(\x0e\x32\x10.qdrant.Distance\x12\x30\n\x0bhnsw_config\x18\x03 \x01(\x0b\x32\x16.qdrant.HnswConfigDiffH\x00\x88\x01\x01\x12<\n\x13quantization_config\x18\x04 \x01(\x0b\x32\x1a.qdrant.QuantizationConfigH\x01\x88\x01\x01\x42\x0e\n\x0c_hnsw_configB\x16\n\x14_quantization_config\"\x82\x01\n\x0fVectorParamsMap\x12-\n\x03map\x18\x01 \x03(\x0b\x32 .qdrant.VectorParamsMap.MapEntry\x1a@\n\x08MapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.qdrant.VectorParams:\x02\x38\x01\"p\n\rVectorsConfig\x12&\n\x06params\x18\x01 \x01(\x0b\x32\x14.qdrant.VectorParamsH\x00\x12-\n\nparams_map\x18\x02 \x01(\x0b\x32\x17.qdrant.VectorParamsMapH\x00\x42\x08\n\x06\x63onfig\"3\n\x18GetCollectionInfoRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"\x18\n\x16ListCollectionsRequest\"%\n\x15\x43ollectionDescription\x12\x0c\n\x04name\x18\x01 \x01(\t\"Q\n\x19GetCollectionInfoResponse\x12&\n\x06result\x18\x01 \x01(\x0b\x32\x16.qdrant.CollectionInfo\x12\x0c\n\x04time\x18\x02 \x01(\x01\"[\n\x17ListCollectionsResponse\x12\x32\n\x0b\x63ollections\x18\x01 \x03(\x0b\x32\x1d.qdrant.CollectionDescription\x12\x0c\n\x04time\x18\x02 \x01(\x01\",\n\x0fOptimizerStatus\x12\n\n\x02ok\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"\x90\x02\n\x0eHnswConfigDiff\x12\x0e\n\x01m\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x19\n\x0c\x65\x66_construct\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12 \n\x13\x66ull_scan_threshold\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12!\n\x14max_indexing_threads\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x14\n\x07on_disk\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12\x16\n\tpayload_m\x18\x06 \x01(\x04H\x05\x88\x01\x01\x42\x04\n\x02_mB\x0f\n\r_ef_constructB\x16\n\x14_full_scan_thresholdB\x17\n\x15_max_indexing_threadsB\n\n\x08_on_diskB\x0c\n\n_payload_m\"y\n\rWalConfigDiff\x12\x1c\n\x0fwal_capacity_mb\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x1f\n\x12wal_segments_ahead\x18\x02 \x01(\x04H\x01\x88\x01\x01\x42\x12\n\x10_wal_capacity_mbB\x15\n\x13_wal_segments_ahead\"\xec\x03\n\x14OptimizersConfigDiff\x12\x1e\n\x11\x64\x65leted_threshold\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12%\n\x18vacuum_min_vector_number\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12#\n\x16\x64\x65\x66\x61ult_segment_number\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x1d\n\x10max_segment_size\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x1d\n\x10memmap_threshold\x18\x05 \x01(\x04H\x04\x88\x01\x01\x12\x1f\n\x12indexing_threshold\x18\x06 \x01(\x04H\x05\x88\x01\x01\x12\x1f\n\x12\x66lush_interval_sec\x18\x07 \x01(\x04H\x06\x88\x01\x01\x12%\n\x18max_optimization_threads\x18\x08 \x01(\x04H\x07\x88\x01\x01\x42\x14\n\x12_deleted_thresholdB\x1b\n\x19_vacuum_min_vector_numberB\x19\n\x17_default_segment_numberB\x13\n\x11_max_segment_sizeB\x13\n\x11_memmap_thresholdB\x15\n\x13_indexing_thresholdB\x15\n\x13_flush_interval_secB\x1b\n\x19_max_optimization_threads\"\x88\x01\n\x12ScalarQuantization\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.qdrant.QuantizationType\x12\x15\n\x08quantile\x18\x02 \x01(\x02H\x00\x88\x01\x01\x12\x17\n\nalways_ram\x18\x03 \x01(\x08H\x01\x88\x01\x01\x42\x0b\n\t_quantileB\r\n\x0b_always_ram\"R\n\x12QuantizationConfig\x12,\n\x06scalar\x18\x01 \x01(\x0b\x32\x1a.qdrant.ScalarQuantizationH\x00\x42\x0e\n\x0cquantization\"\xe1\x05\n\x10\x43reateCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x30\n\x0bhnsw_config\x18\x04 \x01(\x0b\x32\x16.qdrant.HnswConfigDiffH\x00\x88\x01\x01\x12.\n\nwal_config\x18\x05 \x01(\x0b\x32\x15.qdrant.WalConfigDiffH\x01\x88\x01\x01\x12<\n\x11optimizers_config\x18\x06 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiffH\x02\x88\x01\x01\x12\x19\n\x0cshard_number\x18\x07 \x01(\rH\x03\x88\x01\x01\x12\x1c\n\x0fon_disk_payload\x18\x08 \x01(\x08H\x04\x88\x01\x01\x12\x14\n\x07timeout\x18\t \x01(\x04H\x05\x88\x01\x01\x12\x32\n\x0evectors_config\x18\n \x01(\x0b\x32\x15.qdrant.VectorsConfigH\x06\x88\x01\x01\x12\x1f\n\x12replication_factor\x18\x0b \x01(\rH\x07\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x0c \x01(\rH\x08\x88\x01\x01\x12!\n\x14init_from_collection\x18\r \x01(\tH\t\x88\x01\x01\x12<\n\x13quantization_config\x18\x0e \x01(\x0b\x32\x1a.qdrant.QuantizationConfigH\n\x88\x01\x01\x42\x0e\n\x0c_hnsw_configB\r\n\x0b_wal_configB\x14\n\x12_optimizers_configB\x0f\n\r_shard_numberB\x12\n\x10_on_disk_payloadB\n\n\x08_timeoutB\x11\n\x0f_vectors_configB\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factorB\x17\n\x15_init_from_collectionB\x16\n\x14_quantization_configJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"\xdf\x01\n\x10UpdateCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12<\n\x11optimizers_config\x18\x02 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiffH\x00\x88\x01\x01\x12\x14\n\x07timeout\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x31\n\x06params\x18\x04 \x01(\x0b\x32\x1c.qdrant.CollectionParamsDiffH\x02\x88\x01\x01\x42\x14\n\x12_optimizers_configB\n\n\x08_timeoutB\t\n\x07_params\"M\n\x10\x44\x65leteCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x14\n\x07timeout\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\n\n\x08_timeout\";\n\x1b\x43ollectionOperationResponse\x12\x0e\n\x06result\x18\x01 \x01(\x08\x12\x0c\n\x04time\x18\x02 \x01(\x01\"\x90\x02\n\x10\x43ollectionParams\x12\x14\n\x0cshard_number\x18\x03 \x01(\r\x12\x17\n\x0fon_disk_payload\x18\x04 \x01(\x08\x12\x32\n\x0evectors_config\x18\x05 \x01(\x0b\x32\x15.qdrant.VectorsConfigH\x00\x88\x01\x01\x12\x1f\n\x12replication_factor\x18\x06 \x01(\rH\x01\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x07 \x01(\rH\x02\x88\x01\x01\x42\x11\n\x0f_vectors_configB\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factorJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x92\x01\n\x14\x43ollectionParamsDiff\x12\x1f\n\x12replication_factor\x18\x01 \x01(\rH\x00\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x02 \x01(\rH\x01\x88\x01\x01\x42\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factor\"\xa2\x02\n\x10\x43ollectionConfig\x12(\n\x06params\x18\x01 \x01(\x0b\x32\x18.qdrant.CollectionParams\x12+\n\x0bhnsw_config\x18\x02 \x01(\x0b\x32\x16.qdrant.HnswConfigDiff\x12\x36\n\x10optimizer_config\x18\x03 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiff\x12)\n\nwal_config\x18\x04 \x01(\x0b\x32\x15.qdrant.WalConfigDiff\x12<\n\x13quantization_config\x18\x05 \x01(\x0b\x32\x1a.qdrant.QuantizationConfigH\x00\x88\x01\x01\x42\x16\n\x14_quantization_config\"\xbd\x01\n\x0fTextIndexParams\x12(\n\ttokenizer\x18\x01 \x01(\x0e\x32\x15.qdrant.TokenizerType\x12\x16\n\tlowercase\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1a\n\rmin_token_len\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x1a\n\rmax_token_len\x18\x04 \x01(\x04H\x02\x88\x01\x01\x42\x0c\n\n_lowercaseB\x10\n\x0e_min_token_lenB\x10\n\x0e_max_token_len\"Z\n\x12PayloadIndexParams\x12\x34\n\x11text_index_params\x18\x01 \x01(\x0b\x32\x17.qdrant.TextIndexParamsH\x00\x42\x0e\n\x0cindex_params\"\x9d\x01\n\x11PayloadSchemaInfo\x12,\n\tdata_type\x18\x01 \x01(\x0e\x32\x19.qdrant.PayloadSchemaType\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1a.qdrant.PayloadIndexParamsH\x00\x88\x01\x01\x12\x13\n\x06points\x18\x03 \x01(\x04H\x01\x88\x01\x01\x42\t\n\x07_paramsB\t\n\x07_points\"\xba\x03\n\x0e\x43ollectionInfo\x12(\n\x06status\x18\x01 \x01(\x0e\x32\x18.qdrant.CollectionStatus\x12\x31\n\x10optimizer_status\x18\x02 \x01(\x0b\x32\x17.qdrant.OptimizerStatus\x12\x15\n\rvectors_count\x18\x03 \x01(\x04\x12\x16\n\x0esegments_count\x18\x04 \x01(\x04\x12(\n\x06\x63onfig\x18\x07 \x01(\x0b\x32\x18.qdrant.CollectionConfig\x12\x41\n\x0epayload_schema\x18\x08 \x03(\x0b\x32).qdrant.CollectionInfo.PayloadSchemaEntry\x12\x14\n\x0cpoints_count\x18\t \x01(\x04\x12\"\n\x15indexed_vectors_count\x18\n \x01(\x04H\x00\x88\x01\x01\x1aO\n\x12PayloadSchemaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.qdrant.PayloadSchemaInfo:\x02\x38\x01\x42\x18\n\x16_indexed_vectors_countJ\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"[\n\rChangeAliases\x12(\n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x17.qdrant.AliasOperations\x12\x14\n\x07timeout\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\n\n\x08_timeout\"\xa2\x01\n\x0f\x41liasOperations\x12+\n\x0c\x63reate_alias\x18\x01 \x01(\x0b\x32\x13.qdrant.CreateAliasH\x00\x12+\n\x0crename_alias\x18\x02 \x01(\x0b\x32\x13.qdrant.RenameAliasH\x00\x12+\n\x0c\x64\x65lete_alias\x18\x03 \x01(\x0b\x32\x13.qdrant.DeleteAliasH\x00\x42\x08\n\x06\x61\x63tion\":\n\x0b\x43reateAlias\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nalias_name\x18\x02 \x01(\t\"=\n\x0bRenameAlias\x12\x16\n\x0eold_alias_name\x18\x01 \x01(\t\x12\x16\n\x0enew_alias_name\x18\x02 \x01(\t\"!\n\x0b\x44\x65leteAlias\x12\x12\n\nalias_name\x18\x01 \x01(\t\"\x14\n\x12ListAliasesRequest\"7\n\x1cListCollectionAliasesRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"?\n\x10\x41liasDescription\x12\x12\n\nalias_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\"N\n\x13ListAliasesResponse\x12)\n\x07\x61liases\x18\x01 \x03(\x0b\x32\x18.qdrant.AliasDescription\x12\x0c\n\x04time\x18\x02 \x01(\x01*@\n\x08\x44istance\x12\x13\n\x0fUnknownDistance\x10\x00\x12\n\n\x06\x43osine\x10\x01\x12\n\n\x06\x45uclid\x10\x02\x12\x07\n\x03\x44ot\x10\x03*O\n\x10\x43ollectionStatus\x12\x1b\n\x17UnknownCollectionStatus\x10\x00\x12\t\n\x05Green\x10\x01\x12\n\n\x06Yellow\x10\x02\x12\x07\n\x03Red\x10\x03*\\\n\x11PayloadSchemaType\x12\x0f\n\x0bUnknownType\x10\x00\x12\x0b\n\x07Keyword\x10\x01\x12\x0b\n\x07Integer\x10\x02\x12\t\n\x05\x46loat\x10\x03\x12\x07\n\x03Geo\x10\x04\x12\x08\n\x04Text\x10\x05*5\n\x10QuantizationType\x12\x17\n\x13UnknownQuantization\x10\x00\x12\x08\n\x04Int8\x10\x01*B\n\rTokenizerType\x12\x0b\n\x07Unknown\x10\x00\x12\n\n\x06Prefix\x10\x01\x12\x0e\n\nWhitespace\x10\x02\x12\x08\n\x04Word\x10\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x63ollections.proto\x12\x06qdrant\"\xfa\x01\n\x0cVectorParams\x12\x0c\n\x04size\x18\x01 \x01(\x04\x12\"\n\x08\x64istance\x18\x02 \x01(\x0e\x32\x10.qdrant.Distance\x12\x30\n\x0bhnsw_config\x18\x03 \x01(\x0b\x32\x16.qdrant.HnswConfigDiffH\x00\x88\x01\x01\x12<\n\x13quantization_config\x18\x04 \x01(\x0b\x32\x1a.qdrant.QuantizationConfigH\x01\x88\x01\x01\x12\x14\n\x07on_disk\x18\x05 \x01(\x08H\x02\x88\x01\x01\x42\x0e\n\x0c_hnsw_configB\x16\n\x14_quantization_configB\n\n\x08_on_disk\"\x82\x01\n\x0fVectorParamsMap\x12-\n\x03map\x18\x01 \x03(\x0b\x32 .qdrant.VectorParamsMap.MapEntry\x1a@\n\x08MapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.qdrant.VectorParams:\x02\x38\x01\"p\n\rVectorsConfig\x12&\n\x06params\x18\x01 \x01(\x0b\x32\x14.qdrant.VectorParamsH\x00\x12-\n\nparams_map\x18\x02 \x01(\x0b\x32\x17.qdrant.VectorParamsMapH\x00\x42\x08\n\x06\x63onfig\"3\n\x18GetCollectionInfoRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"\x18\n\x16ListCollectionsRequest\"%\n\x15\x43ollectionDescription\x12\x0c\n\x04name\x18\x01 \x01(\t\"Q\n\x19GetCollectionInfoResponse\x12&\n\x06result\x18\x01 \x01(\x0b\x32\x16.qdrant.CollectionInfo\x12\x0c\n\x04time\x18\x02 \x01(\x01\"[\n\x17ListCollectionsResponse\x12\x32\n\x0b\x63ollections\x18\x01 \x03(\x0b\x32\x1d.qdrant.CollectionDescription\x12\x0c\n\x04time\x18\x02 \x01(\x01\",\n\x0fOptimizerStatus\x12\n\n\x02ok\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"\x90\x02\n\x0eHnswConfigDiff\x12\x0e\n\x01m\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x19\n\x0c\x65\x66_construct\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12 \n\x13\x66ull_scan_threshold\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12!\n\x14max_indexing_threads\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x14\n\x07on_disk\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12\x16\n\tpayload_m\x18\x06 \x01(\x04H\x05\x88\x01\x01\x42\x04\n\x02_mB\x0f\n\r_ef_constructB\x16\n\x14_full_scan_thresholdB\x17\n\x15_max_indexing_threadsB\n\n\x08_on_diskB\x0c\n\n_payload_m\"y\n\rWalConfigDiff\x12\x1c\n\x0fwal_capacity_mb\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x1f\n\x12wal_segments_ahead\x18\x02 \x01(\x04H\x01\x88\x01\x01\x42\x12\n\x10_wal_capacity_mbB\x15\n\x13_wal_segments_ahead\"\xec\x03\n\x14OptimizersConfigDiff\x12\x1e\n\x11\x64\x65leted_threshold\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12%\n\x18vacuum_min_vector_number\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12#\n\x16\x64\x65\x66\x61ult_segment_number\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x1d\n\x10max_segment_size\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x1d\n\x10memmap_threshold\x18\x05 \x01(\x04H\x04\x88\x01\x01\x12\x1f\n\x12indexing_threshold\x18\x06 \x01(\x04H\x05\x88\x01\x01\x12\x1f\n\x12\x66lush_interval_sec\x18\x07 \x01(\x04H\x06\x88\x01\x01\x12%\n\x18max_optimization_threads\x18\x08 \x01(\x04H\x07\x88\x01\x01\x42\x14\n\x12_deleted_thresholdB\x1b\n\x19_vacuum_min_vector_numberB\x19\n\x17_default_segment_numberB\x13\n\x11_max_segment_sizeB\x13\n\x11_memmap_thresholdB\x15\n\x13_indexing_thresholdB\x15\n\x13_flush_interval_secB\x1b\n\x19_max_optimization_threads\"\x88\x01\n\x12ScalarQuantization\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.qdrant.QuantizationType\x12\x15\n\x08quantile\x18\x02 \x01(\x02H\x00\x88\x01\x01\x12\x17\n\nalways_ram\x18\x03 \x01(\x08H\x01\x88\x01\x01\x42\x0b\n\t_quantileB\r\n\x0b_always_ram\"l\n\x13ProductQuantization\x12-\n\x0b\x63ompression\x18\x01 \x01(\x0e\x32\x18.qdrant.CompressionRatio\x12\x17\n\nalways_ram\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\r\n\x0b_always_ram\"\x82\x01\n\x12QuantizationConfig\x12,\n\x06scalar\x18\x01 \x01(\x0b\x32\x1a.qdrant.ScalarQuantizationH\x00\x12.\n\x07product\x18\x02 \x01(\x0b\x32\x1b.qdrant.ProductQuantizationH\x00\x42\x0e\n\x0cquantization\"\xe1\x05\n\x10\x43reateCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x30\n\x0bhnsw_config\x18\x04 \x01(\x0b\x32\x16.qdrant.HnswConfigDiffH\x00\x88\x01\x01\x12.\n\nwal_config\x18\x05 \x01(\x0b\x32\x15.qdrant.WalConfigDiffH\x01\x88\x01\x01\x12<\n\x11optimizers_config\x18\x06 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiffH\x02\x88\x01\x01\x12\x19\n\x0cshard_number\x18\x07 \x01(\rH\x03\x88\x01\x01\x12\x1c\n\x0fon_disk_payload\x18\x08 \x01(\x08H\x04\x88\x01\x01\x12\x14\n\x07timeout\x18\t \x01(\x04H\x05\x88\x01\x01\x12\x32\n\x0evectors_config\x18\n \x01(\x0b\x32\x15.qdrant.VectorsConfigH\x06\x88\x01\x01\x12\x1f\n\x12replication_factor\x18\x0b \x01(\rH\x07\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x0c \x01(\rH\x08\x88\x01\x01\x12!\n\x14init_from_collection\x18\r \x01(\tH\t\x88\x01\x01\x12<\n\x13quantization_config\x18\x0e \x01(\x0b\x32\x1a.qdrant.QuantizationConfigH\n\x88\x01\x01\x42\x0e\n\x0c_hnsw_configB\r\n\x0b_wal_configB\x14\n\x12_optimizers_configB\x0f\n\r_shard_numberB\x12\n\x10_on_disk_payloadB\n\n\x08_timeoutB\x11\n\x0f_vectors_configB\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factorB\x17\n\x15_init_from_collectionB\x16\n\x14_quantization_configJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"\xdf\x01\n\x10UpdateCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12<\n\x11optimizers_config\x18\x02 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiffH\x00\x88\x01\x01\x12\x14\n\x07timeout\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x31\n\x06params\x18\x04 \x01(\x0b\x32\x1c.qdrant.CollectionParamsDiffH\x02\x88\x01\x01\x42\x14\n\x12_optimizers_configB\n\n\x08_timeoutB\t\n\x07_params\"M\n\x10\x44\x65leteCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x14\n\x07timeout\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\n\n\x08_timeout\";\n\x1b\x43ollectionOperationResponse\x12\x0e\n\x06result\x18\x01 \x01(\x08\x12\x0c\n\x04time\x18\x02 \x01(\x01\"\x90\x02\n\x10\x43ollectionParams\x12\x14\n\x0cshard_number\x18\x03 \x01(\r\x12\x17\n\x0fon_disk_payload\x18\x04 \x01(\x08\x12\x32\n\x0evectors_config\x18\x05 \x01(\x0b\x32\x15.qdrant.VectorsConfigH\x00\x88\x01\x01\x12\x1f\n\x12replication_factor\x18\x06 \x01(\rH\x01\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x07 \x01(\rH\x02\x88\x01\x01\x42\x11\n\x0f_vectors_configB\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factorJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x92\x01\n\x14\x43ollectionParamsDiff\x12\x1f\n\x12replication_factor\x18\x01 \x01(\rH\x00\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x02 \x01(\rH\x01\x88\x01\x01\x42\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factor\"\xa2\x02\n\x10\x43ollectionConfig\x12(\n\x06params\x18\x01 \x01(\x0b\x32\x18.qdrant.CollectionParams\x12+\n\x0bhnsw_config\x18\x02 \x01(\x0b\x32\x16.qdrant.HnswConfigDiff\x12\x36\n\x10optimizer_config\x18\x03 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiff\x12)\n\nwal_config\x18\x04 \x01(\x0b\x32\x15.qdrant.WalConfigDiff\x12<\n\x13quantization_config\x18\x05 \x01(\x0b\x32\x1a.qdrant.QuantizationConfigH\x00\x88\x01\x01\x42\x16\n\x14_quantization_config\"\xbd\x01\n\x0fTextIndexParams\x12(\n\ttokenizer\x18\x01 \x01(\x0e\x32\x15.qdrant.TokenizerType\x12\x16\n\tlowercase\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1a\n\rmin_token_len\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x1a\n\rmax_token_len\x18\x04 \x01(\x04H\x02\x88\x01\x01\x42\x0c\n\n_lowercaseB\x10\n\x0e_min_token_lenB\x10\n\x0e_max_token_len\"Z\n\x12PayloadIndexParams\x12\x34\n\x11text_index_params\x18\x01 \x01(\x0b\x32\x17.qdrant.TextIndexParamsH\x00\x42\x0e\n\x0cindex_params\"\x9d\x01\n\x11PayloadSchemaInfo\x12,\n\tdata_type\x18\x01 \x01(\x0e\x32\x19.qdrant.PayloadSchemaType\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1a.qdrant.PayloadIndexParamsH\x00\x88\x01\x01\x12\x13\n\x06points\x18\x03 \x01(\x04H\x01\x88\x01\x01\x42\t\n\x07_paramsB\t\n\x07_points\"\xba\x03\n\x0e\x43ollectionInfo\x12(\n\x06status\x18\x01 \x01(\x0e\x32\x18.qdrant.CollectionStatus\x12\x31\n\x10optimizer_status\x18\x02 \x01(\x0b\x32\x17.qdrant.OptimizerStatus\x12\x15\n\rvectors_count\x18\x03 \x01(\x04\x12\x16\n\x0esegments_count\x18\x04 \x01(\x04\x12(\n\x06\x63onfig\x18\x07 \x01(\x0b\x32\x18.qdrant.CollectionConfig\x12\x41\n\x0epayload_schema\x18\x08 \x03(\x0b\x32).qdrant.CollectionInfo.PayloadSchemaEntry\x12\x14\n\x0cpoints_count\x18\t \x01(\x04\x12\"\n\x15indexed_vectors_count\x18\n \x01(\x04H\x00\x88\x01\x01\x1aO\n\x12PayloadSchemaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.qdrant.PayloadSchemaInfo:\x02\x38\x01\x42\x18\n\x16_indexed_vectors_countJ\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"[\n\rChangeAliases\x12(\n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x17.qdrant.AliasOperations\x12\x14\n\x07timeout\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\n\n\x08_timeout\"\xa2\x01\n\x0f\x41liasOperations\x12+\n\x0c\x63reate_alias\x18\x01 \x01(\x0b\x32\x13.qdrant.CreateAliasH\x00\x12+\n\x0crename_alias\x18\x02 \x01(\x0b\x32\x13.qdrant.RenameAliasH\x00\x12+\n\x0c\x64\x65lete_alias\x18\x03 \x01(\x0b\x32\x13.qdrant.DeleteAliasH\x00\x42\x08\n\x06\x61\x63tion\":\n\x0b\x43reateAlias\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nalias_name\x18\x02 \x01(\t\"=\n\x0bRenameAlias\x12\x16\n\x0eold_alias_name\x18\x01 \x01(\t\x12\x16\n\x0enew_alias_name\x18\x02 \x01(\t\"!\n\x0b\x44\x65leteAlias\x12\x12\n\nalias_name\x18\x01 \x01(\t\"\x14\n\x12ListAliasesRequest\"7\n\x1cListCollectionAliasesRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"?\n\x10\x41liasDescription\x12\x12\n\nalias_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\"N\n\x13ListAliasesResponse\x12)\n\x07\x61liases\x18\x01 \x03(\x0b\x32\x18.qdrant.AliasDescription\x12\x0c\n\x04time\x18\x02 \x01(\x01\"7\n\x1c\x43ollectionClusterInfoRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"]\n\x0eLocalShardInfo\x12\x10\n\x08shard_id\x18\x01 \x01(\r\x12\x14\n\x0cpoints_count\x18\x02 \x01(\x04\x12#\n\x05state\x18\x03 \x01(\x0e\x32\x14.qdrant.ReplicaState\"Y\n\x0fRemoteShardInfo\x12\x10\n\x08shard_id\x18\x01 \x01(\r\x12\x0f\n\x07peer_id\x18\x02 \x01(\x04\x12#\n\x05state\x18\x03 \x01(\x0e\x32\x14.qdrant.ReplicaState\"M\n\x11ShardTransferInfo\x12\x10\n\x08shard_id\x18\x01 \x01(\r\x12\x0c\n\x04\x66rom\x18\x02 \x01(\x04\x12\n\n\x02to\x18\x03 \x01(\x04\x12\x0c\n\x04sync\x18\x04 \x01(\x08\"\xd7\x01\n\x1d\x43ollectionClusterInfoResponse\x12\x0f\n\x07peer_id\x18\x01 \x01(\x04\x12\x13\n\x0bshard_count\x18\x02 \x01(\x04\x12,\n\x0clocal_shards\x18\x03 \x03(\x0b\x32\x16.qdrant.LocalShardInfo\x12.\n\rremote_shards\x18\x04 \x03(\x0b\x32\x17.qdrant.RemoteShardInfo\x12\x32\n\x0fshard_transfers\x18\x05 \x03(\x0b\x32\x19.qdrant.ShardTransferInfo\"G\n\tMoveShard\x12\x10\n\x08shard_id\x18\x01 \x01(\r\x12\x14\n\x0c\x66rom_peer_id\x18\x02 \x01(\x04\x12\x12\n\nto_peer_id\x18\x03 \x01(\x04\",\n\x07Replica\x12\x10\n\x08shard_id\x18\x01 \x01(\r\x12\x0f\n\x07peer_id\x18\x02 \x01(\x04\"\x9a\x02\n#UpdateCollectionClusterSetupRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\'\n\nmove_shard\x18\x02 \x01(\x0b\x32\x11.qdrant.MoveShardH\x00\x12,\n\x0freplicate_shard\x18\x03 \x01(\x0b\x32\x11.qdrant.MoveShardH\x00\x12+\n\x0e\x61\x62ort_transfer\x18\x04 \x01(\x0b\x32\x11.qdrant.MoveShardH\x00\x12\'\n\x0c\x64rop_replica\x18\x05 \x01(\x0b\x32\x0f.qdrant.ReplicaH\x00\x12\x14\n\x07timeout\x18\x06 \x01(\x04H\x01\x88\x01\x01\x42\x0b\n\toperationB\n\n\x08_timeout\"6\n$UpdateCollectionClusterSetupResponse\x12\x0e\n\x06result\x18\x01 \x01(\x08*@\n\x08\x44istance\x12\x13\n\x0fUnknownDistance\x10\x00\x12\n\n\x06\x43osine\x10\x01\x12\n\n\x06\x45uclid\x10\x02\x12\x07\n\x03\x44ot\x10\x03*O\n\x10\x43ollectionStatus\x12\x1b\n\x17UnknownCollectionStatus\x10\x00\x12\t\n\x05Green\x10\x01\x12\n\n\x06Yellow\x10\x02\x12\x07\n\x03Red\x10\x03*\\\n\x11PayloadSchemaType\x12\x0f\n\x0bUnknownType\x10\x00\x12\x0b\n\x07Keyword\x10\x01\x12\x0b\n\x07Integer\x10\x02\x12\t\n\x05\x46loat\x10\x03\x12\x07\n\x03Geo\x10\x04\x12\x08\n\x04Text\x10\x05*5\n\x10QuantizationType\x12\x17\n\x13UnknownQuantization\x10\x00\x12\x08\n\x04Int8\x10\x01*=\n\x10\x43ompressionRatio\x12\x06\n\x02x4\x10\x00\x12\x06\n\x02x8\x10\x01\x12\x07\n\x03x16\x10\x02\x12\x07\n\x03x32\x10\x03\x12\x07\n\x03x64\x10\x04*B\n\rTokenizerType\x12\x0b\n\x07Unknown\x10\x00\x12\n\n\x06Prefix\x10\x01\x12\x0e\n\nWhitespace\x10\x02\x12\x08\n\x04Word\x10\x03*Q\n\x0cReplicaState\x12\n\n\x06\x41\x63tive\x10\x00\x12\x08\n\x04\x44\x65\x61\x64\x10\x01\x12\x0b\n\x07Partial\x10\x02\x12\x10\n\x0cInitializing\x10\x03\x12\x0c\n\x08Listener\x10\x04\x62\x06proto3')
 
 _DISTANCE = DESCRIPTOR.enum_types_by_name['Distance']
 Distance = enum_type_wrapper.EnumTypeWrapper(_DISTANCE)
 _COLLECTIONSTATUS = DESCRIPTOR.enum_types_by_name['CollectionStatus']
 CollectionStatus = enum_type_wrapper.EnumTypeWrapper(_COLLECTIONSTATUS)
 _PAYLOADSCHEMATYPE = DESCRIPTOR.enum_types_by_name['PayloadSchemaType']
 PayloadSchemaType = enum_type_wrapper.EnumTypeWrapper(_PAYLOADSCHEMATYPE)
 _QUANTIZATIONTYPE = DESCRIPTOR.enum_types_by_name['QuantizationType']
 QuantizationType = enum_type_wrapper.EnumTypeWrapper(_QUANTIZATIONTYPE)
+_COMPRESSIONRATIO = DESCRIPTOR.enum_types_by_name['CompressionRatio']
+CompressionRatio = enum_type_wrapper.EnumTypeWrapper(_COMPRESSIONRATIO)
 _TOKENIZERTYPE = DESCRIPTOR.enum_types_by_name['TokenizerType']
 TokenizerType = enum_type_wrapper.EnumTypeWrapper(_TOKENIZERTYPE)
+_REPLICASTATE = DESCRIPTOR.enum_types_by_name['ReplicaState']
+ReplicaState = enum_type_wrapper.EnumTypeWrapper(_REPLICASTATE)
 UnknownDistance = 0
 Cosine = 1
 Euclid = 2
 Dot = 3
 UnknownCollectionStatus = 0
 Green = 1
 Yellow = 2
@@ -39,18 +43,28 @@
 Keyword = 1
 Integer = 2
 Float = 3
 Geo = 4
 Text = 5
 UnknownQuantization = 0
 Int8 = 1
+x4 = 0
+x8 = 1
+x16 = 2
+x32 = 3
+x64 = 4
 Unknown = 0
 Prefix = 1
 Whitespace = 2
 Word = 3
+Active = 0
+Dead = 1
+Partial = 2
+Initializing = 3
+Listener = 4
 
 
 _VECTORPARAMS = DESCRIPTOR.message_types_by_name['VectorParams']
 _VECTORPARAMSMAP = DESCRIPTOR.message_types_by_name['VectorParamsMap']
 _VECTORPARAMSMAP_MAPENTRY = _VECTORPARAMSMAP.nested_types_by_name['MapEntry']
 _VECTORSCONFIG = DESCRIPTOR.message_types_by_name['VectorsConfig']
 _GETCOLLECTIONINFOREQUEST = DESCRIPTOR.message_types_by_name['GetCollectionInfoRequest']
@@ -59,14 +73,15 @@
 _GETCOLLECTIONINFORESPONSE = DESCRIPTOR.message_types_by_name['GetCollectionInfoResponse']
 _LISTCOLLECTIONSRESPONSE = DESCRIPTOR.message_types_by_name['ListCollectionsResponse']
 _OPTIMIZERSTATUS = DESCRIPTOR.message_types_by_name['OptimizerStatus']
 _HNSWCONFIGDIFF = DESCRIPTOR.message_types_by_name['HnswConfigDiff']
 _WALCONFIGDIFF = DESCRIPTOR.message_types_by_name['WalConfigDiff']
 _OPTIMIZERSCONFIGDIFF = DESCRIPTOR.message_types_by_name['OptimizersConfigDiff']
 _SCALARQUANTIZATION = DESCRIPTOR.message_types_by_name['ScalarQuantization']
+_PRODUCTQUANTIZATION = DESCRIPTOR.message_types_by_name['ProductQuantization']
 _QUANTIZATIONCONFIG = DESCRIPTOR.message_types_by_name['QuantizationConfig']
 _CREATECOLLECTION = DESCRIPTOR.message_types_by_name['CreateCollection']
 _UPDATECOLLECTION = DESCRIPTOR.message_types_by_name['UpdateCollection']
 _DELETECOLLECTION = DESCRIPTOR.message_types_by_name['DeleteCollection']
 _COLLECTIONOPERATIONRESPONSE = DESCRIPTOR.message_types_by_name['CollectionOperationResponse']
 _COLLECTIONPARAMS = DESCRIPTOR.message_types_by_name['CollectionParams']
 _COLLECTIONPARAMSDIFF = DESCRIPTOR.message_types_by_name['CollectionParamsDiff']
@@ -81,14 +96,23 @@
 _CREATEALIAS = DESCRIPTOR.message_types_by_name['CreateAlias']
 _RENAMEALIAS = DESCRIPTOR.message_types_by_name['RenameAlias']
 _DELETEALIAS = DESCRIPTOR.message_types_by_name['DeleteAlias']
 _LISTALIASESREQUEST = DESCRIPTOR.message_types_by_name['ListAliasesRequest']
 _LISTCOLLECTIONALIASESREQUEST = DESCRIPTOR.message_types_by_name['ListCollectionAliasesRequest']
 _ALIASDESCRIPTION = DESCRIPTOR.message_types_by_name['AliasDescription']
 _LISTALIASESRESPONSE = DESCRIPTOR.message_types_by_name['ListAliasesResponse']
+_COLLECTIONCLUSTERINFOREQUEST = DESCRIPTOR.message_types_by_name['CollectionClusterInfoRequest']
+_LOCALSHARDINFO = DESCRIPTOR.message_types_by_name['LocalShardInfo']
+_REMOTESHARDINFO = DESCRIPTOR.message_types_by_name['RemoteShardInfo']
+_SHARDTRANSFERINFO = DESCRIPTOR.message_types_by_name['ShardTransferInfo']
+_COLLECTIONCLUSTERINFORESPONSE = DESCRIPTOR.message_types_by_name['CollectionClusterInfoResponse']
+_MOVESHARD = DESCRIPTOR.message_types_by_name['MoveShard']
+_REPLICA = DESCRIPTOR.message_types_by_name['Replica']
+_UPDATECOLLECTIONCLUSTERSETUPREQUEST = DESCRIPTOR.message_types_by_name['UpdateCollectionClusterSetupRequest']
+_UPDATECOLLECTIONCLUSTERSETUPRESPONSE = DESCRIPTOR.message_types_by_name['UpdateCollectionClusterSetupResponse']
 VectorParams = _reflection.GeneratedProtocolMessageType('VectorParams', (_message.Message,), {
   'DESCRIPTOR' : _VECTORPARAMS,
   '__module__' : 'collections_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.VectorParams)
   })
 _sym_db.RegisterMessage(VectorParams)
 
@@ -180,14 +204,21 @@
 ScalarQuantization = _reflection.GeneratedProtocolMessageType('ScalarQuantization', (_message.Message,), {
   'DESCRIPTOR' : _SCALARQUANTIZATION,
   '__module__' : 'collections_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.ScalarQuantization)
   })
 _sym_db.RegisterMessage(ScalarQuantization)
 
+ProductQuantization = _reflection.GeneratedProtocolMessageType('ProductQuantization', (_message.Message,), {
+  'DESCRIPTOR' : _PRODUCTQUANTIZATION,
+  '__module__' : 'collections_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.ProductQuantization)
+  })
+_sym_db.RegisterMessage(ProductQuantization)
+
 QuantizationConfig = _reflection.GeneratedProtocolMessageType('QuantizationConfig', (_message.Message,), {
   'DESCRIPTOR' : _QUANTIZATIONCONFIG,
   '__module__' : 'collections_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.QuantizationConfig)
   })
 _sym_db.RegisterMessage(QuantizationConfig)
 
@@ -335,97 +366,184 @@
 ListAliasesResponse = _reflection.GeneratedProtocolMessageType('ListAliasesResponse', (_message.Message,), {
   'DESCRIPTOR' : _LISTALIASESRESPONSE,
   '__module__' : 'collections_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.ListAliasesResponse)
   })
 _sym_db.RegisterMessage(ListAliasesResponse)
 
+CollectionClusterInfoRequest = _reflection.GeneratedProtocolMessageType('CollectionClusterInfoRequest', (_message.Message,), {
+  'DESCRIPTOR' : _COLLECTIONCLUSTERINFOREQUEST,
+  '__module__' : 'collections_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.CollectionClusterInfoRequest)
+  })
+_sym_db.RegisterMessage(CollectionClusterInfoRequest)
+
+LocalShardInfo = _reflection.GeneratedProtocolMessageType('LocalShardInfo', (_message.Message,), {
+  'DESCRIPTOR' : _LOCALSHARDINFO,
+  '__module__' : 'collections_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.LocalShardInfo)
+  })
+_sym_db.RegisterMessage(LocalShardInfo)
+
+RemoteShardInfo = _reflection.GeneratedProtocolMessageType('RemoteShardInfo', (_message.Message,), {
+  'DESCRIPTOR' : _REMOTESHARDINFO,
+  '__module__' : 'collections_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.RemoteShardInfo)
+  })
+_sym_db.RegisterMessage(RemoteShardInfo)
+
+ShardTransferInfo = _reflection.GeneratedProtocolMessageType('ShardTransferInfo', (_message.Message,), {
+  'DESCRIPTOR' : _SHARDTRANSFERINFO,
+  '__module__' : 'collections_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.ShardTransferInfo)
+  })
+_sym_db.RegisterMessage(ShardTransferInfo)
+
+CollectionClusterInfoResponse = _reflection.GeneratedProtocolMessageType('CollectionClusterInfoResponse', (_message.Message,), {
+  'DESCRIPTOR' : _COLLECTIONCLUSTERINFORESPONSE,
+  '__module__' : 'collections_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.CollectionClusterInfoResponse)
+  })
+_sym_db.RegisterMessage(CollectionClusterInfoResponse)
+
+MoveShard = _reflection.GeneratedProtocolMessageType('MoveShard', (_message.Message,), {
+  'DESCRIPTOR' : _MOVESHARD,
+  '__module__' : 'collections_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.MoveShard)
+  })
+_sym_db.RegisterMessage(MoveShard)
+
+Replica = _reflection.GeneratedProtocolMessageType('Replica', (_message.Message,), {
+  'DESCRIPTOR' : _REPLICA,
+  '__module__' : 'collections_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.Replica)
+  })
+_sym_db.RegisterMessage(Replica)
+
+UpdateCollectionClusterSetupRequest = _reflection.GeneratedProtocolMessageType('UpdateCollectionClusterSetupRequest', (_message.Message,), {
+  'DESCRIPTOR' : _UPDATECOLLECTIONCLUSTERSETUPREQUEST,
+  '__module__' : 'collections_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.UpdateCollectionClusterSetupRequest)
+  })
+_sym_db.RegisterMessage(UpdateCollectionClusterSetupRequest)
+
+UpdateCollectionClusterSetupResponse = _reflection.GeneratedProtocolMessageType('UpdateCollectionClusterSetupResponse', (_message.Message,), {
+  'DESCRIPTOR' : _UPDATECOLLECTIONCLUSTERSETUPRESPONSE,
+  '__module__' : 'collections_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.UpdateCollectionClusterSetupResponse)
+  })
+_sym_db.RegisterMessage(UpdateCollectionClusterSetupResponse)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _VECTORPARAMSMAP_MAPENTRY._options = None
   _VECTORPARAMSMAP_MAPENTRY._serialized_options = b'8\001'
   _COLLECTIONINFO_PAYLOADSCHEMAENTRY._options = None
   _COLLECTIONINFO_PAYLOADSCHEMAENTRY._serialized_options = b'8\001'
-  _DISTANCE._serialized_start=5303
-  _DISTANCE._serialized_end=5367
-  _COLLECTIONSTATUS._serialized_start=5369
-  _COLLECTIONSTATUS._serialized_end=5448
-  _PAYLOADSCHEMATYPE._serialized_start=5450
-  _PAYLOADSCHEMATYPE._serialized_end=5542
-  _QUANTIZATIONTYPE._serialized_start=5544
-  _QUANTIZATIONTYPE._serialized_end=5597
-  _TOKENIZERTYPE._serialized_start=5599
-  _TOKENIZERTYPE._serialized_end=5665
+  _DISTANCE._serialized_start=6496
+  _DISTANCE._serialized_end=6560
+  _COLLECTIONSTATUS._serialized_start=6562
+  _COLLECTIONSTATUS._serialized_end=6641
+  _PAYLOADSCHEMATYPE._serialized_start=6643
+  _PAYLOADSCHEMATYPE._serialized_end=6735
+  _QUANTIZATIONTYPE._serialized_start=6737
+  _QUANTIZATIONTYPE._serialized_end=6790
+  _COMPRESSIONRATIO._serialized_start=6792
+  _COMPRESSIONRATIO._serialized_end=6853
+  _TOKENIZERTYPE._serialized_start=6855
+  _TOKENIZERTYPE._serialized_end=6921
+  _REPLICASTATE._serialized_start=6923
+  _REPLICASTATE._serialized_end=7004
   _VECTORPARAMS._serialized_start=30
-  _VECTORPARAMS._serialized_end=246
-  _VECTORPARAMSMAP._serialized_start=249
-  _VECTORPARAMSMAP._serialized_end=379
-  _VECTORPARAMSMAP_MAPENTRY._serialized_start=315
-  _VECTORPARAMSMAP_MAPENTRY._serialized_end=379
-  _VECTORSCONFIG._serialized_start=381
-  _VECTORSCONFIG._serialized_end=493
-  _GETCOLLECTIONINFOREQUEST._serialized_start=495
-  _GETCOLLECTIONINFOREQUEST._serialized_end=546
-  _LISTCOLLECTIONSREQUEST._serialized_start=548
-  _LISTCOLLECTIONSREQUEST._serialized_end=572
-  _COLLECTIONDESCRIPTION._serialized_start=574
-  _COLLECTIONDESCRIPTION._serialized_end=611
-  _GETCOLLECTIONINFORESPONSE._serialized_start=613
-  _GETCOLLECTIONINFORESPONSE._serialized_end=694
-  _LISTCOLLECTIONSRESPONSE._serialized_start=696
-  _LISTCOLLECTIONSRESPONSE._serialized_end=787
-  _OPTIMIZERSTATUS._serialized_start=789
-  _OPTIMIZERSTATUS._serialized_end=833
-  _HNSWCONFIGDIFF._serialized_start=836
-  _HNSWCONFIGDIFF._serialized_end=1108
-  _WALCONFIGDIFF._serialized_start=1110
-  _WALCONFIGDIFF._serialized_end=1231
-  _OPTIMIZERSCONFIGDIFF._serialized_start=1234
-  _OPTIMIZERSCONFIGDIFF._serialized_end=1726
-  _SCALARQUANTIZATION._serialized_start=1729
-  _SCALARQUANTIZATION._serialized_end=1865
-  _QUANTIZATIONCONFIG._serialized_start=1867
-  _QUANTIZATIONCONFIG._serialized_end=1949
-  _CREATECOLLECTION._serialized_start=1952
-  _CREATECOLLECTION._serialized_end=2689
-  _UPDATECOLLECTION._serialized_start=2692
-  _UPDATECOLLECTION._serialized_end=2915
-  _DELETECOLLECTION._serialized_start=2917
-  _DELETECOLLECTION._serialized_end=2994
-  _COLLECTIONOPERATIONRESPONSE._serialized_start=2996
-  _COLLECTIONOPERATIONRESPONSE._serialized_end=3055
-  _COLLECTIONPARAMS._serialized_start=3058
-  _COLLECTIONPARAMS._serialized_end=3330
-  _COLLECTIONPARAMSDIFF._serialized_start=3333
-  _COLLECTIONPARAMSDIFF._serialized_end=3479
-  _COLLECTIONCONFIG._serialized_start=3482
-  _COLLECTIONCONFIG._serialized_end=3772
-  _TEXTINDEXPARAMS._serialized_start=3775
-  _TEXTINDEXPARAMS._serialized_end=3964
-  _PAYLOADINDEXPARAMS._serialized_start=3966
-  _PAYLOADINDEXPARAMS._serialized_end=4056
-  _PAYLOADSCHEMAINFO._serialized_start=4059
-  _PAYLOADSCHEMAINFO._serialized_end=4216
-  _COLLECTIONINFO._serialized_start=4219
-  _COLLECTIONINFO._serialized_end=4661
-  _COLLECTIONINFO_PAYLOADSCHEMAENTRY._serialized_start=4544
-  _COLLECTIONINFO_PAYLOADSCHEMAENTRY._serialized_end=4623
-  _CHANGEALIASES._serialized_start=4663
-  _CHANGEALIASES._serialized_end=4754
-  _ALIASOPERATIONS._serialized_start=4757
-  _ALIASOPERATIONS._serialized_end=4919
-  _CREATEALIAS._serialized_start=4921
-  _CREATEALIAS._serialized_end=4979
-  _RENAMEALIAS._serialized_start=4981
-  _RENAMEALIAS._serialized_end=5042
-  _DELETEALIAS._serialized_start=5044
-  _DELETEALIAS._serialized_end=5077
-  _LISTALIASESREQUEST._serialized_start=5079
-  _LISTALIASESREQUEST._serialized_end=5099
-  _LISTCOLLECTIONALIASESREQUEST._serialized_start=5101
-  _LISTCOLLECTIONALIASESREQUEST._serialized_end=5156
-  _ALIASDESCRIPTION._serialized_start=5158
-  _ALIASDESCRIPTION._serialized_end=5221
-  _LISTALIASESRESPONSE._serialized_start=5223
-  _LISTALIASESRESPONSE._serialized_end=5301
+  _VECTORPARAMS._serialized_end=280
+  _VECTORPARAMSMAP._serialized_start=283
+  _VECTORPARAMSMAP._serialized_end=413
+  _VECTORPARAMSMAP_MAPENTRY._serialized_start=349
+  _VECTORPARAMSMAP_MAPENTRY._serialized_end=413
+  _VECTORSCONFIG._serialized_start=415
+  _VECTORSCONFIG._serialized_end=527
+  _GETCOLLECTIONINFOREQUEST._serialized_start=529
+  _GETCOLLECTIONINFOREQUEST._serialized_end=580
+  _LISTCOLLECTIONSREQUEST._serialized_start=582
+  _LISTCOLLECTIONSREQUEST._serialized_end=606
+  _COLLECTIONDESCRIPTION._serialized_start=608
+  _COLLECTIONDESCRIPTION._serialized_end=645
+  _GETCOLLECTIONINFORESPONSE._serialized_start=647
+  _GETCOLLECTIONINFORESPONSE._serialized_end=728
+  _LISTCOLLECTIONSRESPONSE._serialized_start=730
+  _LISTCOLLECTIONSRESPONSE._serialized_end=821
+  _OPTIMIZERSTATUS._serialized_start=823
+  _OPTIMIZERSTATUS._serialized_end=867
+  _HNSWCONFIGDIFF._serialized_start=870
+  _HNSWCONFIGDIFF._serialized_end=1142
+  _WALCONFIGDIFF._serialized_start=1144
+  _WALCONFIGDIFF._serialized_end=1265
+  _OPTIMIZERSCONFIGDIFF._serialized_start=1268
+  _OPTIMIZERSCONFIGDIFF._serialized_end=1760
+  _SCALARQUANTIZATION._serialized_start=1763
+  _SCALARQUANTIZATION._serialized_end=1899
+  _PRODUCTQUANTIZATION._serialized_start=1901
+  _PRODUCTQUANTIZATION._serialized_end=2009
+  _QUANTIZATIONCONFIG._serialized_start=2012
+  _QUANTIZATIONCONFIG._serialized_end=2142
+  _CREATECOLLECTION._serialized_start=2145
+  _CREATECOLLECTION._serialized_end=2882
+  _UPDATECOLLECTION._serialized_start=2885
+  _UPDATECOLLECTION._serialized_end=3108
+  _DELETECOLLECTION._serialized_start=3110
+  _DELETECOLLECTION._serialized_end=3187
+  _COLLECTIONOPERATIONRESPONSE._serialized_start=3189
+  _COLLECTIONOPERATIONRESPONSE._serialized_end=3248
+  _COLLECTIONPARAMS._serialized_start=3251
+  _COLLECTIONPARAMS._serialized_end=3523
+  _COLLECTIONPARAMSDIFF._serialized_start=3526
+  _COLLECTIONPARAMSDIFF._serialized_end=3672
+  _COLLECTIONCONFIG._serialized_start=3675
+  _COLLECTIONCONFIG._serialized_end=3965
+  _TEXTINDEXPARAMS._serialized_start=3968
+  _TEXTINDEXPARAMS._serialized_end=4157
+  _PAYLOADINDEXPARAMS._serialized_start=4159
+  _PAYLOADINDEXPARAMS._serialized_end=4249
+  _PAYLOADSCHEMAINFO._serialized_start=4252
+  _PAYLOADSCHEMAINFO._serialized_end=4409
+  _COLLECTIONINFO._serialized_start=4412
+  _COLLECTIONINFO._serialized_end=4854
+  _COLLECTIONINFO_PAYLOADSCHEMAENTRY._serialized_start=4737
+  _COLLECTIONINFO_PAYLOADSCHEMAENTRY._serialized_end=4816
+  _CHANGEALIASES._serialized_start=4856
+  _CHANGEALIASES._serialized_end=4947
+  _ALIASOPERATIONS._serialized_start=4950
+  _ALIASOPERATIONS._serialized_end=5112
+  _CREATEALIAS._serialized_start=5114
+  _CREATEALIAS._serialized_end=5172
+  _RENAMEALIAS._serialized_start=5174
+  _RENAMEALIAS._serialized_end=5235
+  _DELETEALIAS._serialized_start=5237
+  _DELETEALIAS._serialized_end=5270
+  _LISTALIASESREQUEST._serialized_start=5272
+  _LISTALIASESREQUEST._serialized_end=5292
+  _LISTCOLLECTIONALIASESREQUEST._serialized_start=5294
+  _LISTCOLLECTIONALIASESREQUEST._serialized_end=5349
+  _ALIASDESCRIPTION._serialized_start=5351
+  _ALIASDESCRIPTION._serialized_end=5414
+  _LISTALIASESRESPONSE._serialized_start=5416
+  _LISTALIASESRESPONSE._serialized_end=5494
+  _COLLECTIONCLUSTERINFOREQUEST._serialized_start=5496
+  _COLLECTIONCLUSTERINFOREQUEST._serialized_end=5551
+  _LOCALSHARDINFO._serialized_start=5553
+  _LOCALSHARDINFO._serialized_end=5646
+  _REMOTESHARDINFO._serialized_start=5648
+  _REMOTESHARDINFO._serialized_end=5737
+  _SHARDTRANSFERINFO._serialized_start=5739
+  _SHARDTRANSFERINFO._serialized_end=5816
+  _COLLECTIONCLUSTERINFORESPONSE._serialized_start=5819
+  _COLLECTIONCLUSTERINFORESPONSE._serialized_end=6034
+  _MOVESHARD._serialized_start=6036
+  _MOVESHARD._serialized_end=6107
+  _REPLICA._serialized_start=6109
+  _REPLICA._serialized_end=6153
+  _UPDATECOLLECTIONCLUSTERSETUPREQUEST._serialized_start=6156
+  _UPDATECOLLECTIONCLUSTERSETUPREQUEST._serialized_end=6438
+  _UPDATECOLLECTIONCLUSTERSETUPRESPONSE._serialized_start=6440
+  _UPDATECOLLECTIONCLUSTERSETUPRESPONSE._serialized_end=6494
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qdrant_client-1.1.7/qdrant_client/grpc/collections_service_pb2.py` & `qdrant_client-1.2.0/qdrant_client/grpc/collections_service_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import collections_pb2 as collections__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x63ollections_service.proto\x12\x06qdrant\x1a\x11\x63ollections.proto2\xfe\x04\n\x0b\x43ollections\x12L\n\x03Get\x12 .qdrant.GetCollectionInfoRequest\x1a!.qdrant.GetCollectionInfoResponse\"\x00\x12I\n\x04List\x12\x1e.qdrant.ListCollectionsRequest\x1a\x1f.qdrant.ListCollectionsResponse\"\x00\x12I\n\x06\x43reate\x12\x18.qdrant.CreateCollection\x1a#.qdrant.CollectionOperationResponse\"\x00\x12I\n\x06Update\x12\x18.qdrant.UpdateCollection\x1a#.qdrant.CollectionOperationResponse\"\x00\x12I\n\x06\x44\x65lete\x12\x18.qdrant.DeleteCollection\x1a#.qdrant.CollectionOperationResponse\"\x00\x12M\n\rUpdateAliases\x12\x15.qdrant.ChangeAliases\x1a#.qdrant.CollectionOperationResponse\"\x00\x12\\\n\x15ListCollectionAliases\x12$.qdrant.ListCollectionAliasesRequest\x1a\x1b.qdrant.ListAliasesResponse\"\x00\x12H\n\x0bListAliases\x12\x1a.qdrant.ListAliasesRequest\x1a\x1b.qdrant.ListAliasesResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x63ollections_service.proto\x12\x06qdrant\x1a\x11\x63ollections.proto2\xe3\x06\n\x0b\x43ollections\x12L\n\x03Get\x12 .qdrant.GetCollectionInfoRequest\x1a!.qdrant.GetCollectionInfoResponse\"\x00\x12I\n\x04List\x12\x1e.qdrant.ListCollectionsRequest\x1a\x1f.qdrant.ListCollectionsResponse\"\x00\x12I\n\x06\x43reate\x12\x18.qdrant.CreateCollection\x1a#.qdrant.CollectionOperationResponse\"\x00\x12I\n\x06Update\x12\x18.qdrant.UpdateCollection\x1a#.qdrant.CollectionOperationResponse\"\x00\x12I\n\x06\x44\x65lete\x12\x18.qdrant.DeleteCollection\x1a#.qdrant.CollectionOperationResponse\"\x00\x12M\n\rUpdateAliases\x12\x15.qdrant.ChangeAliases\x1a#.qdrant.CollectionOperationResponse\"\x00\x12\\\n\x15ListCollectionAliases\x12$.qdrant.ListCollectionAliasesRequest\x1a\x1b.qdrant.ListAliasesResponse\"\x00\x12H\n\x0bListAliases\x12\x1a.qdrant.ListAliasesRequest\x1a\x1b.qdrant.ListAliasesResponse\"\x00\x12\x66\n\x15\x43ollectionClusterInfo\x12$.qdrant.CollectionClusterInfoRequest\x1a%.qdrant.CollectionClusterInfoResponse\"\x00\x12{\n\x1cUpdateCollectionClusterSetup\x12+.qdrant.UpdateCollectionClusterSetupRequest\x1a,.qdrant.UpdateCollectionClusterSetupResponse\"\x00\x62\x06proto3')
 
 
 
 _COLLECTIONS = DESCRIPTOR.services_by_name['Collections']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _COLLECTIONS._serialized_start=57
-  _COLLECTIONS._serialized_end=695
+  _COLLECTIONS._serialized_end=924
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qdrant_client-1.1.7/qdrant_client/grpc/collections_service_pb2_grpc.py` & `qdrant_client-1.2.0/qdrant_client/grpc/collections_service_pb2_grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,14 +50,24 @@
                 response_deserializer=collections__pb2.ListAliasesResponse.FromString,
                 )
         self.ListAliases = channel.unary_unary(
                 '/qdrant.Collections/ListAliases',
                 request_serializer=collections__pb2.ListAliasesRequest.SerializeToString,
                 response_deserializer=collections__pb2.ListAliasesResponse.FromString,
                 )
+        self.CollectionClusterInfo = channel.unary_unary(
+                '/qdrant.Collections/CollectionClusterInfo',
+                request_serializer=collections__pb2.CollectionClusterInfoRequest.SerializeToString,
+                response_deserializer=collections__pb2.CollectionClusterInfoResponse.FromString,
+                )
+        self.UpdateCollectionClusterSetup = channel.unary_unary(
+                '/qdrant.Collections/UpdateCollectionClusterSetup',
+                request_serializer=collections__pb2.UpdateCollectionClusterSetupRequest.SerializeToString,
+                response_deserializer=collections__pb2.UpdateCollectionClusterSetupResponse.FromString,
+                )
 
 
 class CollectionsServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Get(self, request, context):
         """
@@ -119,14 +129,30 @@
         """
         Get list of all aliases for all existing collections
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def CollectionClusterInfo(self, request, context):
+        """
+        Get cluster information for a collection
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UpdateCollectionClusterSetup(self, request, context):
+        """
+        Update cluster setup for a collection
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_CollectionsServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Get': grpc.unary_unary_rpc_method_handler(
                     servicer.Get,
                     request_deserializer=collections__pb2.GetCollectionInfoRequest.FromString,
                     response_serializer=collections__pb2.GetCollectionInfoResponse.SerializeToString,
@@ -162,14 +188,24 @@
                     response_serializer=collections__pb2.ListAliasesResponse.SerializeToString,
             ),
             'ListAliases': grpc.unary_unary_rpc_method_handler(
                     servicer.ListAliases,
                     request_deserializer=collections__pb2.ListAliasesRequest.FromString,
                     response_serializer=collections__pb2.ListAliasesResponse.SerializeToString,
             ),
+            'CollectionClusterInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.CollectionClusterInfo,
+                    request_deserializer=collections__pb2.CollectionClusterInfoRequest.FromString,
+                    response_serializer=collections__pb2.CollectionClusterInfoResponse.SerializeToString,
+            ),
+            'UpdateCollectionClusterSetup': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateCollectionClusterSetup,
+                    request_deserializer=collections__pb2.UpdateCollectionClusterSetupRequest.FromString,
+                    response_serializer=collections__pb2.UpdateCollectionClusterSetupResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'qdrant.Collections', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -307,7 +343,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/qdrant.Collections/ListAliases',
             collections__pb2.ListAliasesRequest.SerializeToString,
             collections__pb2.ListAliasesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CollectionClusterInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qdrant.Collections/CollectionClusterInfo',
+            collections__pb2.CollectionClusterInfoRequest.SerializeToString,
+            collections__pb2.CollectionClusterInfoResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UpdateCollectionClusterSetup(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qdrant.Collections/UpdateCollectionClusterSetup',
+            collections__pb2.UpdateCollectionClusterSetupRequest.SerializeToString,
+            collections__pb2.UpdateCollectionClusterSetupResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `qdrant_client-1.1.7/qdrant_client/grpc/json_with_int_pb2.py` & `qdrant_client-1.2.0/qdrant_client/grpc/json_with_int_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/grpc/points_pb2.py` & `qdrant_client-1.2.0/qdrant_client/grpc/points_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import json_with_int_pb2 as json__with__int__pb2
 from . import collections_pb2 as collections__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cpoints.proto\x12\x06qdrant\x1a\x13json_with_int.proto\x1a\x11\x63ollections.proto\"8\n\rWriteOrdering\x12\'\n\x04type\x18\x01 \x01(\x0e\x32\x19.qdrant.WriteOrderingType\"Y\n\x0fReadConsistency\x12+\n\x04type\x18\x01 \x01(\x0e\x32\x1b.qdrant.ReadConsistencyTypeH\x00\x12\x10\n\x06\x66\x61\x63tor\x18\x02 \x01(\x04H\x00\x42\x07\n\x05value\"<\n\x07PointId\x12\r\n\x03num\x18\x01 \x01(\x04H\x00\x12\x0e\n\x04uuid\x18\x02 \x01(\tH\x00\x42\x12\n\x10point_id_options\"\x16\n\x06Vector\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\"\xa3\x01\n\x0cUpsertPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12#\n\x06points\x18\x03 \x03(\x0b\x32\x13.qdrant.PointStruct\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xa6\x01\n\x0c\x44\x65letePoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\x91\x02\n\tGetPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1c\n\x03ids\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x0cwith_payload\x18\x04 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x05 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x00\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x06 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x01\x88\x01\x01\x42\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x03\x10\x04\"\xc9\x02\n\x10SetPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x36\n\x07payload\x18\x03 \x03(\x0b\x32%.qdrant.SetPayloadPoints.PayloadEntry\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xe3\x01\n\x13\x44\x65letePayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x0c\n\x04keys\x18\x03 \x03(\t\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xac\x01\n\x12\x43learPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xaf\x02\n\x1a\x43reateFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12*\n\nfield_type\x18\x04 \x01(\x0e\x32\x11.qdrant.FieldTypeH\x01\x88\x01\x01\x12;\n\x12\x66ield_index_params\x18\x05 \x01(\x0b\x32\x1a.qdrant.PayloadIndexParamsH\x02\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x03\x88\x01\x01\x42\x07\n\x05_waitB\r\n\x0b_field_typeB\x15\n\x13_field_index_paramsB\x0b\n\t_ordering\"\xa0\x01\n\x1a\x44\x65leteFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"(\n\x16PayloadIncludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"(\n\x16PayloadExcludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"\xa1\x01\n\x13WithPayloadSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12\x31\n\x07include\x18\x02 \x01(\x0b\x32\x1e.qdrant.PayloadIncludeSelectorH\x00\x12\x31\n\x07\x65xclude\x18\x03 \x01(\x0b\x32\x1e.qdrant.PayloadExcludeSelectorH\x00\x42\x12\n\x10selector_options\"\x82\x01\n\x0cNamedVectors\x12\x32\n\x07vectors\x18\x01 \x03(\x0b\x32!.qdrant.NamedVectors.VectorsEntry\x1a>\n\x0cVectorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.qdrant.Vector:\x02\x38\x01\"g\n\x07Vectors\x12 \n\x06vector\x18\x01 \x01(\x0b\x32\x0e.qdrant.VectorH\x00\x12\'\n\x07vectors\x18\x02 \x01(\x0b\x32\x14.qdrant.NamedVectorsH\x00\x42\x11\n\x0fvectors_options\" \n\x0fVectorsSelector\x12\r\n\x05names\x18\x01 \x03(\t\"g\n\x13WithVectorsSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12*\n\x07include\x18\x02 \x01(\x0b\x32\x17.qdrant.VectorsSelectorH\x00\x42\x12\n\x10selector_options\"\\\n\x18QuantizationSearchParams\x12\x13\n\x06ignore\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x14\n\x07rescore\x18\x02 \x01(\x08H\x01\x88\x01\x01\x42\t\n\x07_ignoreB\n\n\x08_rescore\"\x9c\x01\n\x0cSearchParams\x12\x14\n\x07hnsw_ef\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05\x65xact\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12;\n\x0cquantization\x18\x03 \x01(\x0b\x32 .qdrant.QuantizationSearchParamsH\x02\x88\x01\x01\x42\n\n\x08_hnsw_efB\x08\n\x06_exactB\x0f\n\r_quantization\"\xd7\x03\n\x0cSearchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x0e\n\x06vector\x18\x02 \x03(\x02\x12\x1e\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x04 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x07 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x08 \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\t \x01(\x04H\x01\x88\x01\x01\x12\x18\n\x0bvector_name\x18\n \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0b \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0c \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x04\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x0e\n\x0c_vector_nameB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"\xa6\x01\n\x11SearchBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12+\n\rsearch_points\x18\x02 \x03(\x0b\x32\x14.qdrant.SearchPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"\xe5\x02\n\x0cScrollPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12$\n\x06offset\x18\x03 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x08 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x03\x88\x01\x01\x42\t\n\x07_offsetB\x08\n\x06_limitB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"S\n\x0eLookupLocation\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x18\n\x0bvector_name\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_vector_name\"\xc6\x04\n\x0fRecommendPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12!\n\x08positive\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12!\n\x08negative\x18\x03 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x1e\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x05 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x08 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\t \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\n \x01(\x04H\x01\x88\x01\x01\x12\x12\n\x05using\x18\x0b \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0c \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x30\n\x0blookup_from\x18\r \x01(\x0b\x32\x16.qdrant.LookupLocationH\x04\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0e \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x05\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x08\n\x06_usingB\x0f\n\r_with_vectorsB\x0e\n\x0c_lookup_fromB\x13\n\x11_read_consistencyJ\x04\x08\x06\x10\x07\"\xaf\x01\n\x14RecommendBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x10recommend_points\x18\x02 \x03(\x0b\x32\x17.qdrant.RecommendPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"d\n\x0b\x43ountPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12\x12\n\x05\x65xact\x18\x03 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_exact\"M\n\x17PointsOperationResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.UpdateResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"J\n\x0cUpdateResult\x12\x14\n\x0coperation_id\x18\x01 \x01(\x04\x12$\n\x06status\x18\x02 \x01(\x0e\x32\x14.qdrant.UpdateStatus\"\xf5\x01\n\x0bScoredPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x02 \x03(\x0b\x32 .qdrant.ScoredPoint.PayloadEntry\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x0f\n\x07version\x18\x05 \x01(\x04\x12%\n\x07vectors\x18\x06 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x04\x10\x05\"C\n\x0eSearchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"2\n\x0b\x42\x61tchResult\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\"H\n\x13SearchBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"B\n\rCountResponse\x12#\n\x06result\x18\x01 \x01(\x0b\x32\x13.qdrant.CountResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"\x8b\x01\n\x0eScrollResponse\x12.\n\x10next_page_offset\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12&\n\x06result\x18\x02 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x03 \x01(\x01\x42\x13\n\x11_next_page_offset\"\x1c\n\x0b\x43ountResult\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\"\xdb\x01\n\x0eRetrievedPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x34\n\x07payload\x18\x02 \x03(\x0b\x32#.qdrant.RetrievedPoint.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x03\x10\x04\"C\n\x0bGetResponse\x12&\n\x06result\x18\x01 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"F\n\x11RecommendResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"K\n\x16RecommendBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"q\n\x06\x46ilter\x12!\n\x06should\x18\x01 \x03(\x0b\x32\x11.qdrant.Condition\x12\x1f\n\x04must\x18\x02 \x03(\x0b\x32\x11.qdrant.Condition\x12#\n\x08must_not\x18\x03 \x03(\x0b\x32\x11.qdrant.Condition\"\xee\x01\n\tCondition\x12\'\n\x05\x66ield\x18\x01 \x01(\x0b\x32\x16.qdrant.FieldConditionH\x00\x12,\n\x08is_empty\x18\x02 \x01(\x0b\x32\x18.qdrant.IsEmptyConditionH\x00\x12(\n\x06has_id\x18\x03 \x01(\x0b\x32\x16.qdrant.HasIdConditionH\x00\x12 \n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x12*\n\x07is_null\x18\x05 \x01(\x0b\x32\x17.qdrant.IsNullConditionH\x00\x42\x12\n\x10\x63ondition_one_of\"\x1f\n\x10IsEmptyCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x1e\n\x0fIsNullCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\"1\n\x0eHasIdCondition\x12\x1f\n\x06has_id\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\"\xdd\x01\n\x0e\x46ieldCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05match\x18\x02 \x01(\x0b\x32\r.qdrant.Match\x12\x1c\n\x05range\x18\x03 \x01(\x0b\x32\r.qdrant.Range\x12\x30\n\x10geo_bounding_box\x18\x04 \x01(\x0b\x32\x16.qdrant.GeoBoundingBox\x12%\n\ngeo_radius\x18\x05 \x01(\x0b\x32\x11.qdrant.GeoRadius\x12)\n\x0cvalues_count\x18\x06 \x01(\x0b\x32\x13.qdrant.ValuesCount\"\xba\x01\n\x05Match\x12\x11\n\x07keyword\x18\x01 \x01(\tH\x00\x12\x11\n\x07integer\x18\x02 \x01(\x03H\x00\x12\x11\n\x07\x62oolean\x18\x03 \x01(\x08H\x00\x12\x0e\n\x04text\x18\x04 \x01(\tH\x00\x12+\n\x08keywords\x18\x05 \x01(\x0b\x32\x17.qdrant.RepeatedStringsH\x00\x12,\n\x08integers\x18\x06 \x01(\x0b\x32\x18.qdrant.RepeatedIntegersH\x00\x42\r\n\x0bmatch_value\"\"\n\x0fRepeatedStrings\x12\x0f\n\x07strings\x18\x01 \x03(\t\"$\n\x10RepeatedIntegers\x12\x10\n\x08integers\x18\x01 \x03(\x03\"k\n\x05Range\x12\x0f\n\x02lt\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x01H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x01H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"\\\n\x0eGeoBoundingBox\x12\"\n\x08top_left\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12&\n\x0c\x62ottom_right\x18\x02 \x01(\x0b\x32\x10.qdrant.GeoPoint\"=\n\tGeoRadius\x12 \n\x06\x63\x65nter\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12\x0e\n\x06radius\x18\x02 \x01(\x02\"q\n\x0bValuesCount\x12\x0f\n\x02lt\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x04H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"u\n\x0ePointsSelector\x12\'\n\x06points\x18\x01 \x01(\x0b\x32\x15.qdrant.PointsIdsListH\x00\x12 \n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x42\x18\n\x16points_selector_one_of\"-\n\rPointsIdsList\x12\x1c\n\x03ids\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\"\xd5\x01\n\x0bPointStruct\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x03 \x03(\x0b\x32 .qdrant.PointStruct.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x02\x10\x03\"$\n\x08GeoPoint\x12\x0b\n\x03lon\x18\x01 \x01(\x01\x12\x0b\n\x03lat\x18\x02 \x01(\x01*5\n\x11WriteOrderingType\x12\x08\n\x04Weak\x10\x00\x12\n\n\x06Medium\x10\x01\x12\n\n\x06Strong\x10\x02*8\n\x13ReadConsistencyType\x12\x07\n\x03\x41ll\x10\x00\x12\x0c\n\x08Majority\x10\x01\x12\n\n\x06Quorum\x10\x02*p\n\tFieldType\x12\x14\n\x10\x46ieldTypeKeyword\x10\x00\x12\x14\n\x10\x46ieldTypeInteger\x10\x01\x12\x12\n\x0e\x46ieldTypeFloat\x10\x02\x12\x10\n\x0c\x46ieldTypeGeo\x10\x03\x12\x11\n\rFieldTypeText\x10\x04*H\n\x0cUpdateStatus\x12\x17\n\x13UnknownUpdateStatus\x10\x00\x12\x10\n\x0c\x41\x63knowledged\x10\x01\x12\r\n\tCompleted\x10\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cpoints.proto\x12\x06qdrant\x1a\x13json_with_int.proto\x1a\x11\x63ollections.proto\"8\n\rWriteOrdering\x12\'\n\x04type\x18\x01 \x01(\x0e\x32\x19.qdrant.WriteOrderingType\"Y\n\x0fReadConsistency\x12+\n\x04type\x18\x01 \x01(\x0e\x32\x1b.qdrant.ReadConsistencyTypeH\x00\x12\x10\n\x06\x66\x61\x63tor\x18\x02 \x01(\x04H\x00\x42\x07\n\x05value\"<\n\x07PointId\x12\r\n\x03num\x18\x01 \x01(\x04H\x00\x12\x0e\n\x04uuid\x18\x02 \x01(\tH\x00\x42\x12\n\x10point_id_options\"\x16\n\x06Vector\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\"\xa3\x01\n\x0cUpsertPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12#\n\x06points\x18\x03 \x03(\x0b\x32\x13.qdrant.PointStruct\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xa6\x01\n\x0c\x44\x65letePoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\x91\x02\n\tGetPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1c\n\x03ids\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x0cwith_payload\x18\x04 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x05 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x00\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x06 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x01\x88\x01\x01\x42\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x03\x10\x04\"\xaa\x01\n\x12UpdatePointVectors\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12$\n\x06points\x18\x03 \x03(\x0b\x32\x14.qdrant.PointVectors\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"M\n\x0cPointVectors\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12 \n\x07vectors\x18\x02 \x01(\x0b\x32\x0f.qdrant.Vectors\"\xdf\x01\n\x12\x44\x65letePointVectors\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12/\n\x0fpoints_selector\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12(\n\x07vectors\x18\x04 \x01(\x0b\x32\x17.qdrant.VectorsSelector\x12,\n\x08ordering\x18\x05 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xc9\x02\n\x10SetPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x36\n\x07payload\x18\x03 \x03(\x0b\x32%.qdrant.SetPayloadPoints.PayloadEntry\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xe3\x01\n\x13\x44\x65letePayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x0c\n\x04keys\x18\x03 \x03(\t\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xac\x01\n\x12\x43learPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xaf\x02\n\x1a\x43reateFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12*\n\nfield_type\x18\x04 \x01(\x0e\x32\x11.qdrant.FieldTypeH\x01\x88\x01\x01\x12;\n\x12\x66ield_index_params\x18\x05 \x01(\x0b\x32\x1a.qdrant.PayloadIndexParamsH\x02\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x03\x88\x01\x01\x42\x07\n\x05_waitB\r\n\x0b_field_typeB\x15\n\x13_field_index_paramsB\x0b\n\t_ordering\"\xa0\x01\n\x1a\x44\x65leteFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"(\n\x16PayloadIncludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"(\n\x16PayloadExcludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"\xa1\x01\n\x13WithPayloadSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12\x31\n\x07include\x18\x02 \x01(\x0b\x32\x1e.qdrant.PayloadIncludeSelectorH\x00\x12\x31\n\x07\x65xclude\x18\x03 \x01(\x0b\x32\x1e.qdrant.PayloadExcludeSelectorH\x00\x42\x12\n\x10selector_options\"\x82\x01\n\x0cNamedVectors\x12\x32\n\x07vectors\x18\x01 \x03(\x0b\x32!.qdrant.NamedVectors.VectorsEntry\x1a>\n\x0cVectorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.qdrant.Vector:\x02\x38\x01\"g\n\x07Vectors\x12 \n\x06vector\x18\x01 \x01(\x0b\x32\x0e.qdrant.VectorH\x00\x12\'\n\x07vectors\x18\x02 \x01(\x0b\x32\x14.qdrant.NamedVectorsH\x00\x42\x11\n\x0fvectors_options\" \n\x0fVectorsSelector\x12\r\n\x05names\x18\x01 \x03(\t\"g\n\x13WithVectorsSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12*\n\x07include\x18\x02 \x01(\x0b\x32\x17.qdrant.VectorsSelectorH\x00\x42\x12\n\x10selector_options\"\\\n\x18QuantizationSearchParams\x12\x13\n\x06ignore\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x14\n\x07rescore\x18\x02 \x01(\x08H\x01\x88\x01\x01\x42\t\n\x07_ignoreB\n\n\x08_rescore\"\x9c\x01\n\x0cSearchParams\x12\x14\n\x07hnsw_ef\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05\x65xact\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12;\n\x0cquantization\x18\x03 \x01(\x0b\x32 .qdrant.QuantizationSearchParamsH\x02\x88\x01\x01\x42\n\n\x08_hnsw_efB\x08\n\x06_exactB\x0f\n\r_quantization\"\xd7\x03\n\x0cSearchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x0e\n\x06vector\x18\x02 \x03(\x02\x12\x1e\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x04 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x07 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x08 \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\t \x01(\x04H\x01\x88\x01\x01\x12\x18\n\x0bvector_name\x18\n \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0b \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0c \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x04\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x0e\n\x0c_vector_nameB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"\xa6\x01\n\x11SearchBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12+\n\rsearch_points\x18\x02 \x03(\x0b\x32\x14.qdrant.SearchPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"\xdc\x03\n\x11SearchPointGroups\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x0e\n\x06vector\x18\x02 \x03(\x02\x12\x1e\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x04 \x01(\r\x12\x31\n\x0cwith_payload\x18\x05 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x06 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x07 \x01(\x02H\x00\x88\x01\x01\x12\x18\n\x0bvector_name\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\t \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x10\n\x08group_by\x18\n \x01(\t\x12\x12\n\ngroup_size\x18\x0b \x01(\r\x12\x36\n\x10read_consistency\x18\x0c \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x03\x88\x01\x01\x42\x12\n\x10_score_thresholdB\x0e\n\x0c_vector_nameB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistency\"\xe5\x02\n\x0cScrollPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12$\n\x06offset\x18\x03 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x08 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x03\x88\x01\x01\x42\t\n\x07_offsetB\x08\n\x06_limitB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"S\n\x0eLookupLocation\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x18\n\x0bvector_name\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_vector_name\"\xc6\x04\n\x0fRecommendPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12!\n\x08positive\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12!\n\x08negative\x18\x03 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x1e\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x05 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x08 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\t \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\n \x01(\x04H\x01\x88\x01\x01\x12\x12\n\x05using\x18\x0b \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0c \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x30\n\x0blookup_from\x18\r \x01(\x0b\x32\x16.qdrant.LookupLocationH\x04\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0e \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x05\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x08\n\x06_usingB\x0f\n\r_with_vectorsB\x0e\n\x0c_lookup_fromB\x13\n\x11_read_consistencyJ\x04\x08\x06\x10\x07\"\xaf\x01\n\x14RecommendBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x10recommend_points\x18\x02 \x03(\x0b\x32\x17.qdrant.RecommendPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"\xcb\x04\n\x14RecommendPointGroups\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12!\n\x08positive\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12!\n\x08negative\x18\x03 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x1e\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x05 \x01(\r\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x07 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x08 \x01(\x02H\x00\x88\x01\x01\x12\x12\n\x05using\x18\t \x01(\tH\x01\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\n \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x30\n\x0blookup_from\x18\x0b \x01(\x0b\x32\x16.qdrant.LookupLocationH\x03\x88\x01\x01\x12\x10\n\x08group_by\x18\x0c \x01(\t\x12\x12\n\ngroup_size\x18\r \x01(\r\x12\x36\n\x10read_consistency\x18\x0e \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x04\x88\x01\x01\x42\x12\n\x10_score_thresholdB\x08\n\x06_usingB\x0f\n\r_with_vectorsB\x0e\n\x0c_lookup_fromB\x13\n\x11_read_consistency\"d\n\x0b\x43ountPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12\x12\n\x05\x65xact\x18\x03 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_exact\"M\n\x17PointsOperationResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.UpdateResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"J\n\x0cUpdateResult\x12\x14\n\x0coperation_id\x18\x01 \x01(\x04\x12$\n\x06status\x18\x02 \x01(\x0e\x32\x14.qdrant.UpdateStatus\"\xf5\x01\n\x0bScoredPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x02 \x03(\x0b\x32 .qdrant.ScoredPoint.PayloadEntry\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x0f\n\x07version\x18\x05 \x01(\x04\x12%\n\x07vectors\x18\x06 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x04\x10\x05\"\\\n\x07GroupId\x12\x18\n\x0eunsigned_value\x18\x01 \x01(\x04H\x00\x12\x17\n\rinteger_value\x18\x02 \x01(\x03H\x00\x12\x16\n\x0cstring_value\x18\x03 \x01(\tH\x00\x42\x06\n\x04kind\"L\n\nPointGroup\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.GroupId\x12!\n\x04hits\x18\x02 \x03(\x0b\x32\x13.qdrant.ScoredPoint\"2\n\x0cGroupsResult\x12\"\n\x06groups\x18\x01 \x03(\x0b\x32\x12.qdrant.PointGroup\"C\n\x0eSearchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"2\n\x0b\x42\x61tchResult\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\"H\n\x13SearchBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"J\n\x14SearchGroupsResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.GroupsResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"B\n\rCountResponse\x12#\n\x06result\x18\x01 \x01(\x0b\x32\x13.qdrant.CountResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"\x8b\x01\n\x0eScrollResponse\x12.\n\x10next_page_offset\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12&\n\x06result\x18\x02 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x03 \x01(\x01\x42\x13\n\x11_next_page_offset\"\x1c\n\x0b\x43ountResult\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\"\xdb\x01\n\x0eRetrievedPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x34\n\x07payload\x18\x02 \x03(\x0b\x32#.qdrant.RetrievedPoint.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x03\x10\x04\"C\n\x0bGetResponse\x12&\n\x06result\x18\x01 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"F\n\x11RecommendResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"K\n\x16RecommendBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"M\n\x17RecommendGroupsResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.GroupsResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"q\n\x06\x46ilter\x12!\n\x06should\x18\x01 \x03(\x0b\x32\x11.qdrant.Condition\x12\x1f\n\x04must\x18\x02 \x03(\x0b\x32\x11.qdrant.Condition\x12#\n\x08must_not\x18\x03 \x03(\x0b\x32\x11.qdrant.Condition\"\x99\x02\n\tCondition\x12\'\n\x05\x66ield\x18\x01 \x01(\x0b\x32\x16.qdrant.FieldConditionH\x00\x12,\n\x08is_empty\x18\x02 \x01(\x0b\x32\x18.qdrant.IsEmptyConditionH\x00\x12(\n\x06has_id\x18\x03 \x01(\x0b\x32\x16.qdrant.HasIdConditionH\x00\x12 \n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x12*\n\x07is_null\x18\x05 \x01(\x0b\x32\x17.qdrant.IsNullConditionH\x00\x12)\n\x06nested\x18\x06 \x01(\x0b\x32\x17.qdrant.NestedConditionH\x00\x42\x12\n\x10\x63ondition_one_of\"\x1f\n\x10IsEmptyCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x1e\n\x0fIsNullCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\"1\n\x0eHasIdCondition\x12\x1f\n\x06has_id\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\">\n\x0fNestedCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\"\xdd\x01\n\x0e\x46ieldCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05match\x18\x02 \x01(\x0b\x32\r.qdrant.Match\x12\x1c\n\x05range\x18\x03 \x01(\x0b\x32\r.qdrant.Range\x12\x30\n\x10geo_bounding_box\x18\x04 \x01(\x0b\x32\x16.qdrant.GeoBoundingBox\x12%\n\ngeo_radius\x18\x05 \x01(\x0b\x32\x11.qdrant.GeoRadius\x12)\n\x0cvalues_count\x18\x06 \x01(\x0b\x32\x13.qdrant.ValuesCount\"\xa3\x02\n\x05Match\x12\x11\n\x07keyword\x18\x01 \x01(\tH\x00\x12\x11\n\x07integer\x18\x02 \x01(\x03H\x00\x12\x11\n\x07\x62oolean\x18\x03 \x01(\x08H\x00\x12\x0e\n\x04text\x18\x04 \x01(\tH\x00\x12+\n\x08keywords\x18\x05 \x01(\x0b\x32\x17.qdrant.RepeatedStringsH\x00\x12,\n\x08integers\x18\x06 \x01(\x0b\x32\x18.qdrant.RepeatedIntegersH\x00\x12\x33\n\x0f\x65xcept_integers\x18\x07 \x01(\x0b\x32\x18.qdrant.RepeatedIntegersH\x00\x12\x32\n\x0f\x65xcept_keywords\x18\x08 \x01(\x0b\x32\x17.qdrant.RepeatedStringsH\x00\x42\r\n\x0bmatch_value\"\"\n\x0fRepeatedStrings\x12\x0f\n\x07strings\x18\x01 \x03(\t\"$\n\x10RepeatedIntegers\x12\x10\n\x08integers\x18\x01 \x03(\x03\"k\n\x05Range\x12\x0f\n\x02lt\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x01H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x01H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"\\\n\x0eGeoBoundingBox\x12\"\n\x08top_left\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12&\n\x0c\x62ottom_right\x18\x02 \x01(\x0b\x32\x10.qdrant.GeoPoint\"=\n\tGeoRadius\x12 \n\x06\x63\x65nter\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12\x0e\n\x06radius\x18\x02 \x01(\x02\"q\n\x0bValuesCount\x12\x0f\n\x02lt\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x04H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"u\n\x0ePointsSelector\x12\'\n\x06points\x18\x01 \x01(\x0b\x32\x15.qdrant.PointsIdsListH\x00\x12 \n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x42\x18\n\x16points_selector_one_of\"-\n\rPointsIdsList\x12\x1c\n\x03ids\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\"\xd5\x01\n\x0bPointStruct\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x03 \x03(\x0b\x32 .qdrant.PointStruct.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x02\x10\x03\"$\n\x08GeoPoint\x12\x0b\n\x03lon\x18\x01 \x01(\x01\x12\x0b\n\x03lat\x18\x02 \x01(\x01*5\n\x11WriteOrderingType\x12\x08\n\x04Weak\x10\x00\x12\n\n\x06Medium\x10\x01\x12\n\n\x06Strong\x10\x02*8\n\x13ReadConsistencyType\x12\x07\n\x03\x41ll\x10\x00\x12\x0c\n\x08Majority\x10\x01\x12\n\n\x06Quorum\x10\x02*p\n\tFieldType\x12\x14\n\x10\x46ieldTypeKeyword\x10\x00\x12\x14\n\x10\x46ieldTypeInteger\x10\x01\x12\x12\n\x0e\x46ieldTypeFloat\x10\x02\x12\x10\n\x0c\x46ieldTypeGeo\x10\x03\x12\x11\n\rFieldTypeText\x10\x04*H\n\x0cUpdateStatus\x12\x17\n\x13UnknownUpdateStatus\x10\x00\x12\x10\n\x0c\x41\x63knowledged\x10\x01\x12\r\n\tCompleted\x10\x02\x62\x06proto3')
 
 _WRITEORDERINGTYPE = DESCRIPTOR.enum_types_by_name['WriteOrderingType']
 WriteOrderingType = enum_type_wrapper.EnumTypeWrapper(_WRITEORDERINGTYPE)
 _READCONSISTENCYTYPE = DESCRIPTOR.enum_types_by_name['ReadConsistencyType']
 ReadConsistencyType = enum_type_wrapper.EnumTypeWrapper(_READCONSISTENCYTYPE)
 _FIELDTYPE = DESCRIPTOR.enum_types_by_name['FieldType']
 FieldType = enum_type_wrapper.EnumTypeWrapper(_FIELDTYPE)
@@ -46,14 +46,17 @@
 _WRITEORDERING = DESCRIPTOR.message_types_by_name['WriteOrdering']
 _READCONSISTENCY = DESCRIPTOR.message_types_by_name['ReadConsistency']
 _POINTID = DESCRIPTOR.message_types_by_name['PointId']
 _VECTOR = DESCRIPTOR.message_types_by_name['Vector']
 _UPSERTPOINTS = DESCRIPTOR.message_types_by_name['UpsertPoints']
 _DELETEPOINTS = DESCRIPTOR.message_types_by_name['DeletePoints']
 _GETPOINTS = DESCRIPTOR.message_types_by_name['GetPoints']
+_UPDATEPOINTVECTORS = DESCRIPTOR.message_types_by_name['UpdatePointVectors']
+_POINTVECTORS = DESCRIPTOR.message_types_by_name['PointVectors']
+_DELETEPOINTVECTORS = DESCRIPTOR.message_types_by_name['DeletePointVectors']
 _SETPAYLOADPOINTS = DESCRIPTOR.message_types_by_name['SetPayloadPoints']
 _SETPAYLOADPOINTS_PAYLOADENTRY = _SETPAYLOADPOINTS.nested_types_by_name['PayloadEntry']
 _DELETEPAYLOADPOINTS = DESCRIPTOR.message_types_by_name['DeletePayloadPoints']
 _CLEARPAYLOADPOINTS = DESCRIPTOR.message_types_by_name['ClearPayloadPoints']
 _CREATEFIELDINDEXCOLLECTION = DESCRIPTOR.message_types_by_name['CreateFieldIndexCollection']
 _DELETEFIELDINDEXCOLLECTION = DESCRIPTOR.message_types_by_name['DeleteFieldIndexCollection']
 _PAYLOADINCLUDESELECTOR = DESCRIPTOR.message_types_by_name['PayloadIncludeSelector']
@@ -64,39 +67,47 @@
 _VECTORS = DESCRIPTOR.message_types_by_name['Vectors']
 _VECTORSSELECTOR = DESCRIPTOR.message_types_by_name['VectorsSelector']
 _WITHVECTORSSELECTOR = DESCRIPTOR.message_types_by_name['WithVectorsSelector']
 _QUANTIZATIONSEARCHPARAMS = DESCRIPTOR.message_types_by_name['QuantizationSearchParams']
 _SEARCHPARAMS = DESCRIPTOR.message_types_by_name['SearchParams']
 _SEARCHPOINTS = DESCRIPTOR.message_types_by_name['SearchPoints']
 _SEARCHBATCHPOINTS = DESCRIPTOR.message_types_by_name['SearchBatchPoints']
+_SEARCHPOINTGROUPS = DESCRIPTOR.message_types_by_name['SearchPointGroups']
 _SCROLLPOINTS = DESCRIPTOR.message_types_by_name['ScrollPoints']
 _LOOKUPLOCATION = DESCRIPTOR.message_types_by_name['LookupLocation']
 _RECOMMENDPOINTS = DESCRIPTOR.message_types_by_name['RecommendPoints']
 _RECOMMENDBATCHPOINTS = DESCRIPTOR.message_types_by_name['RecommendBatchPoints']
+_RECOMMENDPOINTGROUPS = DESCRIPTOR.message_types_by_name['RecommendPointGroups']
 _COUNTPOINTS = DESCRIPTOR.message_types_by_name['CountPoints']
 _POINTSOPERATIONRESPONSE = DESCRIPTOR.message_types_by_name['PointsOperationResponse']
 _UPDATERESULT = DESCRIPTOR.message_types_by_name['UpdateResult']
 _SCOREDPOINT = DESCRIPTOR.message_types_by_name['ScoredPoint']
 _SCOREDPOINT_PAYLOADENTRY = _SCOREDPOINT.nested_types_by_name['PayloadEntry']
+_GROUPID = DESCRIPTOR.message_types_by_name['GroupId']
+_POINTGROUP = DESCRIPTOR.message_types_by_name['PointGroup']
+_GROUPSRESULT = DESCRIPTOR.message_types_by_name['GroupsResult']
 _SEARCHRESPONSE = DESCRIPTOR.message_types_by_name['SearchResponse']
 _BATCHRESULT = DESCRIPTOR.message_types_by_name['BatchResult']
 _SEARCHBATCHRESPONSE = DESCRIPTOR.message_types_by_name['SearchBatchResponse']
+_SEARCHGROUPSRESPONSE = DESCRIPTOR.message_types_by_name['SearchGroupsResponse']
 _COUNTRESPONSE = DESCRIPTOR.message_types_by_name['CountResponse']
 _SCROLLRESPONSE = DESCRIPTOR.message_types_by_name['ScrollResponse']
 _COUNTRESULT = DESCRIPTOR.message_types_by_name['CountResult']
 _RETRIEVEDPOINT = DESCRIPTOR.message_types_by_name['RetrievedPoint']
 _RETRIEVEDPOINT_PAYLOADENTRY = _RETRIEVEDPOINT.nested_types_by_name['PayloadEntry']
 _GETRESPONSE = DESCRIPTOR.message_types_by_name['GetResponse']
 _RECOMMENDRESPONSE = DESCRIPTOR.message_types_by_name['RecommendResponse']
 _RECOMMENDBATCHRESPONSE = DESCRIPTOR.message_types_by_name['RecommendBatchResponse']
+_RECOMMENDGROUPSRESPONSE = DESCRIPTOR.message_types_by_name['RecommendGroupsResponse']
 _FILTER = DESCRIPTOR.message_types_by_name['Filter']
 _CONDITION = DESCRIPTOR.message_types_by_name['Condition']
 _ISEMPTYCONDITION = DESCRIPTOR.message_types_by_name['IsEmptyCondition']
 _ISNULLCONDITION = DESCRIPTOR.message_types_by_name['IsNullCondition']
 _HASIDCONDITION = DESCRIPTOR.message_types_by_name['HasIdCondition']
+_NESTEDCONDITION = DESCRIPTOR.message_types_by_name['NestedCondition']
 _FIELDCONDITION = DESCRIPTOR.message_types_by_name['FieldCondition']
 _MATCH = DESCRIPTOR.message_types_by_name['Match']
 _REPEATEDSTRINGS = DESCRIPTOR.message_types_by_name['RepeatedStrings']
 _REPEATEDINTEGERS = DESCRIPTOR.message_types_by_name['RepeatedIntegers']
 _RANGE = DESCRIPTOR.message_types_by_name['Range']
 _GEOBOUNDINGBOX = DESCRIPTOR.message_types_by_name['GeoBoundingBox']
 _GEORADIUS = DESCRIPTOR.message_types_by_name['GeoRadius']
@@ -151,14 +162,35 @@
 GetPoints = _reflection.GeneratedProtocolMessageType('GetPoints', (_message.Message,), {
   'DESCRIPTOR' : _GETPOINTS,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.GetPoints)
   })
 _sym_db.RegisterMessage(GetPoints)
 
+UpdatePointVectors = _reflection.GeneratedProtocolMessageType('UpdatePointVectors', (_message.Message,), {
+  'DESCRIPTOR' : _UPDATEPOINTVECTORS,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.UpdatePointVectors)
+  })
+_sym_db.RegisterMessage(UpdatePointVectors)
+
+PointVectors = _reflection.GeneratedProtocolMessageType('PointVectors', (_message.Message,), {
+  'DESCRIPTOR' : _POINTVECTORS,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.PointVectors)
+  })
+_sym_db.RegisterMessage(PointVectors)
+
+DeletePointVectors = _reflection.GeneratedProtocolMessageType('DeletePointVectors', (_message.Message,), {
+  'DESCRIPTOR' : _DELETEPOINTVECTORS,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.DeletePointVectors)
+  })
+_sym_db.RegisterMessage(DeletePointVectors)
+
 SetPayloadPoints = _reflection.GeneratedProtocolMessageType('SetPayloadPoints', (_message.Message,), {
 
   'PayloadEntry' : _reflection.GeneratedProtocolMessageType('PayloadEntry', (_message.Message,), {
     'DESCRIPTOR' : _SETPAYLOADPOINTS_PAYLOADENTRY,
     '__module__' : 'points_pb2'
     # @@protoc_insertion_point(class_scope:qdrant.SetPayloadPoints.PayloadEntry)
     })
@@ -279,14 +311,21 @@
 SearchBatchPoints = _reflection.GeneratedProtocolMessageType('SearchBatchPoints', (_message.Message,), {
   'DESCRIPTOR' : _SEARCHBATCHPOINTS,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.SearchBatchPoints)
   })
 _sym_db.RegisterMessage(SearchBatchPoints)
 
+SearchPointGroups = _reflection.GeneratedProtocolMessageType('SearchPointGroups', (_message.Message,), {
+  'DESCRIPTOR' : _SEARCHPOINTGROUPS,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.SearchPointGroups)
+  })
+_sym_db.RegisterMessage(SearchPointGroups)
+
 ScrollPoints = _reflection.GeneratedProtocolMessageType('ScrollPoints', (_message.Message,), {
   'DESCRIPTOR' : _SCROLLPOINTS,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.ScrollPoints)
   })
 _sym_db.RegisterMessage(ScrollPoints)
 
@@ -307,14 +346,21 @@
 RecommendBatchPoints = _reflection.GeneratedProtocolMessageType('RecommendBatchPoints', (_message.Message,), {
   'DESCRIPTOR' : _RECOMMENDBATCHPOINTS,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.RecommendBatchPoints)
   })
 _sym_db.RegisterMessage(RecommendBatchPoints)
 
+RecommendPointGroups = _reflection.GeneratedProtocolMessageType('RecommendPointGroups', (_message.Message,), {
+  'DESCRIPTOR' : _RECOMMENDPOINTGROUPS,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.RecommendPointGroups)
+  })
+_sym_db.RegisterMessage(RecommendPointGroups)
+
 CountPoints = _reflection.GeneratedProtocolMessageType('CountPoints', (_message.Message,), {
   'DESCRIPTOR' : _COUNTPOINTS,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.CountPoints)
   })
 _sym_db.RegisterMessage(CountPoints)
 
@@ -343,14 +389,35 @@
   'DESCRIPTOR' : _SCOREDPOINT,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.ScoredPoint)
   })
 _sym_db.RegisterMessage(ScoredPoint)
 _sym_db.RegisterMessage(ScoredPoint.PayloadEntry)
 
+GroupId = _reflection.GeneratedProtocolMessageType('GroupId', (_message.Message,), {
+  'DESCRIPTOR' : _GROUPID,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.GroupId)
+  })
+_sym_db.RegisterMessage(GroupId)
+
+PointGroup = _reflection.GeneratedProtocolMessageType('PointGroup', (_message.Message,), {
+  'DESCRIPTOR' : _POINTGROUP,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.PointGroup)
+  })
+_sym_db.RegisterMessage(PointGroup)
+
+GroupsResult = _reflection.GeneratedProtocolMessageType('GroupsResult', (_message.Message,), {
+  'DESCRIPTOR' : _GROUPSRESULT,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.GroupsResult)
+  })
+_sym_db.RegisterMessage(GroupsResult)
+
 SearchResponse = _reflection.GeneratedProtocolMessageType('SearchResponse', (_message.Message,), {
   'DESCRIPTOR' : _SEARCHRESPONSE,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.SearchResponse)
   })
 _sym_db.RegisterMessage(SearchResponse)
 
@@ -364,14 +431,21 @@
 SearchBatchResponse = _reflection.GeneratedProtocolMessageType('SearchBatchResponse', (_message.Message,), {
   'DESCRIPTOR' : _SEARCHBATCHRESPONSE,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.SearchBatchResponse)
   })
 _sym_db.RegisterMessage(SearchBatchResponse)
 
+SearchGroupsResponse = _reflection.GeneratedProtocolMessageType('SearchGroupsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _SEARCHGROUPSRESPONSE,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.SearchGroupsResponse)
+  })
+_sym_db.RegisterMessage(SearchGroupsResponse)
+
 CountResponse = _reflection.GeneratedProtocolMessageType('CountResponse', (_message.Message,), {
   'DESCRIPTOR' : _COUNTRESPONSE,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.CountResponse)
   })
 _sym_db.RegisterMessage(CountResponse)
 
@@ -421,14 +495,21 @@
 RecommendBatchResponse = _reflection.GeneratedProtocolMessageType('RecommendBatchResponse', (_message.Message,), {
   'DESCRIPTOR' : _RECOMMENDBATCHRESPONSE,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.RecommendBatchResponse)
   })
 _sym_db.RegisterMessage(RecommendBatchResponse)
 
+RecommendGroupsResponse = _reflection.GeneratedProtocolMessageType('RecommendGroupsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _RECOMMENDGROUPSRESPONSE,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.RecommendGroupsResponse)
+  })
+_sym_db.RegisterMessage(RecommendGroupsResponse)
+
 Filter = _reflection.GeneratedProtocolMessageType('Filter', (_message.Message,), {
   'DESCRIPTOR' : _FILTER,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.Filter)
   })
 _sym_db.RegisterMessage(Filter)
 
@@ -456,14 +537,21 @@
 HasIdCondition = _reflection.GeneratedProtocolMessageType('HasIdCondition', (_message.Message,), {
   'DESCRIPTOR' : _HASIDCONDITION,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.HasIdCondition)
   })
 _sym_db.RegisterMessage(HasIdCondition)
 
+NestedCondition = _reflection.GeneratedProtocolMessageType('NestedCondition', (_message.Message,), {
+  'DESCRIPTOR' : _NESTEDCONDITION,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.NestedCondition)
+  })
+_sym_db.RegisterMessage(NestedCondition)
+
 FieldCondition = _reflection.GeneratedProtocolMessageType('FieldCondition', (_message.Message,), {
   'DESCRIPTOR' : _FIELDCONDITION,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.FieldCondition)
   })
 _sym_db.RegisterMessage(FieldCondition)
 
@@ -561,142 +649,164 @@
   _NAMEDVECTORS_VECTORSENTRY._serialized_options = b'8\001'
   _SCOREDPOINT_PAYLOADENTRY._options = None
   _SCOREDPOINT_PAYLOADENTRY._serialized_options = b'8\001'
   _RETRIEVEDPOINT_PAYLOADENTRY._options = None
   _RETRIEVEDPOINT_PAYLOADENTRY._serialized_options = b'8\001'
   _POINTSTRUCT_PAYLOADENTRY._options = None
   _POINTSTRUCT_PAYLOADENTRY._serialized_options = b'8\001'
-  _WRITEORDERINGTYPE._serialized_start=7985
-  _WRITEORDERINGTYPE._serialized_end=8038
-  _READCONSISTENCYTYPE._serialized_start=8040
-  _READCONSISTENCYTYPE._serialized_end=8096
-  _FIELDTYPE._serialized_start=8098
-  _FIELDTYPE._serialized_end=8210
-  _UPDATESTATUS._serialized_start=8212
-  _UPDATESTATUS._serialized_end=8284
+  _WRITEORDERINGTYPE._serialized_start=10123
+  _WRITEORDERINGTYPE._serialized_end=10176
+  _READCONSISTENCYTYPE._serialized_start=10178
+  _READCONSISTENCYTYPE._serialized_end=10234
+  _FIELDTYPE._serialized_start=10236
+  _FIELDTYPE._serialized_end=10348
+  _UPDATESTATUS._serialized_start=10350
+  _UPDATESTATUS._serialized_end=10422
   _WRITEORDERING._serialized_start=64
   _WRITEORDERING._serialized_end=120
   _READCONSISTENCY._serialized_start=122
   _READCONSISTENCY._serialized_end=211
   _POINTID._serialized_start=213
   _POINTID._serialized_end=273
   _VECTOR._serialized_start=275
   _VECTOR._serialized_end=297
   _UPSERTPOINTS._serialized_start=300
   _UPSERTPOINTS._serialized_end=463
   _DELETEPOINTS._serialized_start=466
   _DELETEPOINTS._serialized_end=632
   _GETPOINTS._serialized_start=635
   _GETPOINTS._serialized_end=908
-  _SETPAYLOADPOINTS._serialized_start=911
-  _SETPAYLOADPOINTS._serialized_end=1240
-  _SETPAYLOADPOINTS_PAYLOADENTRY._serialized_start=1131
-  _SETPAYLOADPOINTS_PAYLOADENTRY._serialized_end=1192
-  _DELETEPAYLOADPOINTS._serialized_start=1243
-  _DELETEPAYLOADPOINTS._serialized_end=1470
-  _CLEARPAYLOADPOINTS._serialized_start=1473
-  _CLEARPAYLOADPOINTS._serialized_end=1645
-  _CREATEFIELDINDEXCOLLECTION._serialized_start=1648
-  _CREATEFIELDINDEXCOLLECTION._serialized_end=1951
-  _DELETEFIELDINDEXCOLLECTION._serialized_start=1954
-  _DELETEFIELDINDEXCOLLECTION._serialized_end=2114
-  _PAYLOADINCLUDESELECTOR._serialized_start=2116
-  _PAYLOADINCLUDESELECTOR._serialized_end=2156
-  _PAYLOADEXCLUDESELECTOR._serialized_start=2158
-  _PAYLOADEXCLUDESELECTOR._serialized_end=2198
-  _WITHPAYLOADSELECTOR._serialized_start=2201
-  _WITHPAYLOADSELECTOR._serialized_end=2362
-  _NAMEDVECTORS._serialized_start=2365
-  _NAMEDVECTORS._serialized_end=2495
-  _NAMEDVECTORS_VECTORSENTRY._serialized_start=2433
-  _NAMEDVECTORS_VECTORSENTRY._serialized_end=2495
-  _VECTORS._serialized_start=2497
-  _VECTORS._serialized_end=2600
-  _VECTORSSELECTOR._serialized_start=2602
-  _VECTORSSELECTOR._serialized_end=2634
-  _WITHVECTORSSELECTOR._serialized_start=2636
-  _WITHVECTORSSELECTOR._serialized_end=2739
-  _QUANTIZATIONSEARCHPARAMS._serialized_start=2741
-  _QUANTIZATIONSEARCHPARAMS._serialized_end=2833
-  _SEARCHPARAMS._serialized_start=2836
-  _SEARCHPARAMS._serialized_end=2992
-  _SEARCHPOINTS._serialized_start=2995
-  _SEARCHPOINTS._serialized_end=3466
-  _SEARCHBATCHPOINTS._serialized_start=3469
-  _SEARCHBATCHPOINTS._serialized_end=3635
-  _SCROLLPOINTS._serialized_start=3638
-  _SCROLLPOINTS._serialized_end=3995
-  _LOOKUPLOCATION._serialized_start=3997
-  _LOOKUPLOCATION._serialized_end=4080
-  _RECOMMENDPOINTS._serialized_start=4083
-  _RECOMMENDPOINTS._serialized_end=4665
-  _RECOMMENDBATCHPOINTS._serialized_start=4668
-  _RECOMMENDBATCHPOINTS._serialized_end=4843
-  _COUNTPOINTS._serialized_start=4845
-  _COUNTPOINTS._serialized_end=4945
-  _POINTSOPERATIONRESPONSE._serialized_start=4947
-  _POINTSOPERATIONRESPONSE._serialized_end=5024
-  _UPDATERESULT._serialized_start=5026
-  _UPDATERESULT._serialized_end=5100
-  _SCOREDPOINT._serialized_start=5103
-  _SCOREDPOINT._serialized_end=5348
-  _SCOREDPOINT_PAYLOADENTRY._serialized_start=1131
-  _SCOREDPOINT_PAYLOADENTRY._serialized_end=1192
-  _SEARCHRESPONSE._serialized_start=5350
-  _SEARCHRESPONSE._serialized_end=5417
-  _BATCHRESULT._serialized_start=5419
-  _BATCHRESULT._serialized_end=5469
-  _SEARCHBATCHRESPONSE._serialized_start=5471
-  _SEARCHBATCHRESPONSE._serialized_end=5543
-  _COUNTRESPONSE._serialized_start=5545
-  _COUNTRESPONSE._serialized_end=5611
-  _SCROLLRESPONSE._serialized_start=5614
-  _SCROLLRESPONSE._serialized_end=5753
-  _COUNTRESULT._serialized_start=5755
-  _COUNTRESULT._serialized_end=5783
-  _RETRIEVEDPOINT._serialized_start=5786
-  _RETRIEVEDPOINT._serialized_end=6005
-  _RETRIEVEDPOINT_PAYLOADENTRY._serialized_start=1131
-  _RETRIEVEDPOINT_PAYLOADENTRY._serialized_end=1192
-  _GETRESPONSE._serialized_start=6007
-  _GETRESPONSE._serialized_end=6074
-  _RECOMMENDRESPONSE._serialized_start=6076
-  _RECOMMENDRESPONSE._serialized_end=6146
-  _RECOMMENDBATCHRESPONSE._serialized_start=6148
-  _RECOMMENDBATCHRESPONSE._serialized_end=6223
-  _FILTER._serialized_start=6225
-  _FILTER._serialized_end=6338
-  _CONDITION._serialized_start=6341
-  _CONDITION._serialized_end=6579
-  _ISEMPTYCONDITION._serialized_start=6581
-  _ISEMPTYCONDITION._serialized_end=6612
-  _ISNULLCONDITION._serialized_start=6614
-  _ISNULLCONDITION._serialized_end=6644
-  _HASIDCONDITION._serialized_start=6646
-  _HASIDCONDITION._serialized_end=6695
-  _FIELDCONDITION._serialized_start=6698
-  _FIELDCONDITION._serialized_end=6919
-  _MATCH._serialized_start=6922
-  _MATCH._serialized_end=7108
-  _REPEATEDSTRINGS._serialized_start=7110
-  _REPEATEDSTRINGS._serialized_end=7144
-  _REPEATEDINTEGERS._serialized_start=7146
-  _REPEATEDINTEGERS._serialized_end=7182
-  _RANGE._serialized_start=7184
-  _RANGE._serialized_end=7291
-  _GEOBOUNDINGBOX._serialized_start=7293
-  _GEOBOUNDINGBOX._serialized_end=7385
-  _GEORADIUS._serialized_start=7387
-  _GEORADIUS._serialized_end=7448
-  _VALUESCOUNT._serialized_start=7450
-  _VALUESCOUNT._serialized_end=7563
-  _POINTSSELECTOR._serialized_start=7565
-  _POINTSSELECTOR._serialized_end=7682
-  _POINTSIDSLIST._serialized_start=7684
-  _POINTSIDSLIST._serialized_end=7729
-  _POINTSTRUCT._serialized_start=7732
-  _POINTSTRUCT._serialized_end=7945
-  _POINTSTRUCT_PAYLOADENTRY._serialized_start=1131
-  _POINTSTRUCT_PAYLOADENTRY._serialized_end=1192
-  _GEOPOINT._serialized_start=7947
-  _GEOPOINT._serialized_end=7983
+  _UPDATEPOINTVECTORS._serialized_start=911
+  _UPDATEPOINTVECTORS._serialized_end=1081
+  _POINTVECTORS._serialized_start=1083
+  _POINTVECTORS._serialized_end=1160
+  _DELETEPOINTVECTORS._serialized_start=1163
+  _DELETEPOINTVECTORS._serialized_end=1386
+  _SETPAYLOADPOINTS._serialized_start=1389
+  _SETPAYLOADPOINTS._serialized_end=1718
+  _SETPAYLOADPOINTS_PAYLOADENTRY._serialized_start=1609
+  _SETPAYLOADPOINTS_PAYLOADENTRY._serialized_end=1670
+  _DELETEPAYLOADPOINTS._serialized_start=1721
+  _DELETEPAYLOADPOINTS._serialized_end=1948
+  _CLEARPAYLOADPOINTS._serialized_start=1951
+  _CLEARPAYLOADPOINTS._serialized_end=2123
+  _CREATEFIELDINDEXCOLLECTION._serialized_start=2126
+  _CREATEFIELDINDEXCOLLECTION._serialized_end=2429
+  _DELETEFIELDINDEXCOLLECTION._serialized_start=2432
+  _DELETEFIELDINDEXCOLLECTION._serialized_end=2592
+  _PAYLOADINCLUDESELECTOR._serialized_start=2594
+  _PAYLOADINCLUDESELECTOR._serialized_end=2634
+  _PAYLOADEXCLUDESELECTOR._serialized_start=2636
+  _PAYLOADEXCLUDESELECTOR._serialized_end=2676
+  _WITHPAYLOADSELECTOR._serialized_start=2679
+  _WITHPAYLOADSELECTOR._serialized_end=2840
+  _NAMEDVECTORS._serialized_start=2843
+  _NAMEDVECTORS._serialized_end=2973
+  _NAMEDVECTORS_VECTORSENTRY._serialized_start=2911
+  _NAMEDVECTORS_VECTORSENTRY._serialized_end=2973
+  _VECTORS._serialized_start=2975
+  _VECTORS._serialized_end=3078
+  _VECTORSSELECTOR._serialized_start=3080
+  _VECTORSSELECTOR._serialized_end=3112
+  _WITHVECTORSSELECTOR._serialized_start=3114
+  _WITHVECTORSSELECTOR._serialized_end=3217
+  _QUANTIZATIONSEARCHPARAMS._serialized_start=3219
+  _QUANTIZATIONSEARCHPARAMS._serialized_end=3311
+  _SEARCHPARAMS._serialized_start=3314
+  _SEARCHPARAMS._serialized_end=3470
+  _SEARCHPOINTS._serialized_start=3473
+  _SEARCHPOINTS._serialized_end=3944
+  _SEARCHBATCHPOINTS._serialized_start=3947
+  _SEARCHBATCHPOINTS._serialized_end=4113
+  _SEARCHPOINTGROUPS._serialized_start=4116
+  _SEARCHPOINTGROUPS._serialized_end=4592
+  _SCROLLPOINTS._serialized_start=4595
+  _SCROLLPOINTS._serialized_end=4952
+  _LOOKUPLOCATION._serialized_start=4954
+  _LOOKUPLOCATION._serialized_end=5037
+  _RECOMMENDPOINTS._serialized_start=5040
+  _RECOMMENDPOINTS._serialized_end=5622
+  _RECOMMENDBATCHPOINTS._serialized_start=5625
+  _RECOMMENDBATCHPOINTS._serialized_end=5800
+  _RECOMMENDPOINTGROUPS._serialized_start=5803
+  _RECOMMENDPOINTGROUPS._serialized_end=6390
+  _COUNTPOINTS._serialized_start=6392
+  _COUNTPOINTS._serialized_end=6492
+  _POINTSOPERATIONRESPONSE._serialized_start=6494
+  _POINTSOPERATIONRESPONSE._serialized_end=6571
+  _UPDATERESULT._serialized_start=6573
+  _UPDATERESULT._serialized_end=6647
+  _SCOREDPOINT._serialized_start=6650
+  _SCOREDPOINT._serialized_end=6895
+  _SCOREDPOINT_PAYLOADENTRY._serialized_start=1609
+  _SCOREDPOINT_PAYLOADENTRY._serialized_end=1670
+  _GROUPID._serialized_start=6897
+  _GROUPID._serialized_end=6989
+  _POINTGROUP._serialized_start=6991
+  _POINTGROUP._serialized_end=7067
+  _GROUPSRESULT._serialized_start=7069
+  _GROUPSRESULT._serialized_end=7119
+  _SEARCHRESPONSE._serialized_start=7121
+  _SEARCHRESPONSE._serialized_end=7188
+  _BATCHRESULT._serialized_start=7190
+  _BATCHRESULT._serialized_end=7240
+  _SEARCHBATCHRESPONSE._serialized_start=7242
+  _SEARCHBATCHRESPONSE._serialized_end=7314
+  _SEARCHGROUPSRESPONSE._serialized_start=7316
+  _SEARCHGROUPSRESPONSE._serialized_end=7390
+  _COUNTRESPONSE._serialized_start=7392
+  _COUNTRESPONSE._serialized_end=7458
+  _SCROLLRESPONSE._serialized_start=7461
+  _SCROLLRESPONSE._serialized_end=7600
+  _COUNTRESULT._serialized_start=7602
+  _COUNTRESULT._serialized_end=7630
+  _RETRIEVEDPOINT._serialized_start=7633
+  _RETRIEVEDPOINT._serialized_end=7852
+  _RETRIEVEDPOINT_PAYLOADENTRY._serialized_start=1609
+  _RETRIEVEDPOINT_PAYLOADENTRY._serialized_end=1670
+  _GETRESPONSE._serialized_start=7854
+  _GETRESPONSE._serialized_end=7921
+  _RECOMMENDRESPONSE._serialized_start=7923
+  _RECOMMENDRESPONSE._serialized_end=7993
+  _RECOMMENDBATCHRESPONSE._serialized_start=7995
+  _RECOMMENDBATCHRESPONSE._serialized_end=8070
+  _RECOMMENDGROUPSRESPONSE._serialized_start=8072
+  _RECOMMENDGROUPSRESPONSE._serialized_end=8149
+  _FILTER._serialized_start=8151
+  _FILTER._serialized_end=8264
+  _CONDITION._serialized_start=8267
+  _CONDITION._serialized_end=8548
+  _ISEMPTYCONDITION._serialized_start=8550
+  _ISEMPTYCONDITION._serialized_end=8581
+  _ISNULLCONDITION._serialized_start=8583
+  _ISNULLCONDITION._serialized_end=8613
+  _HASIDCONDITION._serialized_start=8615
+  _HASIDCONDITION._serialized_end=8664
+  _NESTEDCONDITION._serialized_start=8666
+  _NESTEDCONDITION._serialized_end=8728
+  _FIELDCONDITION._serialized_start=8731
+  _FIELDCONDITION._serialized_end=8952
+  _MATCH._serialized_start=8955
+  _MATCH._serialized_end=9246
+  _REPEATEDSTRINGS._serialized_start=9248
+  _REPEATEDSTRINGS._serialized_end=9282
+  _REPEATEDINTEGERS._serialized_start=9284
+  _REPEATEDINTEGERS._serialized_end=9320
+  _RANGE._serialized_start=9322
+  _RANGE._serialized_end=9429
+  _GEOBOUNDINGBOX._serialized_start=9431
+  _GEOBOUNDINGBOX._serialized_end=9523
+  _GEORADIUS._serialized_start=9525
+  _GEORADIUS._serialized_end=9586
+  _VALUESCOUNT._serialized_start=9588
+  _VALUESCOUNT._serialized_end=9701
+  _POINTSSELECTOR._serialized_start=9703
+  _POINTSSELECTOR._serialized_end=9820
+  _POINTSIDSLIST._serialized_start=9822
+  _POINTSIDSLIST._serialized_end=9867
+  _POINTSTRUCT._serialized_start=9870
+  _POINTSTRUCT._serialized_end=10083
+  _POINTSTRUCT_PAYLOADENTRY._serialized_start=1609
+  _POINTSTRUCT_PAYLOADENTRY._serialized_end=1670
+  _GEOPOINT._serialized_start=10085
+  _GEOPOINT._serialized_end=10121
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qdrant_client-1.1.7/qdrant_client/grpc/points_service_pb2.py` & `qdrant_client-1.2.0/qdrant_client/grpc/points_service_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import points_pb2 as points__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14points_service.proto\x12\x06qdrant\x1a\x0cpoints.proto\x1a\x1cgoogle/protobuf/struct.proto2\xba\x08\n\x06Points\x12\x41\n\x06Upsert\x12\x14.qdrant.UpsertPoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12\x41\n\x06\x44\x65lete\x12\x14.qdrant.DeletePoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12/\n\x03Get\x12\x11.qdrant.GetPoints\x1a\x13.qdrant.GetResponse\"\x00\x12I\n\nSetPayload\x12\x18.qdrant.SetPayloadPoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12O\n\x10OverwritePayload\x12\x18.qdrant.SetPayloadPoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12O\n\rDeletePayload\x12\x1b.qdrant.DeletePayloadPoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12M\n\x0c\x43learPayload\x12\x1a.qdrant.ClearPayloadPoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12Y\n\x10\x43reateFieldIndex\x12\".qdrant.CreateFieldIndexCollection\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12Y\n\x10\x44\x65leteFieldIndex\x12\".qdrant.DeleteFieldIndexCollection\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12\x38\n\x06Search\x12\x14.qdrant.SearchPoints\x1a\x16.qdrant.SearchResponse\"\x00\x12G\n\x0bSearchBatch\x12\x19.qdrant.SearchBatchPoints\x1a\x1b.qdrant.SearchBatchResponse\"\x00\x12\x38\n\x06Scroll\x12\x14.qdrant.ScrollPoints\x1a\x16.qdrant.ScrollResponse\"\x00\x12\x41\n\tRecommend\x12\x17.qdrant.RecommendPoints\x1a\x19.qdrant.RecommendResponse\"\x00\x12P\n\x0eRecommendBatch\x12\x1c.qdrant.RecommendBatchPoints\x1a\x1e.qdrant.RecommendBatchResponse\"\x00\x12\x35\n\x05\x43ount\x12\x13.qdrant.CountPoints\x1a\x15.qdrant.CountResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14points_service.proto\x12\x06qdrant\x1a\x0cpoints.proto\x1a\x1cgoogle/protobuf/struct.proto2\xf9\n\n\x06Points\x12\x41\n\x06Upsert\x12\x14.qdrant.UpsertPoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12\x41\n\x06\x44\x65lete\x12\x14.qdrant.DeletePoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12/\n\x03Get\x12\x11.qdrant.GetPoints\x1a\x13.qdrant.GetResponse\"\x00\x12N\n\rUpdateVectors\x12\x1a.qdrant.UpdatePointVectors\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12N\n\rDeleteVectors\x12\x1a.qdrant.DeletePointVectors\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12I\n\nSetPayload\x12\x18.qdrant.SetPayloadPoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12O\n\x10OverwritePayload\x12\x18.qdrant.SetPayloadPoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12O\n\rDeletePayload\x12\x1b.qdrant.DeletePayloadPoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12M\n\x0c\x43learPayload\x12\x1a.qdrant.ClearPayloadPoints\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12Y\n\x10\x43reateFieldIndex\x12\".qdrant.CreateFieldIndexCollection\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12Y\n\x10\x44\x65leteFieldIndex\x12\".qdrant.DeleteFieldIndexCollection\x1a\x1f.qdrant.PointsOperationResponse\"\x00\x12\x38\n\x06Search\x12\x14.qdrant.SearchPoints\x1a\x16.qdrant.SearchResponse\"\x00\x12G\n\x0bSearchBatch\x12\x19.qdrant.SearchBatchPoints\x1a\x1b.qdrant.SearchBatchResponse\"\x00\x12I\n\x0cSearchGroups\x12\x19.qdrant.SearchPointGroups\x1a\x1c.qdrant.SearchGroupsResponse\"\x00\x12\x38\n\x06Scroll\x12\x14.qdrant.ScrollPoints\x1a\x16.qdrant.ScrollResponse\"\x00\x12\x41\n\tRecommend\x12\x17.qdrant.RecommendPoints\x1a\x19.qdrant.RecommendResponse\"\x00\x12P\n\x0eRecommendBatch\x12\x1c.qdrant.RecommendBatchPoints\x1a\x1e.qdrant.RecommendBatchResponse\"\x00\x12R\n\x0fRecommendGroups\x12\x1c.qdrant.RecommendPointGroups\x1a\x1f.qdrant.RecommendGroupsResponse\"\x00\x12\x35\n\x05\x43ount\x12\x13.qdrant.CountPoints\x1a\x15.qdrant.CountResponse\"\x00\x62\x06proto3')
 
 
 
 _POINTS = DESCRIPTOR.services_by_name['Points']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _POINTS._serialized_start=77
-  _POINTS._serialized_end=1159
+  _POINTS._serialized_end=1478
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qdrant_client-1.1.7/qdrant_client/grpc/points_service_pb2_grpc.py` & `qdrant_client-1.2.0/qdrant_client/grpc/points_service_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,24 @@
                 response_deserializer=points__pb2.PointsOperationResponse.FromString,
                 )
         self.Get = channel.unary_unary(
                 '/qdrant.Points/Get',
                 request_serializer=points__pb2.GetPoints.SerializeToString,
                 response_deserializer=points__pb2.GetResponse.FromString,
                 )
+        self.UpdateVectors = channel.unary_unary(
+                '/qdrant.Points/UpdateVectors',
+                request_serializer=points__pb2.UpdatePointVectors.SerializeToString,
+                response_deserializer=points__pb2.PointsOperationResponse.FromString,
+                )
+        self.DeleteVectors = channel.unary_unary(
+                '/qdrant.Points/DeleteVectors',
+                request_serializer=points__pb2.DeletePointVectors.SerializeToString,
+                response_deserializer=points__pb2.PointsOperationResponse.FromString,
+                )
         self.SetPayload = channel.unary_unary(
                 '/qdrant.Points/SetPayload',
                 request_serializer=points__pb2.SetPayloadPoints.SerializeToString,
                 response_deserializer=points__pb2.PointsOperationResponse.FromString,
                 )
         self.OverwritePayload = channel.unary_unary(
                 '/qdrant.Points/OverwritePayload',
@@ -65,14 +75,19 @@
                 response_deserializer=points__pb2.SearchResponse.FromString,
                 )
         self.SearchBatch = channel.unary_unary(
                 '/qdrant.Points/SearchBatch',
                 request_serializer=points__pb2.SearchBatchPoints.SerializeToString,
                 response_deserializer=points__pb2.SearchBatchResponse.FromString,
                 )
+        self.SearchGroups = channel.unary_unary(
+                '/qdrant.Points/SearchGroups',
+                request_serializer=points__pb2.SearchPointGroups.SerializeToString,
+                response_deserializer=points__pb2.SearchGroupsResponse.FromString,
+                )
         self.Scroll = channel.unary_unary(
                 '/qdrant.Points/Scroll',
                 request_serializer=points__pb2.ScrollPoints.SerializeToString,
                 response_deserializer=points__pb2.ScrollResponse.FromString,
                 )
         self.Recommend = channel.unary_unary(
                 '/qdrant.Points/Recommend',
@@ -80,14 +95,19 @@
                 response_deserializer=points__pb2.RecommendResponse.FromString,
                 )
         self.RecommendBatch = channel.unary_unary(
                 '/qdrant.Points/RecommendBatch',
                 request_serializer=points__pb2.RecommendBatchPoints.SerializeToString,
                 response_deserializer=points__pb2.RecommendBatchResponse.FromString,
                 )
+        self.RecommendGroups = channel.unary_unary(
+                '/qdrant.Points/RecommendGroups',
+                request_serializer=points__pb2.RecommendPointGroups.SerializeToString,
+                response_deserializer=points__pb2.RecommendGroupsResponse.FromString,
+                )
         self.Count = channel.unary_unary(
                 '/qdrant.Points/Count',
                 request_serializer=points__pb2.CountPoints.SerializeToString,
                 response_deserializer=points__pb2.CountResponse.FromString,
                 )
 
 
@@ -114,14 +134,30 @@
         """
         Retrieve points
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def UpdateVectors(self, request, context):
+        """
+        Update named vectors for point
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteVectors(self, request, context):
+        """
+        Delete named vectors for points
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def SetPayload(self, request, context):
         """
         Set payload for points
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
@@ -178,14 +214,22 @@
         """
         Retrieve closest points based on vector similarity and given filtering conditions
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SearchGroups(self, request, context):
+        """
+        Retrieve closest points based on vector similarity and given filtering conditions, grouped by a given field
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def Scroll(self, request, context):
         """
         Iterate over all or filtered points points
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
@@ -202,14 +246,22 @@
         """
         Look for the points which are closer to stored positive examples and at the same time further to negative examples.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def RecommendGroups(self, request, context):
+        """
+        Look for the points which are closer to stored positive examples and at the same time further to negative examples, grouped by a given field
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def Count(self, request, context):
         """
         Count points in collection with given filtering conditions
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
@@ -228,14 +280,24 @@
                     response_serializer=points__pb2.PointsOperationResponse.SerializeToString,
             ),
             'Get': grpc.unary_unary_rpc_method_handler(
                     servicer.Get,
                     request_deserializer=points__pb2.GetPoints.FromString,
                     response_serializer=points__pb2.GetResponse.SerializeToString,
             ),
+            'UpdateVectors': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateVectors,
+                    request_deserializer=points__pb2.UpdatePointVectors.FromString,
+                    response_serializer=points__pb2.PointsOperationResponse.SerializeToString,
+            ),
+            'DeleteVectors': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteVectors,
+                    request_deserializer=points__pb2.DeletePointVectors.FromString,
+                    response_serializer=points__pb2.PointsOperationResponse.SerializeToString,
+            ),
             'SetPayload': grpc.unary_unary_rpc_method_handler(
                     servicer.SetPayload,
                     request_deserializer=points__pb2.SetPayloadPoints.FromString,
                     response_serializer=points__pb2.PointsOperationResponse.SerializeToString,
             ),
             'OverwritePayload': grpc.unary_unary_rpc_method_handler(
                     servicer.OverwritePayload,
@@ -268,14 +330,19 @@
                     response_serializer=points__pb2.SearchResponse.SerializeToString,
             ),
             'SearchBatch': grpc.unary_unary_rpc_method_handler(
                     servicer.SearchBatch,
                     request_deserializer=points__pb2.SearchBatchPoints.FromString,
                     response_serializer=points__pb2.SearchBatchResponse.SerializeToString,
             ),
+            'SearchGroups': grpc.unary_unary_rpc_method_handler(
+                    servicer.SearchGroups,
+                    request_deserializer=points__pb2.SearchPointGroups.FromString,
+                    response_serializer=points__pb2.SearchGroupsResponse.SerializeToString,
+            ),
             'Scroll': grpc.unary_unary_rpc_method_handler(
                     servicer.Scroll,
                     request_deserializer=points__pb2.ScrollPoints.FromString,
                     response_serializer=points__pb2.ScrollResponse.SerializeToString,
             ),
             'Recommend': grpc.unary_unary_rpc_method_handler(
                     servicer.Recommend,
@@ -283,14 +350,19 @@
                     response_serializer=points__pb2.RecommendResponse.SerializeToString,
             ),
             'RecommendBatch': grpc.unary_unary_rpc_method_handler(
                     servicer.RecommendBatch,
                     request_deserializer=points__pb2.RecommendBatchPoints.FromString,
                     response_serializer=points__pb2.RecommendBatchResponse.SerializeToString,
             ),
+            'RecommendGroups': grpc.unary_unary_rpc_method_handler(
+                    servicer.RecommendGroups,
+                    request_deserializer=points__pb2.RecommendPointGroups.FromString,
+                    response_serializer=points__pb2.RecommendGroupsResponse.SerializeToString,
+            ),
             'Count': grpc.unary_unary_rpc_method_handler(
                     servicer.Count,
                     request_deserializer=points__pb2.CountPoints.FromString,
                     response_serializer=points__pb2.CountResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -350,14 +422,48 @@
         return grpc.experimental.unary_unary(request, target, '/qdrant.Points/Get',
             points__pb2.GetPoints.SerializeToString,
             points__pb2.GetResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def UpdateVectors(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qdrant.Points/UpdateVectors',
+            points__pb2.UpdatePointVectors.SerializeToString,
+            points__pb2.PointsOperationResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteVectors(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qdrant.Points/DeleteVectors',
+            points__pb2.DeletePointVectors.SerializeToString,
+            points__pb2.PointsOperationResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def SetPayload(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -486,14 +592,31 @@
         return grpc.experimental.unary_unary(request, target, '/qdrant.Points/SearchBatch',
             points__pb2.SearchBatchPoints.SerializeToString,
             points__pb2.SearchBatchResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def SearchGroups(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qdrant.Points/SearchGroups',
+            points__pb2.SearchPointGroups.SerializeToString,
+            points__pb2.SearchGroupsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def Scroll(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -537,14 +660,31 @@
         return grpc.experimental.unary_unary(request, target, '/qdrant.Points/RecommendBatch',
             points__pb2.RecommendBatchPoints.SerializeToString,
             points__pb2.RecommendBatchResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def RecommendGroups(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/qdrant.Points/RecommendGroups',
+            points__pb2.RecommendPointGroups.SerializeToString,
+            points__pb2.RecommendGroupsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def Count(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `qdrant_client-1.1.7/qdrant_client/grpc/qdrant_pb2.py` & `qdrant_client-1.2.0/qdrant_client/grpc/qdrant_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/grpc/qdrant_pb2_grpc.py` & `qdrant_client-1.2.0/qdrant_client/grpc/qdrant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/grpc/snapshots_service_pb2.py` & `qdrant_client-1.2.0/qdrant_client/grpc/snapshots_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/grpc/snapshots_service_pb2_grpc.py` & `qdrant_client-1.2.0/qdrant_client/grpc/snapshots_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/http/api/cluster_api.py` & `qdrant_client-1.2.0/qdrant_client/http/api/cluster_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/http/api/collections_api.py` & `qdrant_client-1.2.0/qdrant_client/http/api/collections_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/http/api/points_api.py` & `qdrant_client-1.2.0/qdrant_client/http/api/points_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         path_params = {
             "collection_name": str(collection_name),
         }
 
         body = jsonable_encoder(count_request)
 
         return self.api_client.request(
-            type_=m.InlineResponse20016,
+            type_=m.InlineResponse20017,
             method="POST",
             url="/collections/{collection_name}/points/count",
             path_params=path_params,
             json=body,
         )
 
     def _build_for_delete_payload(
@@ -265,14 +265,45 @@
             method="POST",
             url="/collections/{collection_name}/points/delete",
             path_params=path_params,
             params=query_params,
             json=body,
         )
 
+    def _build_for_delete_vectors(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        ordering: WriteOrdering = None,
+        delete_vectors: m.DeleteVectors = None,
+    ):
+        """
+        Delete named vectors from the given points.
+        """
+        path_params = {
+            "collection_name": str(collection_name),
+        }
+
+        query_params = {}
+        if wait is not None:
+            query_params["wait"] = str(wait).lower()
+        if ordering is not None:
+            query_params["ordering"] = str(ordering)
+
+        body = jsonable_encoder(delete_vectors)
+
+        return self.api_client.request(
+            type_=m.InlineResponse2006,
+            method="POST",
+            url="/collections/{collection_name}/points/vectors/delete",
+            path_params=path_params,
+            params=query_params,
+            json=body,
+        )
+
     def _build_for_get_point(
         self,
         collection_name: str,
         id: m.ExtendedPointId,
         consistency: m.ReadConsistency = None,
     ):
         """
@@ -378,14 +409,42 @@
             method="POST",
             url="/collections/{collection_name}/points/recommend/batch",
             path_params=path_params,
             params=query_params,
             json=body,
         )
 
+    def _build_for_recommend_point_groups(
+        self,
+        collection_name: str,
+        consistency: m.ReadConsistency = None,
+        recommend_groups_request: m.RecommendGroupsRequest = None,
+    ):
+        """
+        Look for the points which are closer to stored positive examples and at the same time further to negative examples, grouped by a given payload field.
+        """
+        path_params = {
+            "collection_name": str(collection_name),
+        }
+
+        query_params = {}
+        if consistency is not None:
+            query_params["consistency"] = str(consistency)
+
+        body = jsonable_encoder(recommend_groups_request)
+
+        return self.api_client.request(
+            type_=m.InlineResponse20016,
+            method="POST",
+            url="/collections/{collection_name}/points/recommend/groups",
+            path_params=path_params,
+            params=query_params,
+            json=body,
+        )
+
     def _build_for_recommend_points(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         recommend_request: m.RecommendRequest = None,
     ):
         """
@@ -462,14 +521,42 @@
             method="POST",
             url="/collections/{collection_name}/points/search/batch",
             path_params=path_params,
             params=query_params,
             json=body,
         )
 
+    def _build_for_search_point_groups(
+        self,
+        collection_name: str,
+        consistency: m.ReadConsistency = None,
+        search_groups_request: m.SearchGroupsRequest = None,
+    ):
+        """
+        Retrieve closest points based on vector similarity and given filtering conditions, grouped by a given payload field
+        """
+        path_params = {
+            "collection_name": str(collection_name),
+        }
+
+        query_params = {}
+        if consistency is not None:
+            query_params["consistency"] = str(consistency)
+
+        body = jsonable_encoder(search_groups_request)
+
+        return self.api_client.request(
+            type_=m.InlineResponse20016,
+            method="POST",
+            url="/collections/{collection_name}/points/search/groups",
+            path_params=path_params,
+            params=query_params,
+            json=body,
+        )
+
     def _build_for_search_points(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         search_request: m.SearchRequest = None,
     ):
         """
@@ -521,14 +608,45 @@
             method="POST",
             url="/collections/{collection_name}/points/payload",
             path_params=path_params,
             params=query_params,
             json=body,
         )
 
+    def _build_for_update_vectors(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        ordering: WriteOrdering = None,
+        update_vectors: m.UpdateVectors = None,
+    ):
+        """
+        Update specified named vectors on points, keep unspecified vectors intact.
+        """
+        path_params = {
+            "collection_name": str(collection_name),
+        }
+
+        query_params = {}
+        if wait is not None:
+            query_params["wait"] = str(wait).lower()
+        if ordering is not None:
+            query_params["ordering"] = str(ordering)
+
+        body = jsonable_encoder(update_vectors)
+
+        return self.api_client.request(
+            type_=m.InlineResponse2006,
+            method="PUT",
+            url="/collections/{collection_name}/points/vectors",
+            path_params=path_params,
+            params=query_params,
+            json=body,
+        )
+
     def _build_for_upsert_points(
         self,
         collection_name: str,
         wait: bool = None,
         ordering: WriteOrdering = None,
         point_insert_operations: m.PointInsertOperations = None,
     ):
@@ -575,15 +693,15 @@
             points_selector=points_selector,
         )
 
     async def count_points(
         self,
         collection_name: str,
         count_request: m.CountRequest = None,
-    ) -> m.InlineResponse20016:
+    ) -> m.InlineResponse20017:
         """
         Count points which matches given filtering condition
         """
         return await self._build_for_count_points(
             collection_name=collection_name,
             count_request=count_request,
         )
@@ -618,14 +736,31 @@
         return await self._build_for_delete_points(
             collection_name=collection_name,
             wait=wait,
             ordering=ordering,
             points_selector=points_selector,
         )
 
+    async def delete_vectors(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        ordering: WriteOrdering = None,
+        delete_vectors: m.DeleteVectors = None,
+    ) -> m.InlineResponse2006:
+        """
+        Delete named vectors from the given points.
+        """
+        return await self._build_for_delete_vectors(
+            collection_name=collection_name,
+            wait=wait,
+            ordering=ordering,
+            delete_vectors=delete_vectors,
+        )
+
     async def get_point(
         self,
         collection_name: str,
         id: m.ExtendedPointId,
         consistency: m.ReadConsistency = None,
     ) -> m.InlineResponse20011:
         """
@@ -680,14 +815,29 @@
         """
         return await self._build_for_recommend_batch_points(
             collection_name=collection_name,
             consistency=consistency,
             recommend_request_batch=recommend_request_batch,
         )
 
+    async def recommend_point_groups(
+        self,
+        collection_name: str,
+        consistency: m.ReadConsistency = None,
+        recommend_groups_request: m.RecommendGroupsRequest = None,
+    ) -> m.InlineResponse20016:
+        """
+        Look for the points which are closer to stored positive examples and at the same time further to negative examples, grouped by a given payload field.
+        """
+        return await self._build_for_recommend_point_groups(
+            collection_name=collection_name,
+            consistency=consistency,
+            recommend_groups_request=recommend_groups_request,
+        )
+
     async def recommend_points(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         recommend_request: m.RecommendRequest = None,
     ) -> m.InlineResponse20014:
         """
@@ -725,14 +875,29 @@
         """
         return await self._build_for_search_batch_points(
             collection_name=collection_name,
             consistency=consistency,
             search_request_batch=search_request_batch,
         )
 
+    async def search_point_groups(
+        self,
+        collection_name: str,
+        consistency: m.ReadConsistency = None,
+        search_groups_request: m.SearchGroupsRequest = None,
+    ) -> m.InlineResponse20016:
+        """
+        Retrieve closest points based on vector similarity and given filtering conditions, grouped by a given payload field
+        """
+        return await self._build_for_search_point_groups(
+            collection_name=collection_name,
+            consistency=consistency,
+            search_groups_request=search_groups_request,
+        )
+
     async def search_points(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         search_request: m.SearchRequest = None,
     ) -> m.InlineResponse20014:
         """
@@ -757,14 +922,31 @@
         return await self._build_for_set_payload(
             collection_name=collection_name,
             wait=wait,
             ordering=ordering,
             set_payload=set_payload,
         )
 
+    async def update_vectors(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        ordering: WriteOrdering = None,
+        update_vectors: m.UpdateVectors = None,
+    ) -> m.InlineResponse2006:
+        """
+        Update specified named vectors on points, keep unspecified vectors intact.
+        """
+        return await self._build_for_update_vectors(
+            collection_name=collection_name,
+            wait=wait,
+            ordering=ordering,
+            update_vectors=update_vectors,
+        )
+
     async def upsert_points(
         self,
         collection_name: str,
         wait: bool = None,
         ordering: WriteOrdering = None,
         point_insert_operations: m.PointInsertOperations = None,
     ) -> m.InlineResponse2006:
@@ -797,15 +979,15 @@
             points_selector=points_selector,
         )
 
     def count_points(
         self,
         collection_name: str,
         count_request: m.CountRequest = None,
-    ) -> m.InlineResponse20016:
+    ) -> m.InlineResponse20017:
         """
         Count points which matches given filtering condition
         """
         return self._build_for_count_points(
             collection_name=collection_name,
             count_request=count_request,
         )
@@ -840,14 +1022,31 @@
         return self._build_for_delete_points(
             collection_name=collection_name,
             wait=wait,
             ordering=ordering,
             points_selector=points_selector,
         )
 
+    def delete_vectors(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        ordering: WriteOrdering = None,
+        delete_vectors: m.DeleteVectors = None,
+    ) -> m.InlineResponse2006:
+        """
+        Delete named vectors from the given points.
+        """
+        return self._build_for_delete_vectors(
+            collection_name=collection_name,
+            wait=wait,
+            ordering=ordering,
+            delete_vectors=delete_vectors,
+        )
+
     def get_point(
         self,
         collection_name: str,
         id: m.ExtendedPointId,
         consistency: m.ReadConsistency = None,
     ) -> m.InlineResponse20011:
         """
@@ -902,14 +1101,29 @@
         """
         return self._build_for_recommend_batch_points(
             collection_name=collection_name,
             consistency=consistency,
             recommend_request_batch=recommend_request_batch,
         )
 
+    def recommend_point_groups(
+        self,
+        collection_name: str,
+        consistency: m.ReadConsistency = None,
+        recommend_groups_request: m.RecommendGroupsRequest = None,
+    ) -> m.InlineResponse20016:
+        """
+        Look for the points which are closer to stored positive examples and at the same time further to negative examples, grouped by a given payload field.
+        """
+        return self._build_for_recommend_point_groups(
+            collection_name=collection_name,
+            consistency=consistency,
+            recommend_groups_request=recommend_groups_request,
+        )
+
     def recommend_points(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         recommend_request: m.RecommendRequest = None,
     ) -> m.InlineResponse20014:
         """
@@ -947,14 +1161,29 @@
         """
         return self._build_for_search_batch_points(
             collection_name=collection_name,
             consistency=consistency,
             search_request_batch=search_request_batch,
         )
 
+    def search_point_groups(
+        self,
+        collection_name: str,
+        consistency: m.ReadConsistency = None,
+        search_groups_request: m.SearchGroupsRequest = None,
+    ) -> m.InlineResponse20016:
+        """
+        Retrieve closest points based on vector similarity and given filtering conditions, grouped by a given payload field
+        """
+        return self._build_for_search_point_groups(
+            collection_name=collection_name,
+            consistency=consistency,
+            search_groups_request=search_groups_request,
+        )
+
     def search_points(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         search_request: m.SearchRequest = None,
     ) -> m.InlineResponse20014:
         """
@@ -979,14 +1208,31 @@
         return self._build_for_set_payload(
             collection_name=collection_name,
             wait=wait,
             ordering=ordering,
             set_payload=set_payload,
         )
 
+    def update_vectors(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        ordering: WriteOrdering = None,
+        update_vectors: m.UpdateVectors = None,
+    ) -> m.InlineResponse2006:
+        """
+        Update specified named vectors on points, keep unspecified vectors intact.
+        """
+        return self._build_for_update_vectors(
+            collection_name=collection_name,
+            wait=wait,
+            ordering=ordering,
+            update_vectors=update_vectors,
+        )
+
     def upsert_points(
         self,
         collection_name: str,
         wait: bool = None,
         ordering: WriteOrdering = None,
         point_insert_operations: m.PointInsertOperations = None,
     ) -> m.InlineResponse2006:
```

### Comparing `qdrant_client-1.1.7/qdrant_client/http/api/service_api.py` & `qdrant_client-1.2.0/qdrant_client/http/api/service_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/http/api/snapshots_api.py` & `qdrant_client-1.2.0/qdrant_client/http/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/http/api_client.py` & `qdrant_client-1.2.0/qdrant_client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/http/exceptions.py` & `qdrant_client-1.2.0/qdrant_client/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/http/models/models.py` & `qdrant_client-1.2.0/qdrant_client/http/models/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,22 @@
 
 
 class CollectionsTelemetry(BaseModel):
     number_of_collections: int = Field(..., description="")
     collections: Optional[List["CollectionTelemetryEnum"]] = Field(default=None, description="")
 
 
+class CompressionRatio(str, Enum):
+    X4 = "x4"
+    X8 = "x8"
+    X16 = "x16"
+    X32 = "x32"
+    X64 = "x64"
+
+
 class ConsensusConfigTelemetry(BaseModel):
     max_message_queue_size: int = Field(..., description="")
     tick_period_ms: int = Field(..., description="")
     bootstrap_timeout_sec: int = Field(..., description="")
 
 
 class ConsensusThreadStatusOneOf(BaseModel):
@@ -334,14 +342,24 @@
         default=None, description="Deletes values from each point in this list"
     )
     filter: Optional["Filter"] = Field(
         default=None, description="Deletes values from points that satisfy this filter condition"
     )
 
 
+class DeleteVectors(BaseModel):
+    points: Optional[List["ExtendedPointId"]] = Field(
+        default=None, description="Deletes values from each point in this list"
+    )
+    filter: Optional["Filter"] = Field(
+        default=None, description="Deletes values from points that satisfy this filter condition"
+    )
+    vector: List[str] = Field(..., description="Vector names")
+
+
 class Distance(str, Enum):
     COSINE = "Cosine"
     EUCLID = "Euclid"
     DOT = "Dot"
 
 
 class DropReplicaOperation(BaseModel):
@@ -417,14 +435,18 @@
     center: "GeoPoint" = Field(
         ...,
         description="Geo filter request  Matches coordinates inside the circle of `radius` and center with coordinates `center`",
     )
     radius: float = Field(..., description="Radius of the area in meters")
 
 
+class GroupsResult(BaseModel):
+    groups: List["PointGroup"] = Field(..., description="")
+
+
 class GrpcTelemetry(BaseModel):
     responses: Dict[str, "OperationDurationStatistics"] = Field(..., description="")
 
 
 class HasIdCondition(BaseModel):
     """
     ID-based filtering condition
@@ -470,15 +492,15 @@
     )
     ef_construct: Optional[int] = Field(
         default=None,
         description="Number of neighbours to consider during the index building. Larger the value - more accurate the search, more time required to build the index.",
     )
     full_scan_threshold: Optional[int] = Field(
         default=None,
-        description="Minimal size (in KiloBytes) of vectors for additional payload-based indexing. If payload chunk is smaller than `full_scan_threshold_kb` additional indexing won&#x27;t be used - in this case full-scan search should be preferred by query planner and additional indexing is not required. Note: 1Kb = 1 vector of size 256",
+        description="Minimal size (in kilobytes) of vectors for additional payload-based indexing. If payload chunk is smaller than `full_scan_threshold_kb` additional indexing won&#x27;t be used - in this case full-scan search should be preferred by query planner and additional indexing is not required. Note: 1Kb = 1 vector of size 256",
     )
     max_indexing_threads: Optional[int] = Field(
         default=None,
         description="Number of parallel threads used for background index building. If 0 - auto selection.",
     )
     on_disk: Optional[bool] = Field(
         default=None,
@@ -595,14 +617,22 @@
 
 
 class InlineResponse20016(BaseModel):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
+    result: Optional["GroupsResult"] = Field(default=None, description="")
+
+
+class InlineResponse20017(BaseModel):
+    time: Optional[float] = Field(default=None, description="Time spent to process this request")
+    status: Literal[
+        "ok",
+    ] = Field(None, description="")
     result: Optional["CountResult"] = Field(default=None, description="")
 
 
 class InlineResponse2002(BaseModel):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
@@ -722,14 +752,24 @@
     """
     Exact match on any of the given values
     """
 
     any: "AnyVariants" = Field(..., description="Exact match on any of the given values")
 
 
+class MatchExcept(BaseModel):
+    """
+    Should have at least one value not matching the any given values
+    """
+
+    except_: "AnyVariants" = Field(
+        ..., description="Should have at least one value not matching the any given values", alias="except"
+    )
+
+
 class MatchText(BaseModel):
     """
     Full-text match of the strings.
     """
 
     text: str = Field(..., description="Full-text match of the strings.")
 
@@ -766,14 +806,27 @@
     Vector data with name
     """
 
     name: str = Field(..., description="Name of vector data")
     vector: List[float] = Field(..., description="Vector data")
 
 
+class Nested(BaseModel):
+    """
+    Select points with payload for a specified nested field
+    """
+
+    key: str = Field(..., description="Select points with payload for a specified nested field")
+    filter: "Filter" = Field(..., description="Select points with payload for a specified nested field")
+
+
+class NestedCondition(BaseModel):
+    nested: "Nested" = Field(..., description="")
+
+
 class OperationDurationStatistics(BaseModel):
     count: int = Field(..., description="")
     fail_count: Optional[int] = Field(default=None, description="")
     avg_duration_micros: Optional[float] = Field(default=None, description="")
     min_duration_micros: Optional[float] = Field(default=None, description="")
     max_duration_micros: Optional[float] = Field(default=None, description="")
     last_responded: Optional[datetime] = Field(default=None, description="")
@@ -794,23 +847,23 @@
     )
     default_segment_number: int = Field(
         ...,
         description="Target amount of segments optimizer will try to keep. Real amount of segments may vary depending on multiple parameters: - Amount of stored points - Current write RPS  It is recommended to select default number of segments as a factor of the number of search threads, so that each segment would be handled evenly by one of the threads. If `default_segment_number = 0`, will be automatically selected by the number of available CPUs.",
     )
     max_segment_size: Optional[int] = Field(
         default=None,
-        description="Do not create segments larger this size (in KiloBytes). Large segments might require disproportionately long indexation times, therefore it makes sense to limit the size of segments.  If indexation speed have more priority for your - make this parameter lower. If search speed is more important - make this parameter higher. Note: 1Kb = 1 vector of size 256 If not set, will be automatically selected considering the number of available CPUs.",
+        description="Do not create segments larger this size (in kilobytes). Large segments might require disproportionately long indexation times, therefore it makes sense to limit the size of segments.  If indexing speed is more important - make this parameter lower. If search speed is more important - make this parameter higher. Note: 1Kb = 1 vector of size 256 If not set, will be automatically selected considering the number of available CPUs.",
     )
     memmap_threshold: Optional[int] = Field(
         default=None,
-        description="Maximum size (in KiloBytes) of vectors to store in-memory per segment. Segments larger than this threshold will be stored as read-only memmaped file. To enable memmap storage, lower the threshold Note: 1Kb = 1 vector of size 256 If not set, mmap will not be used.",
+        description="Maximum size (in kilobytes) of vectors to store in-memory per segment. Segments larger than this threshold will be stored as read-only memmaped file.  Memmap storage is disabled by default, to enable it, set this threshold to a reasonable value.  To disable memmap storage, set this to `0`. Internally it will use the largest threshold possible.  Note: 1Kb = 1 vector of size 256",
     )
-    indexing_threshold: int = Field(
-        ...,
-        description="Maximum size (in KiloBytes) of vectors allowed for plain index. Default value based on &lt;https://github.com/google-research/google-research/blob/master/scann/docs/algorithms.md&gt; Note: 1Kb = 1 vector of size 256",
+    indexing_threshold: Optional[int] = Field(
+        default=None,
+        description="Maximum size (in kilobytes) of vectors allowed for plain index, exceeding this threshold will enable vector indexing  Default value is 20,000, based on &lt;https://github.com/google-research/google-research/blob/master/scann/docs/algorithms.md&gt;.  To disable vector indexing, set to `0`.  Note: 1kB = 1 vector of size 256.",
     )
     flush_interval_sec: int = Field(..., description="Minimum interval between forced flushes.")
     max_optimization_threads: int = Field(..., description="Maximum available threads for optimization workers")
 
 
 class OptimizersConfigDiff(BaseModel):
     deleted_threshold: Optional[float] = Field(
@@ -822,23 +875,23 @@
     )
     default_segment_number: Optional[int] = Field(
         default=None,
         description="Target amount of segments optimizer will try to keep. Real amount of segments may vary depending on multiple parameters: - Amount of stored points - Current write RPS  It is recommended to select default number of segments as a factor of the number of search threads, so that each segment would be handled evenly by one of the threads If `default_segment_number = 0`, will be automatically selected by the number of available CPUs",
     )
     max_segment_size: Optional[int] = Field(
         default=None,
-        description="Do not create segments larger this size (in KiloBytes). Large segments might require disproportionately long indexation times, therefore it makes sense to limit the size of segments.  If indexation speed have more priority for your - make this parameter lower. If search speed is more important - make this parameter higher. Note: 1Kb = 1 vector of size 256",
+        description="Do not create segments larger this size (in kilobytes). Large segments might require disproportionately long indexation times, therefore it makes sense to limit the size of segments.  If indexation speed have more priority for your - make this parameter lower. If search speed is more important - make this parameter higher. Note: 1Kb = 1 vector of size 256",
     )
     memmap_threshold: Optional[int] = Field(
         default=None,
-        description="Maximum size (in KiloBytes) of vectors to store in-memory per segment. Segments larger than this threshold will be stored as read-only memmaped file. To enable memmap storage, lower the threshold Note: 1Kb = 1 vector of size 256",
+        description="Maximum size (in kilobytes) of vectors to store in-memory per segment. Segments larger than this threshold will be stored as read-only memmaped file.  Memmap storage is disabled by default, to enable it, set this threshold to a reasonable value.  To disable memmap storage, set this to `0`.  Note: 1Kb = 1 vector of size 256",
     )
     indexing_threshold: Optional[int] = Field(
         default=None,
-        description="Maximum size (in KiloBytes) of vectors allowed for plain index. Default value based on &lt;https://github.com/google-research/google-research/blob/master/scann/docs/algorithms.md&gt; Note: 1Kb = 1 vector of size 256",
+        description="Maximum size (in kilobytes) of vectors allowed for plain index, exceeding this threshold will enable vector indexing  Default value is 20,000, based on &lt;https://github.com/google-research/google-research/blob/master/scann/docs/algorithms.md&gt;.  To disable vector indexing, set to `0`.  Note: 1kB = 1 vector of size 256.",
     )
     flush_interval_sec: Optional[int] = Field(default=None, description="Minimum interval between forced flushes.")
     max_optimization_threads: Optional[int] = Field(
         default=None, description="Maximum available threads for optimization workers"
     )
 
 
@@ -899,26 +952,37 @@
 
 class PayloadSelectorInclude(BaseModel):
     include: List[str] = Field(..., description="Only include this payload keys")
 
 
 class PayloadStorageTypeOneOf(BaseModel):
     type: Literal[
+        "in_memory",
+    ] = Field(..., description="")
+
+
+class PayloadStorageTypeOneOf1(BaseModel):
+    type: Literal[
         "on_disk",
     ] = Field(..., description="")
 
 
 class PeerInfo(BaseModel):
     """
     Information of a peer in the cluster
     """
 
     uri: str = Field(..., description="Information of a peer in the cluster")
 
 
+class PointGroup(BaseModel):
+    hits: List["ScoredPoint"] = Field(..., description="Scored points that have the same value of the group_by key")
+    id: "GroupId" = Field(..., description="")
+
+
 class PointIdsList(BaseModel):
     points: List["ExtendedPointId"] = Field(..., description="")
 
 
 class PointRequest(BaseModel):
     ids: List["ExtendedPointId"] = Field(..., description="Look for points with ids")
     with_payload: Optional["WithPayloadInterface"] = Field(
@@ -929,22 +993,36 @@
 
 class PointStruct(BaseModel):
     id: "ExtendedPointId" = Field(..., description="")
     vector: "VectorStruct" = Field(..., description="")
     payload: Optional["Payload"] = Field(default=None, description="Payload values (optional)")
 
 
+class PointVectors(BaseModel):
+    id: "ExtendedPointId" = Field(..., description="")
+    vector: "VectorStruct" = Field(..., description="")
+
+
 class PointsBatch(BaseModel):
     batch: "Batch" = Field(..., description="")
 
 
 class PointsList(BaseModel):
     points: List["PointStruct"] = Field(..., description="")
 
 
+class ProductQuantization(BaseModel):
+    product: "ProductQuantizationConfig" = Field(..., description="")
+
+
+class ProductQuantizationConfig(BaseModel):
+    compression: "CompressionRatio" = Field(..., description="")
+    always_ram: Optional[bool] = Field(default=None, description="")
+
+
 class QuantizationSearchParams(BaseModel):
     """
     Additional parameters of the search
     """
 
     ignore: Optional[bool] = Field(
         default=False, description="If true, quantized vectors are ignored. Default is false."
@@ -988,14 +1066,45 @@
 
 class ReadConsistencyType(str, Enum):
     MAJORITY = "majority"
     QUORUM = "quorum"
     ALL = "all"
 
 
+class RecommendGroupsRequest(BaseModel):
+    positive: List["ExtendedPointId"] = Field(..., description="Look for vectors closest to those")
+    negative: Optional[List["ExtendedPointId"]] = Field(default=[], description="Try to avoid vectors like this")
+    filter: Optional["Filter"] = Field(default=None, description="Look only for points which satisfies this conditions")
+    params: Optional["SearchParams"] = Field(default=None, description="Additional search params")
+    with_payload: Optional["WithPayloadInterface"] = Field(
+        default=None, description="Select which payload to return with the response. Default: None"
+    )
+    with_vector: Optional["WithVector"] = Field(
+        default=None, description="Whether to return the point vector with the result?"
+    )
+    score_threshold: Optional[float] = Field(
+        default=None,
+        description="Define a minimal score threshold for the result. If defined, less similar results will not be returned. Score of the returned result might be higher or smaller than the threshold depending on the Distance function used. E.g. for cosine similarity only higher scores will be returned.",
+    )
+    using: Optional["UsingVector"] = Field(
+        default=None,
+        description="Define which vector to use for recommendation, if not specified - try to use default vector",
+    )
+    lookup_from: Optional["LookupLocation"] = Field(
+        default=None,
+        description="The location used to lookup vectors. If not specified - use current collection. Note: the other collection should have the same vector size as the current collection",
+    )
+    group_by: str = Field(
+        ...,
+        description="Payload field to group by, must be a string or number field. If the field contains more than 1 value, all values will be used for grouping. One point can be in multiple groups.",
+    )
+    group_size: int = Field(..., description="Maximum amount of points to return per group")
+    limit: int = Field(..., description="Maximum amount of groups to return")
+
+
 class RecommendRequest(BaseModel):
     """
     Recommendation request. Provides positive and negative examples of the vectors, which are already stored in the collection.  Service should look for the points which are closer to positive examples and at the same time further to negative examples. The concrete way of how to compare negative and positive distances is up to implementation in `segment` crate.
     """
 
     positive: List["ExtendedPointId"] = Field(..., description="Look for vectors closest to those")
     negative: Optional[List["ExtendedPointId"]] = Field(default=[], description="Try to avoid vectors like this")
@@ -1166,14 +1275,36 @@
 
     points: List["Record"] = Field(..., description="List of retrieved points")
     next_page_offset: Optional["ExtendedPointId"] = Field(
         default=None, description="Offset which should be used to retrieve a next page result"
     )
 
 
+class SearchGroupsRequest(BaseModel):
+    vector: "NamedVectorStruct" = Field(..., description="")
+    filter: Optional["Filter"] = Field(default=None, description="Look only for points which satisfies this conditions")
+    params: Optional["SearchParams"] = Field(default=None, description="Additional search params")
+    with_payload: Optional["WithPayloadInterface"] = Field(
+        default=None, description="Select which payload to return with the response. Default: None"
+    )
+    with_vector: Optional["WithVector"] = Field(
+        default=None, description="Whether to return the point vector with the result?"
+    )
+    score_threshold: Optional[float] = Field(
+        default=None,
+        description="Define a minimal score threshold for the result. If defined, less similar results will not be returned. Score of the returned result might be higher or smaller than the threshold depending on the Distance function used. E.g. for cosine similarity only higher scores will be returned.",
+    )
+    group_by: str = Field(
+        ...,
+        description="Payload field to group by, must be a string or number field. If the field contains more than 1 value, all values will be used for grouping. One point can be in multiple groups.",
+    )
+    group_size: int = Field(..., description="Maximum amount of points to return per group")
+    limit: int = Field(..., description="Maximum amount of groups to return")
+
+
 class SearchParams(BaseModel):
     """
     Additional parameters of the search
     """
 
     hnsw_ef: Optional[int] = Field(
         default=None,
@@ -1216,20 +1347,15 @@
 
 class SearchRequestBatch(BaseModel):
     searches: List["SearchRequest"] = Field(..., description="")
 
 
 class SegmentConfig(BaseModel):
     vector_data: Dict[str, "VectorDataConfig"] = Field(..., description="")
-    index: "Indexes" = Field(..., description="")
-    storage_type: "StorageType" = Field(..., description="")
-    payload_storage_type: Optional["PayloadStorageType"] = Field(default=None, description="")
-    quantization_config: Optional["QuantizationConfig"] = Field(
-        default=None, description="Quantization parameters. If none - quantization is disabled."
-    )
+    payload_storage_type: "PayloadStorageType" = Field(..., description="")
 
 
 class SegmentInfo(BaseModel):
     """
     Aggregated information about segment
     """
 
@@ -1264,15 +1390,15 @@
     filter: Optional["Filter"] = Field(
         default=None, description="Assigns payload to each point that satisfy this filter condition"
     )
 
 
 class ShardTransferInfo(BaseModel):
     shard_id: int = Field(..., description="")
-    _from: int = Field(..., description="")
+    from_: int = Field(..., description="", alias="from")
     to: int = Field(..., description="")
     sync: bool = Field(
         ...,
         description="If `true` transfer is a synchronization of a replicas If `false` transfer is a moving of a shard from one peer to another",
     )
 
 
@@ -1301,26 +1427,14 @@
 class StateRole(str, Enum):
     FOLLOWER = "Follower"
     CANDIDATE = "Candidate"
     LEADER = "Leader"
     PRECANDIDATE = "PreCandidate"
 
 
-class StorageTypeOneOf(BaseModel):
-    type: Literal[
-        "in_memory",
-    ] = Field(..., description="")
-
-
-class StorageTypeOneOf1(BaseModel):
-    type: Literal[
-        "mmap",
-    ] = Field(..., description="")
-
-
 class TelemetryData(BaseModel):
     id: str = Field(..., description="")
     app: "AppBuildTelemetry" = Field(..., description="")
     collections: "CollectionsTelemetry" = Field(..., description="")
     cluster: "ClusterTelemetry" = Field(..., description="")
     requests: "RequestsTelemetry" = Field(..., description="")
 
@@ -1363,14 +1477,18 @@
 
 
 class UpdateStatus(str, Enum):
     ACKNOWLEDGED = "acknowledged"
     COMPLETED = "completed"
 
 
+class UpdateVectors(BaseModel):
+    points: List["PointVectors"] = Field(..., description="Points with named vectors")
+
+
 class ValuesCount(BaseModel):
     """
     Values count filter request
     """
 
     lt: Optional[int] = Field(default=None, description="point.key.length() &lt; values_count.lt")
     gt: Optional[int] = Field(default=None, description="point.key.length() &gt; values_count.gt")
@@ -1379,19 +1497,18 @@
 
 
 class VectorDataConfig(BaseModel):
     """
     Config of single vector data storage
     """
 
-    size: int = Field(..., description="Size of a vectors used")
+    size: int = Field(..., description="Size/dimensionality of the vectors used")
     distance: "Distance" = Field(..., description="Config of single vector data storage")
-    hnsw_config: Optional["HnswConfig"] = Field(
-        default=None, description="Vector specific HNSW config that overrides collection config"
-    )
+    storage_type: "VectorStorageType" = Field(..., description="Config of single vector data storage")
+    index: "Indexes" = Field(..., description="Config of single vector data storage")
     quantization_config: Optional["QuantizationConfig"] = Field(
         default=None, description="Vector specific quantization config that overrides collection config"
     )
 
 
 class VectorIndexSearchesTelemetry(BaseModel):
     index_name: Optional[str] = Field(default=None, description="")
@@ -1415,14 +1532,30 @@
         default=None,
         description="Custom params for HNSW index. If none - values from collection configuration are used.",
     )
     quantization_config: Optional["QuantizationConfig"] = Field(
         default=None,
         description="Custom params for quantization. If none - values from collection configuration are used.",
     )
+    on_disk: Optional[bool] = Field(
+        default=None,
+        description="If true, vectors are served from disk, improving RAM usage at the cost of latency Default: false",
+    )
+
+
+class VectorStorageTypeOneOf(str, Enum):
+    MEMORY = "Memory"
+
+
+class VectorStorageTypeOneOf1(str, Enum):
+    MMAP = "Mmap"
+
+
+class VectorStorageTypeOneOf2(str, Enum):
+    CHUNKEDMMAP = "ChunkedMmap"
 
 
 class WalConfig(BaseModel):
     wal_capacity_mb: int = Field(..., description="Size of a single WAL segment in MB")
     wal_segments_ahead: int = Field(..., description="Number of WAL segments to create ahead of actually used ones")
 
 
@@ -1471,33 +1604,39 @@
     CollectionsAggregatedTelemetry,
 ]
 Condition = Union[
     FieldCondition,
     IsEmptyCondition,
     IsNullCondition,
     HasIdCondition,
+    NestedCondition,
     Filter,
 ]
 ConsensusThreadStatus = Union[
     ConsensusThreadStatusOneOf,
     ConsensusThreadStatusOneOf1,
     ConsensusThreadStatusOneOf2,
 ]
 ExtendedPointId = Union[
     StrictInt,
     StrictStr,
 ]
+GroupId = Union[
+    StrictInt,
+    StrictStr,
+]
 Indexes = Union[
     IndexesOneOf,
     IndexesOneOf1,
 ]
 Match = Union[
     MatchValue,
     MatchText,
     MatchAny,
+    MatchExcept,
 ]
 NamedVectorStruct = Union[
     NamedVector,
     List[StrictFloat],
 ]
 OptimizersStatus = Union[
     OptimizersStatusOneOf,
@@ -1507,44 +1646,46 @@
     TextIndexParams,
 ]
 PayloadSelector = Union[
     PayloadSelectorInclude,
     PayloadSelectorExclude,
 ]
 PayloadStorageType = Union[
-    StorageTypeOneOf,
     PayloadStorageTypeOneOf,
+    PayloadStorageTypeOneOf1,
 ]
 PointInsertOperations = Union[
     PointsBatch,
     PointsList,
 ]
 PointsSelector = Union[
     PointIdsList,
     FilterSelector,
 ]
 QuantizationConfig = Union[
     ScalarQuantization,
+    ProductQuantization,
 ]
 ReadConsistency = Union[
     ReadConsistencyType,
     StrictInt,
 ]
-StorageType = Union[
-    StorageTypeOneOf,
-    StorageTypeOneOf1,
-]
 UsingVector = Union[
     StrictStr,
 ]
 ValueVariants = Union[
     StrictBool,
     StrictInt,
     StrictStr,
 ]
+VectorStorageType = Union[
+    VectorStorageTypeOneOf,
+    VectorStorageTypeOneOf1,
+    VectorStorageTypeOneOf2,
+]
 VectorStruct = Union[
     List[StrictFloat],
     Dict[StrictStr, List[StrictFloat]],
 ]
 VectorsConfig = Union[
     VectorParams,
     Dict[StrictStr, VectorParams],
```

### Comparing `qdrant_client-1.1.7/qdrant_client/local/distances.py` & `qdrant_client-1.2.0/qdrant_client/local/distances.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,15 +82,17 @@
     assert np.allclose(calculate_distance(query, vectors, models.Distance.DOT), [14.0, 14.0])
     assert np.allclose(calculate_distance(query, vectors, models.Distance.EUCLID), [0.0, 0.0])
 
     query = np.array([1.0, 0.0, 1.0])
     vectors = np.array([[1.0, 2.0, 3.0], [0.0, 1.0, 0.0]])
 
     assert np.allclose(
-        calculate_distance(query, vectors, models.Distance.COSINE), [0.75592895, 0.0], atol=0.0001
+        calculate_distance(query, vectors, models.Distance.COSINE),
+        [0.75592895, 0.0],
+        atol=0.0001,
     )
     assert np.allclose(
         calculate_distance(query, vectors, models.Distance.DOT), [4.0, 0.0], atol=0.0001
     )
     assert np.allclose(
         calculate_distance(query, vectors, models.Distance.EUCLID),
         [2.82842712, 1.7320508],
```

### Comparing `qdrant_client-1.1.7/qdrant_client/local/geo.py` & `qdrant_client-1.2.0/qdrant_client/local/geo.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/local/local_collection.py` & `qdrant_client-1.2.0/qdrant_client/local/local_collection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import uuid
-from collections import defaultdict
+from collections import OrderedDict, defaultdict
+from copy import deepcopy
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
 from qdrant_client.conversions import common_types as types
 from qdrant_client.http import models
 from qdrant_client.local.distances import (
     DistanceOrder,
     calculate_distance,
     distance_to_order,
 )
 from qdrant_client.local.payload_filters import calculate_payload_mask
+from qdrant_client.local.payload_value_extractor import value_by_key
 from qdrant_client.local.persistence import CollectionPersistence
 
 DEFAULT_VECTOR_NAME = ""
 
 
 class LocalCollection:
     """
@@ -34,41 +36,57 @@
 
         self.vectors: Dict[str, np.ndarray] = {
             name: np.zeros((0, params.size), dtype=np.float32)
             for name, params in vectors_config.items()
         }
         self.payload: List[models.Payload] = []
         self.deleted = np.zeros(0, dtype=bool)
+        self.deleted_per_vector = {name: np.zeros(0, dtype=bool) for name in self.vectors.keys()}
         self.ids: Dict[models.ExtendedPointId, int] = {}  # Mapping from external id to internal id
         self.ids_inv: List[models.ExtendedPointId] = []  # Mapping from internal id to external id
         self.persistent = location is not None
         self.storage = None
         self.config = config
         if location is not None:
             self.storage = CollectionPersistence(location)
         self.load()
 
     def load(self) -> None:
         if self.storage is not None:
             vectors = defaultdict(list)
+            deleted_ids = []
+
             for idx, point in enumerate(self.storage.load()):
                 self.ids[point.id] = idx
                 self.ids_inv.append(point.id)
 
                 vector = point.vector
                 if isinstance(point.vector, list):
                     vector = {DEFAULT_VECTOR_NAME: point.vector}
 
-                for name, vector in vector.items():
-                    vectors[name].append(vector)
+                all_vector_names = list(self.vectors.keys())
+
+                for name in all_vector_names:
+                    v = vector.get(name)
+                    if v is not None:
+                        vectors[name].append(v)
+                    else:
+                        vectors[name].append(
+                            np.ones(self.config.vectors[name].size, dtype=np.float32)
+                        )
+                        deleted_ids.append((idx, name))
 
                 self.payload.append(point.payload)
 
             for name, named_vectors in vectors.items():
                 self.vectors[name] = np.array(named_vectors)
+                self.deleted_per_vector[name] = np.zeros(len(self.payload), dtype=bool)
+
+            for idx, name in deleted_ids:
+                self.deleted_per_vector[name][idx] = 1
 
             self.deleted = np.zeros(len(self.payload), dtype=bool)
 
     @classmethod
     def _resolve_vector_name(
         cls,
         query_vector: Union[
@@ -105,19 +123,18 @@
             if name != DEFAULT_VECTOR_NAME:
                 raise ValueError(f"Vector {name} is not found in the collection")
 
             return self.config.vectors
 
         raise ValueError(f"Malformed config.vectors: {self.config.vectors}")
 
-    def _get_payload(
-        self, idx: int, with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True
-    ) -> Optional[models.Payload]:
-        payload = self.payload[idx]
-
+    @classmethod
+    def _process_payload(
+        cls, payload: dict, with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True
+    ) -> Optional[dict]:
         if not with_payload:
             return None
 
         if isinstance(with_payload, bool):
             return payload
 
         if isinstance(with_payload, list):
@@ -127,24 +144,36 @@
             return {key: payload.get(key) for key in with_payload.include if key in payload}
 
         if isinstance(with_payload, models.PayloadSelectorExclude):
             return {key: payload.get(key) for key in payload if key not in with_payload.exclude}
 
         return payload
 
+    def _get_payload(
+        self,
+        idx: int,
+        with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
+    ) -> Optional[models.Payload]:
+        payload = self.payload[idx]
+        return self._process_payload(payload, with_payload)
+
     def _get_vectors(
         self, idx: int, with_vectors: Union[bool, Sequence[str]] = False
     ) -> Optional[models.VectorStruct]:
         if not with_vectors:
             return None
 
-        vectors = {name: self.vectors[name][idx].tolist() for name in self.vectors}
+        vectors = {
+            name: self.vectors[name][idx].tolist()
+            for name in self.vectors
+            if not self.deleted_per_vector[name][idx]
+        }
 
         if isinstance(with_vectors, list):
-            vectors = {name: vectors[name] for name in with_vectors}
+            vectors = {name: vectors[name] for name in with_vectors if name in vectors}
 
         if len(vectors) == 1 and DEFAULT_VECTOR_NAME in vectors:
             return vectors[DEFAULT_VECTOR_NAME]
 
         return vectors
 
     def search(
@@ -160,15 +189,15 @@
         offset: int = 0,
         with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         score_threshold: Optional[float] = None,
     ) -> List[models.ScoredPoint]:
         payload_mask = calculate_payload_mask(
             payloads=self.payload,
-            payload_fileter=query_filter,
+            payload_filter=query_filter,
             ids_inv=self.ids_inv,
         )
         name, vector = self._resolve_vector_name(query_vector)
 
         result: List[models.ScoredPoint] = []
 
         if name not in self.vectors:
@@ -176,15 +205,15 @@
 
         vectors = self.vectors[name]
         params = self.get_vector_params(name)
         scores = calculate_distance(vector, vectors[: len(self.payload)], params.distance)
         # in deleted: 1 - deleted, 0 - not deleted
         # in payload_mask: 1 - accepted, 0 - rejected
         # in mask: 1 - ok, 0 - rejected
-        mask = payload_mask & ~self.deleted
+        mask = payload_mask & ~self.deleted & ~self.deleted_per_vector[name]
 
         required_order = distance_to_order(params.distance)
 
         if required_order == DistanceOrder.BIGGER_IS_BETTER:
             order = np.argsort(scores)[::-1]
         else:
             order = np.argsort(scores)
@@ -203,26 +232,76 @@
                 if required_order == DistanceOrder.BIGGER_IS_BETTER:
                     if score < score_threshold:
                         break
                 else:
                     if score > score_threshold:
                         break
 
-            scored_point = models.ScoredPoint(
+            scored_point = models.ScoredPoint.construct(
                 id=point_id,
                 score=score,
                 version=0,
                 payload=self._get_payload(idx, with_payload),
                 vector=self._get_vectors(idx, with_vectors),
             )
 
             result.append(scored_point)
 
         return result[offset:]
 
+    def search_groups(
+        self,
+        query_vector: Union[
+            types.NumpyArray,
+            Sequence[float],
+            Tuple[str, List[float]],
+            types.NamedVector,
+        ],
+        group_by: str,
+        query_filter: Optional[models.Filter] = None,
+        limit: int = 10,
+        group_size: int = 1,
+        with_payload: Union[bool, Sequence[str], models.PayloadSelector] = True,
+        with_vectors: Union[bool, Sequence[str]] = False,
+        score_threshold: Optional[float] = None,
+    ) -> models.GroupsResult:
+        points = self.search(
+            query_vector=query_vector,
+            query_filter=query_filter,
+            limit=len(self.ids_inv),
+            with_payload=True,
+            with_vectors=with_vectors,
+            score_threshold=score_threshold,
+        )
+
+        groups = OrderedDict()
+
+        for point in points:
+            if not isinstance(point.payload, dict):
+                continue
+
+            group_values = value_by_key(point.payload, group_by)
+            if group_values is None:
+                continue
+
+            group_values = list(set(v for v in group_values if isinstance(v, (str, int))))
+
+            point.payload = self._process_payload(point.payload, with_payload)
+
+            for group_value in group_values:
+                if group_value not in groups:
+                    groups[group_value] = models.PointGroup(id=group_value, hits=[])
+
+                if len(groups[group_value].hits) >= group_size:
+                    continue
+
+                groups[group_value].hits.append(point)
+
+        return models.GroupsResult(groups=list(groups.values())[:limit])
+
     def retrieve(
         self,
         ids: Sequence[types.PointId],
         with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
     ) -> List[models.Record]:
         result = []
@@ -241,28 +320,23 @@
                     payload=self._get_payload(idx, with_payload),
                     vector=self._get_vectors(idx, with_vectors),
                 )
             )
 
         return result
 
-    def recommend(
+    def _recommend(
         self,
         positive: Sequence[types.PointId],
         negative: Optional[Sequence[types.PointId]] = None,
         query_filter: Optional[types.Filter] = None,
-        limit: int = 10,
-        offset: int = 0,
-        with_payload: Union[bool, List[str], types.PayloadSelector] = True,
-        with_vectors: Union[bool, List[str]] = False,
-        score_threshold: Optional[float] = None,
         using: Optional[str] = None,
         lookup_from_collection: Optional["LocalCollection"] = None,
         lookup_from_vector_name: Optional[str] = None,
-    ) -> List[models.ScoredPoint]:
+    ) -> Tuple[str, List[float], Optional[types.Filter]]:
         collection = self if lookup_from_collection is None else lookup_from_collection
         search_in_vector_name = using if using is not None else DEFAULT_VECTOR_NAME
         vector_name = (
             search_in_vector_name if lookup_from_vector_name is None else lookup_from_vector_name
         )
 
         if len(positive) == 0:
@@ -305,24 +379,84 @@
             query_filter = models.Filter(must_not=[ignore_mentioned_ids])
         else:
             if query_filter.must_not is None:
                 query_filter.must_not = [ignore_mentioned_ids]
             else:
                 query_filter.must_not.append(ignore_mentioned_ids)
 
+        res_vector: List[float] = vector.tolist()  # type: ignore
+        return search_in_vector_name, res_vector, query_filter
+
+    def recommend(
+        self,
+        positive: Sequence[types.PointId],
+        negative: Optional[Sequence[types.PointId]] = None,
+        query_filter: Optional[types.Filter] = None,
+        limit: int = 10,
+        offset: int = 0,
+        with_payload: Union[bool, List[str], types.PayloadSelector] = True,
+        with_vectors: Union[bool, List[str]] = False,
+        score_threshold: Optional[float] = None,
+        using: Optional[str] = None,
+        lookup_from_collection: Optional["LocalCollection"] = None,
+        lookup_from_vector_name: Optional[str] = None,
+    ) -> List[models.ScoredPoint]:
+        search_in_vector_name, vector, query_filter = self._recommend(
+            positive,
+            negative,
+            query_filter,
+            using,
+            lookup_from_collection,
+            lookup_from_vector_name,
+        )
+
         return self.search(
             query_vector=(search_in_vector_name, vector),
             query_filter=query_filter,
             limit=limit,
             offset=offset,
             with_payload=with_payload,
             with_vectors=with_vectors,
             score_threshold=score_threshold,
         )
 
+    def recommend_groups(
+        self,
+        group_by: str,
+        positive: Sequence[types.PointId],
+        negative: Optional[Sequence[types.PointId]] = None,
+        query_filter: Optional[models.Filter] = None,
+        limit: int = 10,
+        group_size: int = 1,
+        score_threshold: Optional[float] = None,
+        with_payload: Union[bool, Sequence[str], models.PayloadSelector] = True,
+        with_vectors: Union[bool, Sequence[str]] = False,
+        using: Optional[str] = None,
+        lookup_from_collection: Optional["LocalCollection"] = None,
+        lookup_from_vector_name: Optional[str] = None,
+    ) -> types.GroupsResult:
+        search_in_vector_name, vector, query_filter = self._recommend(
+            positive,
+            negative,
+            query_filter,
+            using,
+            lookup_from_collection,
+            lookup_from_vector_name,
+        )
+        return self.search_groups(
+            query_vector=(search_in_vector_name, vector),
+            query_filter=query_filter,
+            group_by=group_by,
+            group_size=group_size,
+            limit=limit,
+            with_payload=with_payload,
+            with_vectors=with_vectors,
+            score_threshold=score_threshold,
+        )
+
     @classmethod
     def _universal_id(cls, point_id: models.ExtendedPointId) -> Tuple[str, int]:
         if isinstance(point_id, str):
             return point_id, 0
         elif isinstance(point_id, int):
             return "", point_id
         raise TypeError(f"Incompatible point id type: {type(point_id)}")
@@ -340,15 +474,15 @@
 
         sorted_ids = sorted(self.ids.items(), key=lambda x: self._universal_id(x[0]))
 
         result: List[types.Record] = []
 
         payload_mask = calculate_payload_mask(
             payloads=self.payload,
-            payload_fileter=scroll_filter,
+            payload_filter=scroll_filter,
             ids_inv=self.ids_inv,
         )
 
         mask = payload_mask & ~self.deleted
 
         for point_id, idx in sorted_ids:
             if offset is not None and self._universal_id(point_id) < self._universal_id(offset):
@@ -372,35 +506,36 @@
             return result[:limit], result[limit].id
         else:
             return result, None
 
     def count(self, count_filter: Optional[types.Filter] = None) -> models.CountResult:
         payload_mask = calculate_payload_mask(
             payloads=self.payload,
-            payload_fileter=count_filter,
+            payload_filter=count_filter,
             ids_inv=self.ids_inv,
         )
         mask = payload_mask & ~self.deleted
         return models.CountResult(count=np.count_nonzero(mask))
 
     def _update_point(self, point: models.PointStruct) -> None:
         idx = self.ids[point.id]
         self.payload[idx] = point.payload
 
         if isinstance(point.vector, list):
             vectors = {DEFAULT_VECTOR_NAME: point.vector}
         else:
             vectors = point.vector
 
-        assert (
-            vectors.keys() == self.vectors.keys()
-        ), f"Expected all vectors to be present: {vectors.keys()} != {self.vectors.keys()}"
-
-        for vector_name, vector in vectors.items():
-            self.vectors[vector_name][idx] = vector
+        for vector_name, named_vectors in self.vectors.items():
+            vector = vectors.get(vector_name)
+            if vector is not None:
+                self.vectors[vector_name][idx] = vector
+                self.deleted_per_vector[vector_name][idx] = 0
+            else:
+                self.deleted_per_vector[vector_name][idx] = 1
 
         self.deleted[idx] = 0
 
     def _add_point(self, point: models.PointStruct) -> None:
         idx = len(self.ids)
         self.ids[point.id] = idx
         self.ids_inv.append(point.id)
@@ -408,26 +543,33 @@
         self.deleted = np.append(self.deleted, 0)
 
         if isinstance(point.vector, list):
             vectors = {DEFAULT_VECTOR_NAME: point.vector}
         else:
             vectors = point.vector
 
-        assert (
-            vectors.keys() == self.vectors.keys()
-        ), f"Expected all vectors to be present: {vectors.keys()} != {self.vectors.keys()}"
-
-        for vector_name, vector in vectors.items():
-            named_vectors = self.vectors[vector_name]
+        for vector_name, named_vectors in self.vectors.items():
+            vector = vectors.get(vector_name)
             if named_vectors.shape[0] <= idx:
                 named_vectors = np.resize(named_vectors, (idx * 2 + 1, named_vectors.shape[1]))
 
-            vector_np = np.array(vector)
-            named_vectors[idx] = vector_np
-            self.vectors[vector_name] = named_vectors
+            if vector is None:
+                # Add fake vector and mark as removed
+                fake_vector = np.ones(named_vectors.shape[1])
+                named_vectors[idx] = fake_vector
+                self.deleted_per_vector[vector_name] = np.append(
+                    self.deleted_per_vector[vector_name], 1
+                )
+            else:
+                vector_np = np.array(vector)
+                named_vectors[idx] = vector_np
+                self.vectors[vector_name] = named_vectors
+                self.deleted_per_vector[vector_name] = np.append(
+                    self.deleted_per_vector[vector_name], 0
+                )
 
     def _upsert_point(self, point: models.PointStruct) -> None:
         if isinstance(point.id, str):
             # try to parse as UUID
             try:
                 _uuid = uuid.UUID(point.id)
             except ValueError as e:
@@ -465,37 +607,73 @@
                         payload=payload,
                         vector=vector,
                     )
                 )
         else:
             raise ValueError(f"Unsupported type: {type(points)}")
 
+    def _update_named_vectors(self, idx: int, vectors: Dict[str, List[float]]) -> None:
+        for vector_name, vector in vectors.items():
+            self.vectors[vector_name][idx] = np.array(vector)
+
+    def update_vectors(self, vectors: Sequence[types.PointVectors]) -> None:
+        for vector in vectors:
+            point_id = vector.id
+            idx = self.ids[point_id]
+            vector_struct = vector.vector
+            if isinstance(vector_struct, list):
+                fixed_vectors = {DEFAULT_VECTOR_NAME: vector_struct}
+            else:
+                fixed_vectors = vector_struct
+            self._update_named_vectors(idx, fixed_vectors)
+            self._persist_by_id(point_id)
+
+    def delete_vectors(
+        self,
+        vectors: Sequence[str],
+        selector: Union[
+            models.Filter,
+            List[models.ExtendedPointId],
+            models.FilterSelector,
+            models.PointIdsList,
+        ],
+    ) -> None:
+        ids = self._selector_to_ids(selector)
+        for point_id in ids:
+            idx = self.ids[point_id]
+            for vector_name in vectors:
+                self.deleted_per_vector[vector_name][idx] = 1
+            self._persist_by_id(point_id)
+
     def _delete_ids(self, ids: List[types.PointId]) -> None:
         for point_id in ids:
             idx = self.ids[point_id]
             self.deleted[idx] = 1
 
         if self.storage is not None:
             for point_id in ids:
                 self.storage.delete(point_id)
 
     def _filter_to_ids(self, delete_filter: types.Filter) -> List[models.ExtendedPointId]:
         mask = calculate_payload_mask(
             payloads=self.payload,
-            payload_fileter=delete_filter,
+            payload_filter=delete_filter,
             ids_inv=self.ids_inv,
         )
         mask = mask & ~self.deleted
         ids = [point_id for point_id, idx in self.ids.items() if mask[idx]]
         return ids
 
     def _selector_to_ids(
         self,
         selector: Union[
-            models.Filter, List[models.ExtendedPointId], models.FilterSelector, models.PointIdsList
+            models.Filter,
+            List[models.ExtendedPointId],
+            models.FilterSelector,
+            models.PointIdsList,
         ],
     ) -> List[models.ExtendedPointId]:
         if isinstance(selector, list):
             return selector
         elif isinstance(selector, models.Filter):
             return self._filter_to_ids(selector)
         elif isinstance(selector, models.PointIdsList):
@@ -504,15 +682,18 @@
             return self._filter_to_ids(selector.filter)
         else:
             raise ValueError(f"Unsupported selector type: {type(selector)}")
 
     def delete(
         self,
         selector: Union[
-            models.Filter, List[models.ExtendedPointId], models.FilterSelector, models.PointIdsList
+            models.Filter,
+            List[models.ExtendedPointId],
+            models.FilterSelector,
+            models.PointIdsList,
         ],
     ) -> None:
         ids = self._selector_to_ids(selector)
         self._delete_ids(ids)
 
     def _persist_by_id(self, point_id: models.ExtendedPointId) -> None:
         if self.storage is not None:
@@ -524,15 +705,18 @@
             )
             self.storage.persist(point)
 
     def set_payload(
         self,
         payload: models.Payload,
         selector: Union[
-            models.Filter, List[models.ExtendedPointId], models.FilterSelector, models.PointIdsList
+            models.Filter,
+            List[models.ExtendedPointId],
+            models.FilterSelector,
+            models.PointIdsList,
         ],
     ) -> None:
         ids = self._selector_to_ids(selector)
         for point_id in ids:
             idx = self.ids[point_id]
             self.payload[idx] = {
                 **(self.payload[idx] or {}),
@@ -540,42 +724,51 @@
             }
             self._persist_by_id(point_id)
 
     def overwrite_payload(
         self,
         payload: models.Payload,
         selector: Union[
-            models.Filter, List[models.ExtendedPointId], models.FilterSelector, models.PointIdsList
+            models.Filter,
+            List[models.ExtendedPointId],
+            models.FilterSelector,
+            models.PointIdsList,
         ],
     ) -> None:
         ids = self._selector_to_ids(selector)
         for point_id in ids:
             idx = self.ids[point_id]
             self.payload[idx] = payload
             self._persist_by_id(point_id)
 
     def delete_payload(
         self,
         keys: Sequence[str],
         selector: Union[
-            models.Filter, List[models.ExtendedPointId], models.FilterSelector, models.PointIdsList
+            models.Filter,
+            List[models.ExtendedPointId],
+            models.FilterSelector,
+            models.PointIdsList,
         ],
     ) -> None:
         ids = self._selector_to_ids(selector)
         for point_id in ids:
             idx = self.ids[point_id]
             for key in keys:
                 if key in self.payload[idx]:
                     self.payload[idx].pop(key)
             self._persist_by_id(point_id)
 
     def clear_payload(
         self,
         selector: Union[
-            models.Filter, List[models.ExtendedPointId], models.FilterSelector, models.PointIdsList
+            models.Filter,
+            List[models.ExtendedPointId],
+            models.FilterSelector,
+            models.PointIdsList,
         ],
     ) -> None:
         ids = self._selector_to_ids(selector)
         for point_id in ids:
             idx = self.ids[point_id]
             self.payload[idx] = {}
             self._persist_by_id(point_id)
```

### Comparing `qdrant_client-1.1.7/qdrant_client/local/payload_filters.py` & `qdrant_client-1.2.0/qdrant_client/local/payload_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,17 +67,23 @@
 def check_match(condition: models.Match, value: Any) -> bool:
     if isinstance(condition, models.MatchValue):
         return value == condition.value
     if isinstance(condition, models.MatchText):
         return value is not None and condition.text in value
     if isinstance(condition, models.MatchAny):
         return value in condition.any
+    if isinstance(condition, models.MatchExcept):
+        return value not in condition.except_
     raise ValueError(f"Unknown match condition: {condition}")
 
 
+def check_nested_filter(nested_filter: models.Filter, values: List[Any]) -> bool:
+    return any(check_filter(nested_filter, v, point_id=-1) for v in values)
+
+
 def check_condition(
     condition: models.Condition, payload: dict, point_id: models.ExtendedPointId
 ) -> bool:
     if isinstance(condition, models.IsNullCondition):
         values = value_by_key(payload, condition.is_null.key)
         if values is None:
             return False
@@ -106,14 +112,19 @@
             return any(check_geo_bounding_box(condition.geo_bounding_box, v) for v in values)
         if condition.geo_radius is not None:
             if values is None:
                 return False
             return any(check_geo_radius(condition.geo_radius, v) for v in values)
         if condition.values_count is not None:
             return check_values_count(condition.values_count, values)
+    elif isinstance(condition, models.NestedCondition):
+        values = value_by_key(payload, condition.nested.key)
+        if values is None:
+            return False
+        return check_nested_filter(condition.nested.filter, values)
     elif isinstance(condition, models.Filter):
         return check_filter(condition, payload, point_id)
     else:
         raise ValueError(f"Unknown condition: {condition}")
     return False
 
 
@@ -132,34 +143,34 @@
 def check_should(
     conditions: List[models.Condition], payload: dict, point_id: models.ExtendedPointId
 ) -> bool:
     return any(check_condition(condition, payload, point_id) for condition in conditions)
 
 
 def check_filter(
-    payload_fileter: models.Filter, payload: dict, point_id: models.ExtendedPointId
+    payload_filter: models.Filter, payload: dict, point_id: models.ExtendedPointId
 ) -> bool:
-    if payload_fileter.must is not None:
-        if not check_must(payload_fileter.must, payload, point_id):
+    if payload_filter.must is not None:
+        if not check_must(payload_filter.must, payload, point_id):
             return False
-    if payload_fileter.must_not is not None:
-        if not check_must_not(payload_fileter.must_not, payload, point_id):
+    if payload_filter.must_not is not None:
+        if not check_must_not(payload_filter.must_not, payload, point_id):
             return False
-    if payload_fileter.should is not None:
-        if not check_should(payload_fileter.should, payload, point_id):
+    if payload_filter.should is not None:
+        if not check_should(payload_filter.should, payload, point_id):
             return False
     return True
 
 
 def calculate_payload_mask(
     payloads: List[dict],
-    payload_fileter: Optional[models.Filter],
+    payload_filter: Optional[models.Filter],
     ids_inv: List[models.ExtendedPointId],
 ) -> np.ndarray:
-    if payload_fileter is None:
+    if payload_filter is None:
         return np.ones(len(payloads), dtype=bool)
 
     mask = np.zeros(len(payloads), dtype=bool)
     for i, payload in enumerate(payloads):
-        if check_filter(payload_fileter, payload, ids_inv[i]):
+        if check_filter(payload_filter, payload, ids_inv[i]):
             mask[i] = True
     return mask
```

### Comparing `qdrant_client-1.1.7/qdrant_client/local/payload_value_extractor.py` & `qdrant_client-1.2.0/qdrant_client/local/payload_value_extractor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/local/persistence.py` & `qdrant_client-1.2.0/qdrant_client/local/persistence.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/local/qdrant_local.py` & `qdrant_client-1.2.0/qdrant_client/local/qdrant_local.py`

 * *Files 14% similar despite different names*

```diff
@@ -98,15 +98,18 @@
         if collection_name in self.collections:
             return self.collections[collection_name]
         if collection_name in self.aliases:
             return self.collections[self.aliases[collection_name]]
         raise ValueError(f"Collection {collection_name} not found")
 
     def search_batch(
-        self, collection_name: str, requests: Sequence[types.SearchRequest], **kwargs: Any
+        self,
+        collection_name: str,
+        requests: Sequence[types.SearchRequest],
+        **kwargs: Any,
     ) -> List[List[types.ScoredPoint]]:
         collection = self._get_collection(collection_name)
 
         return [
             collection.search(
                 query_vector=request.vector,
                 query_filter=request.filter,
@@ -144,16 +147,50 @@
             limit=limit,
             offset=offset,
             with_payload=with_payload,
             with_vectors=with_vectors,
             score_threshold=score_threshold,
         )
 
+    def search_groups(
+        self,
+        collection_name: str,
+        query_vector: Union[
+            types.NumpyArray,
+            Sequence[float],
+            Tuple[str, List[float]],
+            types.NamedVector,
+        ],
+        group_by: str,
+        query_filter: Optional[rest_models.Filter] = None,
+        search_params: Optional[rest_models.SearchParams] = None,
+        limit: int = 10,
+        group_size: int = 1,
+        with_payload: Union[bool, Sequence[str], rest_models.PayloadSelector] = True,
+        with_vectors: Union[bool, Sequence[str]] = False,
+        score_threshold: Optional[float] = None,
+        **kwargs: Any,
+    ) -> types.GroupsResult:
+        collection = self._get_collection(collection_name)
+        return collection.search_groups(
+            query_vector=query_vector,
+            query_filter=query_filter,
+            limit=limit,
+            group_by=group_by,
+            group_size=group_size,
+            with_payload=with_payload,
+            with_vectors=with_vectors,
+            score_threshold=score_threshold,
+        )
+
     def recommend_batch(
-        self, collection_name: str, requests: Sequence[types.RecommendRequest], **kwargs: Any
+        self,
+        collection_name: str,
+        requests: Sequence[types.RecommendRequest],
+        **kwargs: Any,
     ) -> List[List[types.ScoredPoint]]:
         collection = self._get_collection(collection_name)
 
         return [
             collection.recommend(
                 positive=request.positive,
                 negative=request.negative,
@@ -196,14 +233,50 @@
             using=using,
             lookup_from_collection=self._get_collection(lookup_from.collection)
             if lookup_from
             else None,
             lookup_from_vector_name=lookup_from.vector if lookup_from else None,
         )
 
+    def recommend_groups(
+        self,
+        collection_name: str,
+        group_by: str,
+        positive: Sequence[types.PointId],
+        negative: Optional[Sequence[types.PointId]] = None,
+        query_filter: Optional[types.Filter] = None,
+        search_params: Optional[types.SearchParams] = None,
+        limit: int = 10,
+        group_size: int = 1,
+        score_threshold: Optional[float] = None,
+        with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
+        with_vectors: Union[bool, Sequence[str]] = False,
+        using: Optional[str] = None,
+        lookup_from: Optional[types.LookupLocation] = None,
+        consistency: Optional[types.ReadConsistency] = None,
+        **kwargs: Any,
+    ) -> types.GroupsResult:
+        collection = self._get_collection(collection_name)
+        return collection.recommend_groups(
+            positive=positive,
+            negative=negative,
+            group_by=group_by,
+            group_size=group_size,
+            query_filter=query_filter,
+            limit=limit,
+            with_payload=with_payload,
+            with_vectors=with_vectors,
+            score_threshold=score_threshold,
+            using=using,
+            lookup_from_collection=self._get_collection(lookup_from.collection)
+            if lookup_from
+            else None,
+            lookup_from_vector_name=lookup_from.vector if lookup_from else None,
+        )
+
     def scroll(
         self,
         collection_name: str,
         scroll_filter: Optional[types.Filter] = None,
         limit: int = 10,
         offset: Optional[types.PointId] = None,
         with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
@@ -232,14 +305,35 @@
     def upsert(
         self, collection_name: str, points: types.Points, **kwargs: Any
     ) -> types.UpdateResult:
         collection = self._get_collection(collection_name)
         collection.upsert(points)
         return self._default_update_result()
 
+    def update_vectors(
+        self,
+        collection_name: str,
+        vectors: Sequence[types.PointVectors],
+        **kwargs: Any,
+    ) -> types.UpdateResult:
+        collection = self._get_collection(collection_name)
+        collection.update_vectors(vectors)
+        return self._default_update_result()
+
+    def delete_vectors(
+        self,
+        collection_name: str,
+        vectors: Sequence[str],
+        points: types.PointsSelector,
+        **kwargs: Any,
+    ) -> types.UpdateResult:
+        collection = self._get_collection(collection_name)
+        collection.delete_vectors(vectors, points)
+        return self._default_update_result()
+
     def retrieve(
         self,
         collection_name: str,
         ids: Sequence[types.PointId],
         with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         **kwargs: Any,
```

### Comparing `qdrant_client-1.1.7/qdrant_client/parallel_processor.py` & `qdrant_client-1.2.0/qdrant_client/parallel_processor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/proto/collections.proto` & `qdrant_client-1.2.0/qdrant_client/proto/collections.proto`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 package qdrant;
 
 message VectorParams {
   uint64 size = 1; // Size of the vectors
   Distance distance = 2; // Distance function used for comparing vectors
   optional HnswConfigDiff hnsw_config = 3; // Configuration of vector HNSW graph. If omitted - the collection configuration will be used
   optional QuantizationConfig quantization_config = 4; // Configuration of vector quantization config. If omitted - the collection configuration will be used
+  optional bool on_disk = 5; // If true - serve vectors from disk. If set to false, the vectors will be loaded in RAM.
 }
 
 message VectorParamsMap {
   map<string, VectorParams> map = 1;
 }
 
 message VectorsConfig {
@@ -64,14 +65,22 @@
 }
 
 enum QuantizationType {
   UnknownQuantization = 0;
   Int8 = 1;
 }
 
+enum CompressionRatio {
+  x4 = 0;
+  x8 = 1;
+  x16 = 2;
+  x32 = 3;
+  x64 = 4;
+}
+
 message OptimizerStatus {
   bool ok = 1;
   string error = 2;
 }
 
 message HnswConfigDiff {
   /*
@@ -125,34 +134,43 @@
    - Current write RPS.
 
   It is recommended to select the default number of segments as a factor of the number of search threads,
   so that each segment would be handled evenly by one of the threads.
   */
   optional uint64 default_segment_number = 3;
   /*
-  Do not create segments larger this size (in KiloBytes).
+  Do not create segments larger this size (in kilobytes).
   Large segments might require disproportionately long indexation times,
   therefore it makes sense to limit the size of segments.
 
-  If indexation speed has more priority for you - make this parameter lower.
+  If indexing speed is more important - make this parameter lower.
   If search speed is more important - make this parameter higher.
   Note: 1Kb = 1 vector of size 256
+  If not set, will be automatically selected considering the number of available CPUs.
   */
   optional uint64 max_segment_size = 4;
   /*
-  Maximum size (in KiloBytes) of vectors to store in-memory per segment.
-  Segments larger than this threshold will be stored as a read-only memmaped file.
-  To enable memmap storage, lower the threshold
+  Maximum size (in kilobytes) of vectors to store in-memory per segment.
+  Segments larger than this threshold will be stored as read-only memmaped file.
+
+  Memmap storage is disabled by default, to enable it, set this threshold to a reasonable value.
+
+  To disable memmap storage, set this to `0`.
+
   Note: 1Kb = 1 vector of size 256
   */
   optional uint64 memmap_threshold = 5;
   /*
-  Maximum size (in KiloBytes) of vectors allowed for plain index.
-  Default value based on https://github.com/google-research/google-research/blob/master/scann/docs/algorithms.md
-  Note: 1Kb = 1 vector of size 256
+  Maximum size (in kilobytes) of vectors allowed for plain index, exceeding this threshold will enable vector indexing
+
+  Default value is 20,000, based on <https://github.com/google-research/google-research/blob/master/scann/docs/algorithms.md>.
+
+  To disable vector indexing, set to `0`.
+
+  Note: 1kB = 1 vector of size 256.
   */
   optional uint64 indexing_threshold = 6;
   /*
   Interval between forced flushes.
   */
   optional uint64 flush_interval_sec = 7;
   /*
@@ -163,17 +181,23 @@
 
 message ScalarQuantization {
   QuantizationType type = 1; // Type of quantization
   optional float quantile = 2; // Number of bits to use for quantization
   optional bool always_ram = 3; // If true - quantized vectors always will be stored in RAM, ignoring the config of main storage
 }
 
+message ProductQuantization {
+  CompressionRatio compression = 1; // Compression ratio
+  optional bool always_ram = 2; // If true - quantized vectors always will be stored in RAM, ignoring the config of main storage
+}
+
 message QuantizationConfig {
   oneof quantization {
     ScalarQuantization scalar = 1;
+    ProductQuantization product = 2;
   }
 }
 
 message CreateCollection {
   string collection_name = 1; // Name of the collection
   reserved 2; // Deprecated
   reserved 3; // Deprecated
@@ -308,7 +332,72 @@
   string collection_name = 2; // Name of the collection
 }
 
 message ListAliasesResponse {
   repeated AliasDescription aliases = 1;
   double time = 2; // Time spent to process
 }
+
+message CollectionClusterInfoRequest {
+  string collection_name = 1; // Name of the collection
+}
+
+enum ReplicaState {
+  Active = 0; // Active and sound
+  Dead = 1; // Failed for some reason
+  Partial = 2; // The shard is partially loaded and is currently receiving data from other shards
+  Initializing = 3; // Collection is being created
+  Listener = 4; // A shard which receives data, but is not used for search; Useful for backup shards
+}
+
+message LocalShardInfo {
+  uint32 shard_id = 1; // Local shard id
+  uint64 points_count = 2; // Number of points in the shard
+  ReplicaState state = 3;  // Is replica active
+}
+
+message RemoteShardInfo {
+  uint32 shard_id = 1; // Local shard id
+  uint64 peer_id = 2; // Remote peer id
+  ReplicaState state = 3; // Is replica active
+}
+
+message ShardTransferInfo {
+  uint32 shard_id = 1; // Local shard id
+  uint64 from = 2;
+  uint64 to = 3;
+  bool sync = 4; // If `true` transfer is a synchronization of a replicas; If `false` transfer is a moving of a shard from one peer to another
+}
+
+message CollectionClusterInfoResponse {
+  uint64 peer_id = 1;  // ID of this peer
+  uint64 shard_count = 2; // Total number of shards
+  repeated LocalShardInfo local_shards = 3; // Local shards
+  repeated RemoteShardInfo remote_shards = 4; // Remote shards
+  repeated ShardTransferInfo shard_transfers = 5; // Shard transfers
+}
+
+message MoveShard {
+  uint32 shard_id = 1; // Local shard id
+  uint64 from_peer_id = 2;
+  uint64 to_peer_id = 3;
+}
+
+message Replica {
+  uint32 shard_id = 1;
+  uint64 peer_id = 2;
+}
+
+message UpdateCollectionClusterSetupRequest {
+  string collection_name = 1; // Name of the collection
+  oneof operation {
+    MoveShard move_shard = 2;
+    MoveShard replicate_shard = 3;
+    MoveShard abort_transfer = 4;
+    Replica drop_replica = 5;
+  }
+  optional uint64 timeout = 6; // Wait timeout for operation commit in seconds, if not specified - default value will be supplied
+}
+
+message UpdateCollectionClusterSetupResponse {
+  bool result = 1;
+}
```

### Comparing `qdrant_client-1.1.7/qdrant_client/proto/collections_service.proto` & `qdrant_client-1.2.0/qdrant_client/proto/collections_service.proto`

 * *Files 11% similar despite different names*

```diff
@@ -33,8 +33,16 @@
   Get list of all aliases for a collection
   */
   rpc ListCollectionAliases (ListCollectionAliasesRequest) returns (ListAliasesResponse) {}
   /*
   Get list of all aliases for all existing collections
   */
   rpc ListAliases (ListAliasesRequest) returns (ListAliasesResponse) {}
+  /*
+  Get cluster information for a collection
+  */
+  rpc CollectionClusterInfo (CollectionClusterInfoRequest) returns (CollectionClusterInfoResponse) {}
+  /*
+  Update cluster setup for a collection
+  */
+  rpc UpdateCollectionClusterSetup (UpdateCollectionClusterSetupRequest) returns (UpdateCollectionClusterSetupResponse) {}
 }
```

### Comparing `qdrant_client-1.1.7/qdrant_client/proto/json_with_int.proto` & `qdrant_client-1.2.0/qdrant_client/proto/json_with_int.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/proto/points.proto` & `qdrant_client-1.2.0/qdrant_client/proto/points.proto`

 * *Files 9% similar despite different names*

```diff
@@ -67,14 +67,34 @@
   repeated PointId ids = 2; // List of points to retrieve
   reserved 3; // deprecated "with_vector" field
   WithPayloadSelector with_payload = 4; // Options for specifying which payload to include or not
   optional WithVectorsSelector with_vectors = 5; // Options for specifying which vectors to include into response
   optional ReadConsistency read_consistency = 6; // Options for specifying read consistency guarantees
 }
 
+message UpdatePointVectors {
+  string collection_name = 1; // name of the collection
+  optional bool wait = 2; // Wait until the changes have been applied?
+  repeated PointVectors points = 3; // List of points and vectors to update
+  optional WriteOrdering ordering = 4; // Write ordering guarantees
+}
+
+message PointVectors {
+  PointId id = 1; // ID to update vectors for
+  Vectors vectors = 2; // Named vectors to update, leave others intact
+}
+
+message DeletePointVectors {
+  string collection_name = 1; // name of the collection
+  optional bool wait = 2; // Wait until the changes have been applied?
+  PointsSelector points_selector = 3; // Affected points
+  VectorsSelector vectors = 4; // List of vector names to delete
+  optional WriteOrdering ordering = 5; // Write ordering guarantees
+}
+
 message SetPayloadPoints {
   string collection_name = 1; // name of the collection
   optional bool wait = 2; // Wait until the changes have been applied?
   map<string, Value> payload = 3; // New payload values
   reserved 4; // List of point to modify, deprecated
   optional PointsSelector points_selector = 5; // Affected points
   optional WriteOrdering ordering = 6; // Write ordering guarantees
@@ -205,14 +225,29 @@
 
 message SearchBatchPoints {
   string collection_name = 1; // Name of the collection
   repeated SearchPoints search_points = 2;
   optional ReadConsistency read_consistency = 3; // Options for specifying read consistency guarantees
 }
 
+message SearchPointGroups {
+  string collection_name = 1; // Name of the collection
+  repeated float vector = 2; // Vector to compare against
+  Filter filter = 3; // Filter conditions - return only those points that satisfy the specified conditions
+  uint32 limit = 4; // Max number of result
+  WithPayloadSelector with_payload = 5; // Options for specifying which payload to include or not
+  SearchParams params = 6; // Search config
+  optional float score_threshold = 7; // If provided - cut off results with worse scores
+  optional string vector_name = 8; // Which vector to use for search, if not specified - use default vector
+  optional WithVectorsSelector with_vectors = 9; // Options for specifying which vectors to include into response
+  string group_by = 10; // Payload field to group by, must be a string or number field. If there are multiple values for the field, all of them will be used. One point can be in multiple groups.
+  uint32 group_size = 11; // Maximum amount of points to return per group
+  optional ReadConsistency read_consistency = 12; // Options for specifying read consistency guarantees
+}
+
 message ScrollPoints {
   string collection_name = 1;
   Filter filter = 2; // Filter conditions - return only those points that satisfy the specified conditions
   optional PointId offset = 3; // Start with this ID
   optional uint32 limit = 4; // Max number of result
   reserved 5; // deprecated "with_vector" field
   WithPayloadSelector with_payload = 6; // Options for specifying which payload to include or not
@@ -244,14 +279,31 @@
 
 message RecommendBatchPoints {
   string collection_name = 1; // Name of the collection
   repeated RecommendPoints recommend_points = 2;
   optional ReadConsistency read_consistency = 3; // Options for specifying read consistency guarantees
 }
 
+message RecommendPointGroups {
+  string collection_name = 1; // Name of the collection
+  repeated PointId positive = 2; // Look for vectors closest to those
+  repeated PointId negative = 3; // Try to avoid vectors like this
+  Filter filter = 4; // Filter conditions - return only those points that satisfy the specified conditions
+  uint32 limit = 5; // Max number of groups in result
+  WithPayloadSelector with_payload = 6; // Options for specifying which payload to include or not
+  SearchParams params = 7; // Search config
+  optional float score_threshold = 8; // If provided - cut off results with worse scores
+  optional string using = 9; // Define which vector to use for recommendation, if not specified - default vector
+  optional WithVectorsSelector with_vectors = 10; // Options for specifying which vectors to include into response
+  optional LookupLocation lookup_from = 11; // Name of the collection to use for points lookup, if not specified - use current collection
+  string group_by = 12; // Payload field to group by, must be a string or number field. If there are multiple values for the field, all of them will be used. One point can be in multiple groups.
+  uint32 group_size = 13; // Maximum amount of points to return per group
+  optional ReadConsistency read_consistency = 14; // Options for specifying read consistency guarantees
+}
+
 message CountPoints {
   string collection_name = 1; // name of the collection
   Filter filter = 2; // Filter conditions - return only those points that satisfy the specified conditions
   optional bool exact = 3; // If `true` - return exact count, if `false` - return approximate count
 }
 
 // ---------------------------------------------
@@ -279,28 +331,53 @@
   map<string, Value> payload = 2; // Payload
   float score = 3; // Similarity score
   reserved 4; // deprecated "vector" field
   uint64 version = 5; // Last update operation applied to this point
   optional Vectors vectors = 6; // Vectors to search
 }
 
+message GroupId {
+  oneof kind {
+    // Represents a double value.
+    uint64 unsigned_value = 1;
+    // Represents an integer value
+    int64 integer_value = 2;
+    // Represents a string value.
+    string string_value = 3;
+  }
+}
+
+message PointGroup {
+  GroupId id = 1; // Group id
+  repeated ScoredPoint hits = 2; // Points in the group
+}
+
+message GroupsResult {
+  repeated PointGroup groups = 1; // Groups
+}
+
 message SearchResponse {
   repeated ScoredPoint result = 1;
   double time = 2; // Time spent to process
 }
 
 message BatchResult {
   repeated ScoredPoint result = 1;
 }
 
 message SearchBatchResponse {
   repeated BatchResult result = 1;
   double time = 2; // Time spent to process
 }
 
+message SearchGroupsResponse {
+  GroupsResult result = 1;
+  double time = 2; // Time spent to process
+}
+
 message CountResponse {
   CountResult result = 1;
   double time = 2; // Time spent to process
 }
 
 message ScrollResponse {
   optional PointId next_page_offset = 1; // Use this offset for the next query
@@ -330,14 +407,19 @@
 }
 
 message RecommendBatchResponse {
   repeated BatchResult result = 1;
   double time = 2; // Time spent to process
 }
 
+message RecommendGroupsResponse {
+  GroupsResult result = 1;
+  double time = 2; // Time spent to process
+}
+
 // ---------------------------------------------
 // ------------- Filter Conditions -------------
 // ---------------------------------------------
 
 message Filter {
   repeated Condition should = 1; // At least one of those conditions should match
   repeated Condition must = 2; // All conditions must match
@@ -347,14 +429,15 @@
 message Condition {
   oneof condition_one_of {
     FieldCondition field = 1;
     IsEmptyCondition is_empty = 2;
     HasIdCondition has_id = 3;
     Filter filter = 4;
     IsNullCondition is_null = 5;
+    NestedCondition nested = 6;
   }
 }
 
 message IsEmptyCondition {
   string key = 1;
 }
 
@@ -362,14 +445,19 @@
     string key = 1;
 }
 
 message HasIdCondition {
   repeated PointId has_id = 1;
 }
 
+message NestedCondition {
+  string key = 1; // Path to nested object
+  Filter filter = 2; // Filter condition
+}
+
 message FieldCondition {
   string key = 1;
   Match match = 2; // Check if point has field with a given value
   Range range = 3; // Check if points value lies in a given range
   GeoBoundingBox geo_bounding_box = 4; // Check if points geolocation lies in a given area
   GeoRadius geo_radius = 5; // Check if geo point is within a given radius
   ValuesCount values_count = 6; // Check number of values for a specific field
@@ -379,14 +467,16 @@
   oneof match_value {
     string keyword = 1; // Match string keyword
     int64 integer = 2; // Match integer
     bool boolean = 3; // Match boolean
     string text = 4; // Match text
     RepeatedStrings keywords = 5; // Match multiple keywords
     RepeatedIntegers integers = 6; // Match multiple integers
+    RepeatedIntegers except_integers = 7; // Match any other value except those integers
+    RepeatedStrings except_keywords = 8; // Match any other value except those keywords
   }
 }
 
 message RepeatedStrings {
   repeated string strings = 1;
 }
```

### Comparing `qdrant_client-1.1.7/qdrant_client/proto/points_service.proto` & `qdrant_client-1.2.0/qdrant_client/proto/points_service.proto`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,22 @@
    */
   rpc Delete (DeletePoints) returns (PointsOperationResponse) {}
   /*
   Retrieve points
    */
   rpc Get (GetPoints) returns (GetResponse) {}
   /*
+  Update named vectors for point
+   */
+  rpc UpdateVectors (UpdatePointVectors) returns (PointsOperationResponse) {}
+  /*
+  Delete named vectors for points
+   */
+  rpc DeleteVectors (DeletePointVectors) returns (PointsOperationResponse) {}
+  /*
   Set payload for points
    */
   rpc SetPayload (SetPayloadPoints) returns (PointsOperationResponse) {}
   /*
   Overwrite payload for points
    */
   rpc OverwritePayload (SetPayloadPoints) returns (PointsOperationResponse) {}
@@ -48,23 +56,31 @@
    */
   rpc Search (SearchPoints) returns (SearchResponse) {}
   /*
    Retrieve closest points based on vector similarity and given filtering conditions
     */
   rpc SearchBatch (SearchBatchPoints) returns (SearchBatchResponse) {}
   /*
+  Retrieve closest points based on vector similarity and given filtering conditions, grouped by a given field
+   */
+  rpc SearchGroups (SearchPointGroups) returns (SearchGroupsResponse) {}
+  /*
   Iterate over all or filtered points points
   */
   rpc Scroll (ScrollPoints) returns (ScrollResponse) {}
   /*
   Look for the points which are closer to stored positive examples and at the same time further to negative examples.
    */
   rpc Recommend (RecommendPoints) returns (RecommendResponse) {}
   /*
   Look for the points which are closer to stored positive examples and at the same time further to negative examples.
    */
   rpc RecommendBatch (RecommendBatchPoints) returns (RecommendBatchResponse) {}
+    /*
+  Look for the points which are closer to stored positive examples and at the same time further to negative examples, grouped by a given field
+   */
+  rpc RecommendGroups (RecommendPointGroups) returns (RecommendGroupsResponse) {}
   /*
    Count points in collection with given filtering conditions
    */
   rpc Count (CountPoints) returns (CountResponse) {}
 }
```

### Comparing `qdrant_client-1.1.7/qdrant_client/proto/snapshots_service.proto` & `qdrant_client-1.2.0/qdrant_client/proto/snapshots_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/qdrant_client/qdrant_client.py` & `qdrant_client-1.2.0/qdrant_client/qdrant_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -186,22 +186,28 @@
                 - 'quorum' - query the majority of replicas, return values present in all of them
                 - 'all' - query all replicas, and return values present in all replicas
 
         Returns:
             List of search responses
         """
         return self._client.search_batch(
-            collection_name=collection_name, requests=requests, consistency=consistency, **kwargs
+            collection_name=collection_name,
+            requests=requests,
+            consistency=consistency,
+            **kwargs,
         )
 
     def search(
         self,
         collection_name: str,
         query_vector: Union[
-            types.NumpyArray, Sequence[float], Tuple[str, List[float]], types.NamedVector
+            types.NumpyArray,
+            Sequence[float],
+            Tuple[str, List[float]],
+            types.NamedVector,
         ],
         query_filter: Optional[types.Filter] = None,
         search_params: Optional[types.SearchParams] = None,
         limit: int = 10,
         offset: int = 0,
         with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
@@ -285,14 +291,97 @@
             with_vectors=with_vectors,
             score_threshold=score_threshold,
             append_payload=append_payload,
             consistency=consistency,
             **kwargs,
         )
 
+    def search_groups(
+        self,
+        collection_name: str,
+        query_vector: Union[
+            types.NumpyArray,
+            Sequence[float],
+            Tuple[str, List[float]],
+            types.NamedVector,
+        ],
+        group_by: str,
+        query_filter: Optional[types.Filter] = None,
+        search_params: Optional[types.SearchParams] = None,
+        limit: int = 10,
+        group_size: int = 1,
+        with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
+        with_vectors: Union[bool, Sequence[str]] = False,
+        score_threshold: Optional[float] = None,
+        consistency: Optional[types.ReadConsistency] = None,
+        **kwargs: Any,
+    ) -> types.GroupsResult:
+        """Search for closest vectors grouped by payload field.
+
+        Searches best matches for query vector grouped by the value of payload field.
+        Useful to obtain most relevant results for each category, deduplicate results,
+        finding the best representation vector for the same entity.
+
+        Args:
+            collection_name: Collection to search in
+            query_vector:
+                Search for vectors closest to this.
+                Can be either a vector itself, or a named vector, or a tuple of vector name and vector itself
+            group_by: Name of the payload field to group by.
+                Field must be of type "keyword" or "integer".
+                Nested fields are specified using dot notation, e.g. "nested_field.subfield".
+            query_filter:
+                - Exclude vectors which doesn't fit given conditions.
+                - If `None` - search among all vectors
+            search_params: Additional search params
+            limit: How many groups return
+            group_size: How many results return for each group
+            with_payload:
+                - Specify which stored payload should be attached to the result.
+                - If `True` - attach all payload
+                - If `False` - do not attach any payload
+                - If List of string - include only specified fields
+                - If `PayloadSelector` - use explicit rules
+            with_vectors:
+                - If `True` - Attach stored vector to the search result.
+                - If `False` - Do not attach vector.
+                - If List of string - include only specified fields
+                - Default: `False`
+            score_threshold: Minimal score threshold for the result.
+                If defined, less similar results will not be returned.
+                Score of the returned result might be higher or smaller than the threshold depending
+                on the Distance function used.
+                E.g. for cosine similarity only higher scores will be returned.
+            consistency:
+                Read consistency of the search. Defines how many replicas should be queried before returning the result.
+                Values:
+                - int - number of replicas to query, values should present in all queried replicas
+                - 'majority' - query all replicas, but return values present in the majority of replicas
+                - 'quorum' - query the majority of replicas, return values present in all of them
+                - 'all' - query all replicas, and return values present in all replicas
+
+        Returns:
+            List of groups with not more than `group_size` hits in each group.
+            Each group also contains an id of the group, which is the value of the payload field.
+        """
+        return self._client.search_groups(
+            collection_name=collection_name,
+            query_vector=query_vector,
+            group_by=group_by,
+            query_filter=query_filter,
+            search_params=search_params,
+            limit=limit,
+            group_size=group_size,
+            with_payload=with_payload,
+            with_vectors=with_vectors,
+            score_threshold=score_threshold,
+            consistency=consistency,
+            **kwargs,
+        )
+
     def recommend_batch(
         self,
         collection_name: str,
         requests: Sequence[types.RecommendRequest],
         consistency: Optional[types.ReadConsistency] = None,
         **kwargs: Any,
     ) -> List[List[types.ScoredPoint]]:
@@ -309,15 +398,18 @@
                 - 'quorum' - query the majority of replicas, return values present in all of them
                 - 'all' - query all replicas, and return values present in all replicas
 
         Returns:
             List of recommend responses
         """
         return self._client.recommend_batch(
-            collection_name=collection_name, requests=requests, consistency=consistency, **kwargs
+            collection_name=collection_name,
+            requests=requests,
+            consistency=consistency,
+            **kwargs,
         )
 
     def recommend(
         self,
         collection_name: str,
         positive: Sequence[types.PointId],
         negative: Optional[Sequence[types.PointId]] = None,
@@ -405,14 +497,112 @@
             score_threshold=score_threshold,
             using=using,
             lookup_from=lookup_from,
             consistency=consistency,
             **kwargs,
         )
 
+    def recommend_groups(
+        self,
+        collection_name: str,
+        group_by: str,
+        positive: Sequence[types.PointId],
+        negative: Optional[Sequence[types.PointId]] = None,
+        query_filter: Optional[types.Filter] = None,
+        search_params: Optional[types.SearchParams] = None,
+        limit: int = 10,
+        group_size: int = 1,
+        score_threshold: Optional[float] = None,
+        with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
+        with_vectors: Union[bool, Sequence[str]] = False,
+        using: Optional[str] = None,
+        lookup_from: Optional[types.LookupLocation] = None,
+        consistency: Optional[types.ReadConsistency] = None,
+        **kwargs: Any,
+    ) -> types.GroupsResult:
+        """Recommend point groups: search for similar points based on already stored in Qdrant examples
+        and groups by payload field.
+
+        Recommend best matches for given stored examples grouped by the value of payload field.
+        Useful to obtain most relevant results for each category, deduplicate results,
+        finding the best representation vector for the same entity.
+
+        Args:
+            collection_name: Collection to search in
+            positive:
+                List of stored point IDs, which should be used as reference for similarity search.
+                If there is only one ID provided - this request is equivalent to the regular search with vector of that point.
+                If there are more than one IDs, Qdrant will attempt to search for similar to all of them.
+                Recommendation for multiple vectors is experimental. Its behaviour may change in the future.
+            negative:
+                List of stored point IDs, which should be dissimilar to the search result.
+                Negative examples is an experimental functionality. Its behaviour may change in the future.
+            group_by: Name of the payload field to group by.
+                Field must be of type "keyword" or "integer".
+                Nested fields are specified using dot notation, e.g. "nested_field.subfield".
+            query_filter:
+                - Exclude vectors which doesn't fit given conditions.
+                - If `None` - search among all vectors
+            search_params: Additional search params
+            limit: How many groups return
+            group_size: How many results return for each group
+            with_payload:
+                - Specify which stored payload should be attached to the result.
+                - If `True` - attach all payload
+                - If `False` - do not attach any payload
+                - If List of string - include only specified fields
+                - If `PayloadSelector` - use explicit rules
+            with_vectors:
+                - If `True` - Attach stored vector to the search result.
+                - If `False` - Do not attach vector.
+                - If List of string - include only specified fields
+                - Default: `False`
+            score_threshold:
+                Define a minimal score threshold for the result.
+                If defined, less similar results will not be returned.
+                Score of the returned result might be higher or smaller than the threshold depending
+                on the Distance function used.
+                E.g. for cosine similarity only higher scores will be returned.
+            using:
+                Name of the vectors to use for recommendations.
+                If `None` - use default vectors.
+            lookup_from:
+                Defines a location (collection and vector field name), used to lookup vectors for recommendations.
+                If `None` - use current collection will be used.
+            consistency:
+                Read consistency of the search. Defines how many replicas should be queried before returning the result.
+                Values:
+                - int - number of replicas to query, values should present in all queried replicas
+                - 'majority' - query all replicas, but return values present in the majority of replicas
+                - 'quorum' - query the majority of replicas, return values present in all of them
+                - 'all' - query all replicas, and return values present in all replicas
+
+        Returns:
+            List of groups with not more than `group_size` hits in each group.
+            Each group also contains an id of the group, which is the value of the payload field.
+
+        """
+        return self._client.recommend_groups(
+            collection_name=collection_name,
+            group_by=group_by,
+            positive=positive,
+            negative=negative,
+            query_filter=query_filter,
+            search_params=search_params,
+            limit=limit,
+            group_size=group_size,
+            score_threshold=score_threshold,
+            with_payload=with_payload,
+            with_vectors=with_vectors,
+            using=using,
+            lookup_from=lookup_from,
+            consistency=consistency,
+            **kwargs,
+        )
+
     def scroll(
         self,
         collection_name: str,
         scroll_filter: Optional[types.Filter] = None,
         limit: int = 10,
         offset: Optional[types.PointId] = None,
         with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
@@ -482,15 +672,18 @@
                 If `True` - provide the exact count of points matching the filter.
                 If `False` - provide the approximate count of points matching the filter. Works faster.
 
         Returns:
             Amount of points in the collection matching the filter.
         """
         return self._client.count(
-            collection_name=collection_name, count_filter=count_filter, exact=exact, **kwargs
+            collection_name=collection_name,
+            count_filter=count_filter,
+            exact=exact,
+            **kwargs,
         )
 
     def upsert(
         self,
         collection_name: str,
         points: types.Points,
         wait: bool = True,
@@ -516,15 +709,93 @@
                 - 'strong' - Write operations go through the permanent leader,
                     consistent, but may be unavailable if leader is down
 
         Returns:
             Operation result
         """
         return self._client.upsert(
-            collection_name=collection_name, points=points, wait=wait, ordering=ordering, **kwargs
+            collection_name=collection_name,
+            points=points,
+            wait=wait,
+            ordering=ordering,
+            **kwargs,
+        )
+
+    def update_vectors(
+        self,
+        collection_name: str,
+        vectors: Sequence[types.PointVectors],
+        wait: bool = True,
+        ordering: Optional[types.WriteOrdering] = None,
+        **kwargs: Any,
+    ) -> types.UpdateResult:
+        """Update specified vectors in the collection. Keeps payload and unspecified vectors unchanged.
+
+        Args:
+            collection_name: Name of the collection to update vectors in
+            vectors: List of (id, vector) pairs to update. Vector might be a list of numbers or a dict of named vectors.
+                Example
+                - `PointVectors(id=1, vector=[1, 2, 3])`
+                - `PointVectors(id=2, vector={'vector_1': [1, 2, 3], 'vector_2': [4, 5, 6]})`
+            wait: Await for the results to be processed.
+            ordering: Define strategy for ordering of the points. Possible values:
+                - 'weak' - write operations may be reordered, works faster, default
+                - 'medium' - write operations go through dynamically selected leader,
+                    may be inconsistent for a short period of time in case of leader change
+                - 'strong' - Write operations go through the permanent leader,
+                    consistent, but may be unavailable if leader is down
+
+        Returns:
+            Operation result
+        """
+        return self._client.update_vectors(
+            collection_name=collection_name,
+            vectors=vectors,
+            wait=wait,
+            ordering=ordering,
+        )
+
+    def delete_vectors(
+        self,
+        collection_name: str,
+        vectors: Sequence[str],
+        points: types.PointsSelector,
+        wait: bool = True,
+        ordering: Optional[types.WriteOrdering] = None,
+        **kwargs: Any,
+    ) -> types.UpdateResult:
+        """Delete specified vector from the collection. Does not affect payload.
+
+        Args:
+            collection_name: Name of the collection to delete vector from
+            vectors:
+                List of names of the vectors to delete.
+                Use `""` to delete the default vector.
+                At least one vector should be specified.
+            points: Selects points based on list of IDs or filter
+                 Examples
+                    - `points=[1, 2, 3, "cd3b53f0-11a7-449f-bc50-d06310e7ed90"]`
+                    - `points=Filter(must=[FieldCondition(key='rand_number', range=Range(gte=0.7))])`
+            wait: Await for the results to be processed.
+            ordering: Define strategy for ordering of the points. Possible values:
+                - 'weak' - write operations may be reordered, works faster, default
+                - 'medium' - write operations go through dynamically selected leader,
+                    may be inconsistent for a short period of time in case of leader change
+                - 'strong' - Write operations go through the permanent leader,
+                    consistent, but may be unavailable if leader is down
+
+        Returns:
+            Operation result
+        """
+        return self._client.delete_vectors(
+            collection_name=collection_name,
+            vectors=vectors,
+            points=points,
+            wait=wait,
+            ordering=ordering,
         )
 
     def retrieve(
         self,
         collection_name: str,
         ids: Sequence[types.PointId],
         with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
@@ -581,15 +852,15 @@
         Args:
             collection_name: Name of the collection
             wait: Await for the results to be processed.
 
                 - If `true`, result will be returned only when all changes are applied
                 - If `false`, result will be returned immediately after the confirmation of receiving.
             points_selector: Selects points based on list of IDs or filter
-                Example:
+                Examples
                     - `points=[1, 2, 3, "cd3b53f0-11a7-449f-bc50-d06310e7ed90"]`
                     - `points=Filter(must=[FieldCondition(key='rand_number', range=Range(gte=0.7))])`
             ordering: Define strategy for ordering of the points. Possible values:
 
                 - 'weak' - write operations may be reordered, works faster, default
                 - 'medium' - write operations go through dynamically selected leader,
                     may be inconsistent for a short period of time in case of leader change
@@ -637,15 +908,15 @@
             collection_name: Name of the collection
             wait: Await for the results to be processed.
 
                 - If `true`, result will be returned only when all changes are applied
                 - If `false`, result will be returned immediately after the confirmation of receiving.
             payload: Key-value pairs of payload to assign
             points: List of affected points, filter or points selector.
-             Example:
+             Example
                 - `points=[1, 2, 3, "cd3b53f0-11a7-449f-bc50-d06310e7ed90"]`
                 - `points=Filter(must=[FieldCondition(key='rand_number', range=Range(gte=0.7))])`
             ordering:
                 Define strategy for ordering of the points. Possible values:
                 - 'weak' - write operations may be reordered, works faster, default
                 - 'medium' - write operations go through dynamically selected leader,
                     may be inconsistent for a short period of time in case of leader change
@@ -696,15 +967,15 @@
             collection_name: Name of the collection
             wait: Await for the results to be processed.
 
                 - If `true`, result will be returned only when all changes are applied
                 - If `false`, result will be returned immediately after the confirmation of receiving.
             payload: Key-value pairs of payload to assign
             points: List of affected points, filter or points selector.
-             Example:
+             Example
                 - `points=[1, 2, 3, "cd3b53f0-11a7-449f-bc50-d06310e7ed90"]`
                 - `points=Filter(must=[FieldCondition(key='rand_number', range=Range(gte=0.7))])`
             ordering:
                 Define strategy for ordering of the points. Possible values:
                 - 'weak' - write operations may be reordered, works faster, default
                 - 'medium' - write operations go through dynamically selected leader,
                     may be inconsistent for a short period of time in case of leader change
@@ -738,15 +1009,15 @@
             collection_name: Name of the collection
             wait: Await for the results to be processed.
 
                 - If `true`, result will be returned only when all changes are applied
                 - If `false`, result will be returned immediately after the confirmation of receiving.
             keys: List of payload keys to remove
             points: List of affected points, filter or points selector.
-                Example:
+                Example
                    - `points=[1, 2, 3, "cd3b53f0-11a7-449f-bc50-d06310e7ed90"]`
                    - `points=Filter(must=[FieldCondition(key='rand_number', range=Range(gte=0.7))])`
             ordering:
                 Define strategy for ordering of the points. Possible values:
                 - 'weak' - write operations may be reordered, works faster, default
                 - 'medium' - write operations go through dynamically selected leader,
                     may be inconsistent for a short period of time in case of leader change
@@ -778,15 +1049,15 @@
         Args:
             collection_name: Name of the collection
             wait: Await for the results to be processed.
 
                 - If `true`, result will be returned only when all changes are applied
                 - If `false`, result will be returned immediately after the confirmation of receiving.
             points_selector: List of affected points, filter or points selector.
-                Example:
+                Example
                    - `points=[1, 2, 3, "cd3b53f0-11a7-449f-bc50-d06310e7ed90"]`
                    - `points=Filter(must=[FieldCondition(key='rand_number', range=Range(gte=0.7))])`
             ordering:
                 Define strategy for ordering of the points. Possible values:
                 - 'weak' - write operations may be reordered, works faster, default
                 - 'medium' - write operations go through dynamically selected leader,
                     may be inconsistent for a short period of time in case of leader change
@@ -820,15 +1091,17 @@
                 Wait for operation commit timeout in seconds.
                 If timeout is reached - request will return with service error.
 
         Returns:
             Operation result
         """
         return self._client.update_collection_aliases(
-            change_aliases_operations=change_aliases_operations, timeout=timeout, **kwargs
+            change_aliases_operations=change_aliases_operations,
+            timeout=timeout,
+            **kwargs,
         )
 
     def get_collection_aliases(
         self, collection_name: str, **kwargs: Any
     ) -> types.CollectionsAliasesResponse:
         """Get collection aliases
 
@@ -1293,15 +1566,18 @@
                 Defines source of truth for snapshot recovery
                     - `snapshot` means - prefer snapshot data over the current state
                     - `replica` means - prefer existing data over the snapshot
                 Default: `replica`
 
         """
         return self._client.recover_snapshot(
-            collection_name=collection_name, location=location, priority=priority, **kwargs
+            collection_name=collection_name,
+            location=location,
+            priority=priority,
+            **kwargs,
         )
 
     def lock_storage(self, reason: str, **kwargs: Any) -> types.LocksOption:
         """Lock storage for writing."""
         return self._client.lock_storage(reason=reason, **kwargs)
 
     def unlock_storage(self, **kwargs: Any) -> types.LocksOption:
```

### Comparing `qdrant_client-1.1.7/qdrant_client/uploader/grpc_uploader.py` & `qdrant_client-1.2.0/qdrant_client/uploader/grpc_uploader.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from qdrant_client.conversions.conversion import RestToGrpc, payload_to_grpc
 from qdrant_client.grpc import PointId, PointsStub, PointStruct
 from qdrant_client.http.models import Batch
 from qdrant_client.uploader.uploader import BaseUploader
 
 
 def upload_batch_grpc(
-    points_client: PointsStub, collection_name: str, batch: Union[Batch, Tuple], max_retries: int
+    points_client: PointsStub,
+    collection_name: str,
+    batch: Union[Batch, Tuple],
+    max_retries: int,
 ) -> bool:
     ids_batch, vectors_batch, payload_batch = batch
     if payload_batch is None:
         payload_batch = (None for _ in count())
 
     points = [
         PointStruct(
@@ -39,15 +42,20 @@
             continue
 
     return False  # suppress mypy complaints
 
 
 class GrpcBatchUploader(BaseUploader):
     def __init__(
-        self, host: str, port: int, collection_name: str, max_retries: int, **kwargs: Any
+        self,
+        host: str,
+        port: int,
+        collection_name: str,
+        max_retries: int,
+        **kwargs: Any,
     ):
         self.collection_name = collection_name
         self._host = host
         self._port = port
         self.max_retries = max_retries
         self._kwargs = kwargs
```

### Comparing `qdrant_client-1.1.7/qdrant_client/uploader/rest_uploader.py` & `qdrant_client-1.2.0/qdrant_client/uploader/rest_uploader.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 from qdrant_client.http import SyncApis
 from qdrant_client.http.models import Batch, PointsList, PointStruct
 from qdrant_client.uploader.uploader import BaseUploader
 
 
 def upload_batch(
-    openapi_client: SyncApis, collection_name: str, batch: Union[Tuple, Batch], max_retries: int
+    openapi_client: SyncApis,
+    collection_name: str,
+    batch: Union[Tuple, Batch],
+    max_retries: int,
 ) -> bool:
     ids_batch, vectors_batch, payload_batch = batch
 
     # Make sure we do not send too many ids in case there is an iterable over vectors,
     # and we do not know how many ids are required in advance
     if len(ids_batch) > len(vectors_batch):
         ids_batch = ids_batch[: len(vectors_batch)]
@@ -30,15 +33,16 @@
         )
         for idx, vector, payload in zip(ids_batch, vectors_batch, payload_batch)
     ]
 
     for attempt in range(max_retries):
         try:
             openapi_client.points_api.upsert_points(
-                collection_name=collection_name, point_insert_operations=PointsList(points=points)
+                collection_name=collection_name,
+                point_insert_operations=PointsList(points=points),
             )
             return True
         except Exception as e:
             if attempt == (max_retries - 1):  # pylint: disable=broad-except
                 logging.exception(e)
                 return False
         else:
```

### Comparing `qdrant_client-1.1.7/qdrant_client/uploader/uploader.py` & `qdrant_client-1.2.0/qdrant_client/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.7/PKG-INFO` & `qdrant_client-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-client
-Version: 1.1.7
+Version: 1.2.0
 Summary: Client library for the Qdrant vector search engine
 Home-page: https://github.com/qdrant/qdrant-client
 Keywords: vector,search,neural,matching,client
 Author: Andrey Vasnetsov
 Author-email: andrey@qdrant.tech
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Requires-Dist: grpcio (>=1.41.0)
 Requires-Dist: grpcio-tools (>=1.41.0)
 Requires-Dist: httpx[http2] (>=0.14.0)
 Requires-Dist: numpy (<1.21) ; python_version < "3.8"
 Requires-Dist: numpy (>=1.21) ; python_version >= "3.8"
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: pydantic (>=1.8,<2.0)
-Requires-Dist: typing-extensions (>=4.0.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.0.0,<4.6.0)
 Requires-Dist: urllib3 (>=1.26.14,<2.0.0)
 Project-URL: Repository, https://github.com/qdrant/qdrant-client
 Description-Content-Type: text/markdown
 
 
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: qdrant-client Version: 1.1.7 Summary: Client
+Metadata-Version: 2.1 Name: qdrant-client Version: 1.2.0 Summary: Client
 library for the Qdrant vector search engine Home-page: https://github.com/
 qdrant/qdrant-client Keywords: vector,search,neural,matching,client Author:
 Andrey Vasnetsov Author-email: andrey@qdrant.tech Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: grpcio (>=1.41.0) Requires-Dist: grpcio-tools (>=1.41.0)
 Requires-Dist: httpx[http2] (>=0.14.0) Requires-Dist: numpy (<1.21) ;
 python_version < "3.8" Requires-Dist: numpy (>=1.21) ; python_version >= "3.8"
 Requires-Dist: portalocker (>=2.7.0,<3.0.0) Requires-Dist: pydantic
-(>=1.8,<2.0) Requires-Dist: typing-extensions (>=4.0.0,<5.0.0) Requires-Dist:
+(>=1.8,<2.0) Requires-Dist: typing-extensions (>=4.0.0,<4.6.0) Requires-Dist:
 urllib3 (>=1.26.14,<2.0.0) Project-URL: Repository, https://github.com/qdrant/
 qdrant-client Description-Content-Type: text/markdown
                                    [Qdrant]
           Python Client library for the Qdrant vector search engine.
   [PyPI_version] [OpenAPI_Docs] [Apache_2.0_License] [Discord] [Roadmap_2023]
 # Python Qdrant Client Client library and SDK for the [Qdrant](https://
 github.com/qdrant/qdrant) vector search engine. Library contains type
```

