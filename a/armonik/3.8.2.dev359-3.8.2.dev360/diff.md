# Comparing `tmp/armonik-3.8.2.dev359.tar.gz` & `tmp/armonik-3.8.2.dev360.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armonik-3.8.2.dev359.tar", last modified: Wed May 24 09:31:39 2023, max compression
+gzip compressed data, was "armonik-3.8.2.dev360.tar", last modified: Wed May 24 09:32:16 2023, max compression
```

## Comparing `armonik-3.8.2.dev359.tar` & `armonik-3.8.2.dev360.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:39.653351 armonik-3.8.2.dev359/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-24 09:31:39.649351 armonik-3.8.2.dev359/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:31:39.653351 armonik-3.8.2.dev359/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:39.637351 armonik-3.8.2.dev359/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:39.637351 armonik-3.8.2.dev359/src/armonik/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:39.641351 armonik-3.8.2.dev359/src/armonik/client/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/client/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/client/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:39.641351 armonik-3.8.2.dev359/src/armonik/common/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/common/enumwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:39.637351 armonik-3.8.2.dev359/src/armonik/protogen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:39.645351 armonik-3.8.2.dev359/src/armonik/protogen/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/applications_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/applications_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/applications_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/auth_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/auth_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/auth_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/events_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/events_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/events_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/partitions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/partitions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/partitions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/results_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/results_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/results_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/sessions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/sessions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/sessions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/submitter_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/submitter_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/submitter_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/tasks_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/tasks_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/tasks_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/versions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/versions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/client/versions_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:39.649351 armonik-3.8.2.dev359/src/armonik/protogen/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/agent_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/agent_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/agent_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/applications_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/applications_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/applications_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/auth_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/auth_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/auth_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/events_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/events_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/events_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/objects_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/objects_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/objects_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/partitions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/partitions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/partitions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/result_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/result_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/result_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/results_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/results_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/results_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/session_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/session_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/session_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/sessions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/sessions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/sessions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/submitter_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/submitter_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/submitter_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/task_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/task_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/task_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/tasks_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17588 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/tasks_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/tasks_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/versions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/versions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/versions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/worker_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/worker_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/common/worker_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:39.649351 armonik-3.8.2.dev359/src/armonik/protogen/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/worker/agent_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/worker/agent_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/worker/agent_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/worker/worker_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/worker/worker_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-24 09:31:33.000000 armonik-3.8.2.dev359/src/armonik/protogen/worker/worker_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:39.649351 armonik-3.8.2.dev359/src/armonik/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/worker/seqlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/worker/taskhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-24 09:31:22.000000 armonik-3.8.2.dev359/src/armonik/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:31:39.641351 armonik-3.8.2.dev359/src/armonik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-24 09:31:39.000000 armonik-3.8.2.dev359/src/armonik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-24 09:31:39.000000 armonik-3.8.2.dev359/src/armonik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:31:39.000000 armonik-3.8.2.dev359/src/armonik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 09:31:39.000000 armonik-3.8.2.dev359/src/armonik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 09:31:39.000000 armonik-3.8.2.dev359/src/armonik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:16.347414 armonik-3.8.2.dev360/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-24 09:32:16.347414 armonik-3.8.2.dev360/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:32:16.347414 armonik-3.8.2.dev360/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:16.335415 armonik-3.8.2.dev360/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:16.335415 armonik-3.8.2.dev360/src/armonik/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:16.335415 armonik-3.8.2.dev360/src/armonik/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/client/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/client/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:16.335415 armonik-3.8.2.dev360/src/armonik/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/common/enumwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:16.335415 armonik-3.8.2.dev360/src/armonik/protogen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:16.339414 armonik-3.8.2.dev360/src/armonik/protogen/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/applications_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/applications_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/applications_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/auth_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/auth_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/auth_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/events_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/events_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/events_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/partitions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/partitions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/partitions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/results_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/results_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/results_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/sessions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/sessions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/sessions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/submitter_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/submitter_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/submitter_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/tasks_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/tasks_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/tasks_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/versions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/versions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/client/versions_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:16.343414 armonik-3.8.2.dev360/src/armonik/protogen/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/agent_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/agent_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/agent_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/applications_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/applications_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/applications_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/auth_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/auth_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/auth_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/events_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/events_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/events_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/objects_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/objects_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/objects_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/partitions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/partitions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/partitions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/result_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/result_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/result_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/results_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/results_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/results_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/session_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/session_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/session_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/sessions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/sessions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/sessions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/submitter_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/submitter_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/submitter_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/task_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/task_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/task_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/tasks_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17588 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/tasks_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/tasks_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/versions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/versions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/versions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/worker_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/worker_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/common/worker_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:16.343414 armonik-3.8.2.dev360/src/armonik/protogen/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/worker/agent_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/worker/agent_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/worker/agent_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/worker/worker_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/worker/worker_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-24 09:32:10.000000 armonik-3.8.2.dev360/src/armonik/protogen/worker/worker_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:16.347414 armonik-3.8.2.dev360/src/armonik/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/worker/seqlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/worker/taskhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-24 09:31:59.000000 armonik-3.8.2.dev360/src/armonik/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:32:16.335415 armonik-3.8.2.dev360/src/armonik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-24 09:32:16.000000 armonik-3.8.2.dev360/src/armonik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-24 09:32:16.000000 armonik-3.8.2.dev360/src/armonik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:32:16.000000 armonik-3.8.2.dev360/src/armonik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 09:32:16.000000 armonik-3.8.2.dev360/src/armonik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 09:32:16.000000 armonik-3.8.2.dev360/src/armonik.egg-info/top_level.txt
```

### Comparing `armonik-3.8.2.dev359/PKG-INFO` & `armonik-3.8.2.dev360/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev359
+Version: 3.8.2.dev360
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev359/README.md` & `armonik-3.8.2.dev360/README.md`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/pyproject.toml` & `armonik-3.8.2.dev360/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/client/submitter.py` & `armonik-3.8.2.dev360/src/armonik/client/submitter.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/client/tasks.py` & `armonik-3.8.2.dev360/src/armonik/client/tasks.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/common/enumwrapper.py` & `armonik-3.8.2.dev360/src/armonik/common/enumwrapper.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/common/helpers.py` & `armonik-3.8.2.dev360/src/armonik/common/helpers.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/common/objects.py` & `armonik-3.8.2.dev360/src/armonik/common/objects.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/applications_service_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/applications_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/applications_service_pb2_grpc.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/applications_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/auth_service_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/auth_service_pb2_grpc.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/events_service_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/events_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/events_service_pb2_grpc.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/events_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/partitions_service_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/partitions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/partitions_service_pb2_grpc.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/partitions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/results_service_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/results_service_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 _sym_db = _symbol_database.Default()
 
 
 from ..common import objects_pb2 as objects__pb2
 from ..common import results_common_pb2 as results__common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15results_service.proto\x12\x1b\x61rmonik.api.grpc.v1.results\x1a\robjects.proto\x1a\x14results_common.proto2\x97\x08\n\x07Results\x12r\n\x0bListResults\x12/.armonik.api.grpc.v1.results.ListResultsRequest\x1a\x30.armonik.api.grpc.v1.results.ListResultsResponse\"\x00\x12y\n\x0eGetOwnerTaskId\x12\x32.armonik.api.grpc.v1.results.GetOwnerTaskIdRequest\x1a\x33.armonik.api.grpc.v1.results.GetOwnerTaskIdResponse\x12\x90\x01\n\x15\x43reateResultsMetaData\x12\x39.armonik.api.grpc.v1.results.CreateResultsMetaDataRequest\x1a:.armonik.api.grpc.v1.results.CreateResultsMetaDataResponse\"\x00\x12x\n\rCreateResults\x12\x31.armonik.api.grpc.v1.results.CreateResultsRequest\x1a\x32.armonik.api.grpc.v1.results.CreateResultsResponse\"\x00\x12\x83\x01\n\x10UploadResultData\x12\x34.armonik.api.grpc.v1.results.UploadResultDataRequest\x1a\x35.armonik.api.grpc.v1.results.UploadResultDataResponse\"\x00(\x01\x12\x89\x01\n\x12\x44ownloadResultData\x12\x36.armonik.api.grpc.v1.results.DownloadResultDataRequest\x1a\x37.armonik.api.grpc.v1.results.DownloadResultDataResponse\"\x00\x30\x01\x12\x84\x01\n\x11\x44\x65leteResultsData\x12\x35.armonik.api.grpc.v1.results.DeleteResultsDataRequest\x1a\x36.armonik.api.grpc.v1.results.DeleteResultsDataResponse\"\x00\x12w\n\x17GetServiceConfiguration\x12\x1a.armonik.api.grpc.v1.Empty\x1a@.armonik.api.grpc.v1.results.ResultsServiceConfigurationResponseB\x1e\xaa\x02\x1b\x41rmoniK.Api.gRPC.V1.Resultsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15results_service.proto\x12\x1b\x61rmonik.api.grpc.v1.results\x1a\robjects.proto\x1a\x14results_common.proto2\x85\t\n\x07Results\x12r\n\x0bListResults\x12/.armonik.api.grpc.v1.results.ListResultsRequest\x1a\x30.armonik.api.grpc.v1.results.ListResultsResponse\"\x00\x12l\n\tGetResult\x12-.armonik.api.grpc.v1.results.GetResultRequest\x1a..armonik.api.grpc.v1.results.GetResultResponse\"\x00\x12y\n\x0eGetOwnerTaskId\x12\x32.armonik.api.grpc.v1.results.GetOwnerTaskIdRequest\x1a\x33.armonik.api.grpc.v1.results.GetOwnerTaskIdResponse\x12\x90\x01\n\x15\x43reateResultsMetaData\x12\x39.armonik.api.grpc.v1.results.CreateResultsMetaDataRequest\x1a:.armonik.api.grpc.v1.results.CreateResultsMetaDataResponse\"\x00\x12x\n\rCreateResults\x12\x31.armonik.api.grpc.v1.results.CreateResultsRequest\x1a\x32.armonik.api.grpc.v1.results.CreateResultsResponse\"\x00\x12\x83\x01\n\x10UploadResultData\x12\x34.armonik.api.grpc.v1.results.UploadResultDataRequest\x1a\x35.armonik.api.grpc.v1.results.UploadResultDataResponse\"\x00(\x01\x12\x89\x01\n\x12\x44ownloadResultData\x12\x36.armonik.api.grpc.v1.results.DownloadResultDataRequest\x1a\x37.armonik.api.grpc.v1.results.DownloadResultDataResponse\"\x00\x30\x01\x12\x84\x01\n\x11\x44\x65leteResultsData\x12\x35.armonik.api.grpc.v1.results.DeleteResultsDataRequest\x1a\x36.armonik.api.grpc.v1.results.DeleteResultsDataResponse\"\x00\x12w\n\x17GetServiceConfiguration\x12\x1a.armonik.api.grpc.v1.Empty\x1a@.armonik.api.grpc.v1.results.ResultsServiceConfigurationResponseB\x1e\xaa\x02\x1b\x41rmoniK.Api.gRPC.V1.Resultsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'results_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\033ArmoniK.Api.gRPC.V1.Results'
   _RESULTS._serialized_start=92
-  _RESULTS._serialized_end=1139
+  _RESULTS._serialized_end=1249
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/results_service_pb2_grpc.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/results_service_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,19 @@
             channel: A grpc.Channel.
         """
         self.ListResults = channel.unary_unary(
                 '/armonik.api.grpc.v1.results.Results/ListResults',
                 request_serializer=results__common__pb2.ListResultsRequest.SerializeToString,
                 response_deserializer=results__common__pb2.ListResultsResponse.FromString,
                 )
+        self.GetResult = channel.unary_unary(
+                '/armonik.api.grpc.v1.results.Results/GetResult',
+                request_serializer=results__common__pb2.GetResultRequest.SerializeToString,
+                response_deserializer=results__common__pb2.GetResultResponse.FromString,
+                )
         self.GetOwnerTaskId = channel.unary_unary(
                 '/armonik.api.grpc.v1.results.Results/GetOwnerTaskId',
                 request_serializer=results__common__pb2.GetOwnerTaskIdRequest.SerializeToString,
                 response_deserializer=results__common__pb2.GetOwnerTaskIdResponse.FromString,
                 )
         self.CreateResultsMetaData = channel.unary_unary(
                 '/armonik.api.grpc.v1.results.Results/CreateResultsMetaData',
@@ -68,14 +73,22 @@
         """*
         Get a results list using pagination, filters and sorting
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetResult(self, request, context):
+        """*
+        Get a result by id.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetOwnerTaskId(self, request, context):
         """*
         Get the id of the task that should produce the result
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
@@ -133,14 +146,19 @@
 def add_ResultsServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ListResults': grpc.unary_unary_rpc_method_handler(
                     servicer.ListResults,
                     request_deserializer=results__common__pb2.ListResultsRequest.FromString,
                     response_serializer=results__common__pb2.ListResultsResponse.SerializeToString,
             ),
+            'GetResult': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetResult,
+                    request_deserializer=results__common__pb2.GetResultRequest.FromString,
+                    response_serializer=results__common__pb2.GetResultResponse.SerializeToString,
+            ),
             'GetOwnerTaskId': grpc.unary_unary_rpc_method_handler(
                     servicer.GetOwnerTaskId,
                     request_deserializer=results__common__pb2.GetOwnerTaskIdRequest.FromString,
                     response_serializer=results__common__pb2.GetOwnerTaskIdResponse.SerializeToString,
             ),
             'CreateResultsMetaData': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateResultsMetaData,
@@ -198,14 +216,31 @@
         return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.results.Results/ListResults',
             results__common__pb2.ListResultsRequest.SerializeToString,
             results__common__pb2.ListResultsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetResult(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.results.Results/GetResult',
+            results__common__pb2.GetResultRequest.SerializeToString,
+            results__common__pb2.GetResultResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetOwnerTaskId(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/sessions_service_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/sessions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/sessions_service_pb2_grpc.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/sessions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/submitter_service_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/submitter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/submitter_service_pb2_grpc.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/submitter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/tasks_service_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/tasks_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/tasks_service_pb2_grpc.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/tasks_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/versions_service_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/versions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/client/versions_service_pb2_grpc.py` & `armonik-3.8.2.dev360/src/armonik/protogen/client/versions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/agent_common_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/agent_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/agent_common_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/agent_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/applications_common_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/applications_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/applications_common_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/applications_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/auth_common_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/auth_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/auth_common_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/auth_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/events_common_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/events_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/events_common_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/events_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/objects_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/objects_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/objects_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/objects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/partitions_common_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/partitions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/partitions_common_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/partitions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/result_status_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/result_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/results_common_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/results_common_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import result_status_pb2 as result__status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14results_common.proto\x12\x1b\x61rmonik.api.grpc.v1.results\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13result_status.proto\"\xb0\x02\n\tResultRaw\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rowner_task_id\x18\x03 \x01(\t\x12?\n\x06status\x18\x04 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10wait_for_data_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tresult_id\x18\x08 \x01(\t\"\x90\t\n\x12ListResultsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x46\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x36.armonik.api.grpc.v1.results.ListResultsRequest.Filter\x12\x42\n\x04sort\x18\x04 \x01(\x0b\x32\x34.armonik.api.grpc.v1.results.ListResultsRequest.Sort\x1a\xda\x03\n\x06\x46ilter\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rowner_task_id\x18\x03 \x01(\t\x12?\n\x06status\x18\x04 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12\x31\n\rcreated_after\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63ompleted_after\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x63ompleted_before\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x13wait_for_data_after\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14wait_for_data_before\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tresult_id\x18\x0b \x01(\t\x1a\xa6\x01\n\x04Sort\x12K\n\x05\x66ield\x18\x01 \x01(\x0e\x32<.armonik.api.grpc.v1.results.ListResultsRequest.OrderByField\x12Q\n\tdirection\x18\x02 \x01(\x0e\x32>.armonik.api.grpc.v1.results.ListResultsRequest.OrderDirection\"\xe0\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x01\x12\x17\n\x13ORDER_BY_FIELD_NAME\x10\x02\x12 \n\x1cORDER_BY_FIELD_OWNER_TASK_ID\x10\x03\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x04\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x05\x12\x1c\n\x18ORDER_BY_FIELD_RESULT_ID\x10\x06\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"~\n\x13ListResultsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\">\n\x15GetOwnerTaskIdRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\t\"\xb9\x01\n\x16GetOwnerTaskIdResponse\x12V\n\x0bresult_task\x18\x01 \x03(\x0b\x32\x41.armonik.api.grpc.v1.results.GetOwnerTaskIdResponse.MapResultTask\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a\x33\n\rMapResultTask\x12\x11\n\tresult_id\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"\xa9\x01\n\x1c\x43reateResultsMetaDataRequest\x12W\n\x07results\x18\x01 \x03(\x0b\x32\x46.armonik.api.grpc.v1.results.CreateResultsMetaDataRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a\x1c\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\"X\n\x1d\x43reateResultsMetaDataResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"\xa7\x01\n\x14\x43reateResultsRequest\x12O\n\x07results\x18\x01 \x03(\x0b\x32>.armonik.api.grpc.v1.results.CreateResultsRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a*\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"P\n\x15\x43reateResultsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"\xc7\x01\n\x17UploadResultDataRequest\x12S\n\x02id\x18\x01 \x01(\x0b\x32\x45.armonik.api.grpc.v1.results.UploadResultDataRequest.ResultIdentifierH\x00\x12\x14\n\ndata_chunk\x18\x02 \x01(\x0cH\x00\x1a\x39\n\x10ResultIdentifier\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\tB\x06\n\x04type\"R\n\x18UploadResultDataResponse\x12\x36\n\x06result\x18\x01 \x01(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"B\n#ResultsServiceConfigurationResponse\x12\x1b\n\x13\x64\x61ta_chunk_max_size\x18\x01 \x01(\x05\"B\n\x19\x44ownloadResultDataRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\t\"0\n\x1a\x44ownloadResultDataResponse\x12\x12\n\ndata_chunk\x18\x01 \x01(\x0c\"A\n\x18\x44\x65leteResultsDataRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\t\"B\n\x19\x44\x65leteResultsDataResponse\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\tB\x1e\xaa\x02\x1b\x41rmoniK.Api.gRPC.V1.Resultsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14results_common.proto\x12\x1b\x61rmonik.api.grpc.v1.results\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13result_status.proto\"\xb0\x02\n\tResultRaw\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rowner_task_id\x18\x03 \x01(\t\x12?\n\x06status\x18\x04 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10wait_for_data_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tresult_id\x18\x08 \x01(\t\"\x90\t\n\x12ListResultsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x46\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x36.armonik.api.grpc.v1.results.ListResultsRequest.Filter\x12\x42\n\x04sort\x18\x04 \x01(\x0b\x32\x34.armonik.api.grpc.v1.results.ListResultsRequest.Sort\x1a\xda\x03\n\x06\x46ilter\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rowner_task_id\x18\x03 \x01(\t\x12?\n\x06status\x18\x04 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12\x31\n\rcreated_after\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63ompleted_after\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x63ompleted_before\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x13wait_for_data_after\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14wait_for_data_before\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tresult_id\x18\x0b \x01(\t\x1a\xa6\x01\n\x04Sort\x12K\n\x05\x66ield\x18\x01 \x01(\x0e\x32<.armonik.api.grpc.v1.results.ListResultsRequest.OrderByField\x12Q\n\tdirection\x18\x02 \x01(\x0e\x32>.armonik.api.grpc.v1.results.ListResultsRequest.OrderDirection\"\xe0\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x01\x12\x17\n\x13ORDER_BY_FIELD_NAME\x10\x02\x12 \n\x1cORDER_BY_FIELD_OWNER_TASK_ID\x10\x03\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x04\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x05\x12\x1c\n\x18ORDER_BY_FIELD_RESULT_ID\x10\x06\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"~\n\x13ListResultsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"%\n\x10GetResultRequest\x12\x11\n\tresult_id\x18\x01 \x01(\t\"K\n\x11GetResultResponse\x12\x36\n\x06result\x18\x01 \x01(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\">\n\x15GetOwnerTaskIdRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\t\"\xb9\x01\n\x16GetOwnerTaskIdResponse\x12V\n\x0bresult_task\x18\x01 \x03(\x0b\x32\x41.armonik.api.grpc.v1.results.GetOwnerTaskIdResponse.MapResultTask\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a\x33\n\rMapResultTask\x12\x11\n\tresult_id\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"\xa9\x01\n\x1c\x43reateResultsMetaDataRequest\x12W\n\x07results\x18\x01 \x03(\x0b\x32\x46.armonik.api.grpc.v1.results.CreateResultsMetaDataRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a\x1c\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\"X\n\x1d\x43reateResultsMetaDataResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"\xa7\x01\n\x14\x43reateResultsRequest\x12O\n\x07results\x18\x01 \x03(\x0b\x32>.armonik.api.grpc.v1.results.CreateResultsRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a*\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"P\n\x15\x43reateResultsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"\xc7\x01\n\x17UploadResultDataRequest\x12S\n\x02id\x18\x01 \x01(\x0b\x32\x45.armonik.api.grpc.v1.results.UploadResultDataRequest.ResultIdentifierH\x00\x12\x14\n\ndata_chunk\x18\x02 \x01(\x0cH\x00\x1a\x39\n\x10ResultIdentifier\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\tB\x06\n\x04type\"R\n\x18UploadResultDataResponse\x12\x36\n\x06result\x18\x01 \x01(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"B\n#ResultsServiceConfigurationResponse\x12\x1b\n\x13\x64\x61ta_chunk_max_size\x18\x01 \x01(\x05\"B\n\x19\x44ownloadResultDataRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\t\"0\n\x1a\x44ownloadResultDataResponse\x12\x12\n\ndata_chunk\x18\x01 \x01(\x0c\"A\n\x18\x44\x65leteResultsDataRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\t\"B\n\x19\x44\x65leteResultsDataResponse\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\tB\x1e\xaa\x02\x1b\x41rmoniK.Api.gRPC.V1.Resultsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'results_common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\033ArmoniK.Api.gRPC.V1.Results'
@@ -33,42 +33,46 @@
   _LISTRESULTSREQUEST_SORT._serialized_end=1254
   _LISTRESULTSREQUEST_ORDERBYFIELD._serialized_start=1257
   _LISTRESULTSREQUEST_ORDERBYFIELD._serialized_end=1481
   _LISTRESULTSREQUEST_ORDERDIRECTION._serialized_start=1483
   _LISTRESULTSREQUEST_ORDERDIRECTION._serialized_end=1583
   _LISTRESULTSRESPONSE._serialized_start=1585
   _LISTRESULTSRESPONSE._serialized_end=1711
-  _GETOWNERTASKIDREQUEST._serialized_start=1713
-  _GETOWNERTASKIDREQUEST._serialized_end=1775
-  _GETOWNERTASKIDRESPONSE._serialized_start=1778
-  _GETOWNERTASKIDRESPONSE._serialized_end=1963
-  _GETOWNERTASKIDRESPONSE_MAPRESULTTASK._serialized_start=1912
-  _GETOWNERTASKIDRESPONSE_MAPRESULTTASK._serialized_end=1963
-  _CREATERESULTSMETADATAREQUEST._serialized_start=1966
-  _CREATERESULTSMETADATAREQUEST._serialized_end=2135
-  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_start=2107
-  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_end=2135
-  _CREATERESULTSMETADATARESPONSE._serialized_start=2137
-  _CREATERESULTSMETADATARESPONSE._serialized_end=2225
-  _CREATERESULTSREQUEST._serialized_start=2228
-  _CREATERESULTSREQUEST._serialized_end=2395
-  _CREATERESULTSREQUEST_RESULTCREATE._serialized_start=2353
-  _CREATERESULTSREQUEST_RESULTCREATE._serialized_end=2395
-  _CREATERESULTSRESPONSE._serialized_start=2397
-  _CREATERESULTSRESPONSE._serialized_end=2477
-  _UPLOADRESULTDATAREQUEST._serialized_start=2480
-  _UPLOADRESULTDATAREQUEST._serialized_end=2679
-  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_start=2614
-  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_end=2671
-  _UPLOADRESULTDATARESPONSE._serialized_start=2681
-  _UPLOADRESULTDATARESPONSE._serialized_end=2763
-  _RESULTSSERVICECONFIGURATIONRESPONSE._serialized_start=2765
-  _RESULTSSERVICECONFIGURATIONRESPONSE._serialized_end=2831
-  _DOWNLOADRESULTDATAREQUEST._serialized_start=2833
-  _DOWNLOADRESULTDATAREQUEST._serialized_end=2899
-  _DOWNLOADRESULTDATARESPONSE._serialized_start=2901
-  _DOWNLOADRESULTDATARESPONSE._serialized_end=2949
-  _DELETERESULTSDATAREQUEST._serialized_start=2951
-  _DELETERESULTSDATAREQUEST._serialized_end=3016
-  _DELETERESULTSDATARESPONSE._serialized_start=3018
-  _DELETERESULTSDATARESPONSE._serialized_end=3084
+  _GETRESULTREQUEST._serialized_start=1713
+  _GETRESULTREQUEST._serialized_end=1750
+  _GETRESULTRESPONSE._serialized_start=1752
+  _GETRESULTRESPONSE._serialized_end=1827
+  _GETOWNERTASKIDREQUEST._serialized_start=1829
+  _GETOWNERTASKIDREQUEST._serialized_end=1891
+  _GETOWNERTASKIDRESPONSE._serialized_start=1894
+  _GETOWNERTASKIDRESPONSE._serialized_end=2079
+  _GETOWNERTASKIDRESPONSE_MAPRESULTTASK._serialized_start=2028
+  _GETOWNERTASKIDRESPONSE_MAPRESULTTASK._serialized_end=2079
+  _CREATERESULTSMETADATAREQUEST._serialized_start=2082
+  _CREATERESULTSMETADATAREQUEST._serialized_end=2251
+  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_start=2223
+  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_end=2251
+  _CREATERESULTSMETADATARESPONSE._serialized_start=2253
+  _CREATERESULTSMETADATARESPONSE._serialized_end=2341
+  _CREATERESULTSREQUEST._serialized_start=2344
+  _CREATERESULTSREQUEST._serialized_end=2511
+  _CREATERESULTSREQUEST_RESULTCREATE._serialized_start=2469
+  _CREATERESULTSREQUEST_RESULTCREATE._serialized_end=2511
+  _CREATERESULTSRESPONSE._serialized_start=2513
+  _CREATERESULTSRESPONSE._serialized_end=2593
+  _UPLOADRESULTDATAREQUEST._serialized_start=2596
+  _UPLOADRESULTDATAREQUEST._serialized_end=2795
+  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_start=2730
+  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_end=2787
+  _UPLOADRESULTDATARESPONSE._serialized_start=2797
+  _UPLOADRESULTDATARESPONSE._serialized_end=2879
+  _RESULTSSERVICECONFIGURATIONRESPONSE._serialized_start=2881
+  _RESULTSSERVICECONFIGURATIONRESPONSE._serialized_end=2947
+  _DOWNLOADRESULTDATAREQUEST._serialized_start=2949
+  _DOWNLOADRESULTDATAREQUEST._serialized_end=3015
+  _DOWNLOADRESULTDATARESPONSE._serialized_start=3017
+  _DOWNLOADRESULTDATARESPONSE._serialized_end=3065
+  _DELETERESULTSDATAREQUEST._serialized_start=3067
+  _DELETERESULTSDATAREQUEST._serialized_end=3132
+  _DELETERESULTSDATARESPONSE._serialized_start=3134
+  _DELETERESULTSDATARESPONSE._serialized_end=3200
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/results_common_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/results_common_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,26 @@
         def __init__(self, result_id: _Optional[str] = ..., task_id: _Optional[str] = ...) -> None: ...
     RESULT_TASK_FIELD_NUMBER: _ClassVar[int]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     result_task: _containers.RepeatedCompositeFieldContainer[GetOwnerTaskIdResponse.MapResultTask]
     session_id: str
     def __init__(self, result_task: _Optional[_Iterable[_Union[GetOwnerTaskIdResponse.MapResultTask, _Mapping]]] = ..., session_id: _Optional[str] = ...) -> None: ...
 
+class GetResultRequest(_message.Message):
+    __slots__ = ["result_id"]
+    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+    result_id: str
+    def __init__(self, result_id: _Optional[str] = ...) -> None: ...
+
+class GetResultResponse(_message.Message):
+    __slots__ = ["result"]
+    RESULT_FIELD_NUMBER: _ClassVar[int]
+    result: ResultRaw
+    def __init__(self, result: _Optional[_Union[ResultRaw, _Mapping]] = ...) -> None: ...
+
 class ListResultsRequest(_message.Message):
     __slots__ = ["filter", "page", "page_size", "sort"]
     class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     class Filter(_message.Message):
```

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/session_status_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/session_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/sessions_common_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/sessions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/sessions_common_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/sessions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/submitter_common_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/submitter_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/submitter_common_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/submitter_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/task_status_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/task_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/task_status_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/task_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/tasks_common_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/tasks_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/tasks_common_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/tasks_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/versions_common_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/versions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/versions_common_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/versions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/worker_common_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/common/worker_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/common/worker_common_pb2.pyi` & `armonik-3.8.2.dev360/src/armonik/protogen/common/worker_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/worker/agent_service_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/worker/agent_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/worker/agent_service_pb2_grpc.py` & `armonik-3.8.2.dev360/src/armonik/protogen/worker/agent_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/worker/worker_service_pb2.py` & `armonik-3.8.2.dev360/src/armonik/protogen/worker/worker_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/protogen/worker/worker_service_pb2_grpc.py` & `armonik-3.8.2.dev360/src/armonik/protogen/worker/worker_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/worker/seqlogger.py` & `armonik-3.8.2.dev360/src/armonik/worker/seqlogger.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/worker/taskhandler.py` & `armonik-3.8.2.dev360/src/armonik/worker/taskhandler.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik/worker/worker.py` & `armonik-3.8.2.dev360/src/armonik/worker/worker.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev359/src/armonik.egg-info/PKG-INFO` & `armonik-3.8.2.dev360/src/armonik.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev359
+Version: 3.8.2.dev360
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev359/src/armonik.egg-info/SOURCES.txt` & `armonik-3.8.2.dev360/src/armonik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

