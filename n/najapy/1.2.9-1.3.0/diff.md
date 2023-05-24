# Comparing `tmp/najapy-1.2.9.tar.gz` & `tmp/najapy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "najapy-1.2.9.tar", last modified: Wed Mar 29 02:51:06 2023, max compression
+gzip compressed data, was "najapy-1.3.0.tar", last modified: Wed May 24 09:28:16 2023, max compression
```

## Comparing `najapy-1.2.9.tar` & `najapy-1.3.0.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.972034 najapy-1.2.9/
--rw-r--r--   0 lanqiao    (501) staff       (20)    11357 2022-07-06 03:22:18.000000 najapy-1.2.9/LICENSE
--rw-r--r--   0 lanqiao    (501) staff       (20)     2700 2023-03-29 02:51:06.971110 najapy-1.2.9/PKG-INFO
--rw-r--r--   0 lanqiao    (501) staff       (20)     2236 2022-07-06 03:22:18.000000 najapy-1.2.9/README.md
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.914990 najapy-1.2.9/najapy/
--rw-r--r--   0 lanqiao    (501) staff       (20)       48 2023-03-29 01:57:28.000000 najapy-1.2.9/najapy/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.918575 najapy-1.2.9/najapy/asyncio/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/asyncio/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3731 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/asyncio/future.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.920379 najapy-1.2.9/najapy/cache/
--rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/cache/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3920 2023-01-10 03:44:10.000000 najapy-1.2.9/najapy/cache/base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    10386 2023-03-28 07:02:41.000000 najapy-1.2.9/najapy/cache/redis.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.926833 najapy-1.2.9/najapy/common/
--rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/common/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     8923 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/common/async_base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    21982 2023-03-17 06:07:48.000000 najapy-1.2.9/najapy/common/base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2827 2023-03-02 04:19:59.000000 najapy-1.2.9/najapy/common/buffer.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      564 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/common/error.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     6647 2022-10-14 09:29:48.000000 najapy-1.2.9/najapy/common/excel.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/common/interface.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/common/metaclass.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1681 2023-03-17 09:08:13.000000 najapy-1.2.9/najapy/common/process.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     8528 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/common/struct.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2607 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/common/task.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.928231 najapy-1.2.9/najapy/database/
--rw-r--r--   0 lanqiao    (501) staff       (20)       49 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/database/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3750 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/database/mongo.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    15285 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/database/mysql.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.929227 najapy-1.2.9/najapy/enum/
--rw-r--r--   0 lanqiao    (501) staff       (20)       19 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/enum/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3141 2023-02-07 09:30:47.000000 najapy-1.2.9/najapy/enum/base_enum.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.930841 najapy-1.2.9/najapy/event/
--rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/event/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3443 2023-03-20 10:41:03.000000 najapy-1.2.9/najapy/event/async_event.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1210 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/event/event.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.931922 najapy-1.2.9/najapy/frame/
--rwxr-xr-x   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/frame/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.936392 najapy-1.2.9/najapy/frame/fastapi/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/frame/fastapi/__init__.py
--rwxr-xr-x   0 lanqiao    (501) staff       (20)     3263 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/frame/fastapi/base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3067 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/frame/fastapi/form.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1042 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/frame/fastapi/response.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1723 2023-03-02 04:30:39.000000 najapy-1.2.9/najapy/frame/fastapi/ws.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3334 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/frame/logging.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.938615 najapy-1.2.9/najapy/net/
--rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/net/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     8066 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/net/http.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.939236 najapy-1.2.9/najapy/scaffold/
--rw-r--r--   0 lanqiao    (501) staff       (20)       16 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.940629 najapy-1.2.9/najapy/scaffold/fastapi_example_project/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.943051 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.943538 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.944496 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)       75 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/base_model.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.945977 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/
--rw-r--r--   0 lanqiao    (501) staff       (20)        1 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3629 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.947629 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      842 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      315 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/activate.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.948664 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/apps/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/apps/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.952594 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/external_view.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/internal_view.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/model.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/schemas.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/service.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.960340 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/conf/
--rw-r--r--   0 lanqiao    (501) staff       (20)     3486 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.dev.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.rel.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      107 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/conf/gunicorn.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.dev.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.rel.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      983 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1276 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/main.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      582 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/router.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.960770 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/services/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/services/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.961852 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/utils/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/utils/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1655 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      161 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/scaffold/fastapi_example_project/manage.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.962845 najapy-1.2.9/najapy/static/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/static/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)   208075 2022-07-06 03:22:18.000000 najapy-1.2.9/najapy/static/cacert.pem
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.917705 najapy-1.2.9/najapy.egg-info/
--rw-r--r--   0 lanqiao    (501) staff       (20)     2700 2023-03-29 02:51:06.000000 najapy-1.2.9/najapy.egg-info/PKG-INFO
--rw-r--r--   0 lanqiao    (501) staff       (20)     3949 2023-03-29 02:51:06.000000 najapy-1.2.9/najapy.egg-info/SOURCES.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)        1 2023-03-29 02:51:06.000000 najapy-1.2.9/najapy.egg-info/dependency_links.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)      499 2023-03-29 02:51:06.000000 najapy-1.2.9/najapy.egg-info/requires.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)       13 2023-03-29 02:51:06.000000 najapy-1.2.9/najapy.egg-info/top_level.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)       38 2023-03-29 02:51:06.972316 najapy-1.2.9/setup.cfg
--rw-r--r--   0 lanqiao    (501) staff       (20)     1898 2023-03-29 01:56:02.000000 najapy-1.2.9/setup.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.966040 najapy-1.2.9/tests/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-10-14 09:29:48.000000 najapy-1.2.9/tests/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      166 2022-10-14 09:29:48.000000 najapy-1.2.9/tests/main.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      863 2023-03-02 04:30:39.000000 najapy-1.2.9/tests/test_buffer.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3059 2023-01-12 02:07:34.000000 najapy-1.2.9/tests/test_func_cache.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-03-29 02:51:06.970331 najapy-1.2.9/tests/test_redis/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-03-15 01:19:41.000000 najapy-1.2.9/tests/test_redis/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     6863 2023-03-20 02:43:59.000000 najapy-1.2.9/tests/test_redis/conftest.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1337 2023-03-16 04:32:18.000000 najapy-1.2.9/tests/test_redis/mocks.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    26721 2023-03-29 02:50:21.000000 najapy-1.2.9/tests/test_redis/test_commands.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    10554 2023-03-20 02:45:47.000000 najapy-1.2.9/tests/test_redis/test_connection_pool.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2889 2023-03-27 06:50:02.000000 najapy-1.2.9/tests/test_redis/test_distributed_event.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2079 2023-03-24 10:25:17.000000 najapy-1.2.9/tests/test_redis/test_lock.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2587 2023-03-27 06:38:07.000000 najapy-1.2.9/tests/test_redis/test_pub_sub.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      923 2023-03-27 06:32:52.000000 najapy-1.2.9/tests/test_redis/test_share_cache.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1319 2022-11-21 08:43:49.000000 najapy-1.2.9/tests/test_utils.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.238783 najapy-1.3.0/
+-rw-r--r--   0 lanqiao    (501) staff       (20)    11357 2022-07-06 03:22:18.000000 najapy-1.3.0/LICENSE
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2700 2023-05-24 09:28:16.237525 najapy-1.3.0/PKG-INFO
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2236 2022-07-06 03:22:18.000000 najapy-1.3.0/README.md
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.146727 najapy-1.3.0/najapy/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       48 2023-05-24 07:51:05.000000 najapy-1.3.0/najapy/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.151073 najapy-1.3.0/najapy/asyncio/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/asyncio/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3731 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/asyncio/future.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.153917 najapy-1.3.0/najapy/cache/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/cache/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     4209 2023-05-24 08:53:21.000000 najapy-1.3.0/najapy/cache/base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    10506 2023-05-24 07:59:26.000000 najapy-1.3.0/najapy/cache/redis.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.164336 najapy-1.3.0/najapy/common/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     8923 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/async_base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    21982 2023-03-17 06:07:48.000000 najapy-1.3.0/najapy/common/base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2827 2023-03-02 04:19:59.000000 najapy-1.3.0/najapy/common/buffer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      564 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/error.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     6647 2022-10-14 09:29:48.000000 najapy-1.3.0/najapy/common/excel.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/interface.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/metaclass.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1681 2023-03-17 09:08:13.000000 najapy-1.3.0/najapy/common/process.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     8528 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/struct.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2607 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/common/task.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.167287 najapy-1.3.0/najapy/database/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       49 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/database/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3750 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/database/mongo.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    15285 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/database/mysql.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.168930 najapy-1.3.0/najapy/enum/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       19 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/enum/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3141 2023-02-07 09:30:47.000000 najapy-1.3.0/najapy/enum/base_enum.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.175118 najapy-1.3.0/najapy/event/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/event/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3443 2023-03-20 10:41:03.000000 najapy-1.3.0/najapy/event/async_event.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1210 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/event/event.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.177235 najapy-1.3.0/najapy/frame/
+-rwxr-xr-x   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.180622 najapy-1.3.0/najapy/frame/fastapi/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/fastapi/__init__.py
+-rwxr-xr-x   0 lanqiao    (501) staff       (20)     3263 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/fastapi/base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3067 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/fastapi/form.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1042 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/fastapi/response.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1723 2023-03-02 04:30:39.000000 najapy-1.3.0/najapy/frame/fastapi/ws.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3334 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/frame/logging.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.182276 najapy-1.3.0/najapy/net/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/net/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     8066 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/net/http.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.183038 najapy-1.3.0/najapy/scaffold/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       16 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.184519 najapy-1.3.0/najapy/scaffold/fastapi_example_project/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.191698 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.192923 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.194246 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)       75 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/base_model.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.196572 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        1 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3629 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.198805 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      842 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      315 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/activate.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.200446 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.204074 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/external_view.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/internal_view.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/model.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/schemas.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/service.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.213139 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3486 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.dev.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.rel.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      107 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/gunicorn.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.dev.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.rel.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      983 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1276 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/main.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      582 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/router.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.213545 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/services/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/services/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.214605 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/utils/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/utils/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1655 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      161 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/scaffold/fastapi_example_project/manage.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.216414 najapy-1.3.0/najapy/static/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/static/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)   208075 2022-07-06 03:22:18.000000 najapy-1.3.0/najapy/static/cacert.pem
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.150036 najapy-1.3.0/najapy.egg-info/
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2700 2023-05-24 09:28:15.000000 najapy-1.3.0/najapy.egg-info/PKG-INFO
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3949 2023-05-24 09:28:16.000000 najapy-1.3.0/najapy.egg-info/SOURCES.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)        1 2023-05-24 09:28:15.000000 najapy-1.3.0/najapy.egg-info/dependency_links.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)      499 2023-05-24 09:28:15.000000 najapy-1.3.0/najapy.egg-info/requires.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)       13 2023-05-24 09:28:15.000000 najapy-1.3.0/najapy.egg-info/top_level.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)       38 2023-05-24 09:28:16.239210 najapy-1.3.0/setup.cfg
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1898 2023-03-29 01:56:02.000000 najapy-1.3.0/setup.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.225534 najapy-1.3.0/tests/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-10-14 09:29:48.000000 najapy-1.3.0/tests/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      166 2022-10-14 09:29:48.000000 najapy-1.3.0/tests/main.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      863 2023-03-02 04:30:39.000000 najapy-1.3.0/tests/test_buffer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3059 2023-01-12 02:07:34.000000 najapy-1.3.0/tests/test_func_cache.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-05-24 09:28:16.235584 najapy-1.3.0/tests/test_redis/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-03-15 01:19:41.000000 najapy-1.3.0/tests/test_redis/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     6863 2023-03-20 02:43:59.000000 najapy-1.3.0/tests/test_redis/conftest.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1337 2023-03-16 04:32:18.000000 najapy-1.3.0/tests/test_redis/mocks.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    26721 2023-03-29 02:50:21.000000 najapy-1.3.0/tests/test_redis/test_commands.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    10554 2023-03-20 02:45:47.000000 najapy-1.3.0/tests/test_redis/test_connection_pool.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2889 2023-03-27 06:50:02.000000 najapy-1.3.0/tests/test_redis/test_distributed_event.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2079 2023-03-24 10:25:17.000000 najapy-1.3.0/tests/test_redis/test_lock.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2587 2023-03-27 06:38:07.000000 najapy-1.3.0/tests/test_redis/test_pub_sub.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      923 2023-03-30 08:02:33.000000 najapy-1.3.0/tests/test_redis/test_share_cache.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1319 2022-11-21 08:43:49.000000 najapy-1.3.0/tests/test_utils.py
```

### Comparing `najapy-1.2.9/LICENSE` & `najapy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/PKG-INFO` & `najapy-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: najapy
-Version: 1.2.9
+Version: 1.3.0
 Summary: Async Suite For Python
 Home-page: https://github.com/lanqiao-dev/najapy.git
 Author: lanqiao
 Author-email: 
 License: Apache License Version 2.0
 Platform: all
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `najapy-1.2.9/README.md` & `najapy-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/asyncio/future.py` & `najapy-1.3.0/najapy/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/cache/base.py` & `najapy-1.3.0/najapy/cache/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     def has(self, key):
         return key in self._cache
 
     def get(self, key, default=None):
         return self._cache.get(key, default)
 
     def set(self, key, val):
+        if val is None:
+            return
+
         self._cache[key] = val
 
     def incr(self, key, val=1):
         res = self.get(key, 0) + val
 
         self.set(key, res)
 
@@ -44,14 +47,27 @@
 
     def size(self):
         return len(self._cache)
 
     def clear(self):
         return self._cache.clear()
 
+    @property
+    def cache(self):
+        return self._cache
+
+    def __getitem__(self, key):
+        self.get(key)
+
+    def __setitem__(self, key, value):
+        self.set(key, value)
+
+    def __delitem__(self, key):
+        self.delete(key)
+
 
 class FuncCache:
     """函数缓存
 
     使用堆栈缓存实现的函数缓存，在有效期内函数签名一致就会命中缓存
     includes: 可从关键字参数中指定某些参数作为缓存key值
     excludes: 可从关键字参数中指定某些参数不作为缓存key值
```

### Comparing `najapy-1.2.9/najapy/cache/redis.py` & `najapy-1.3.0/najapy/cache/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
     async def cache_health(self):
 
         result = False
 
         async with await self.get_cache_client() as cache:
             result = bool(await cache.time())
+            Utils.log.info(f"Redis Pool Idle Current Connect Nums: {cache.pool.pool.qsize()}/{cache.pool.max_connections}")
 
         return result
 
     async def get_cache_client(self, *args, **kwargs):
         """提供redis客户端
         """
         client = None
@@ -204,15 +205,15 @@
 
         await self._init_connection()
 
         config = self.connection_kwargs
 
         Utils.log.info(
             f"Redis Pool [{config[r'host']}:{config[r'port']}] ({self._name}) initialized: "
-            f"{self._min_connections}/{self.max_connections}"
+            f"{self.pool.qsize()}/{self.max_connections}"
         )
 
         return self
 
 
 class CacheClient(Redis, AsyncContextManager):
     """Redis客户端对象，使用with进行上下文管理
```

### Comparing `najapy-1.2.9/najapy/common/async_base.py` & `najapy-1.3.0/najapy/common/async_base.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/common/base.py` & `najapy-1.3.0/najapy/common/base.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/common/buffer.py` & `najapy-1.3.0/najapy/common/buffer.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/common/error.py` & `najapy-1.3.0/najapy/common/error.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/common/excel.py` & `najapy-1.3.0/najapy/common/excel.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/common/interface.py` & `najapy-1.3.0/najapy/common/interface.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/common/metaclass.py` & `najapy-1.3.0/najapy/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/common/process.py` & `najapy-1.3.0/najapy/common/process.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/common/struct.py` & `najapy-1.3.0/najapy/common/struct.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/common/task.py` & `najapy-1.3.0/najapy/common/task.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/database/mongo.py` & `najapy-1.3.0/najapy/database/mongo.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/database/mysql.py` & `najapy-1.3.0/najapy/database/mysql.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/enum/base_enum.py` & `najapy-1.3.0/najapy/enum/base_enum.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/event/async_event.py` & `najapy-1.3.0/najapy/event/async_event.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/event/event.py` & `najapy-1.3.0/najapy/event/event.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/frame/fastapi/base.py` & `najapy-1.3.0/najapy/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/frame/fastapi/form.py` & `najapy-1.3.0/najapy/frame/fastapi/form.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/frame/fastapi/response.py` & `najapy-1.3.0/najapy/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/frame/fastapi/ws.py` & `najapy-1.3.0/najapy/frame/fastapi/ws.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/frame/logging.py` & `najapy-1.3.0/najapy/frame/logging.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/net/http.py` & `najapy-1.3.0/najapy/net/http.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py` & `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py` & `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py` & `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py` & `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/main.py` & `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/main.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/router.py` & `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/router.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py` & `najapy-1.3.0/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy/static/cacert.pem` & `najapy-1.3.0/najapy/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/najapy.egg-info/PKG-INFO` & `najapy-1.3.0/najapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: najapy
-Version: 1.2.9
+Version: 1.3.0
 Summary: Async Suite For Python
 Home-page: https://github.com/lanqiao-dev/najapy.git
 Author: lanqiao
 Author-email: 
 License: Apache License Version 2.0
 Platform: all
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `najapy-1.2.9/najapy.egg-info/SOURCES.txt` & `najapy-1.3.0/najapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/setup.py` & `najapy-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/tests/test_buffer.py` & `najapy-1.3.0/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/tests/test_func_cache.py` & `najapy-1.3.0/tests/test_func_cache.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/tests/test_redis/conftest.py` & `najapy-1.3.0/tests/test_redis/conftest.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/tests/test_redis/mocks.py` & `najapy-1.3.0/tests/test_redis/mocks.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/tests/test_redis/test_commands.py` & `najapy-1.3.0/tests/test_redis/test_commands.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/tests/test_redis/test_connection_pool.py` & `najapy-1.3.0/tests/test_redis/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/tests/test_redis/test_distributed_event.py` & `najapy-1.3.0/tests/test_redis/test_distributed_event.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/tests/test_redis/test_lock.py` & `najapy-1.3.0/tests/test_redis/test_lock.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/tests/test_redis/test_pub_sub.py` & `najapy-1.3.0/tests/test_redis/test_pub_sub.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/tests/test_redis/test_share_cache.py` & `najapy-1.3.0/tests/test_redis/test_share_cache.py`

 * *Files identical despite different names*

### Comparing `najapy-1.2.9/tests/test_utils.py` & `najapy-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*

