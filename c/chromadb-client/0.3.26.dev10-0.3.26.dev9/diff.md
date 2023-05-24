# Comparing `tmp/chromadb-client-0.3.26.dev10.tar.gz` & `tmp/chromadb-client-0.3.26.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb-client-0.3.26.dev10.tar", last modified: Wed May 24 20:41:18 2023, max compression
+gzip compressed data, was "chromadb-client-0.3.26.dev9.tar", last modified: Wed May 24 20:22:06 2023, max compression
```

## Comparing `chromadb-client-0.3.26.dev10.tar` & `chromadb-client-0.3.26.dev9.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.305805 chromadb-client-0.3.26.dev10/
--rw-r--r--   0 hammad     (501) staff       (20)       84 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/.dockerignore
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.280742 chromadb-client-0.3.26.dev10/.github/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.286468 chromadb-client-0.3.26.dev10/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 hammad     (501) staff       (20)     1512 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev10/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 hammad     (501) staff       (20)     1520 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev10/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 hammad     (501) staff       (20)     1384 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev10/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.287181 chromadb-client-0.3.26.dev10/.github/workflows/
--rw-r--r--   0 hammad     (501) staff       (20)     1187 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 hammad     (501) staff       (20)     1338 2023-05-24 20:37:51.000000 chromadb-client-0.3.26.dev10/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 hammad     (501) staff       (20)     4169 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/.github/workflows/chroma-release.yml
--rw-r--r--   0 hammad     (501) staff       (20)     1205 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/.github/workflows/chroma-test.yml
--rw-r--r--   0 hammad     (501) staff       (20)     1734 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 hammad     (501) staff       (20)      228 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/.gitignore
--rw-r--r--   0 hammad     (501) staff       (20)     1030 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/.pre-commit-config.yaml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.287308 chromadb-client-0.3.26.dev10/.vscode/
--rw-r--r--   0 hammad     (501) staff       (20)      978 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/.vscode/settings.json
--rw-r--r--   0 hammad     (501) staff       (20)     3323 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/DEVELOP.md
--rw-r--r--   0 hammad     (501) staff       (20)      619 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/Dockerfile
--rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-02-13 21:59:42.000000 chromadb-client-0.3.26.dev10/LICENSE
--rw-r--r--   0 hammad     (501) staff       (20)     2178 2023-05-24 20:41:18.305652 chromadb-client-0.3.26.dev10/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)     1627 2023-05-24 20:41:15.000000 chromadb-client-0.3.26.dev10/README.md
--rw-r--r--   0 hammad     (501) staff       (20)      619 2023-03-30 18:05:39.000000 chromadb-client-0.3.26.dev10/RELEASE_PROCESS.md
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.288956 chromadb-client-0.3.26.dev10/bin/
--rw-r--r--   0 hammad     (501) staff       (20)     1610 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/bin/backup.sh
--rwxr-xr-x   0 hammad     (501) staff       (20)      110 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev10/bin/build
--rwxr-xr-x   0 hammad     (501) staff       (20)      234 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev10/bin/docker_entrypoint.sh
--rw-r--r--   0 hammad     (501) staff       (20)     6462 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/bin/generate_cloudformation.py
--rwxr-xr-x   0 hammad     (501) staff       (20)      463 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/bin/integration-test
--rw-r--r--   0 hammad     (501) staff       (20)     1688 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/bin/restore.sh
--rw-r--r--   0 hammad     (501) staff       (20)     1105 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/bin/setup_linux.sh
--rw-r--r--   0 hammad     (501) staff       (20)      451 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/bin/setup_mac.sh
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.289081 chromadb-client-0.3.26.dev10/bin/templates/
--rw-r--r--   0 hammad     (501) staff       (20)      985 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev10/bin/templates/docker-compose.yml
--rwxr-xr-x   0 hammad     (501) staff       (20)      451 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev10/bin/test-package.sh
--rwxr-xr-x   0 hammad     (501) staff       (20)      297 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/bin/test-remote
--rw-r--r--   0 hammad     (501) staff       (20)      205 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/bin/test.py
--rwxr-xr-x   0 hammad     (501) staff       (20)      151 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/bin/version
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.289748 chromadb-client-0.3.26.dev10/chromadb/
--rw-r--r--   0 hammad     (501) staff       (20)      895 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.290332 chromadb-client-0.3.26.dev10/chromadb/api/
--rw-r--r--   0 hammad     (501) staff       (20)    10960 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev10/chromadb/api/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)    12141 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev10/chromadb/api/fastapi.py
--rw-r--r--   0 hammad     (501) staff       (20)    17500 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev10/chromadb/api/local.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.290453 chromadb-client-0.3.26.dev10/chromadb/api/models/
--rw-r--r--   0 hammad     (501) staff       (20)    15170 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev10/chromadb/api/models/Collection.py
--rw-r--r--   0 hammad     (501) staff       (20)    10780 2023-05-19 22:52:05.000000 chromadb-client-0.3.26.dev10/chromadb/api/types.py
--rw-r--r--   0 hammad     (501) staff       (20)      168 2023-03-24 17:22:43.000000 chromadb-client-0.3.26.dev10/chromadb/app.py
--rw-r--r--   0 hammad     (501) staff       (20)     4195 2023-05-24 20:12:36.000000 chromadb-client-0.3.26.dev10/chromadb/config.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.291139 chromadb-client-0.3.26.dev10/chromadb/db/
--rw-r--r--   0 hammad     (501) staff       (20)     3260 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/db/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     4816 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev10/chromadb/db/base.py
--rw-r--r--   0 hammad     (501) staff       (20)    21674 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/db/clickhouse.py
--rw-r--r--   0 hammad     (501) staff       (20)    17967 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/db/duckdb.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.291388 chromadb-client-0.3.26.dev10/chromadb/db/impl/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/db/impl/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     4766 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/db/impl/sqlite.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.291636 chromadb-client-0.3.26.dev10/chromadb/db/index/
--rw-r--r--   0 hammad     (501) staff       (20)      447 2023-03-30 18:05:39.000000 chromadb-client-0.3.26.dev10/chromadb/db/index/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)    11060 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev10/chromadb/db/index/hnswlib.py
--rw-r--r--   0 hammad     (501) staff       (20)     8090 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/db/migrations.py
--rw-r--r--   0 hammad     (501) staff       (20)     1293 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev10/chromadb/errors.py
--rw-r--r--   0 hammad     (501) staff       (20)       22 2023-05-24 20:41:15.000000 chromadb-client-0.3.26.dev10/chromadb/is_thin_client.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.291767 chromadb-client-0.3.26.dev10/chromadb/server/
--rw-r--r--   0 hammad     (501) staff       (20)      172 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/chromadb/server/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.292046 chromadb-client-0.3.26.dev10/chromadb/server/fastapi/
--rw-r--r--   0 hammad     (501) staff       (20)     9064 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev10/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     2134 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.292399 chromadb-client-0.3.26.dev10/chromadb/telemetry/
--rw-r--r--   0 hammad     (501) staff       (20)     3165 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/telemetry/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)      591 2023-03-26 23:12:08.000000 chromadb-client-0.3.26.dev10/chromadb/telemetry/events.py
--rw-r--r--   0 hammad     (501) staff       (20)     1083 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.292793 chromadb-client-0.3.26.dev10/chromadb/test/
--rw-r--r--   0 hammad     (501) staff       (20)     3110 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/test/conftest.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.293035 chromadb-client-0.3.26.dev10/chromadb/test/db/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.293814 chromadb-client-0.3.26.dev10/chromadb/test/db/migrations/
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 hammad     (501) staff       (20)     1168 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev10/chromadb/test/db/test_base.py
--rw-r--r--   0 hammad     (501) staff       (20)     4999 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/test/db/test_migrations.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.293936 chromadb-client-0.3.26.dev10/chromadb/test/hnswlib/
--rw-r--r--   0 hammad     (501) staff       (20)     2337 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/test/hnswlib/test_hnswlib.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.295135 chromadb-client-0.3.26.dev10/chromadb/test/property/
--rw-r--r--   0 hammad     (501) staff       (20)     9698 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/chromadb/test/property/invariants.py
--rw-r--r--   0 hammad     (501) staff       (20)    15532 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/chromadb/test/property/strategies.py
--rw-r--r--   0 hammad     (501) staff       (20)     1942 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/chromadb/test/property/test_add.py
--rw-r--r--   0 hammad     (501) staff       (20)     6211 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/test/property/test_collections.py
--rw-r--r--   0 hammad     (501) staff       (20)     8333 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 hammad     (501) staff       (20)     9590 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 hammad     (501) staff       (20)     6297 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/test/property/test_filtering.py
--rw-r--r--   0 hammad     (501) staff       (20)     4899 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/chromadb/test/property/test_persist.py
--rw-r--r--   0 hammad     (501) staff       (20)    40187 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev10/chromadb/test/test_api.py
--rw-r--r--   0 hammad     (501) staff       (20)     2195 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/chromadb/test/test_chroma.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.295379 chromadb-client-0.3.26.dev10/chromadb/utils/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2023-03-25 00:05:13.000000 chromadb-client-0.3.26.dev10/chromadb/utils/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)    16026 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/chromadb/utils/embedding_functions.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.296038 chromadb-client-0.3.26.dev10/chromadb_client.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)     2178 2023-05-24 20:41:18.000000 chromadb-client-0.3.26.dev10/chromadb_client.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)     4875 2023-05-24 20:41:18.000000 chromadb-client-0.3.26.dev10/chromadb_client.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2023-05-24 20:41:18.000000 chromadb-client-0.3.26.dev10/chromadb_client.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)      112 2023-05-24 20:41:18.000000 chromadb-client-0.3.26.dev10/chromadb_client.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)        9 2023-05-24 20:41:18.000000 chromadb-client-0.3.26.dev10/chromadb_client.egg-info/top_level.txt
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.283159 chromadb-client-0.3.26.dev10/clients/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.298271 chromadb-client-0.3.26.dev10/clients/js/
--rw-r--r--   0 hammad     (501) staff       (20)       66 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/.gitignore
--rw-r--r--   0 hammad     (501) staff       (20)       32 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/.prettierignore
--rw-r--r--   0 hammad     (501) staff       (20)        3 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/.prettierrc.json
--rw-r--r--   0 hammad     (501) staff       (20)     1200 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/DEVELOP.md
--rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev10/clients/js/LICENSE
--rw-r--r--   0 hammad     (501) staff       (20)     1266 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/README.md
--rw-r--r--   0 hammad     (501) staff       (20)      324 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/config.yml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.282771 chromadb-client-0.3.26.dev10/clients/js/examples/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.299073 chromadb-client-0.3.26.dev10/clients/js/examples/browser/
--rw-r--r--   0 hammad     (501) staff       (20)      358 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/examples/browser/README.md
--rw-r--r--   0 hammad     (501) staff       (20)     1690 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/examples/browser/app.ts
--rw-r--r--   0 hammad     (501) staff       (20)      834 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/examples/browser/index.html
--rw-r--r--   0 hammad     (501) staff       (20)      409 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/examples/browser/package.json
--rw-r--r--   0 hammad     (501) staff       (20)    71072 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev10/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.299789 chromadb-client-0.3.26.dev10/clients/js/examples/node/
--rw-r--r--   0 hammad     (501) staff       (20)       57 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/examples/node/README.md
--rw-r--r--   0 hammad     (501) staff       (20)     1191 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/examples/node/app.js
--rw-r--r--   0 hammad     (501) staff       (20)    46542 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev10/clients/js/examples/node/package-lock.json
--rw-r--r--   0 hammad     (501) staff       (20)      503 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev10/clients/js/examples/node/package.json
--rw-r--r--   0 hammad     (501) staff       (20)    17116 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev10/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 hammad     (501) staff       (20)     1075 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/genapi.sh
--rw-r--r--   0 hammad     (501) staff       (20)      469 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/jest.config.ts
--rw-r--r--   0 hammad     (501) staff       (20)      153 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev10/clients/js/openapitools.json
--rw-r--r--   0 hammad     (501) staff       (20)   450648 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev10/clients/js/package-lock.json
--rw-r--r--   0 hammad     (501) staff       (20)     1401 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/clients/js/package.json
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.300433 chromadb-client-0.3.26.dev10/clients/js/src/
--rw-r--r--   0 hammad     (501) staff       (20)     8084 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/src/ChromaClient.ts
--rw-r--r--   0 hammad     (501) staff       (20)    19403 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev10/clients/js/src/Collection.ts
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.300901 chromadb-client-0.3.26.dev10/clients/js/src/embeddings/
--rw-r--r--   0 hammad     (501) staff       (20)      937 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 hammad     (501) staff       (20)       91 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 hammad     (501) staff       (20)     1562 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.301787 chromadb-client-0.3.26.dev10/clients/js/src/generated/
--rw-r--r--   0 hammad     (501) staff       (20)      921 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/src/generated/README.md
--rw-r--r--   0 hammad     (501) staff       (20)    56700 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/src/generated/api.ts
--rw-r--r--   0 hammad     (501) staff       (20)     1478 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/src/generated/configuration.ts
--rw-r--r--   0 hammad     (501) staff       (20)      429 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/src/generated/index.ts
--rw-r--r--   0 hammad     (501) staff       (20)     5862 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/src/generated/models.ts
--rw-r--r--   0 hammad     (501) staff       (20)     1307 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/src/generated/runtime.ts
--rw-r--r--   0 hammad     (501) staff       (20)      320 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/src/index.ts
--rw-r--r--   0 hammad     (501) staff       (20)     1719 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/src/types.ts
--rw-r--r--   0 hammad     (501) staff       (20)     2001 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/src/utils.ts
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.303528 chromadb-client-0.3.26.dev10/clients/js/test/
--rw-r--r--   0 hammad     (501) staff       (20)     2625 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/test/add.collections.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     7586 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev10/clients/js/test/client.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     3284 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/test/collection.client.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     2551 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/test/collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)      451 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/test/data.ts
--rw-r--r--   0 hammad     (501) staff       (20)      711 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     2381 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev10/clients/js/test/get.collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)      206 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/test/initClient.ts
--rw-r--r--   0 hammad     (501) staff       (20)      577 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     1990 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev10/clients/js/test/query.collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     2160 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/test/update.collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)      802 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)      367 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/clients/js/tsconfig.json
--rw-r--r--   0 hammad     (501) staff       (20)      110 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/tsconfig.module.json
--rw-r--r--   0 hammad     (501) staff       (20)   157735 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/clients/js/yarn.lock
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.304057 chromadb-client-0.3.26.dev10/clients/python/
--rw-r--r--   0 hammad     (501) staff       (20)     1627 2023-05-24 20:37:51.000000 chromadb-client-0.3.26.dev10/clients/python/README.md
--rwxr-xr-x   0 hammad     (501) staff       (20)     1203 2023-05-24 17:49:03.000000 chromadb-client-0.3.26.dev10/clients/python/build_python_thin_client.sh
--rw-r--r--   0 hammad     (501) staff       (20)       22 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev10/clients/python/is_thin_client.py
--rw-r--r--   0 hammad     (501) staff       (20)     1166 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev10/clients/python/pyproject.toml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.304314 chromadb-client-0.3.26.dev10/config/
--rw-r--r--   0 hammad     (501) staff       (20)      385 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/config/backup_disk.xml
--rw-r--r--   0 hammad     (501) staff       (20)      233 2023-03-06 21:32:56.000000 chromadb-client-0.3.26.dev10/config/chroma_users.xml
--rw-r--r--   0 hammad     (501) staff       (20)     1080 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/docker-compose.server.example.yml
--rw-r--r--   0 hammad     (501) staff       (20)     1230 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/docker-compose.test.yml
--rw-r--r--   0 hammad     (501) staff       (20)     1226 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/docker-compose.yml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.304765 chromadb-client-0.3.26.dev10/examples/
--rw-r--r--   0 hammad     (501) staff       (20)    10346 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/examples/alternative_embeddings.ipynb
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.283488 chromadb-client-0.3.26.dev10/examples/deployments/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:41:18.305431 chromadb-client-0.3.26.dev10/examples/deployments/google-cloud-compute/
--rw-r--r--   0 hammad     (501) staff       (20)      611 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev10/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 hammad     (501) staff       (20)      444 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev10/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 hammad     (501) staff       (20)      125 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev10/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 hammad     (501) staff       (20)     2237 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev10/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 hammad     (501) staff       (20)      181 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev10/examples/deployments/google-cloud-compute/variables.tf
--rw-r--r--   0 hammad     (501) staff       (20)     5830 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev10/examples/local_persistence.ipynb
--rw-r--r--   0 hammad     (501) staff       (20)     5493 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev10/examples/where_filtering.ipynb
--rw-r--r--   0 hammad     (501) staff       (20)      495 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/log_config.yml
--rw-r--r--   0 hammad     (501) staff       (20)      372 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev10/pull_request_template.md
--rw-r--r--   0 hammad     (501) staff       (20)     1166 2023-05-24 20:41:15.000000 chromadb-client-0.3.26.dev10/pyproject.toml
--rw-r--r--   0 hammad     (501) staff       (20)      312 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev10/requirements.txt
--rw-r--r--   0 hammad     (501) staff       (20)      146 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev10/requirements_dev.txt
--rw-r--r--   0 hammad     (501) staff       (20)       38 2023-05-24 20:41:18.305842 chromadb-client-0.3.26.dev10/setup.cfg
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.696671 chromadb-client-0.3.26.dev9/
+-rw-r--r--   0 hammad     (501) staff       (20)       84 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.dockerignore
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.672731 chromadb-client-0.3.26.dev9/.github/
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.678024 chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 hammad     (501) staff       (20)     1512 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 hammad     (501) staff       (20)     1520 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 hammad     (501) staff       (20)     1384 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.678737 chromadb-client-0.3.26.dev9/.github/workflows/
+-rw-r--r--   0 hammad     (501) staff       (20)     1187 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 hammad     (501) staff       (20)     1321 2023-05-24 20:17:49.000000 chromadb-client-0.3.26.dev9/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 hammad     (501) staff       (20)     4169 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.github/workflows/chroma-release.yml
+-rw-r--r--   0 hammad     (501) staff       (20)     1205 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.github/workflows/chroma-test.yml
+-rw-r--r--   0 hammad     (501) staff       (20)     1734 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 hammad     (501) staff       (20)      228 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.gitignore
+-rw-r--r--   0 hammad     (501) staff       (20)     1030 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/.pre-commit-config.yaml
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.678848 chromadb-client-0.3.26.dev9/.vscode/
+-rw-r--r--   0 hammad     (501) staff       (20)      978 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/.vscode/settings.json
+-rw-r--r--   0 hammad     (501) staff       (20)     3323 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/DEVELOP.md
+-rw-r--r--   0 hammad     (501) staff       (20)      619 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/Dockerfile
+-rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-02-13 21:59:42.000000 chromadb-client-0.3.26.dev9/LICENSE
+-rw-r--r--   0 hammad     (501) staff       (20)     2109 2023-05-24 20:22:06.696530 chromadb-client-0.3.26.dev9/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)     1559 2023-05-24 20:22:04.000000 chromadb-client-0.3.26.dev9/README.md
+-rw-r--r--   0 hammad     (501) staff       (20)      619 2023-03-30 18:05:39.000000 chromadb-client-0.3.26.dev9/RELEASE_PROCESS.md
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.680522 chromadb-client-0.3.26.dev9/bin/
+-rw-r--r--   0 hammad     (501) staff       (20)     1610 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/backup.sh
+-rwxr-xr-x   0 hammad     (501) staff       (20)      110 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev9/bin/build
+-rwxr-xr-x   0 hammad     (501) staff       (20)      234 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev9/bin/docker_entrypoint.sh
+-rw-r--r--   0 hammad     (501) staff       (20)     6462 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/generate_cloudformation.py
+-rwxr-xr-x   0 hammad     (501) staff       (20)      463 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/integration-test
+-rw-r--r--   0 hammad     (501) staff       (20)     1688 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/restore.sh
+-rw-r--r--   0 hammad     (501) staff       (20)     1105 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/setup_linux.sh
+-rw-r--r--   0 hammad     (501) staff       (20)      451 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/setup_mac.sh
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.680657 chromadb-client-0.3.26.dev9/bin/templates/
+-rw-r--r--   0 hammad     (501) staff       (20)      985 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev9/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 hammad     (501) staff       (20)      451 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev9/bin/test-package.sh
+-rwxr-xr-x   0 hammad     (501) staff       (20)      297 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/test-remote
+-rw-r--r--   0 hammad     (501) staff       (20)      205 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/test.py
+-rwxr-xr-x   0 hammad     (501) staff       (20)      151 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/version
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.681349 chromadb-client-0.3.26.dev9/chromadb/
+-rw-r--r--   0 hammad     (501) staff       (20)      895 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.681899 chromadb-client-0.3.26.dev9/chromadb/api/
+-rw-r--r--   0 hammad     (501) staff       (20)    10960 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/chromadb/api/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)    12141 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/chromadb/api/fastapi.py
+-rw-r--r--   0 hammad     (501) staff       (20)    17500 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/chromadb/api/local.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.682050 chromadb-client-0.3.26.dev9/chromadb/api/models/
+-rw-r--r--   0 hammad     (501) staff       (20)    15170 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/chromadb/api/models/Collection.py
+-rw-r--r--   0 hammad     (501) staff       (20)    10780 2023-05-19 22:52:05.000000 chromadb-client-0.3.26.dev9/chromadb/api/types.py
+-rw-r--r--   0 hammad     (501) staff       (20)      168 2023-03-24 17:22:43.000000 chromadb-client-0.3.26.dev9/chromadb/app.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4195 2023-05-24 20:12:36.000000 chromadb-client-0.3.26.dev9/chromadb/config.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.682700 chromadb-client-0.3.26.dev9/chromadb/db/
+-rw-r--r--   0 hammad     (501) staff       (20)     3260 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/db/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4816 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/chromadb/db/base.py
+-rw-r--r--   0 hammad     (501) staff       (20)    21674 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/db/clickhouse.py
+-rw-r--r--   0 hammad     (501) staff       (20)    17967 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/db/duckdb.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.682968 chromadb-client-0.3.26.dev9/chromadb/db/impl/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/db/impl/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4766 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/db/impl/sqlite.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.683233 chromadb-client-0.3.26.dev9/chromadb/db/index/
+-rw-r--r--   0 hammad     (501) staff       (20)      447 2023-03-30 18:05:39.000000 chromadb-client-0.3.26.dev9/chromadb/db/index/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)    11060 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/chromadb/db/index/hnswlib.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8090 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/db/migrations.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1293 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/chromadb/errors.py
+-rw-r--r--   0 hammad     (501) staff       (20)       22 2023-05-24 20:22:04.000000 chromadb-client-0.3.26.dev9/chromadb/is_thin_client.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.683372 chromadb-client-0.3.26.dev9/chromadb/server/
+-rw-r--r--   0 hammad     (501) staff       (20)      172 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/server/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.683618 chromadb-client-0.3.26.dev9/chromadb/server/fastapi/
+-rw-r--r--   0 hammad     (501) staff       (20)     9064 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2134 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.683982 chromadb-client-0.3.26.dev9/chromadb/telemetry/
+-rw-r--r--   0 hammad     (501) staff       (20)     3165 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/telemetry/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)      591 2023-03-26 23:12:08.000000 chromadb-client-0.3.26.dev9/chromadb/telemetry/events.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1083 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.684399 chromadb-client-0.3.26.dev9/chromadb/test/
+-rw-r--r--   0 hammad     (501) staff       (20)     3110 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/conftest.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.684654 chromadb-client-0.3.26.dev9/chromadb/test/db/
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.685436 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 hammad     (501) staff       (20)     1168 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/test_base.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4999 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/test_migrations.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.685555 chromadb-client-0.3.26.dev9/chromadb/test/hnswlib/
+-rw-r--r--   0 hammad     (501) staff       (20)     2337 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/hnswlib/test_hnswlib.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.686491 chromadb-client-0.3.26.dev9/chromadb/test/property/
+-rw-r--r--   0 hammad     (501) staff       (20)     9698 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/invariants.py
+-rw-r--r--   0 hammad     (501) staff       (20)    15532 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/strategies.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1942 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_add.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6211 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_collections.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8333 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 hammad     (501) staff       (20)     9590 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6297 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4899 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_persist.py
+-rw-r--r--   0 hammad     (501) staff       (20)    40187 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/chromadb/test/test_api.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2195 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/test_chroma.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.686711 chromadb-client-0.3.26.dev9/chromadb/utils/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2023-03-25 00:05:13.000000 chromadb-client-0.3.26.dev9/chromadb/utils/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)    16026 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/utils/embedding_functions.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.687353 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)     2109 2023-05-24 20:22:06.000000 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)     4875 2023-05-24 20:22:06.000000 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2023-05-24 20:22:06.000000 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)      112 2023-05-24 20:22:06.000000 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        9 2023-05-24 20:22:06.000000 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/top_level.txt
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.675142 chromadb-client-0.3.26.dev9/clients/
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.689580 chromadb-client-0.3.26.dev9/clients/js/
+-rw-r--r--   0 hammad     (501) staff       (20)       66 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/.gitignore
+-rw-r--r--   0 hammad     (501) staff       (20)       32 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/.prettierignore
+-rw-r--r--   0 hammad     (501) staff       (20)        3 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/.prettierrc.json
+-rw-r--r--   0 hammad     (501) staff       (20)     1200 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/DEVELOP.md
+-rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/LICENSE
+-rw-r--r--   0 hammad     (501) staff       (20)     1266 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/README.md
+-rw-r--r--   0 hammad     (501) staff       (20)      324 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/config.yml
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.674574 chromadb-client-0.3.26.dev9/clients/js/examples/
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.690307 chromadb-client-0.3.26.dev9/clients/js/examples/browser/
+-rw-r--r--   0 hammad     (501) staff       (20)      358 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/examples/browser/README.md
+-rw-r--r--   0 hammad     (501) staff       (20)     1690 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/examples/browser/app.ts
+-rw-r--r--   0 hammad     (501) staff       (20)      834 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/examples/browser/index.html
+-rw-r--r--   0 hammad     (501) staff       (20)      409 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/examples/browser/package.json
+-rw-r--r--   0 hammad     (501) staff       (20)    71072 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.690946 chromadb-client-0.3.26.dev9/clients/js/examples/node/
+-rw-r--r--   0 hammad     (501) staff       (20)       57 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/examples/node/README.md
+-rw-r--r--   0 hammad     (501) staff       (20)     1191 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/examples/node/app.js
+-rw-r--r--   0 hammad     (501) staff       (20)    46542 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/examples/node/package-lock.json
+-rw-r--r--   0 hammad     (501) staff       (20)      503 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/examples/node/package.json
+-rw-r--r--   0 hammad     (501) staff       (20)    17116 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 hammad     (501) staff       (20)     1075 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/genapi.sh
+-rw-r--r--   0 hammad     (501) staff       (20)      469 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/jest.config.ts
+-rw-r--r--   0 hammad     (501) staff       (20)      153 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/openapitools.json
+-rw-r--r--   0 hammad     (501) staff       (20)   450648 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/package-lock.json
+-rw-r--r--   0 hammad     (501) staff       (20)     1401 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/clients/js/package.json
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.691580 chromadb-client-0.3.26.dev9/clients/js/src/
+-rw-r--r--   0 hammad     (501) staff       (20)     8084 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 hammad     (501) staff       (20)    19403 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/clients/js/src/Collection.ts
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.692004 chromadb-client-0.3.26.dev9/clients/js/src/embeddings/
+-rw-r--r--   0 hammad     (501) staff       (20)      937 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 hammad     (501) staff       (20)       91 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     1562 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.692839 chromadb-client-0.3.26.dev9/clients/js/src/generated/
+-rw-r--r--   0 hammad     (501) staff       (20)      921 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/README.md
+-rw-r--r--   0 hammad     (501) staff       (20)    56700 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/api.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     1478 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 hammad     (501) staff       (20)      429 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/index.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     5862 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/models.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     1307 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 hammad     (501) staff       (20)      320 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/index.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     1719 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/types.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     2001 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/utils.ts
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.694569 chromadb-client-0.3.26.dev9/clients/js/test/
+-rw-r--r--   0 hammad     (501) staff       (20)     2625 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     7586 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/clients/js/test/client.test.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     3284 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     2551 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/collection.test.ts
+-rw-r--r--   0 hammad     (501) staff       (20)      451 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/test/data.ts
+-rw-r--r--   0 hammad     (501) staff       (20)      711 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     2381 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 hammad     (501) staff       (20)      206 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/initClient.ts
+-rw-r--r--   0 hammad     (501) staff       (20)      577 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     1990 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 hammad     (501) staff       (20)     2160 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 hammad     (501) staff       (20)      802 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 hammad     (501) staff       (20)      367 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/tsconfig.json
+-rw-r--r--   0 hammad     (501) staff       (20)      110 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/tsconfig.module.json
+-rw-r--r--   0 hammad     (501) staff       (20)   157735 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/yarn.lock
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.695065 chromadb-client-0.3.26.dev9/clients/python/
+-rw-r--r--   0 hammad     (501) staff       (20)     1559 2023-05-24 17:49:30.000000 chromadb-client-0.3.26.dev9/clients/python/README.md
+-rwxr-xr-x   0 hammad     (501) staff       (20)     1203 2023-05-24 17:49:03.000000 chromadb-client-0.3.26.dev9/clients/python/build_python_thin_client.sh
+-rw-r--r--   0 hammad     (501) staff       (20)       22 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/clients/python/is_thin_client.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1166 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/clients/python/pyproject.toml
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.695292 chromadb-client-0.3.26.dev9/config/
+-rw-r--r--   0 hammad     (501) staff       (20)      385 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/config/backup_disk.xml
+-rw-r--r--   0 hammad     (501) staff       (20)      233 2023-03-06 21:32:56.000000 chromadb-client-0.3.26.dev9/config/chroma_users.xml
+-rw-r--r--   0 hammad     (501) staff       (20)     1080 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/docker-compose.server.example.yml
+-rw-r--r--   0 hammad     (501) staff       (20)     1230 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/docker-compose.test.yml
+-rw-r--r--   0 hammad     (501) staff       (20)     1226 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/docker-compose.yml
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.695694 chromadb-client-0.3.26.dev9/examples/
+-rw-r--r--   0 hammad     (501) staff       (20)    10346 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/examples/alternative_embeddings.ipynb
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.675509 chromadb-client-0.3.26.dev9/examples/deployments/
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.696348 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 hammad     (501) staff       (20)      611 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 hammad     (501) staff       (20)      444 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 hammad     (501) staff       (20)      125 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 hammad     (501) staff       (20)     2237 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 hammad     (501) staff       (20)      181 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/variables.tf
+-rw-r--r--   0 hammad     (501) staff       (20)     5830 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/examples/local_persistence.ipynb
+-rw-r--r--   0 hammad     (501) staff       (20)     5493 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/examples/where_filtering.ipynb
+-rw-r--r--   0 hammad     (501) staff       (20)      495 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/log_config.yml
+-rw-r--r--   0 hammad     (501) staff       (20)      372 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/pull_request_template.md
+-rw-r--r--   0 hammad     (501) staff       (20)     1166 2023-05-24 20:22:04.000000 chromadb-client-0.3.26.dev9/pyproject.toml
+-rw-r--r--   0 hammad     (501) staff       (20)      312 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/requirements.txt
+-rw-r--r--   0 hammad     (501) staff       (20)      146 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/requirements_dev.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2023-05-24 20:22:06.696710 chromadb-client-0.3.26.dev9/setup.cfg
```

### Comparing `chromadb-client-0.3.26.dev10/.github/ISSUE_TEMPLATE/bug_report.yaml` & `chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/.github/ISSUE_TEMPLATE/feature_request.yaml` & `chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/.github/workflows/chroma-integration-test.yml` & `chromadb-client-0.3.26.dev9/.github/workflows/chroma-integration-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/.github/workflows/chroma-release-python-client.yml` & `chromadb-client-0.3.26.dev9/.github/workflows/chroma-release-python-client.yml`

 * *Files 5% similar despite different names*

```diff
@@ -38,8 +38,8 @@
       with:
         password: ${{ secrets.TEST_PYPI_PYTHON_CLIENT_PUBLISH_KEY }}
         repository_url: https://test.pypi.org/legacy/
     - name: Publish to PyPI
       if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
-        password: ${{ secrets.PYPI_PYTHON_CLIENT_PUBLISH_KEY }}
+        password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `chromadb-client-0.3.26.dev10/.github/workflows/chroma-release.yml` & `chromadb-client-0.3.26.dev9/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/.github/workflows/chroma-test.yml` & `chromadb-client-0.3.26.dev9/.github/workflows/chroma-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/.github/workflows/pr-review-checklist.yml` & `chromadb-client-0.3.26.dev9/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/.pre-commit-config.yaml` & `chromadb-client-0.3.26.dev9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/.vscode/settings.json` & `chromadb-client-0.3.26.dev9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/DEVELOP.md` & `chromadb-client-0.3.26.dev9/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/Dockerfile` & `chromadb-client-0.3.26.dev9/Dockerfile`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/LICENSE` & `chromadb-client-0.3.26.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/PKG-INFO` & `chromadb-client-0.3.26.dev9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb-client
-Version: 0.3.26.dev10
+Version: 0.3.26.dev9
 Summary: Chroma Client.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -28,17 +28,15 @@
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest",
-                                  chroma_server_host="localhost",
-                                  chroma_server_port=8000))
+client = chromadb.Client(Settings(chroma_api_impl="rest", chroma_server_host="localhost", chroma_server_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.26.dev10 Summary:
+Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.26.dev9 Summary:
 Chroma Client. Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-client-0.3.26.dev10/README.md` & `chromadb-client-0.3.26.dev9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest",
-                                  chroma_server_host="localhost",
-                                  chroma_server_port=8000))
+client = chromadb.Client(Settings(chroma_api_impl="rest", chroma_server_host="localhost", chroma_server_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

### Comparing `chromadb-client-0.3.26.dev10/RELEASE_PROCESS.md` & `chromadb-client-0.3.26.dev9/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/bin/backup.sh` & `chromadb-client-0.3.26.dev9/bin/backup.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/bin/generate_cloudformation.py` & `chromadb-client-0.3.26.dev9/bin/generate_cloudformation.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/bin/restore.sh` & `chromadb-client-0.3.26.dev9/bin/restore.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/bin/setup_linux.sh` & `chromadb-client-0.3.26.dev9/bin/setup_linux.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/bin/templates/docker-compose.yml` & `chromadb-client-0.3.26.dev9/bin/templates/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/__init__.py` & `chromadb-client-0.3.26.dev9/chromadb/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/api/__init__.py` & `chromadb-client-0.3.26.dev9/chromadb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/api/fastapi.py` & `chromadb-client-0.3.26.dev9/chromadb/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/api/local.py` & `chromadb-client-0.3.26.dev9/chromadb/api/local.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/api/models/Collection.py` & `chromadb-client-0.3.26.dev9/chromadb/api/models/Collection.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/api/types.py` & `chromadb-client-0.3.26.dev9/chromadb/api/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/config.py` & `chromadb-client-0.3.26.dev9/chromadb/config.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/db/__init__.py` & `chromadb-client-0.3.26.dev9/chromadb/db/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/db/base.py` & `chromadb-client-0.3.26.dev9/chromadb/db/base.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/db/clickhouse.py` & `chromadb-client-0.3.26.dev9/chromadb/db/clickhouse.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/db/duckdb.py` & `chromadb-client-0.3.26.dev9/chromadb/db/duckdb.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/db/impl/sqlite.py` & `chromadb-client-0.3.26.dev9/chromadb/db/impl/sqlite.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/db/index/hnswlib.py` & `chromadb-client-0.3.26.dev9/chromadb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/db/migrations.py` & `chromadb-client-0.3.26.dev9/chromadb/db/migrations.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/errors.py` & `chromadb-client-0.3.26.dev9/chromadb/errors.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/server/fastapi/__init__.py` & `chromadb-client-0.3.26.dev9/chromadb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/server/fastapi/types.py` & `chromadb-client-0.3.26.dev9/chromadb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/telemetry/__init__.py` & `chromadb-client-0.3.26.dev9/chromadb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/telemetry/events.py` & `chromadb-client-0.3.26.dev9/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/telemetry/posthog.py` & `chromadb-client-0.3.26.dev9/chromadb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/conftest.py` & `chromadb-client-0.3.26.dev9/chromadb/test/conftest.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/db/test_base.py` & `chromadb-client-0.3.26.dev9/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/db/test_migrations.py` & `chromadb-client-0.3.26.dev9/chromadb/test/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/hnswlib/test_hnswlib.py` & `chromadb-client-0.3.26.dev9/chromadb/test/hnswlib/test_hnswlib.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/property/invariants.py` & `chromadb-client-0.3.26.dev9/chromadb/test/property/invariants.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/property/strategies.py` & `chromadb-client-0.3.26.dev9/chromadb/test/property/strategies.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/property/test_add.py` & `chromadb-client-0.3.26.dev9/chromadb/test/property/test_add.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/property/test_collections.py` & `chromadb-client-0.3.26.dev9/chromadb/test/property/test_collections.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/property/test_cross_version_persist.py` & `chromadb-client-0.3.26.dev9/chromadb/test/property/test_cross_version_persist.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/property/test_embeddings.py` & `chromadb-client-0.3.26.dev9/chromadb/test/property/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/property/test_filtering.py` & `chromadb-client-0.3.26.dev9/chromadb/test/property/test_filtering.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/property/test_persist.py` & `chromadb-client-0.3.26.dev9/chromadb/test/property/test_persist.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/test_api.py` & `chromadb-client-0.3.26.dev9/chromadb/test/test_api.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/test/test_chroma.py` & `chromadb-client-0.3.26.dev9/chromadb/test/test_chroma.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb/utils/embedding_functions.py` & `chromadb-client-0.3.26.dev9/chromadb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/chromadb_client.egg-info/PKG-INFO` & `chromadb-client-0.3.26.dev9/chromadb_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb-client
-Version: 0.3.26.dev10
+Version: 0.3.26.dev9
 Summary: Chroma Client.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -28,17 +28,15 @@
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest",
-                                  chroma_server_host="localhost",
-                                  chroma_server_port=8000))
+client = chromadb.Client(Settings(chroma_api_impl="rest", chroma_server_host="localhost", chroma_server_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.26.dev10 Summary:
+Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.26.dev9 Summary:
 Chroma Client. Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-client-0.3.26.dev10/chromadb_client.egg-info/SOURCES.txt` & `chromadb-client-0.3.26.dev9/chromadb_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/DEVELOP.md` & `chromadb-client-0.3.26.dev9/clients/js/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/LICENSE` & `chromadb-client-0.3.26.dev9/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/README.md` & `chromadb-client-0.3.26.dev9/clients/js/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/examples/browser/app.ts` & `chromadb-client-0.3.26.dev9/clients/js/examples/browser/app.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/examples/browser/index.html` & `chromadb-client-0.3.26.dev9/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/examples/browser/yarn.lock` & `chromadb-client-0.3.26.dev9/clients/js/examples/browser/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/examples/node/app.js` & `chromadb-client-0.3.26.dev9/clients/js/examples/node/app.js`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/examples/node/package-lock.json` & `chromadb-client-0.3.26.dev9/clients/js/examples/node/package-lock.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/examples/node/yarn.lock` & `chromadb-client-0.3.26.dev9/clients/js/examples/node/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/genapi.sh` & `chromadb-client-0.3.26.dev9/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/package-lock.json` & `chromadb-client-0.3.26.dev9/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/package.json` & `chromadb-client-0.3.26.dev9/clients/js/package.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/src/ChromaClient.ts` & `chromadb-client-0.3.26.dev9/clients/js/src/ChromaClient.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/src/Collection.ts` & `chromadb-client-0.3.26.dev9/clients/js/src/Collection.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `chromadb-client-0.3.26.dev9/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `chromadb-client-0.3.26.dev9/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/src/generated/README.md` & `chromadb-client-0.3.26.dev9/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/src/generated/api.ts` & `chromadb-client-0.3.26.dev9/clients/js/src/generated/api.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/src/generated/configuration.ts` & `chromadb-client-0.3.26.dev9/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/src/generated/models.ts` & `chromadb-client-0.3.26.dev9/clients/js/src/generated/models.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/src/generated/runtime.ts` & `chromadb-client-0.3.26.dev9/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/src/types.ts` & `chromadb-client-0.3.26.dev9/clients/js/src/types.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/src/utils.ts` & `chromadb-client-0.3.26.dev9/clients/js/src/utils.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/test/add.collections.test.ts` & `chromadb-client-0.3.26.dev9/clients/js/test/add.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/test/client.test.ts` & `chromadb-client-0.3.26.dev9/clients/js/test/client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/test/collection.client.test.ts` & `chromadb-client-0.3.26.dev9/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/test/collection.test.ts` & `chromadb-client-0.3.26.dev9/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/test/delete.collection.test.ts` & `chromadb-client-0.3.26.dev9/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/test/get.collection.test.ts` & `chromadb-client-0.3.26.dev9/clients/js/test/get.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/test/peek.collection.test.ts` & `chromadb-client-0.3.26.dev9/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/test/query.collection.test.ts` & `chromadb-client-0.3.26.dev9/clients/js/test/query.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/test/update.collection.test.ts` & `chromadb-client-0.3.26.dev9/clients/js/test/update.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/test/upsert.collections.test.ts` & `chromadb-client-0.3.26.dev9/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/js/yarn.lock` & `chromadb-client-0.3.26.dev9/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/python/README.md` & `chromadb-client-0.3.26.dev9/clients/python/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest",
-                                  chroma_server_host="localhost",
-                                  chroma_server_port=8000))
+client = chromadb.Client(Settings(chroma_api_impl="rest", chroma_server_host="localhost", chroma_server_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

### Comparing `chromadb-client-0.3.26.dev10/clients/python/build_python_thin_client.sh` & `chromadb-client-0.3.26.dev9/clients/python/build_python_thin_client.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/clients/python/pyproject.toml` & `chromadb-client-0.3.26.dev9/clients/python/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/docker-compose.server.example.yml` & `chromadb-client-0.3.26.dev9/docker-compose.server.example.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/docker-compose.test.yml` & `chromadb-client-0.3.26.dev9/docker-compose.test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/docker-compose.yml` & `chromadb-client-0.3.26.dev9/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/examples/alternative_embeddings.ipynb` & `chromadb-client-0.3.26.dev9/examples/alternative_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/examples/deployments/google-cloud-compute/README.md` & `chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/examples/deployments/google-cloud-compute/startup.sh` & `chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/startup.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/examples/local_persistence.ipynb` & `chromadb-client-0.3.26.dev9/examples/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/examples/where_filtering.ipynb` & `chromadb-client-0.3.26.dev9/examples/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev10/pyproject.toml` & `chromadb-client-0.3.26.dev9/pyproject.toml`

 * *Files identical despite different names*

