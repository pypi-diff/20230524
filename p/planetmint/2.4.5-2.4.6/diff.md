# Comparing `tmp/planetmint-2.4.5.tar.gz` & `tmp/planetmint-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmint-2.4.5.tar", max compression
+gzip compressed data, was "planetmint-2.4.6.tar", max compression
```

## Comparing `planetmint-2.4.5.tar` & `planetmint-2.4.6.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    34523 2023-04-21 09:09:09.220714 planetmint-2.4.5/LICENSE
--rw-r--r--   0        0        0     1614 2023-04-21 09:09:09.220714 planetmint-2.4.5/LICENSES.md
--rw-r--r--   0        0        0     3126 2023-04-21 09:09:09.220714 planetmint-2.4.5/README.md
--rw-r--r--   0        0        0     1796 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/README.md
--rw-r--r--   0        0        0      205 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/__init__.py
--rw-r--r--   0        0        0    10928 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/application_logic.py
--rw-r--r--   0        0        0      104 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/block.py
--rw-r--r--   0        0        0     4896 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/parallel_validation.py
--rw-r--r--   0        0        0     2994 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/rpc.py
--rw-r--r--   0        0        0     5291 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/abci/utils.py
--rw-r--r--   0        0        0       86 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/application/__init__.py
--rw-r--r--   0        0        0      833 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/application/basevalidationrules.py
--rw-r--r--   0        0        0    23644 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/application/validator.py
--rw-r--r--   0        0        0     2319 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/README.md
--rw-r--r--   0        0        0      705 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/__init__.py
--rw-r--r--   0        0        0     4464 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/connection.py
--rw-r--r--   0        0        0      891 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/exceptions.py
--rw-r--r--   0        0        0     1192 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/localmongodb/__init__.py
--rw-r--r--   0        0        0     6303 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/localmongodb/connection.py
--rw-r--r--   0        0        0     9498 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/localmongodb/query.py
--rw-r--r--   0        0        0     2995 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/localmongodb/schema.py
--rw-r--r--   0        0        0      438 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/__init__.py
--rw-r--r--   0        0        0      938 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/asset.py
--rw-r--r--   0        0        0      727 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/block.py
--rw-r--r--   0        0        0     3050 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/dbtransaction.py
--rw-r--r--   0        0        0      446 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/fulfills.py
--rw-r--r--   0        0        0     1971 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/input.py
--rw-r--r--   0        0        0      603 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/metadata.py
--rw-r--r--   0        0        0     4387 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/output.py
--rw-r--r--   0        0        0      600 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/models/script.py
--rw-r--r--   0        0        0    10645 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/query.py
--rw-r--r--   0        0        0     4516 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/schema.py
--rw-r--r--   0        0        0      127 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/__init__.py
--rw-r--r--   0        0        0      917 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/const.py
--rw-r--r--   0        0        0    13774 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/opt/init.lua
--rw-r--r--   0        0        0        0 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/sync_io/__init__.py
--rw-r--r--   0        0        0     2714 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/sync_io/connection.py
--rw-r--r--   0        0        0    19154 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/sync_io/query.py
--rw-r--r--   0        0        0     1154 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/sync_io/schema.py
--rw-r--r--   0        0        0      916 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/tarantool/tarantool.md
--rw-r--r--   0        0        0     1123 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/backend/utils.py
--rw-r--r--   0        0        0        0 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/commands/__init__.py
--rw-r--r--   0        0        0     1015 2023-04-21 09:09:09.236715 planetmint-2.4.5/planetmint/commands/election_types.py
--rw-r--r--   0        0        0    14105 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/commands/planetmint.py
--rw-r--r--   0        0        0     4976 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/commands/utils.py
--rw-r--r--   0        0        0     6711 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/config.py
--rw-r--r--   0        0        0    12361 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/config_utils.py
--rw-r--r--   0        0        0      401 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/const.py
--rw-r--r--   0        0        0      390 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/ipc/__init__.py
--rw-r--r--   0        0        0      951 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/ipc/events.py
--rw-r--r--   0        0        0     2195 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/ipc/exchange.py
--rw-r--r--   0        0        0        0 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/model/__init__.py
--rw-r--r--   0        0        0    14245 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/model/dataaccessor.py
--rw-r--r--   0        0        0     3442 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/start.py
--rw-r--r--   0        0        0        0 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/utils/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/utils/lazy.py
--rw-r--r--   0        0        0     2253 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/utils/processes.py
--rw-r--r--   0        0        0      261 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/utils/python.py
--rw-r--r--   0        0        0      239 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/utils/singleton.py
--rw-r--r--   0        0        0      327 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/version.py
--rw-r--r--   0        0        0        0 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/routes.py
--rw-r--r--   0        0        0     3671 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/server.py
--rw-r--r--   0        0        0      947 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/strip_content_type_middleware.py
--rw-r--r--   0        0        0        0 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/__init__.py
--rw-r--r--   0        0        0     1240 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/assets.py
--rw-r--r--   0        0        0     1525 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/base.py
--rw-r--r--   0        0        0     2345 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/blocks.py
--rw-r--r--   0        0        0     1817 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/info.py
--rw-r--r--   0        0        0     1428 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/metadata.py
--rw-r--r--   0        0        0     1464 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/outputs.py
--rw-r--r--   0        0        0     1631 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/parameters.py
--rw-r--r--   0        0        0     4785 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/transactions.py
--rw-r--r--   0        0        0      677 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/views/validators.py
--rw-r--r--   0        0        0     3548 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/websocket_dispatcher.py
--rw-r--r--   0        0        0     4906 2023-04-21 09:09:09.240715 planetmint-2.4.5/planetmint/web/websocket_server.py
--rw-r--r--   0        0        0     2664 2023-04-21 09:09:09.240715 planetmint-2.4.5/pyproject.toml
--rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 planetmint-2.4.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-24 07:48:03.918978 planetmint-2.4.6/LICENSE
+-rw-r--r--   0        0        0     1614 2023-05-24 07:48:03.918978 planetmint-2.4.6/LICENSES.md
+-rw-r--r--   0        0        0     3126 2023-05-24 07:48:03.918978 planetmint-2.4.6/README.md
+-rw-r--r--   0        0        0     1796 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/README.md
+-rw-r--r--   0        0        0      205 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/abci/__init__.py
+-rw-r--r--   0        0        0    10923 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/abci/application_logic.py
+-rw-r--r--   0        0        0      104 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/abci/block.py
+-rw-r--r--   0        0        0     4896 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/abci/parallel_validation.py
+-rw-r--r--   0        0        0     2994 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/abci/rpc.py
+-rw-r--r--   0        0        0     5260 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/abci/utils.py
+-rw-r--r--   0        0        0       86 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/application/__init__.py
+-rw-r--r--   0        0        0      833 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/application/basevalidationrules.py
+-rw-r--r--   0        0        0    23610 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/application/validator.py
+-rw-r--r--   0        0        0     2319 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/README.md
+-rw-r--r--   0        0        0      705 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/__init__.py
+-rw-r--r--   0        0        0     4464 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/connection.py
+-rw-r--r--   0        0        0      891 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/localmongodb/__init__.py
+-rw-r--r--   0        0        0     6300 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/localmongodb/connection.py
+-rw-r--r--   0        0        0     9498 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/localmongodb/query.py
+-rw-r--r--   0        0        0     2995 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/localmongodb/schema.py
+-rw-r--r--   0        0        0      438 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/models/__init__.py
+-rw-r--r--   0        0        0      938 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/models/asset.py
+-rw-r--r--   0        0        0      727 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/models/block.py
+-rw-r--r--   0        0        0     3050 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/models/dbtransaction.py
+-rw-r--r--   0        0        0      446 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/models/fulfills.py
+-rw-r--r--   0        0        0     1971 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/models/input.py
+-rw-r--r--   0        0        0      603 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/models/metadata.py
+-rw-r--r--   0        0        0     3597 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/models/output.py
+-rw-r--r--   0        0        0      600 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/models/script.py
+-rw-r--r--   0        0        0    10645 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/query.py
+-rw-r--r--   0        0        0     4516 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/schema.py
+-rw-r--r--   0        0        0      127 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/tarantool/__init__.py
+-rw-r--r--   0        0        0      917 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/tarantool/const.py
+-rw-r--r--   0        0        0    13774 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/tarantool/opt/init.lua
+-rw-r--r--   0        0        0        0 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/tarantool/sync_io/__init__.py
+-rw-r--r--   0        0        0     2714 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/tarantool/sync_io/connection.py
+-rw-r--r--   0        0        0    19154 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/tarantool/sync_io/query.py
+-rw-r--r--   0        0        0     1154 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/tarantool/sync_io/schema.py
+-rw-r--r--   0        0        0      916 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/tarantool/tarantool.md
+-rw-r--r--   0        0        0     1123 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/backend/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/commands/__init__.py
+-rw-r--r--   0        0        0     1015 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/commands/election_types.py
+-rw-r--r--   0        0        0    14264 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/commands/planetmint.py
+-rw-r--r--   0        0        0     4976 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/commands/utils.py
+-rw-r--r--   0        0        0     6645 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/config.py
+-rw-r--r--   0        0        0    12361 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/config_utils.py
+-rw-r--r--   0        0        0      401 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/const.py
+-rw-r--r--   0        0        0      390 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/ipc/__init__.py
+-rw-r--r--   0        0        0      951 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/ipc/events.py
+-rw-r--r--   0        0        0     2195 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/ipc/exchange.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/model/__init__.py
+-rw-r--r--   0        0        0    14133 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/model/dataaccessor.py
+-rw-r--r--   0        0        0     3461 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/start.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/utils/__init__.py
+-rw-r--r--   0        0        0     1153 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/utils/lazy.py
+-rw-r--r--   0        0        0     2253 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/utils/processes.py
+-rw-r--r--   0        0        0      261 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/utils/python.py
+-rw-r--r--   0        0        0      239 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/utils/singleton.py
+-rw-r--r--   0        0        0      327 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/version.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/web/__init__.py
+-rw-r--r--   0        0        0     1341 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/web/routes.py
+-rw-r--r--   0        0        0     3671 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/web/server.py
+-rw-r--r--   0        0        0      947 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/web/strip_content_type_middleware.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/web/views/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-24 07:48:03.938978 planetmint-2.4.6/planetmint/web/views/assets.py
+-rw-r--r--   0        0        0     1525 2023-05-24 07:48:03.942978 planetmint-2.4.6/planetmint/web/views/base.py
+-rw-r--r--   0        0        0     2345 2023-05-24 07:48:03.942978 planetmint-2.4.6/planetmint/web/views/blocks.py
+-rw-r--r--   0        0        0     1817 2023-05-24 07:48:03.942978 planetmint-2.4.6/planetmint/web/views/info.py
+-rw-r--r--   0        0        0     1428 2023-05-24 07:48:03.942978 planetmint-2.4.6/planetmint/web/views/metadata.py
+-rw-r--r--   0        0        0     1464 2023-05-24 07:48:03.942978 planetmint-2.4.6/planetmint/web/views/outputs.py
+-rw-r--r--   0        0        0     1631 2023-05-24 07:48:03.942978 planetmint-2.4.6/planetmint/web/views/parameters.py
+-rw-r--r--   0        0        0     4785 2023-05-24 07:48:03.942978 planetmint-2.4.6/planetmint/web/views/transactions.py
+-rw-r--r--   0        0        0      677 2023-05-24 07:48:03.942978 planetmint-2.4.6/planetmint/web/views/validators.py
+-rw-r--r--   0        0        0     3548 2023-05-24 07:48:03.942978 planetmint-2.4.6/planetmint/web/websocket_dispatcher.py
+-rw-r--r--   0        0        0     4906 2023-05-24 07:48:03.942978 planetmint-2.4.6/planetmint/web/websocket_server.py
+-rw-r--r--   0        0        0     2664 2023-05-24 07:48:03.942978 planetmint-2.4.6/pyproject.toml
+-rw-r--r--   0        0        0     4926 1970-01-01 00:00:00.000000 planetmint-2.4.6/PKG-INFO
```

### Comparing `planetmint-2.4.5/LICENSE` & `planetmint-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/LICENSES.md` & `planetmint-2.4.6/LICENSES.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/README.md` & `planetmint-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/README.md` & `planetmint-2.4.6/planetmint/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/abci/application_logic.py` & `planetmint-2.4.6/planetmint/abci/application_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,15 @@
         height = 0
         try:
             known_chain = self.validator.models.get_latest_abci_chain()
             if known_chain is not None:
                 chain_id = known_chain["chain_id"]
 
                 if known_chain["is_synced"]:
-                    msg = (
-                        f"Got invalid InitChain ABCI request ({genesis}) - " f"the chain {chain_id} is already synced."
-                    )
+                    msg = f"Got invalid InitChain ABCI request ({genesis}) - the chain {chain_id} is already synced."
                     logger.error(msg)
                     sys.exit(1)
                 if chain_id != genesis.chain_id:
                     validators = self.validator.models.get_validators()
                     self.log_abci_migration_error(chain_id, validators)
                     sys.exit(1)
                 # set migration values for app hash and height
@@ -234,26 +232,27 @@
         pre_commit_state = dict(height=self.new_height, transactions=self.block_txn_ids)
         try:
             self.validator.models.store_pre_commit_state(pre_commit_state)
 
             block_txn_hash = calculate_hash(self.block_txn_ids)
             block = self.validator.models.get_latest_block()
 
-            logger.debug("BLOCK: ", block)
-
+            logger.debug(f"BLOCK: {block}")
             if self.block_txn_ids:
                 self.block_txn_hash = calculate_hash([block["app_hash"], block_txn_hash])
             else:
                 self.block_txn_hash = block["app_hash"]
 
             validator_update = self.validator.process_block(self.new_height, self.block_transactions)
         except DBConcurrencyError:
             sys.exit(1)
         except ValueError:
             sys.exit(1)
+        except TypeError:
+            sys.exit(1)
 
         return ResponseEndBlock(validator_updates=validator_update)
 
     def commit(self):
         """Store the new height and along with block hash."""
 
         self.abort_if_abci_chain_is_not_synced()
@@ -274,15 +273,15 @@
             self.validator.models.store_block(block._asdict())
         except DBConcurrencyError:
             sys.exit(1)
         except ValueError:
             sys.exit(1)
 
         logger.debug(
-            "Commit-ing new block with hash: apphash=%s ," "height=%s, txn ids=%s",
+            "Commit-ing new block with hash: apphash=%s, height=%s, txn ids=%s",
             data,
             self.new_height,
             self.block_txn_ids,
         )
 
         if self.events_queue:
             event = Event(
```

### Comparing `planetmint-2.4.5/planetmint/abci/parallel_validation.py` & `planetmint-2.4.6/planetmint/abci/parallel_validation.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/abci/rpc.py` & `planetmint-2.4.6/planetmint/abci/rpc.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/abci/utils.py` & `planetmint-2.4.6/planetmint/abci/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 
     new_validators_dict = {**validators_dict, **updates_dict}
     return list(new_validators_dict.values())
 
 
 def get_public_key_decoder(pk):
     encoding = pk["type"]
-    decoder = base64.b64decode
 
     if encoding == "ed25519-base16":
         decoder = base64.b16decode
     elif encoding == "ed25519-base32":
         decoder = base64.b32decode
     elif encoding == "ed25519-base64":
         decoder = base64.b64decode
```

### Comparing `planetmint-2.4.5/planetmint/application/basevalidationrules.py` & `planetmint-2.4.6/planetmint/application/basevalidationrules.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/application/validator.py` & `planetmint-2.4.6/planetmint/application/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,15 @@
 
     @staticmethod
     def validate_asset_id(tx: Transaction, input_txs: list):
         # validate asset
         if tx.operation != Transaction.COMPOSE:
             asset_id = tx.get_asset_id(input_txs)
             if asset_id != Transaction.read_out_asset_id(tx):
-                raise AssetIdMismatch(
-                    ("The asset id of the input does not" " match the asset id of the" " transaction")
-                )
+                raise AssetIdMismatch(("The asset id of the input does not match the asset id of the transaction"))
         else:
             asset_ids = Transaction.get_asset_ids(input_txs)
             if Transaction.read_out_asset_id(tx) in asset_ids:
                 raise AssetIdMismatch(("The asset ID of the compose must be different to all of its input asset IDs"))
 
     @staticmethod
     def validate_input_conditions(tx: Transaction, input_conditions: list[Output]):
@@ -101,17 +99,17 @@
         Validator.validate_inputs_distinct(tx)
 
         input_amount = sum([input_condition.amount for input_condition in input_conditions])
         output_amount = sum([output_condition.amount for output_condition in tx.outputs])
 
         if output_amount != input_amount:
             raise AmountError(
-                (
-                    "The amount used in the inputs `{}`" " needs to be same as the amount used" " in the outputs `{}`"
-                ).format(input_amount, output_amount)
+                "The amount used in the inputs `{}` needs to be same as the amount used in the outputs `{}`".format(
+                    input_amount, output_amount
+                )
             )
 
         return True
 
     def validate_create_inputs(self, tx, current_transactions=[]) -> bool:
         duplicates = any(txn for txn in current_transactions if txn.id == tx.id)
         if self.models.is_committed(tx.id) or duplicates:
@@ -198,23 +196,24 @@
 
         # NOTE: Check if the proposer is a validator.
         [election_initiator_node_pub_key] = transaction.inputs[0].owners_before
         if election_initiator_node_pub_key not in current_validators.keys():
             raise InvalidProposer("Public key is not a part of the validator set")
 
         # NOTE: Check if all validators have been assigned votes equal to their voting power
-        if not self.is_same_topology(current_validators, transaction.outputs):
+        if not Validator.is_same_topology(current_validators, transaction.outputs):
             raise UnequalValidatorSet("Validator set much be exactly same to the outputs of election")
 
         if transaction.operation == VALIDATOR_ELECTION:
             self.validate_validator_election(transaction)
 
         return transaction
 
-    def is_same_topology(cls, current_topology, election_topology):
+    @staticmethod
+    def is_same_topology(current_topology, election_topology):
         voters = {}
         for voter in election_topology:
             if len(voter.public_keys) > 1:
                 return False
 
             [public_key] = voter.public_keys
             voting_power = voter.amount
```

### Comparing `planetmint-2.4.5/planetmint/backend/README.md` & `planetmint-2.4.6/planetmint/backend/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/__init__.py` & `planetmint-2.4.6/planetmint/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/connection.py` & `planetmint-2.4.6/planetmint/backend/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/exceptions.py` & `planetmint-2.4.6/planetmint/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/localmongodb/__init__.py` & `planetmint-2.4.6/planetmint/backend/localmongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/localmongodb/connection.py` & `planetmint-2.4.6/planetmint/backend/localmongodb/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         return self.query()[self.dbname][name]
 
     def run(self, query):
         try:
             try:
                 return query.run(self.connect())
             except pymongo.errors.AutoReconnect:
-                logger.warning("Lost connection to the database, " "retrying query.")
+                logger.warning("Lost connection to the database, retrying query.")
                 return query.run(self.connect())
         except pymongo.errors.AutoReconnect as exc:
             raise ConnectionError from exc
         except pymongo.errors.DuplicateKeyError as exc:
             raise DuplicateKeyError from exc
         except pymongo.errors.OperationFailure as exc:
             print(f"DETAILS: {exc.details}")
```

### Comparing `planetmint-2.4.5/planetmint/backend/localmongodb/query.py` & `planetmint-2.4.6/planetmint/backend/localmongodb/query.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/localmongodb/schema.py` & `planetmint-2.4.6/planetmint/backend/localmongodb/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/models/asset.py` & `planetmint-2.4.6/planetmint/backend/models/asset.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/models/block.py` & `planetmint-2.4.6/planetmint/backend/models/block.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/models/dbtransaction.py` & `planetmint-2.4.6/planetmint/backend/models/dbtransaction.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/models/input.py` & `planetmint-2.4.6/planetmint/backend/models/input.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/models/metadata.py` & `planetmint-2.4.6/planetmint/backend/models/metadata.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/models/output.py` & `planetmint-2.4.6/planetmint/backend/models/output.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,20 +64,22 @@
     transaction_id: str = ""
     public_keys: List[str] = field(default_factory=list)
     index: int = 0
     condition: Condition = field(default_factory=Condition)
 
     @staticmethod
     def outputs_dict(output: dict, transaction_id: str = "") -> Output:
-        out_dict: Output
-        if output["condition"]["details"].get("subconditions") is None:
-            out_dict = Output.output_with_public_key(output, transaction_id)
-        else:
-            out_dict = Output.output_with_sub_conditions(output, transaction_id)
-        return out_dict
+        return Output(
+            transaction_id=transaction_id,
+            public_keys=output["public_keys"],
+            amount=output["amount"],
+            condition=Condition(
+                uri=output["condition"]["uri"], details=ConditionDetails.from_dict(output["condition"]["details"])
+            ),
+        )
 
     @staticmethod
     def from_tuple(output: tuple) -> Output:
         return Output(
             id=output[0],
             amount=output[1],
             public_keys=output[2],
@@ -106,29 +108,7 @@
             "condition": self.condition.to_dict(),
             "amount": str(self.amount),
         }
 
     @staticmethod
     def list_to_dict(output_list: list[Output]) -> list[dict]:
         return [output.to_dict() for output in output_list or []]
-
-    @staticmethod
-    def output_with_public_key(output, transaction_id) -> Output:
-        return Output(
-            transaction_id=transaction_id,
-            public_keys=output["public_keys"],
-            amount=output["amount"],
-            condition=Condition(
-                uri=output["condition"]["uri"], details=ConditionDetails.from_dict(output["condition"]["details"])
-            ),
-        )
-
-    @staticmethod
-    def output_with_sub_conditions(output, transaction_id) -> Output:
-        return Output(
-            transaction_id=transaction_id,
-            public_keys=output["public_keys"],
-            amount=output["amount"],
-            condition=Condition(
-                uri=output["condition"]["uri"], details=ConditionDetails.from_dict(output["condition"]["details"])
-            ),
-        )
```

### Comparing `planetmint-2.4.5/planetmint/backend/models/script.py` & `planetmint-2.4.6/planetmint/backend/models/script.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/query.py` & `planetmint-2.4.6/planetmint/backend/query.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/schema.py` & `planetmint-2.4.6/planetmint/backend/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/tarantool/const.py` & `planetmint-2.4.6/planetmint/backend/tarantool/const.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/tarantool/opt/init.lua` & `planetmint-2.4.6/planetmint/backend/tarantool/opt/init.lua`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/tarantool/sync_io/connection.py` & `planetmint-2.4.6/planetmint/backend/tarantool/sync_io/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/tarantool/sync_io/query.py` & `planetmint-2.4.6/planetmint/backend/tarantool/sync_io/query.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/tarantool/sync_io/schema.py` & `planetmint-2.4.6/planetmint/backend/tarantool/sync_io/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/tarantool/tarantool.md` & `planetmint-2.4.6/planetmint/backend/tarantool/tarantool.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/backend/utils.py` & `planetmint-2.4.6/planetmint/backend/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/commands/election_types.py` & `planetmint-2.4.6/planetmint/commands/election_types.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/commands/planetmint.py` & `planetmint-2.4.6/planetmint/commands/planetmint.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 from planetmint.application.validator import Validator
 from planetmint.backend import schema
 from planetmint.commands import utils
 from planetmint.commands.utils import configure_planetmint, input_on_stderr
 from planetmint.config_utils import setup_logging
-from planetmint.abci.rpc import MODE_COMMIT, MODE_LIST
+from planetmint.abci.rpc import ABCI_RPC, MODE_COMMIT, MODE_LIST
 from planetmint.abci.utils import load_node_key, public_key_from_base64
 from planetmint.commands.election_types import elections
 from planetmint.version import __tm_supported_versions__
 from planetmint.config import Config
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
@@ -107,22 +107,26 @@
 
 
 @configure_planetmint
 def run_election(args):
     """Initiate and manage elections"""
 
     b = Validator()
+    abci_rpc = ABCI_RPC()
 
-    # Call the function specified by args.action, as defined above
-    globals()[f"run_election_{args.action}"](args, b)
+    if args.action == "show":
+        run_election_show(args, b)
+    else:
+        # Call the function specified by args.action, as defined above
+        globals()[f"run_election_{args.action}"](args, b, abci_rpc)
 
 
-def run_election_new(args, planet):
+def run_election_new(args, planet, abci_rpc):
     election_type = args.election_type.replace("-", "_")
-    globals()[f"run_election_new_{election_type}"](args, planet)
+    globals()[f"run_election_new_{election_type}"](args, planet, abci_rpc)
 
 
 def create_new_election(sk, planet, election_class, data, abci_rpc):
     try:
         key = load_node_key(sk)
         voters = planet.get_recipients_list()
         election = election_class.generate([key.public_key], voters, data, None).sign([key.private_key])
@@ -182,15 +186,15 @@
     :param planet: an instance of Planetmint
     :return: election_id or `False` in case of failure
     """
 
     return create_new_election(args.sk, planet, ChainMigrationElection, [{"data": {}}], abci_rpc)
 
 
-def run_election_approve(args, validator: Validator, abci_rpc):
+def run_election_approve(args, validator: Validator, abci_rpc: ABCI_RPC):
     """Approve an election
 
     :param args: dict
         args = {
         'election_id': the election_id of the election (str)
         'sk': the path to the private key of the signer (str)
         }
```

### Comparing `planetmint-2.4.5/planetmint/commands/utils.py` & `planetmint-2.4.6/planetmint/commands/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/config.py` & `planetmint-2.4.6/planetmint/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,38 +113,34 @@
 
     def get(self):
         return self._private_real_config
 
     def set(self, config):
         self._private_real_config = config
 
-    def get_db_key_map(sefl, db):
-        return sefl.__private_database_keys_map[db]
+    def get_db_key_map(self, db):
+        return self.__private_database_keys_map[db]
 
     def get_db_map(sefl, db):
         return sefl.__private_database_map[db]
 
 
 DEFAULT_LOG_DIR = os.getcwd()
 DEFAULT_LOGGING_CONFIG = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
         "console": {
             "class": "logging.Formatter",
-            "format": (
-                "[%(asctime)s] [%(levelname)s] (%(name)s) " "%(message)s (%(processName)-10s - pid: %(process)d)"
-            ),
+            "format": ("[%(asctime)s] [%(levelname)s] (%(name)s) %(message)s (%(processName)-10s - pid: %(process)d)"),
             "datefmt": "%Y-%m-%d %H:%M:%S",
         },
         "file": {
             "class": "logging.Formatter",
-            "format": (
-                "[%(asctime)s] [%(levelname)s] (%(name)s) " "%(message)s (%(processName)-10s - pid: %(process)d)"
-            ),
+            "format": ("[%(asctime)s] [%(levelname)s] (%(name)s) %(message)s (%(processName)-10s - pid: %(process)d)"),
             "datefmt": "%Y-%m-%d %H:%M:%S",
         },
     },
     "handlers": {
         "console": {
             "class": "logging.StreamHandler",
             "formatter": "console",
```

### Comparing `planetmint-2.4.5/planetmint/config_utils.py` & `planetmint-2.4.6/planetmint/config_utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/ipc/events.py` & `planetmint-2.4.6/planetmint/ipc/events.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/ipc/exchange.py` & `planetmint-2.4.6/planetmint/ipc/exchange.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/model/dataaccessor.py` & `planetmint-2.4.6/planetmint/model/dataaccessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,18 +333,16 @@
         .. important:: The leaves of the tree will need to be sorted in
             some kind of lexicographical order.
 
         Returns:
             str: Merkle root in hexadecimal form.
         """
         utxoset = backend.query.get_unspent_outputs(self.connection)
-        # TODO Once ready, use the already pre-computed utxo_hash field.
         # See common/transactions.py for details.
 
         hashes = [
             sha3_256("{}{}".format(utxo["transaction_id"], utxo["output_index"]).encode()).digest() for utxo in utxoset
         ]
 
         print(sorted(hashes))
 
-        # TODO Notice the sorted call!
         return merkleroot(sorted(hashes))
```

### Comparing `planetmint-2.4.5/planetmint/start.py` & `planetmint-2.4.6/planetmint/start.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © 2020 Interplanetary Database Association e.V.,
 # Planetmint and IPDB software contributors.
 # SPDX-License-Identifier: (Apache-2.0 AND CC-BY-4.0)
 # Code is Apache-2.0 and docs are CC-BY-4.0
 
+import sys
 import logging
 import setproctitle
 
 from planetmint.config import Config
 from planetmint.application.validator import Validator
 from planetmint.abci.application_logic import ApplicationLogic
 from planetmint.abci.parallel_validation import ParallelValidationApp
@@ -90,8 +91,8 @@
         start_abci_server(args)
     else:
         start_web_api(args)
         start_abci_server(args)
 
 
 if __name__ == "__main__":
-    start()
+    start(sys.argv)
```

### Comparing `planetmint-2.4.5/planetmint/utils/lazy.py` & `planetmint-2.4.6/planetmint/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/utils/processes.py` & `planetmint-2.4.6/planetmint/utils/processes.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/routes.py` & `planetmint-2.4.6/planetmint/web/routes.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/server.py` & `planetmint-2.4.6/planetmint/web/server.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/strip_content_type_middleware.py` & `planetmint-2.4.6/planetmint/web/strip_content_type_middleware.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/views/assets.py` & `planetmint-2.4.6/planetmint/web/views/assets.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/views/base.py` & `planetmint-2.4.6/planetmint/web/views/base.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/views/blocks.py` & `planetmint-2.4.6/planetmint/web/views/blocks.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/views/info.py` & `planetmint-2.4.6/planetmint/web/views/info.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/views/metadata.py` & `planetmint-2.4.6/planetmint/web/views/metadata.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/views/outputs.py` & `planetmint-2.4.6/planetmint/web/views/outputs.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/views/parameters.py` & `planetmint-2.4.6/planetmint/web/views/parameters.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/views/transactions.py` & `planetmint-2.4.6/planetmint/web/views/transactions.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/views/validators.py` & `planetmint-2.4.6/planetmint/web/views/validators.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/websocket_dispatcher.py` & `planetmint-2.4.6/planetmint/web/websocket_dispatcher.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/planetmint/web/websocket_server.py` & `planetmint-2.4.6/planetmint/web/websocket_server.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.5/pyproject.toml` & `planetmint-2.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "planetmint"
-version = "2.4.5"
+version = "2.4.6"
 description = "Planetmint: The Blockchain Database"
 authors = ["Planetmint contributors"]
 license = "AGPLv3"
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
@@ -33,15 +33,15 @@
 jsonschema = "4.16.0"
 logstats = "0.3.0"
 packaging = ">=22.0"
 pymongo = "3.11.4"
 tarantool = ">=0.12.1"
 python-rapidjson = ">=1.0"
 pyyaml = "6.0.0"
-requests = "2.25.1"
+requests = "2.31.0"
 setproctitle = "1.2.2"
 werkzeug = "2.0.3"
 nest-asyncio = "1.5.5"
 protobuf = "3.20.2"
 planetmint-ipld = ">=0.0.3"
 pyasn1 = ">=0.4.8"
 python-decouple = "^3.7"
```

### Comparing `planetmint-2.4.5/PKG-INFO` & `planetmint-2.4.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmint
-Version: 2.4.5
+Version: 2.4.6
 Summary: Planetmint: The Blockchain Database
 License: AGPLv3
 Author: Planetmint contributors
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,14 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development
 Requires-Dist: abci (>=0.8.3,<0.9.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asynctnt (>=2.0.1,<3.0.0)
 Requires-Dist: base58 (==2.1.1)
@@ -37,15 +36,15 @@
 Requires-Dist: planetmint-transactions (>=0.8.0)
 Requires-Dist: protobuf (==3.20.2)
 Requires-Dist: pyasn1 (>=0.4.8)
 Requires-Dist: pymongo (==3.11.4)
 Requires-Dist: python-decouple (>=3.7,<4.0)
 Requires-Dist: python-rapidjson (>=1.0)
 Requires-Dist: pyyaml (==6.0.0)
-Requires-Dist: requests (==2.25.1)
+Requires-Dist: requests (==2.31.0)
 Requires-Dist: setproctitle (==1.2.2)
 Requires-Dist: tarantool (>=0.12.1)
 Requires-Dist: werkzeug (==2.0.3)
 Description-Content-Type: text/markdown
 
 <!---
 Copyright © 2020 Interplanetary Database Association e.V.,
```

