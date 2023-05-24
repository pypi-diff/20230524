# Comparing `tmp/aetcd-1.0.0a2.tar.gz` & `tmp/aetcd-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aetcd-1.0.0a2.tar", last modified: Fri Jan 14 08:30:34 2022, max compression
+gzip compressed data, was "aetcd-1.0.0a4.tar", last modified: Wed May 24 13:07:34 2023, max compression
```

## Comparing `aetcd-1.0.0a2.tar` & `aetcd-1.0.0a4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 08:30:34.836223 aetcd-1.0.0a2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 08:30:34.828223 aetcd-1.0.0a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 08:30:34.832223 aetcd-1.0.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    10141 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-01-14 08:30:34.836223 aetcd-1.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 08:30:34.832223 aetcd-1.0.0a2/aetcd/
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    44865 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2193 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/leases.py
--rw-r--r--   0 runner    (1001) docker     (121)     4206 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/locks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/members.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 08:30:34.832223 aetcd-1.0.0a2/aetcd/rpc/
--rw-r--r--   0 runner    (1001) docker     (121)     6600 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9453 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/rpc/auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/rpc/auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7251 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/rpc/kv_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/rpc/kv_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)   221377 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/rpc/rpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    68034 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/rpc/rpc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9157 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/rtypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/transactions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13047 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/aetcd/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 08:30:34.832223 aetcd-1.0.0a2/aetcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-01-14 08:30:34.000000 aetcd-1.0.0a2/aetcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-01-14 08:30:34.000000 aetcd-1.0.0a2/aetcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-14 08:30:34.000000 aetcd-1.0.0a2/aetcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-14 08:30:33.000000 aetcd-1.0.0a2/aetcd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-01-14 08:30:34.000000 aetcd-1.0.0a2/aetcd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-14 08:30:34.000000 aetcd-1.0.0a2/aetcd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 08:30:34.832223 aetcd-1.0.0a2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/docs/guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/docs/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 08:30:34.832223 aetcd-1.0.0a2/proto/
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/proto/auth.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/proto/kv.proto
--rw-r--r--   0 runner    (1001) docker     (121)    32648 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/proto/rpc.proto
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-01-14 08:30:34.836223 aetcd-1.0.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 08:30:34.832223 aetcd-1.0.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 08:30:34.836223 aetcd-1.0.0a2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/integration/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/integration/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    11033 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/integration/test_kv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/integration/test_lease.py
--rw-r--r--   0 runner    (1001) docker     (121)     2974 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/integration/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/integration/test_maintenance.py
--rw-r--r--   0 runner    (1001) docker     (121)     6374 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/integration/test_watch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4115 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8643 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/test_rtypes.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-01-14 08:30:06.000000 aetcd-1.0.0a2/tests/test_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:07:34.415434 aetcd-1.0.0a4/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:07:34.407433 aetcd-1.0.0a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:07:34.407433 aetcd-1.0.0a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    10141 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2261 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2947 2023-05-24 13:07:34.415434 aetcd-1.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:07:34.411433 aetcd-1.0.0a4/aetcd/
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45985 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/leases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/locks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/members.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:07:34.411433 aetcd-1.0.0a4/aetcd/rpc/
+-rw-r--r--   0 runner    (1001) docker     (122)     6600 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1786 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/rpc/auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/rpc/auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/rpc/kv_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/rpc/kv_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29643 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/rpc/rpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    68034 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/rpc/rpc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9101 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/rtypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/aetcd/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:07:34.411433 aetcd-1.0.0a4/aetcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2947 2023-05-24 13:07:34.000000 aetcd-1.0.0a4/aetcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-05-24 13:07:34.000000 aetcd-1.0.0a4/aetcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 13:07:34.000000 aetcd-1.0.0a4/aetcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 13:07:19.000000 aetcd-1.0.0a4/aetcd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-05-24 13:07:34.000000 aetcd-1.0.0a4/aetcd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-24 13:07:34.000000 aetcd-1.0.0a4/aetcd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:07:34.415434 aetcd-1.0.0a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      953 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     3995 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3482 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/docs/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/docs/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:07:34.415434 aetcd-1.0.0a4/proto/
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/proto/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/proto/kv.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    32648 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/proto/rpc.proto
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-24 13:07:34.415434 aetcd-1.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:07:34.415434 aetcd-1.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 13:07:34.415434 aetcd-1.0.0a4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/integration/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/integration/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11970 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/integration/test_kv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/integration/test_lease.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/integration/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2104 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/integration/test_maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6584 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/integration/test_watch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4115 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8643 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/test_rtypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-05-24 13:06:53.000000 aetcd-1.0.0a4/tests/test_watcher.py
```

### Comparing `aetcd-1.0.0a2/.github/workflows/ci.yml` & `aetcd-1.0.0a4/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,26 @@
     branches: ['master']
     tags: ['v*']
 
   pull_request:
     branches: ['master']
 
   schedule:
-    # Daily at 4 AM UTC
-    - cron: '0 4 * * *'
+    # Every hour
+    - cron: '0 * * * *'
 
 jobs:
   lint:
     name: Run lint
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: ['ubuntu-20.04']
-        python: ['3.8', '3.9', '3.10']
+        python: ['3.8', '3.9', '3.10', '3.11']
     steps:
     - name: Checkout source repository for Python ${{ matrix.python }}
       uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python }}
       uses: actions/setup-python@v2
       with:
@@ -35,17 +35,17 @@
 
   test:
     name: Run tests
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        etcd: ['3.3.27']
+        etcd: ['3.3.27', '3.4.23', '3.5.7']
         os: ['ubuntu-20.04']
-        python: ['3.8', '3.9', '3.10']
+        python: ['3.8', '3.9', '3.10', '3.11']
     steps:
       - name: Checkout source repository for Python ${{ matrix.python }}
         uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python }}
         uses: actions/setup-python@v2
         with:
@@ -58,14 +58,15 @@
           sudo cp etcd-v${{ matrix.etcd }}-linux-amd64/etcd* /usr/bin
           popd
 
       - name: Set up dependencies for Python ${{ matrix.python_version }}
         run: make bootstrap
 
       - name: Run tests on Python ${{ matrix.python }}
+        timeout-minutes: 10
         run: make testcluster
 
       - name: Run genproto
         run: |
           make genproto
 
       - name: Upload coverage report
```

### Comparing `aetcd-1.0.0a2/LICENSE` & `aetcd-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/Makefile` & `aetcd-1.0.0a4/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .DEFAULT: help
 .PHONY: bootstrap build clean help genproto lint outdated test testcluster testreport upload
 
-VENV = .venv
-PYTHON_BIN ?= python3
-PYTHON = $(VENV)/bin/$(PYTHON_BIN)
+VENV=.venv
+PYTHON_BIN?=python3
+PYTHON=$(VENV)/bin/$(PYTHON_BIN)
 
 help:
 	@echo "Please use \`$(MAKE) <target>' where <target> is one of the following:"
 	@echo "  help        - show help information"
 	@echo "  bootstrap  - setup packaging dependencies and initialize venv"
 	@echo "  build       - build project packages"
 	@echo "  genproto    - process .proto files and generate gRPC stubs"
@@ -18,16 +18,17 @@
 	@echo "  testreport  - run project tests and open HTML coverage report"
 	@echo "  upload      - upload built packages to package repository"
 	@echo "  clean       - clean up project environment and all the build artifacts"
 
 bootstrap: $(VENV)/bin/activate
 $(VENV)/bin/activate:
 	$(PYTHON_BIN) -m venv $(VENV)
-	$(PYTHON) -m pip install pip==21.3.1 setuptools==60.1.0 wheel==0.37.1
+	$(PYTHON) -m pip install pip==23.0 setuptools==67.3.2 wheel==0.38.4
 	$(PYTHON) -m pip install -e .[dev,doc,test]
+	$(PYTHON) -m pip install 'pifpaf @ git+https://github.com/jd/pifpaf.git@80cc13bd7e4b0cb286d15659c9fe7958e8600cd9#egg=aetcd'
 
 build: bootstrap
 	$(PYTHON) setup.py sdist bdist_wheel
 
 genproto: bootstrap
 	$(PYTHON) -m grpc_tools.protoc -Iproto \
 		--python_out=aetcd/rpc/ \
@@ -40,15 +41,15 @@
 lint: bootstrap
 	$(PYTHON) -m flake8 aetcd tests
 
 test: bootstrap
 	$(PYTHON) -m pytest
 
 testcluster: bootstrap
-	$(PYTHON) -m pifpaf -e TEST run etcd --cluster -- $(PYTHON) -m pytest --cov-report=xml
+	$(PYTHON) -m pifpaf -e TEST --debug run etcd --cluster -- $(PYTHON) -m pytest --with-cluster --cov-report=xml
 
 testreport: bootstrap
 	$(PYTHON) -m pytest --cov-report=html
 	xdg-open htmlcov/index.html
 
 upload: build
 	$(PYTHON) -m twine upload dist/*
```

### Comparing `aetcd-1.0.0a2/PKG-INFO` & `aetcd-1.0.0a4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: aetcd
-Version: 1.0.0a2
+Version: 1.0.0a4
 Summary: Python asyncio-based client for etcd
 Home-page: https://github.com/martyanov/aetcd
 Author: Andrey Martyanov
 Author-email: andrey@martyanov.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://aetcd.readthedocs.io
 Project-URL: Code, https://github.com/martyanov/aetcd
 Project-URL: Issues, https://github.com/martyanov/aetcd/issues
 Keywords: etcd3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
@@ -89,9 +89,7 @@
 
 .. _etcd3aio: https://github.com/hron/etcd3aio
 .. _python-etcd3: https://github.com/kragniz/python-etcd3
 .. _kragniz: https://github.com/kragniz
 .. _hron: https://github.com/hron
 .. _gjcarneiro: https://github.com/gjcarneiro
 .. _people: https://github.com/martyanov/aetcd/graphs/contributors
-
-
```

### Comparing `aetcd-1.0.0a2/README.rst` & `aetcd-1.0.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/aetcd/__init__.py` & `aetcd-1.0.0a4/aetcd/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .client import Alarm  # noqa: F401
 from .client import Client  # noqa: F401
 from .client import Status  # noqa: F401
 from .client import Transactions  # noqa: F401
 from .exceptions import ClientError  # noqa: F401
 from .exceptions import ConnectionFailedError  # noqa: F401
 from .exceptions import ConnectionTimeoutError  # noqa: F401
+from .exceptions import DuplicateLeaseError  # noqa: F401
 from .exceptions import InternalError  # noqa: F401
 from .exceptions import InvalidArgumentError  # noqa: F401
 from .exceptions import PreconditionFailedError  # noqa: F401
 from .exceptions import RevisionCompactedError  # noqa: F401
 from .exceptions import WatchTimeoutError  # noqa: F401
 from .leases import Lease  # noqa: F401
 from .locks import Lock  # noqa: F401
```

### Comparing `aetcd-1.0.0a2/aetcd/client.py` & `aetcd-1.0.0a4/aetcd/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,21 @@
             f'provided function {f.__name__!r} is neither a coroutine nor an async generator')
 
     return functools.wraps(f)(handler)
 
 
 def _ensure_connected(f):
     if inspect.iscoroutinefunction(f):
-        async def handler(*args, **kwargs):
-            await args[0].connect()
-            return await f(*args, **kwargs)
+        async def handler(self, *args, **kwargs):
+            await self.connect()
+            return await f(self, *args, **kwargs)
     elif inspect.isasyncgenfunction(f):
-        async def handler(*args, **kwargs):
-            await args[0].connect()
-            async for data in f(*args, **kwargs):
+        async def handler(self, *args, **kwargs):
+            await self.connect()
+            async for data in f(self, *args, **kwargs):
                 yield data
     else:
         raise RuntimeError(
             f'provided function {f.__name__!r} is neither a coroutine nor an async generator')
 
     return functools.wraps(f)(handler)
 
@@ -108,33 +108,41 @@
 
     :param int timeout:
         Connection timeout in seconds.
 
     :param dict options:
         Options provided to the underlying gRPC channel.
 
+    :param int connect_wait_timeout:
+        Connecting wait timeout, since connection could be initiated
+        from multiple coroutines.
+
     :return:
         A :class:`~aetcd.client.Client` instance.
     """
 
     def __init__(
         self,
         host: str = 'localhost',
         port: int = 2379,
         username: typing.Optional[str] = None,
         password: typing.Optional[str] = None,
         timeout: typing.Optional[int] = None,
         options: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        connect_wait_timeout: int = 3,
     ):
         self._host = host
         self._port = port
         self._username = username
         self._password = password
         self._timeout = timeout
         self._options = options or {}
+        self._connect_wait_timeout = connect_wait_timeout
+        self._connected = asyncio.Event()
+        self._is_connecting = False
 
         cred_params = (self._username, self._password)
         if any(cred_params) and None in cred_params:
             raise Exception(
                 'if using authentication credentials both username and password '
                 'must be provided')
 
@@ -150,56 +158,86 @@
         self.kvstub = None
         self.clusterstub = None
         self.leasestub = None
         self.maintenancestub = None
 
         self._watcher = None
 
+    @_handle_errors
     async def connect(self) -> None:
         """Establish a connection to an etcd."""
-        if self.channel:
+        if self._connected.is_set():
             return
 
-        target = f'{self._host}:{self._port}'
-        self.channel = rpc.insecure_channel(target, options=self._options.items())
-
-        cred_params = [c is not None for c in (self._username, self._password)]
-        if all(cred_params):
-            self.auth_stub = rpc.AuthStub(self.channel)
-            auth_request = rpc.AuthenticateRequest(
-                name=self._username,
-                password=self._password,
+        if self._is_connecting:
+            # Another task is establishing a connection, just wait
+            await asyncio.wait_for(
+                self._connected.wait(),
+                self._connect_wait_timeout,
             )
+            return
 
-            resp = await self.auth_stub.Authenticate(auth_request, timeout=self._timeout)
-            self.metadata = (('token', resp.token),)
+        try:
+            self._is_connecting = True
+            target = f'{self._host}:{self._port}'
+            self.channel = rpc.insecure_channel(target, options=self._options.items())
+
+            cred_params = [c is not None for c in (self._username, self._password)]
+            if all(cred_params):
+                self.auth_stub = rpc.AuthStub(self.channel)
+                auth_request = rpc.AuthenticateRequest(
+                    name=self._username,
+                    password=self._password,
+                )
+
+                resp = await self.auth_stub.Authenticate(auth_request, timeout=self._timeout)
+                self.metadata = (('token', resp.token),)
+
+            self.kvstub = rpc.KVStub(self.channel)
+            self.clusterstub = rpc.ClusterStub(self.channel)
+            self.leasestub = rpc.LeaseStub(self.channel)
+            self.maintenancestub = rpc.MaintenanceStub(self.channel)
+
+            # Initialize a watcher
+            self._watcher = watcher.Watcher(
+                rpc.WatchStub(self.channel),
+                timeout=self._timeout,
+                metadata=self.metadata,
+            )
 
-        self.kvstub = rpc.KVStub(self.channel)
-        self.clusterstub = rpc.ClusterStub(self.channel)
-        self.leasestub = rpc.LeaseStub(self.channel)
-        self.maintenancestub = rpc.MaintenanceStub(self.channel)
-
-        # Initialize a watcher
-        self._watcher = watcher.Watcher(
-            rpc.WatchStub(self.channel),
-            timeout=self._timeout,
-        )
+            self._connected.set()
+        finally:
+            self._is_connecting = False
 
     async def close(self) -> None:
-        """Close established connection and frees allocated resources."""
+        """Close established connection and frees allocated resources.
+
+        It could be called while other operation is being executed.
+        """
+        if not self._connected.is_set() and self._is_connecting:
+            # Wait for the previous request to complete
+            await asyncio.wait_for(
+                self._connected.wait(),
+                self._connect_wait_timeout,
+            )
+
         if self.channel:
             # Shutdown the watcher
             if self._watcher is not None:
                 await self._watcher.shutdown()
 
             # Close the underlying RPC channel
-            await self.channel.close()
+            if self.channel:
+                # Check it again since it could be modified by a concurrent task
+                await self.channel.close()
 
             self._init_channel_attrs()
 
+        self._connected.clear()
+
     async def __aenter__(self):
         await self.connect()
         return self
 
     async def __aexit__(self, *args):
         await self.close()
 
@@ -529,17 +567,21 @@
 
         return rtypes.DeleteRange(
             delete_response.header,
             delete_response.deleted,
             delete_response.prev_kvs,
         )
 
-    @_handle_errors
-    @_ensure_connected
-    async def replace(self, key, initial_value, new_value):
+    async def replace(
+        self,
+        key: bytes,
+        initial_value: bytes,
+        new_value: bytes,
+        lease: typing.Optional[typing.Union[int, leases.Lease]] = None,
+    ):
         """Atomically replace the value of a key with a new value.
 
         This compares the current value of a key, then replaces it with a new
         value if it is equal to a specified value. This operation takes place
         in a transaction.
 
         :param key:
@@ -547,27 +589,31 @@
 
         :param bytes initial_value:
             Old value to replace.
 
         :param bytes new_value:
             New value of the key
 
+        :param lease:
+            Lease to associate with this key.
+        :type lease:
+            either :class:`~aetcd.leases.Lease`, or ``int`` (ID of a lease), or ``None``
+
         :return:
             A status of transaction, ``True`` if the replace was successful,
             ``False`` otherwise.
         """
         status, _ = await self.transaction(
             compare=[
                 self.transactions.value(key) == initial_value,
             ],
             success=[
-                self.transactions.put(key, new_value),
-            ],
-            failure=[
+                self.transactions.put(key, new_value, lease=lease),
             ],
+            failure=[],
         )
 
         return status
 
     @_handle_errors
     @_ensure_connected
     async def watch(
@@ -662,16 +708,14 @@
 
         return rtypes.Watch(
             iterator,
             cancel,
             watcher_callback.watch_id,
         )
 
-    @_handle_errors
-    @_ensure_connected
     async def watch_prefix(
         self,
         key_prefix: bytes,
         range_end: typing.Optional[bytes] = None,
         start_revision: typing.Optional[int] = None,
         progress_notify: bool = False,
         kind: typing.Optional[rtypes.EventKind] = None,
@@ -798,16 +842,14 @@
         try:
             return await asyncio.wait_for(event_queue.get(), timeout)
         except asyncio.TimeoutError:
             raise exceptions.WatchTimeoutError
         finally:
             await self._watcher.cancel(watcher_callback.watch_id)
 
-    @_handle_errors
-    @_ensure_connected
     async def watch_prefix_once(
         self,
         key_prefix: bytes,
         timeout: typing.Optional[int] = None,
         range_end: typing.Optional[bytes] = None,
         start_revision: typing.Optional[int] = None,
         progress_notify: bool = False,
@@ -919,16 +961,15 @@
             timeout=self._timeout,
             metadata=self.metadata,
         )
 
         responses = []
         for response in txn_response.responses:
             response_type = response.WhichOneof('response')
-            if response_type in ['response_put', 'response_delete_range',
-                                 'response_txn']:
+            if response_type in ['response_put', 'response_delete_range', 'response_txn']:
                 responses.append(response)
 
             elif response_type == 'response_range':
                 range_kvs = []
                 for kv in response.response_range.kvs:
                     range_kvs.append(
                         (
@@ -961,17 +1002,19 @@
         """
         lease_grant_request = rpc.LeaseGrantRequest(TTL=ttl, ID=lease_id)
         lease_grant_response = await self.leasestub.LeaseGrant(
             lease_grant_request,
             timeout=self._timeout,
             metadata=self.metadata,
         )
-        return leases.Lease(lease_id=lease_grant_response.ID,
-                            ttl=lease_grant_response.TTL,
-                            etcd_client=self)
+        return leases.Lease(
+            lease_id=lease_grant_response.ID,
+            ttl=lease_grant_response.TTL,
+            etcd_client=self,
+        )
 
     @_handle_errors
     @_ensure_connected
     async def revoke_lease(self, lease_id):
         """Revoke a lease.
 
         :param lease_id:
@@ -1037,19 +1080,21 @@
             if m.id == status_response.leader:
                 leader = m
                 break
         else:
             # raise exception?
             leader = None
 
-        return Status(status_response.version,
-                      status_response.dbSize,
-                      leader,
-                      status_response.raftIndex,
-                      status_response.raftTerm)
+        return Status(
+            status_response.version,
+            status_response.dbSize,
+            leader,
+            status_response.raftIndex,
+            status_response.raftTerm,
+        )
 
     @_handle_errors
     @_ensure_connected
     async def add_member(self, urls):
         """Add a member into the cluster.
 
         :return:
@@ -1192,25 +1237,25 @@
         :param member_id:
             The cluster member ID to create an alarm to.
             If 0, the alarm is created for all the members of the cluster.
 
         :return:
             A sequence of :class:`~aetcd.client.Alarm`.
         """
-        alarm_request = self._build_alarm_request('activate',
-                                                  member_id,
-                                                  'no space')
+        alarm_request = self._build_alarm_request('activate', member_id, 'no space')
         alarm_response = await self.maintenancestub.Alarm(
             alarm_request,
             timeout=self._timeout,
             metadata=self.metadata,
         )
 
-        return [Alarm(alarm.alarm, alarm.memberID)
-                for alarm in alarm_response.alarms]
+        return [
+            Alarm(alarm.alarm, alarm.memberID)
+            for alarm in alarm_response.alarms
+        ]
 
     @_handle_errors
     @_ensure_connected
     async def list_alarms(self, member_id=0, alarm_type='none'):
         """List the activated alarms.
 
         :param member_id:
@@ -1219,17 +1264,15 @@
         :param alarm_type:
             The cluster member ID to create an alarm to.
             If 0, the alarm is created for all the members of the cluster.
 
         :return:
             A sequence of :class:`~aetcd.client.Alarm`.
         """
-        alarm_request = self._build_alarm_request('get',
-                                                  member_id,
-                                                  alarm_type)
+        alarm_request = self._build_alarm_request('get', member_id, alarm_type)
         alarm_response = await self.maintenancestub.Alarm(
             alarm_request,
             timeout=self._timeout,
             metadata=self.metadata,
         )
 
         for alarm in alarm_response.alarms:
@@ -1242,25 +1285,25 @@
 
         :param member_id:
             The cluster member id to cancel an alarm.
             If 0, the alarm is canceled for all the members of the cluster.
 
         :return: A sequence of :class:`~aetcd.client.Alarm`.
         """
-        alarm_request = self._build_alarm_request('deactivate',
-                                                  member_id,
-                                                  'no space')
+        alarm_request = self._build_alarm_request('deactivate', member_id, 'no space')
         alarm_response = await self.maintenancestub.Alarm(
             alarm_request,
             timeout=self._timeout,
             metadata=self.metadata,
         )
 
-        return [Alarm(alarm.alarm, alarm.memberID)
-                for alarm in alarm_response.alarms]
+        return [
+            Alarm(alarm.alarm, alarm.memberID)
+            for alarm in alarm_response.alarms
+        ]
 
     @_handle_errors
     @_ensure_connected
     async def snapshot(self, file_obj):
         """Take a snapshot of the database.
 
         :param file_obj:
@@ -1370,27 +1413,25 @@
 
         Returns list from an input list of etcd3.transactions.{Put, Get,
         Delete, Txn} objects.
         """
         request_ops = []
         for op in ops:
             if isinstance(op, transactions.Put):
-                request = self._build_put_request(op.key, op.value,
-                                                  op.lease, op.prev_kv)
+                request = self._build_put_request(op.key, op.value, op.lease, op.prev_kv)
                 request_op = rpc.RequestOp(request_put=request)
                 request_ops.append(request_op)
 
             elif isinstance(op, transactions.Get):
                 request = self._build_get_range_request(op.key, op.range_end)
                 request_op = rpc.RequestOp(request_range=request)
                 request_ops.append(request_op)
 
             elif isinstance(op, transactions.Delete):
-                request = self._build_delete_request(op.key, op.range_end,
-                                                     op.prev_kv)
+                request = self._build_delete_request(op.key, op.range_end, op.prev_kv)
                 request_op = rpc.RequestOp(request_delete_range=request)
                 request_ops.append(request_op)
 
             elif isinstance(op, transactions.Txn):
                 compare = [c.build_message() for c in op.compare]
                 success_ops = self._ops_to_requests(op.success)
                 failure_ops = self._ops_to_requests(op.failure)
```

### Comparing `aetcd-1.0.0a2/aetcd/exceptions.py` & `aetcd-1.0.0a4/aetcd/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,26 @@
     """Raises on etcd internal errors."""
 
 
 class InvalidArgumentError(ClientError):
     """Raises on errors associated with incorrect arguments being provided."""
 
 
+class UnauthenticatedError(ClientError):
+    """Raises on etcd unauthenticated errors."""
+
+
 class PreconditionFailedError(ClientError):
     """Raises on etcd server precondition errors."""
 
 
+class DuplicateLeaseError(ClientError):
+    """Raised on attempt to create lease with already existing id."""
+
+
 class RevisionCompactedError(ClientError):
     """Raises when requested and previous revisions were already compacted."""
 
     def __init__(self, compacted_revision):
         #: Revision bellow values were compacted.
         self.compacted_revision = compacted_revision
 
@@ -48,24 +56,29 @@
 
 _EXCEPTIONS_BY_CODE = {
     rpc.StatusCode.DEADLINE_EXCEEDED: ConnectionTimeoutError,
     rpc.StatusCode.FAILED_PRECONDITION: PreconditionFailedError,
     rpc.StatusCode.INTERNAL: InternalError,
     rpc.StatusCode.INVALID_ARGUMENT: InvalidArgumentError,
     rpc.StatusCode.UNAVAILABLE: ConnectionFailedError,
+    rpc.StatusCode.UNAUTHENTICATED: UnauthenticatedError,
 }
 
 
 def _handle_exception(error: Exception):
     # If the error is one of the client errors, raise as is
     if isinstance(error, ClientError):
         raise error
 
     # Query RPC error mapping and raise one of the matched client errors
     if isinstance(error, rpc.AioRpcError):
         e = _EXCEPTIONS_BY_CODE.get(error.code())
+        error_details = error.details()
+
         if e is not None:
-            raise e(error.details()) from error
-        raise ClientError(error.details()) from error
+            if e is PreconditionFailedError and 'lease already exists' in error_details:
+                raise DuplicateLeaseError
+            raise e(error_details) from error
+        raise ClientError(error_details) from error
 
     # Fallback to wrap original error with the client error
     raise ClientError(error)
```

### Comparing `aetcd-1.0.0a2/aetcd/leases.py` & `aetcd-1.0.0a4/aetcd/leases.py`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/aetcd/locks.py` & `aetcd-1.0.0a4/aetcd/locks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import time
+import asyncio
 import uuid
 
 from . import exceptions
 from . import rtypes
 
 
 class Lock:
@@ -89,24 +89,25 @@
             Maximum time to wait before returning. ``None`` means
             forever, any other value equal or greater than 0 is
             the number of seconds.
 
         :return:
             ``True`` if the lock has been acquired, ``False`` otherwise.
         """
+        loop = asyncio.get_running_loop()
         deadline = None
         if timeout is not None:
-            deadline = time.time() + timeout
+            deadline = loop.time() + timeout
 
         while True:
             if await self._try_acquire():
                 return True
 
             if deadline is not None:
-                remaining_timeout = max(deadline - time.time(), 0)
+                remaining_timeout = max(deadline - loop.time(), 0)
                 if remaining_timeout == 0:
                     return False
             else:
                 remaining_timeout = None
 
             await self._wait_for_delete_event(remaining_timeout)
```

### Comparing `aetcd-1.0.0a2/aetcd/members.py` & `aetcd-1.0.0a4/aetcd/members.py`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/aetcd/rpc/__init__.py` & `aetcd-1.0.0a4/aetcd/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/aetcd/rpc/rpc_pb2_grpc.py` & `aetcd-1.0.0a4/aetcd/rpc/rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/aetcd/rtypes.py` & `aetcd-1.0.0a4/aetcd/rtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,16 +250,15 @@
         'prev_kv',
     ]
 
     def __init__(self, kind, kv, prev_kv=None):
         #: The kind of event. If the type is a ``PUT``, it indicates
         #: new data has been stored to the key. If the type is a ``DELETE``,
         #: it indicates the key was deleted.
-        self.kind: EventKind = rpc.Event.EventType.DESCRIPTOR.values_by_number[
-            kind].name
+        self.kind: EventKind = rpc.Event.EventType.DESCRIPTOR.values_by_number[kind].name
 
         #: Holds the key-value for the event.
         #: A ``PUT`` event contains current key-value pair.
         #: A ``PUT`` event with version that equals to 1 indicates the creation of a key.
         #: A ``DELETE`` event contains the deleted key with
         #: its modification revision set to the revision of deletion.
         self.kv: KeyValue = KeyValue(kv)
@@ -290,17 +289,16 @@
     ):
         self._iterator = iterator
         self._cancel = cancel_func
 
         #: The ID of the watcher that emits the events.
         self.watch_id: int = watch_id
 
-    async def __aiter__(self):
-        async for event in self._iterator():
-            yield event
+    def __aiter__(self):
+        return self._iterator()
 
     async def cancel(self):
         """Cancel the watcher so that no more events are emitted."""
         await self._cancel()
 
     def __repr__(self):
         return f'Watch[watch_id={self.watch_id!r}]'
```

### Comparing `aetcd-1.0.0a2/aetcd/transactions.py` & `aetcd-1.0.0a4/aetcd/transactions.py`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/aetcd/utils.py` & `aetcd-1.0.0a4/aetcd/utils.py`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/aetcd/watcher.py` & `aetcd-1.0.0a4/aetcd/watcher.py`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/aetcd.egg-info/PKG-INFO` & `aetcd-1.0.0a4/aetcd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: aetcd
-Version: 1.0.0a2
+Version: 1.0.0a4
 Summary: Python asyncio-based client for etcd
 Home-page: https://github.com/martyanov/aetcd
 Author: Andrey Martyanov
 Author-email: andrey@martyanov.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://aetcd.readthedocs.io
 Project-URL: Code, https://github.com/martyanov/aetcd
 Project-URL: Issues, https://github.com/martyanov/aetcd/issues
 Keywords: etcd3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
@@ -89,9 +89,7 @@
 
 .. _etcd3aio: https://github.com/hron/etcd3aio
 .. _python-etcd3: https://github.com/kragniz/python-etcd3
 .. _kragniz: https://github.com/kragniz
 .. _hron: https://github.com/hron
 .. _gjcarneiro: https://github.com/gjcarneiro
 .. _people: https://github.com/martyanov/aetcd/graphs/contributors
-
-
```

### Comparing `aetcd-1.0.0a2/aetcd.egg-info/SOURCES.txt` & `aetcd-1.0.0a4/aetcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/docs/Makefile` & `aetcd-1.0.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/docs/changelog.rst` & `aetcd-1.0.0a4/docs/changelog.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,55 @@
 =========
 Changelog
 =========
 
+1.0.0a4 (2023-05-24)
+--------------------
+
+Dependencies
+^^^^^^^^^^^^
+
+* Remove pifpaf from dependencies
+
+1.0.0a3 (2023-05-24)
+--------------------
+
+Improvements
+^^^^^^^^^^^^
+
+* Use monotonic timer in locks implementation
+* Limit client connect and close waiting time
+* Support lease in replace operation (#21)
+* Replace sync subprocess call with async version (#25)
+* Add UnauthenticatedError
+* Add Python 3.11 support
+* Add duplicate lease exception (#22)
+* Add 3.4 and 3.5 ETCD versions to CI matrix (#26)
+* Set timeout for tests job on CI (#27)
+* Add keepalive ETCD client settings in integration tests (#28)
+* Fix test for serializable read
+
+Bugfixes
+^^^^^^^^
+
+* Fix Connect and Watch iterator
+
+Dependencies
+^^^^^^^^^^^^
+
+* Bump packaging dependencies: pip 23.0, setuptools 67.3.2, wheel 0.38.4
+* Bump twine to 4.0.2
+* Bump flake8 to 6.0.0 and update related plugins
+* Bump pytest-asyncio to 0.20.3
+* Bump pytest to 7.2.1
+* Bump pytest-cov to 4.0.0
+* Bump pytest-mock to 3.10.0
+* Bump sphinx to 6.1.3 and sphinx_rtd_theme to 1.2.0
+* Bump grpcio to 1.51.1 and protobuf to 4+
+
 1.0.0a2 (2022-01-14)
 --------------------
 
 Features
 ^^^^^^^^
 
 * ``grpclib`` was replaced with ``grpc.aio``
```

### Comparing `aetcd-1.0.0a2/docs/contributing.rst` & `aetcd-1.0.0a4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/docs/guide.rst` & `aetcd-1.0.0a4/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/docs/installation.rst` & `aetcd-1.0.0a4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/proto/auth.proto` & `aetcd-1.0.0a4/proto/auth.proto`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/proto/kv.proto` & `aetcd-1.0.0a4/proto/kv.proto`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/proto/rpc.proto` & `aetcd-1.0.0a4/proto/rpc.proto`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/setup.py` & `aetcd-1.0.0a4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,45 +31,45 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     project_urls={
         'Documentation': 'https://aetcd.readthedocs.io',
         'Code': 'https://github.com/martyanov/aetcd',
         'Issues': 'https://github.com/martyanov/aetcd/issues',
     },
     python_requires='>=3.8,<4.0',
     setup_requires=[
         'setuptools_scm==6.3.2',
     ],
     install_requires=[
-        'grpcio>1.41,<2',
-        'protobuf>3,<4',
+        'grpcio>1.51,<2',
+        'protobuf>4,<5',
     ],
     extras_require={
         'dev': [
             'flake8-commas==2.1.0',
-            'flake8-docstrings==1.6.0',
-            'flake8-isort==4.1.1',
-            'flake8-quotes==3.3.1',
-            'flake8==4.0.1',
-            'grpcio-tools==1.43.0',
-            'pep8-naming==0.12.1',
-            'twine==3.7.1',
+            'flake8-docstrings==1.7.0',
+            'flake8-isort==6.0.0',
+            'flake8-quotes==3.3.2',
+            'flake8==6.0.0',
+            'grpcio-tools==1.51.1',
+            'pep8-naming==0.13.3',
+            'twine==4.0.2',
         ],
         'doc': [
-            'sphinx==4.3.2',
-            'sphinx_rtd_theme==1.0.0',
+            'sphinx==6.1.3',
+            'sphinx_rtd_theme==1.2.0',
         ],
         'test': [
-            'pifpaf==3.1.5',
-            'pytest-asyncio==0.16.0',
-            'pytest-cov==3.0.0',
-            'pytest-mock==3.6.1',
-            'pytest==6.2.5',
+            'pytest-asyncio==0.20.3',
+            'pytest-cov==4.0.0',
+            'pytest-mock==3.10.0',
+            'pytest==7.2.1',
         ],
     },
 )
```

### Comparing `aetcd-1.0.0a2/tests/conftest.py` & `aetcd-1.0.0a4/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import pytest
 
 import aetcd
 import aetcd.rpc
 
 
+def pytest_addoption(parser):
+    parser.addoption(
+        '--with-cluster',
+        action='store_true',
+        default=False,
+        help='Run tests with ETCD cluster',
+    )
+
+
 @pytest.fixture
 async def etcd():
     # TODO: Rewrite the mock and related tests without side-effects
     async with aetcd.Client() as client:
         yield client
```

### Comparing `aetcd-1.0.0a2/tests/integration/conftest.py` & `aetcd-1.0.0a4/tests/integration/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,48 @@
+import asyncio
+import asyncio.subprocess
 import contextlib
 import json
 import os
-import subprocess
 import urllib.parse
 
 import pytest
 
 import aetcd
 
 
 @pytest.fixture(scope='session', autouse=True)
 def setup():
     os.environ['ETCDCTL_API'] = '3'
 
 
 @pytest.fixture(scope='session')
+@pytest.mark.asyncio
 def etcdctl():
-    def _etcdctl(*args, ignore_result=False):
+    async def _etcdctl(*args, ignore_result=False):
         endpoint = os.environ.get('TEST_ETCD_HTTP_URL')
         if endpoint:
             args = ['--endpoints', endpoint] + list(args)
         args = ['etcdctl', '-w', 'json'] + list(args)
-        output = subprocess.check_output(args)
+
+        proc = await asyncio.create_subprocess_exec(
+            *args,
+            stdout=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.PIPE,
+        )
+
+        stdout, stderr = await proc.communicate()
+
+        if proc.returncode != 0:
+            raise Exception(f'Error during awaiting process with args {args!r}: {stderr}')
+
         if ignore_result:
             return None
-        return json.loads(output.decode('utf-8'))
+
+        return json.loads(stdout.decode('utf-8'))
     return _etcdctl
 
 
 @pytest.fixture
 async def client(etcdctl):
     host = 'localhost'
     port = 2379
@@ -50,20 +64,24 @@
     ):
         async with aetcd.Client(
             host=host,
             port=port,
             username=username,
             password=password,
             timeout=timeout,
-            options=options,
+            options={
+                'keepalive_time_ms': 6000,
+                'keepalive_permit_without_calls': True,
+                'http2_max_pings_without_data': 0,
+            },
         ) as client:
             yield client
 
-        etcdctl('del', '--prefix', '')
-        result = etcdctl('get', '--prefix', '')
+        await etcdctl('del', '--prefix', '')
+        result = await etcdctl('get', '--prefix', '')
         assert 'kvs' not in result
 
     return _client
 
 
 @pytest.fixture
 async def etcd(client):
```

### Comparing `aetcd-1.0.0a2/tests/integration/test_kv.py` & `aetcd-1.0.0a4/tests/integration/test_kv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import base64
 import contextlib
 import os
 import signal
 import string
 import subprocess
 
@@ -22,78 +23,85 @@
     finally:
         for pid in pids:
             os.kill(pid, signal.SIGCONT)
 
 
 @pytest.mark.asyncio
 async def test_get_key(etcdctl, etcd):
-    etcdctl('put', '/key', 'value')
+    await etcdctl('put', '/key', 'value')
     result = await etcd.get(b'/key')
     assert result.value == b'value'
 
 
 @pytest.mark.asyncio
 async def test_get_key_has_revision(etcdctl, etcd):
-    etcdctl('put', '/key', 'value')
+    await etcdctl('put', '/key', 'value')
     result = await etcd.get(b'/key')
     assert result.header.revision > 0
 
 
+@pytest.mark.skipif(
+    "config.getoption('--with-cluster') is False",
+    reason='ETCD cluster was not run',
+)
 @pytest.mark.asyncio
 async def test_get_key_with_serializable(etcdctl, etcd):
-    etcdctl('put', '/key', 'value')
+    await etcdctl('put', '/key', 'value')
+    await etcdctl('put', '/key', 'updated_value')
     with _out_quorum():
         result = await etcd.get(b'/key', serializable=True)
-    assert result.value == b'value'
+
+    # Serializable read may return stale data
+    assert result is None or result.value in (b'value', b'updated_value')
 
 
 @pytest.mark.asyncio
 async def test_get_key_unknown(etcd):
     result = await etcd.get(b'unknown')
     assert result is None
 
 
 @pytest.mark.asyncio
 async def test_get_prefix(etcdctl, etcd):
     for i in range(20):
-        etcdctl('put', f'/inrange{i}', 'in range')
+        await etcdctl('put', f'/inrange{i}', 'in range')
 
     for i in range(5):
-        etcdctl('put', f'/notinrange{i}', 'not in range')
+        await etcdctl('put', f'/notinrange{i}', 'not in range')
 
     results = list(await etcd.get_prefix(b'/inrange'))
 
     assert len(results) == 20
     for result in results:
         assert result.value == b'in range'
 
 
 @pytest.mark.asyncio
 async def test_get_prefix_with_keys_only(etcdctl, etcd):
     for i in range(20):
-        etcdctl('put', f'/inrange{i}', 'in range')
+        await etcdctl('put', f'/inrange{i}', 'in range')
 
     for i in range(5):
-        etcdctl('put', f'/notinrange{i}', 'not in range')
+        await etcdctl('put', f'/notinrange{i}', 'not in range')
 
     results = list(await etcd.get_prefix(b'/inrange', keys_only=True))
 
     assert len(results) == 20
     for result in results:
         assert result.key.startswith(b'/inrange')
         assert not result.value
 
 
 @pytest.mark.asyncio
 async def test_get_range(etcdctl, etcd):
     for char in string.ascii_lowercase:
         if char < 'p':
-            etcdctl('put', '/key' + char, 'in range')
+            await etcdctl('put', '/key' + char, 'in range')
         else:
-            etcdctl('put', '/key' + char, 'not in range')
+            await etcdctl('put', '/key' + char, 'not in range')
 
     results = list(await etcd.get_range(b'/keya', b'/keyp'))
 
     assert len(results) == 15
     for result in results:
         assert result.value == b'in range'
 
@@ -103,15 +111,15 @@
     def remove_prefix(key, prefix):
         return key[len(prefix):]
 
     initial_keys = 'abcde'
     initial_values = 'qwert'
 
     for k, v in zip(initial_keys, initial_values):
-        etcdctl('put', f'/key{k}', v)
+        await etcdctl('put', f'/key{k}', v)
 
     keys = b''
     for result in await etcd.get_prefix(b'/key', sort_order='ascend'):
         keys += remove_prefix(result.key, b'/key')
 
     assert keys == initial_keys.encode('utf-8')
 
@@ -124,27 +132,27 @@
 
     assert reverse_keys == (''.join(reversed(initial_keys))).encode('utf-8')
 
 
 @pytest.mark.asyncio
 async def test_get_range_not_found(etcdctl, etcd):
     for i in range(5):
-        etcdctl('put', f'/inrange{i}', 'not in range')
+        await etcdctl('put', f'/inrange{i}', 'not in range')
 
     results = list(await etcd.get_prefix(b'/notinrange'))
     assert not results
 
 
 @pytest.mark.asyncio
 async def test_get_all(etcdctl, etcd):
     for i in range(20):
-        etcdctl('put', f'/inrange{i}', 'value')
+        await etcdctl('put', f'/inrange{i}', 'value')
 
     for i in range(5):
-        etcdctl('put', f'/notinrange{i}', 'value')
+        await etcdctl('put', f'/notinrange{i}', 'value')
 
     results = list(await etcd.get_all())
 
     assert len(results) == 25
     for result in results:
         assert result.value == b'value'
 
@@ -154,34 +162,34 @@
     result = list(await etcd.get_all())
     assert not result
 
 
 @pytest.mark.asyncio
 async def test_put_key(etcdctl, etcd):
     await etcd.put(b'/key', b'value')
-    result = etcdctl('get', '/key')
+    result = await etcdctl('get', '/key')
     assert base64.b64decode(result['kvs'][0]['value']) == b'value'
 
 
 @pytest.mark.asyncio
 async def test_put_key_has_revision(etcd):
     response = await etcd.put(b'/key', b'value')
     assert response.header.revision > 0
 
 
 @pytest.mark.asyncio
 async def test_put_key_with_prev_kv(etcdctl, etcd):
-    etcdctl('put', '/key', 'old_value')
+    await etcdctl('put', '/key', 'old_value')
     result = await etcd.put(b'/key', b'value', prev_kv=True)
     assert result.prev_kv.value == b'old_value'
 
 
 @pytest.mark.asyncio
 async def test_delete_key(etcdctl, etcd):
-    etcdctl('put', '/key', 'value')
+    await etcdctl('put', '/key', 'value')
 
     result = await etcd.get(b'/key')
     assert result.value == b'value'
 
     result = await etcd.delete(b'/key')
     assert result
     assert result.deleted == 1
@@ -191,35 +199,35 @@
 
     result = await etcd.delete(b'unknown')
     assert result is None
 
 
 @pytest.mark.asyncio
 async def test_delete_key_has_revision(etcdctl, etcd):
-    etcdctl('put', '/key', 'value')
+    await etcdctl('put', '/key', 'value')
 
     result = await etcd.delete(b'/key')
     assert result.header.revision > 0
 
 
 @pytest.mark.asyncio
 async def test_delete_key_with_prev_kv(etcdctl, etcd):
-    etcdctl('put', '/key', 'old_value')
+    await etcdctl('put', '/key', 'old_value')
     result = await etcd.delete(
         b'/key',
         prev_kv=True,
     )
     assert result.prev_kv.value == b'old_value'
     assert result.deleted == 1
 
 
 @pytest.mark.asyncio
 async def test_delete_prefix_keys(etcdctl, etcd):
-    etcdctl('put', '/key1', 'value1')
-    etcdctl('put', '/key2', 'value2')
+    await etcdctl('put', '/key1', 'value1')
+    await etcdctl('put', '/key2', 'value2')
 
     result = await etcd.get(b'/key1')
     assert result.value == b'value1'
 
     result = await etcd.get(b'/key2')
     assert result.value == b'value2'
 
@@ -231,16 +239,16 @@
 
     result = await etcd.get(b'/key2')
     assert result is None
 
 
 @pytest.mark.asyncio
 async def test_delete_prefix_keys_with_prev_kv(etcdctl, etcd):
-    etcdctl('put', '/key1', 'value1')
-    etcdctl('put', '/key2', 'value2')
+    await etcdctl('put', '/key1', 'value1')
+    await etcdctl('put', '/key2', 'value2')
 
     response = await etcd.delete_prefix(b'/key', prev_kv=True)
     assert response.deleted == 2
 
     kv1, kv2 = response.prev_kvs
     assert kv1.value == b'value1'
     assert kv2.value == b'value2'
@@ -252,15 +260,15 @@
         '/key\1': 'value0',
         '/key1': 'value1',
         '/key2': 'value2',
         '/key3': 'value3',
         '/key3\1': 'value30',
         '/key4': 'value4',
     }.items():
-        etcdctl('put', k, v)
+        await etcdctl('put', k, v)
 
     result = await etcd.get(b'/key2')
     assert result.value == b'value2'
 
     result = await etcd.get(b'/key4')
     assert result.value == b'value4'
 
@@ -278,16 +286,16 @@
 
     result = await etcd.get(b'/key4')
     assert result.value == b'value4'
 
 
 @pytest.mark.asyncio
 async def test_delete_range_keys_with_prev_kv(etcdctl, etcd):
-    etcdctl('put', '/key1', 'value1')
-    etcdctl('put', '/key2', 'value2')
+    await etcdctl('put', '/key1', 'value1')
+    await etcdctl('put', '/key2', 'value2')
 
     response = await etcd.delete_range(b'/key1', b'/key3', prev_kv=True)
     assert response.deleted == 2
 
     kv1, kv2 = response.prev_kvs
     assert kv1.value == b'value1'
     assert kv2.value == b'value2'
@@ -299,43 +307,59 @@
     status = await etcd.replace(b'/key', b'value1', b'value2')
     result = await etcd.get(b'/key')
     assert result.value == b'value2'
     assert status is True
 
 
 @pytest.mark.asyncio
+async def test_replace_with_lease_success(etcd):
+    lease = await etcd.lease(ttl=3)
+    await etcd.put(b'/test_key', b'value1')
+    status = await etcd.replace(b'/test_key', b'value1', b'value2', lease=lease)
+    result = await etcd.get(b'/test_key')
+    assert result.value == b'value2'
+    assert status is True
+
+    # Wait for the lease to expire
+    await asyncio.sleep((await lease.granted_ttl()) + 1)
+
+    result = await etcd.get(b'/test_key')
+    assert result is None
+
+
+@pytest.mark.asyncio
 async def test_replace_fail(etcd):
     await etcd.put(b'/key', b'value1')
     status = await etcd.replace(b'/key', b'value2', b'value3')
     result = await etcd.get(b'/key')
     assert result.value == b'value1'
     assert status is False
 
 
 @pytest.mark.asyncio
 async def test_transaction_success(etcdctl, etcd):
-    etcdctl('put', '/key', 'value')
+    await etcdctl('put', '/key', 'value')
     await etcd.transaction(
         compare=[etcd.transactions.value(b'/key') == b'value'],
         success=[etcd.transactions.put(b'/key', b'success')],
         failure=[etcd.transactions.put(b'/key', b'failure')],
     )
-    result = etcdctl('get', '/key')
+    result = await etcdctl('get', '/key')
     assert base64.b64decode(result['kvs'][0]['value']) == b'success'
 
 
 @pytest.mark.asyncio
 async def test_transaction_failure(etcdctl, etcd):
-    etcdctl('put', '/key', 'value1')
+    await etcdctl('put', '/key', 'value1')
     await etcd.transaction(
         compare=[etcd.transactions.value(b'/key') == b'value2'],
         success=[etcd.transactions.put(b'/key', b'success')],
         failure=[etcd.transactions.put(b'/key', b'failure')],
     )
-    result = etcdctl('get', '/key')
+    result = await etcdctl('get', '/key')
     assert base64.b64decode(result['kvs'][0]['value']) == b'failure'
 
 
 @pytest.mark.asyncio
 async def test_nested_transactions(etcd):
     await etcd.transaction(
         compare=[],
```

### Comparing `aetcd-1.0.0a2/tests/integration/test_lease.py` & `aetcd-1.0.0a4/tests/integration/test_lease.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import asyncio
 
 import pytest
 
+import aetcd.exceptions
+
 
 @pytest.mark.asyncio
 async def test_lease_grant(etcd):
     lease = await etcd.lease(1)
 
     assert isinstance(lease.ttl, int)
     assert isinstance(lease.id, int)
@@ -40,7 +42,15 @@
     assert result.value == b'value'
     assert (await lease.remaining_ttl()) <= (await lease.granted_ttl())
 
     # Wait for the lease to expire
     await asyncio.sleep((await lease.granted_ttl()) + 1)
     result = await etcd.get(key)
     assert result is None
+
+
+@pytest.mark.asyncio
+async def test_lease_create_with_already_existing_id(etcd):
+    await etcd.lease(10, lease_id=123)
+
+    with pytest.raises(aetcd.exceptions.DuplicateLeaseError):
+        await etcd.lease(15, lease_id=123)
```

### Comparing `aetcd-1.0.0a2/tests/integration/test_lock.py` & `aetcd-1.0.0a4/tests/integration/test_lock.py`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/tests/integration/test_maintenance.py` & `aetcd-1.0.0a4/tests/integration/test_maintenance.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,8 +78,8 @@
 
 @pytest.mark.asyncio
 async def test_snapshot(etcdctl, etcd):
     with tempfile.NamedTemporaryFile() as f:
         await etcd.snapshot(f)
         f.flush()
 
-        etcdctl('snapshot', 'status', f.name)
+        await etcdctl('snapshot', 'status', f.name)
```

### Comparing `aetcd-1.0.0a2/tests/integration/test_watch.py` & `aetcd-1.0.0a4/tests/integration/test_watch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 import asyncio
 import base64
-import threading
-import time
 
 import pytest
 
 import aetcd.exceptions
 import aetcd.rpc
 import aetcd.utils
 
 
 @pytest.fixture
 def etcdctl_put(etcdctl):
-    def _etcdctl_put(key, value):
-        etcdctl('put', key, value)
-        result = etcdctl('get', key)
+    async def _etcdctl_put(key, value):
+        await etcdctl('put', key, value)
+        result = await etcdctl('get', key)
         assert base64.b64decode(
             result['kvs'][0]['value']) == aetcd.utils.to_bytes(value)
     return _etcdctl_put
 
 
 @pytest.mark.asyncio
 async def test_watch_key(etcdctl, etcd, etcdctl_put):
-    def update_key():
+    async def update_key():
         # Sleep to make watch can get the event
-        time.sleep(3)
-        etcdctl_put('key', '0')
-        time.sleep(1)
-        etcdctl_put('key', '1')
-        time.sleep(1)
-        etcdctl_put('key', '2')
-        time.sleep(1)
-        etcdctl_put('key', '3')
-        time.sleep(1)
+        await asyncio.sleep(3)
+        await etcdctl_put('key', '0')
+        await asyncio.sleep(1)
+        await etcdctl_put('key', '1')
+        await asyncio.sleep(1)
+        await etcdctl_put('key', '2')
+        await asyncio.sleep(1)
+        await etcdctl_put('key', '3')
+        await asyncio.sleep(1)
 
-    t = threading.Thread(name='update_key', target=update_key)
-    t.start()
+    t = asyncio.create_task(update_key(), name='update_key')
 
     change_count = 0
     w = await etcd.watch(b'key')
     async for event in w:
         assert event.kv.key == b'key'
         assert event.kv.value == aetcd.utils.to_bytes(str(change_count))
 
@@ -47,34 +44,33 @@
         assert event.kv.value != b'3'
 
         change_count += 1
         if change_count > 2:
             # If cancel not work, we will block in this for-loop forever
             await w.cancel()
 
-    t.join()
+    await t
 
 
 @pytest.mark.asyncio
 async def test_watch_key_with_revision_compacted(etcdctl, etcd, etcdctl_put):
     # Some data to compact
-    etcdctl('put', 'key', '0')
+    await etcdctl('put', 'key', '0')
     result = await etcd.get(b'key')
     revision = result.mod_revision
 
     # Compact etcd and test watcher
     await etcd.compact(revision)
 
-    def update_key():
-        etcdctl_put('key', '1')
-        etcdctl_put('key', '2')
-        etcdctl_put('key', '3')
+    async def update_key():
+        await etcdctl_put('key', '1')
+        await etcdctl_put('key', '2')
+        await etcdctl_put('key', '3')
 
-    t = threading.Thread(name='update_key', target=update_key)
-    t.start()
+    t = asyncio.create_task(update_key(), name='update_key')
 
     async def watch_compacted_revision_test():
         w = await etcd.watch(b'key', start_revision=(revision - 1))
 
         error_raised = False
         compacted_revision = 0
         try:
@@ -103,33 +99,32 @@
 
             change_count += 1
             if change_count > 2:
                 await w.cancel()
 
     await watch_compacted_revision_test()
 
-    t.join()
+    await t
 
 
 @pytest.mark.asyncio
 async def test_watch_key_prefix(etcdctl, etcd, etcdctl_put):
-    def update_key_prefix():
+    async def update_key_prefix():
         # Sleep to make watch can get the event
-        time.sleep(3)
-        etcdctl_put('/key0', '0')
-        time.sleep(1)
-        etcdctl_put('/key1', '1')
-        time.sleep(1)
-        etcdctl_put('/key2', '2')
-        time.sleep(1)
-        etcdctl_put('/key3', '3')
-        time.sleep(1)
+        await asyncio.sleep(3)
+        await etcdctl_put('/key0', '0')
+        await asyncio.sleep(1)
+        await etcdctl_put('/key1', '1')
+        await asyncio.sleep(1)
+        await etcdctl_put('/key2', '2')
+        await asyncio.sleep(1)
+        await etcdctl_put('/key3', '3')
+        await asyncio.sleep(1)
 
-    t = threading.Thread(name='update_key_prefix', target=update_key_prefix)
-    t.start()
+    t = asyncio.create_task(update_key_prefix(), name='update_key_prefix')
 
     change_count = 0
     w = await etcd.watch_prefix(b'/key')
     async for event in w:
         assert event.kv.key == aetcd.utils.to_bytes(f'/key{change_count}')
         assert event.kv.value == aetcd.utils.to_bytes(str(change_count))
 
@@ -137,29 +132,28 @@
         assert event.kv.value != b'3'
 
         change_count += 1
         if change_count > 2:
             # If cancel not work, we will block in this for-loop forever
             await w.cancel()
 
-    t.join()
+    await t
 
 
 @pytest.mark.asyncio
 async def test_watch_key_once_with_put_kind(etcdctl, etcd, etcdctl_put):
-    def update_key():
+    async def update_key():
         # Sleep to make watch can get the event
-        time.sleep(2)
-        etcdctl_put('key', '1')
-        time.sleep(1)
-        etcdctl_put('key', '2')
-        time.sleep(1)
+        await asyncio.sleep(2)
+        await etcdctl_put('key', '1')
+        await asyncio.sleep(1)
+        await etcdctl_put('key', '2')
+        await asyncio.sleep(1)
 
-    t = threading.Thread(name='update_key', target=update_key)
-    t.start()
+    t = asyncio.create_task(update_key(), name='update_key')
 
     put_count = 0
     w = await etcd.watch(b'key', kind=aetcd.EventKind.PUT, prev_kv=True)
     async for event in w:
         assert event.kv.key == b'key'
 
         if put_count == 0:
@@ -171,47 +165,46 @@
         put_count += 1
         if put_count > 1:
             # If cancel not work, we will block in this for-loop forever
             await w.cancel()
 
     assert put_count == 2
 
-    t.join()
+    await t
 
 
 @pytest.mark.asyncio
 async def test_watch_key_once_with_delete_kind(etcdctl, etcd, etcdctl_put):
-    def update_key():
+    async def update_key():
         # Sleep to make watch can get the event
-        time.sleep(2)
-        etcdctl_put('key', '1')
-        time.sleep(1)
-        etcdctl('del', 'key')
-        time.sleep(1)
-        etcdctl_put('key', '2')
-        time.sleep(1)
-        etcdctl('del', 'key')
-        time.sleep(1)
+        await asyncio.sleep(2)
+        await etcdctl_put('key', '1')
+        await asyncio.sleep(1)
+        await etcdctl('del', 'key')
+        await asyncio.sleep(1)
+        await etcdctl_put('key', '2')
+        await asyncio.sleep(1)
+        await etcdctl('del', 'key')
+        await asyncio.sleep(1)
 
-    t = threading.Thread(name='update_key', target=update_key)
-    t.start()
+    t = asyncio.create_task(update_key(), name='update_key')
 
     del_count = 0
     w = await etcd.watch(b'key', kind=aetcd.EventKind.DELETE)
     async for event in w:
         assert event.kv.key == b'key'
 
         del_count += 1
         if del_count > 1:
             # If cancel not work, we will block in this for-loop forever
             await w.cancel()
 
     assert del_count == 2
 
-    t.join()
+    await t
 
 
 @pytest.mark.asyncio
 async def test_watch_key_prefix_once_sequential(etcd):
     with pytest.raises(aetcd.exceptions.WatchTimeoutError):
         await etcd.watch_prefix_once(b'/key', 1)
 
@@ -223,14 +216,14 @@
 
 
 @pytest.mark.asyncio
 async def test_watch_key_ignores_global_timeout(client, etcdctl_put):
     async with client(timeout=2) as etcd:
         w = await etcd.watch(b'key')
         await asyncio.sleep(3)
-        etcdctl_put('key', '1')
+        await etcdctl_put('key', '1')
 
         async for event in w:
             assert event.kv.value == b'1'
             break
 
         await w.cancel()
```

### Comparing `aetcd-1.0.0a2/tests/test_client.py` & `aetcd-1.0.0a4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/tests/test_exceptions.py` & `aetcd-1.0.0a4/tests/test_exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -45,20 +45,45 @@
         aetcd.exceptions._handle_exception(error)
 
     error = rpc_error(aetcd.rpc.StatusCode.UNAVAILABLE)
 
     with pytest.raises(aetcd.exceptions.ConnectionFailedError):
         aetcd.exceptions._handle_exception(error)
 
+    error = rpc_error(aetcd.rpc.StatusCode.UNAUTHENTICATED)
+
+    with pytest.raises(aetcd.exceptions.UnauthenticatedError):
+        aetcd.exceptions._handle_exception(error)
+
 
 def test__handle_exception_with_unknown_rpc_errors(rpc_error):
     error = rpc_error(aetcd.rpc.StatusCode.DATA_LOSS, 'disk failure')
 
     with pytest.raises(aetcd.exceptions.ClientError, match='disk failure'):
         aetcd.exceptions._handle_exception(error)
 
 
 def test__handle_exception_with_unknown_errors(rpc_error):
     error = Exception('unknown error')
 
     with pytest.raises(aetcd.exceptions.ClientError, match='unknown error'):
         aetcd.exceptions._handle_exception(error)
+
+
+def test__handle_exception_with_duplicate_lease_error(rpc_error):
+    error = rpc_error(
+        code=aetcd.rpc.StatusCode.FAILED_PRECONDITION,
+        details='etcdserver: lease already exists',
+    )
+
+    with pytest.raises(aetcd.exceptions.DuplicateLeaseError):
+        aetcd.exceptions._handle_exception(error)
+
+
+def test__handle_exception_with_duplicate_lease_error_and_internal_rpc_error(rpc_error):
+    error = rpc_error(
+        code=aetcd.rpc.StatusCode.INTERNAL,
+        details='etcdserver: lease already exists',
+    )
+
+    with pytest.raises(aetcd.exceptions.InternalError):
+        aetcd.exceptions._handle_exception(error)
```

### Comparing `aetcd-1.0.0a2/tests/test_rtypes.py` & `aetcd-1.0.0a4/tests/test_rtypes.py`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/tests/test_utils.py` & `aetcd-1.0.0a4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aetcd-1.0.0a2/tests/test_watcher.py` & `aetcd-1.0.0a4/tests/test_watcher.py`

 * *Files identical despite different names*

