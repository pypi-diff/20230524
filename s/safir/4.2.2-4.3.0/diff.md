# Comparing `tmp/safir-4.2.2.tar.gz` & `tmp/safir-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safir-4.2.2.tar", last modified: Wed May 17 22:55:47 2023, max compression
+gzip compressed data, was "safir-4.3.0.tar", last modified: Tue May 23 23:05:04 2023, max compression
```

## Comparing `safir-4.2.2.tar` & `safir-4.3.0.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.243249 safir-4.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 22:55:35.000000 safir-4.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-17 22:55:35.000000 safir-4.2.2/.github/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-17 22:55:35.000000 safir-4.2.2/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-17 22:55:35.000000 safir-4.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 22:55:35.000000 safir-4.2.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-17 22:55:35.000000 safir-4.2.2/.github/workflows/periodic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-17 22:55:35.000000 safir-4.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-17 22:55:35.000000 safir-4.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-17 22:55:35.000000 safir-4.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 22:55:35.000000 safir-4.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-17 22:55:35.000000 safir-4.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-17 22:55:47.243249 safir-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-17 22:55:35.000000 safir-4.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 22:55:35.000000 safir-4.2.2/changelog.d/_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-17 22:55:35.000000 safir-4.2.2/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-17 22:55:35.000000 safir-4.2.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-17 22:55:35.000000 safir-4.2.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 22:55:35.000000 safir-4.2.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.231248 safir-4.2.2/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-17 22:55:35.000000 safir-4.2.2/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 22:55:35.000000 safir-4.2.2/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-17 22:55:35.000000 safir-4.2.2/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-17 22:55:35.000000 safir-4.2.2/docs/documenteer.toml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-17 22:55:35.000000 safir-4.2.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.231248 safir-4.2.2/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/arq.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/datetime.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/fastapi-errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/gafaelfawr.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/gcs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.231248 safir-4.2.2/docs/user-guide/github-apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/github-apps/api-resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/github-apps/create-a-github-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/github-apps/handling-webhooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/github-apps/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/github-apps/webhook-models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/http-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/ivoa.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/kubernetes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/pydantic-redis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/pydantic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/set-up-from-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/slack-webhook.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/uvicorn.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/x-forwarded.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-17 22:55:35.000000 safir-4.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:55:47.243249 safir-4.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/db_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/gafaelfawr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/github/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/github/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/github/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/github/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/middleware/ivoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/middleware/x_forwarded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/slack/blockkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/slack/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/testing/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    74785 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/testing/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/testing/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/testing/uvicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-17 22:55:47.000000 safir-4.2.2/src/safir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-17 22:55:47.000000 safir-4.2.2/src/safir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:55:47.000000 safir-4.2.2/src/safir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-17 22:55:47.000000 safir-4.2.2/src/safir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 22:55:47.000000 safir-4.2.2/src/safir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-17 22:55:35.000000 safir-4.2.2/tests/asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 22:55:35.000000 safir-4.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-17 22:55:35.000000 safir-4.2.2/tests/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-17 22:55:35.000000 safir-4.2.2/tests/datetime_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/arq_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/db_session_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/gafaelfawr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/http_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/logger_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-17 22:55:35.000000 safir-4.2.2/tests/fastapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-17 22:55:35.000000 safir-4.2.2/tests/gcs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/tests/github/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/github/data/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/check_run_created.json
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/check_suite_completed.json
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/installation.json
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/installation_repositories.json
--rw-r--r--   0 runner    (1001) docker     (123)    26334 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/pull_request_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/push_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/webhooks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-17 22:55:35.000000 safir-4.2.2/tests/kubernetes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-05-17 22:55:35.000000 safir-4.2.2/tests/logging_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-17 22:55:35.000000 safir-4.2.2/tests/metadata_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-17 22:55:35.000000 safir-4.2.2/tests/middleware/ivoa_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-17 22:55:35.000000 safir-4.2.2/tests/middleware/x_forwarded_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-17 22:55:35.000000 safir-4.2.2/tests/models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-17 22:55:35.000000 safir-4.2.2/tests/pydantic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-17 22:55:35.000000 safir-4.2.2/tests/redis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-17 22:55:35.000000 safir-4.2.2/tests/safir_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-17 22:55:35.000000 safir-4.2.2/tests/slack/blockkit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-17 22:55:35.000000 safir-4.2.2/tests/slack/webhook_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-17 22:55:35.000000 safir-4.2.2/tests/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-17 22:55:35.000000 safir-4.2.2/tests/testing/gcs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-17 22:55:35.000000 safir-4.2.2/tests/testing/kubernetes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-17 22:55:35.000000 safir-4.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-23 23:04:52.000000 safir-4.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.433803 safir-4.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-23 23:04:52.000000 safir-4.3.0/.github/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-23 23:04:52.000000 safir-4.3.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-23 23:04:52.000000 safir-4.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.433803 safir-4.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-23 23:04:52.000000 safir-4.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-23 23:04:52.000000 safir-4.3.0/.github/workflows/periodic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-23 23:04:52.000000 safir-4.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-23 23:04:52.000000 safir-4.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-05-23 23:04:52.000000 safir-4.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-23 23:04:52.000000 safir-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 23:04:52.000000 safir-4.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-23 23:05:04.445803 safir-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-23 23:04:52.000000 safir-4.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.433803 safir-4.3.0/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 23:04:52.000000 safir-4.3.0/changelog.d/_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.437803 safir-4.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 23:04:52.000000 safir-4.3.0/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-23 23:04:52.000000 safir-4.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-05-23 23:04:52.000000 safir-4.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-23 23:04:52.000000 safir-4.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.437803 safir-4.3.0/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-23 23:04:52.000000 safir-4.3.0/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 23:04:52.000000 safir-4.3.0/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-23 23:04:52.000000 safir-4.3.0/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-23 23:04:52.000000 safir-4.3.0/docs/documenteer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-23 23:04:52.000000 safir-4.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.437803 safir-4.3.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/arq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/datetime.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/fastapi-errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/gafaelfawr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/gcs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.437803 safir-4.3.0/docs/user-guide/github-apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/github-apps/api-resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/github-apps/create-a-github-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/github-apps/handling-webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/github-apps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/github-apps/webhook-models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/http-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/ivoa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/kubernetes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/pydantic-redis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/pydantic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/set-up-from-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/slack-webhook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/uvicorn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/x-forwarded.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-23 23:04:52.000000 safir-4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 23:05:04.445803 safir-4.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.433803 safir-4.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/db_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/gafaelfawr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/github/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/github/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/github/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/middleware/ivoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/middleware/x_forwarded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/slack/blockkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/slack/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/testing/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77235 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/testing/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/testing/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/testing/uvicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-23 23:05:04.000000 safir-4.3.0/src/safir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-23 23:05:04.000000 safir-4.3.0/src/safir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:05:04.000000 safir-4.3.0/src/safir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-23 23:05:04.000000 safir-4.3.0/src/safir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 23:05:04.000000 safir-4.3.0/src/safir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-23 23:04:52.000000 safir-4.3.0/tests/asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-23 23:04:52.000000 safir-4.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-23 23:04:52.000000 safir-4.3.0/tests/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-23 23:04:52.000000 safir-4.3.0/tests/datetime_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/arq_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/db_session_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/gafaelfawr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/http_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-23 23:04:52.000000 safir-4.3.0/tests/fastapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-23 23:04:52.000000 safir-4.3.0/tests/gcs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.433803 safir-4.3.0/tests/github/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/github/data/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/check_run_created.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/check_suite_completed.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/installation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/installation_repositories.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26334 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/pull_request_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/push_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/webhooks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-23 23:04:52.000000 safir-4.3.0/tests/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-05-23 23:04:52.000000 safir-4.3.0/tests/logging_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-23 23:04:52.000000 safir-4.3.0/tests/metadata_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-23 23:04:52.000000 safir-4.3.0/tests/middleware/ivoa_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-23 23:04:52.000000 safir-4.3.0/tests/middleware/x_forwarded_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-23 23:04:52.000000 safir-4.3.0/tests/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-23 23:04:52.000000 safir-4.3.0/tests/pydantic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-23 23:04:52.000000 safir-4.3.0/tests/redis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 23:04:52.000000 safir-4.3.0/tests/safir_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-23 23:04:52.000000 safir-4.3.0/tests/slack/blockkit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-23 23:04:52.000000 safir-4.3.0/tests/slack/webhook_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-23 23:04:52.000000 safir-4.3.0/tests/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-23 23:04:52.000000 safir-4.3.0/tests/testing/gcs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-05-23 23:04:52.000000 safir-4.3.0/tests/testing/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-23 23:04:52.000000 safir-4.3.0/tox.ini
```

### Comparing `safir-4.2.2/.github/workflows/ci.yaml` & `safir-4.3.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/.github/workflows/periodic.yaml` & `safir-4.3.0/.github/workflows/periodic.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/.gitignore` & `safir-4.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/.pre-commit-config.yaml` & `safir-4.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/CHANGELOG.md` & `safir-4.3.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 Versioning follows [semver](https://semver.org/).
 
 This project uses [scriv](https://scriv.readthedocs.io/en/stable/) to maintain the change log.
 Changes for the upcoming release can be found in [changelog.d](https://github.com/lsst-sqre/safir/tree/main/changelog.d/).
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-4.3.0'></a>
+## 4.3.0 (2023-05-23)
+
+### New features
+
+- All `delete_*` APIs in the mock Kubernetes API now support `grace_period_seconds` and a `V1DeleteOptions` body. Both are ignored.
+- `delete_namespaced_job` in the mock Kubernetes API now requires `propagation_policy` to be passed as a keyword argument if provided, and does not require it be set. It is validated against the values recognized by Kubernetes, and if set to `Orphan`, pods created by the job are not deleted.
+
+### Bug fixes
+
+- When reporting an error response to Slack using `SlackWebException`, put the response body in an attachment instead of a regular block, since it may be a full HTML error page. An attachment tells Slack to hide long content by default unless the viewer expands it.
+
 <a id='changelog-4.2.2'></a>
 ## 4.2.2 (2023-05-17)
 
 ### Bug fixes
 
 - Revert the documentation change in 4.2.1 to restore cross-references, since the docs-linkcheck failure appears to be a false positive.
```

### Comparing `safir-4.2.2/LICENSE` & `safir-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/PKG-INFO` & `safir-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 4.2.2
+Version: 4.3.0
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `safir-4.2.2/README.md` & `safir-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/_rst_epilog.rst` & `safir-4.3.0/docs/_rst_epilog.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/api.rst` & `safir-4.3.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/changelog.md` & `safir-4.3.0/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 Versioning follows [semver](https://semver.org/).
 
 This project uses [scriv](https://scriv.readthedocs.io/en/stable/) to maintain the change log.
 Changes for the upcoming release can be found in [changelog.d](https://github.com/lsst-sqre/safir/tree/main/changelog.d/).
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-4.3.0'></a>
+## 4.3.0 (2023-05-23)
+
+### New features
+
+- All `delete_*` APIs in the mock Kubernetes API now support `grace_period_seconds` and a `V1DeleteOptions` body. Both are ignored.
+- `delete_namespaced_job` in the mock Kubernetes API now requires `propagation_policy` to be passed as a keyword argument if provided, and does not require it be set. It is validated against the values recognized by Kubernetes, and if set to `Orphan`, pods created by the job are not deleted.
+
+### Bug fixes
+
+- When reporting an error response to Slack using `SlackWebException`, put the response body in an attachment instead of a regular block, since it may be a full HTML error page. An attachment tells Slack to hide long content by default unless the viewer expands it.
+
 <a id='changelog-4.2.2'></a>
 ## 4.2.2 (2023-05-17)
 
 ### Bug fixes
 
 - Revert the documentation change in 4.2.1 to restore cross-references, since the docs-linkcheck failure appears to be a false positive.
```

### Comparing `safir-4.2.2/docs/dev/development.rst` & `safir-4.3.0/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/dev/release.rst` & `safir-4.3.0/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/documenteer.toml` & `safir-4.3.0/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/index.rst` & `safir-4.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/arq.rst` & `safir-4.3.0/docs/user-guide/arq.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/database.rst` & `safir-4.3.0/docs/user-guide/database.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/datetime.rst` & `safir-4.3.0/docs/user-guide/datetime.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/fastapi-errors.rst` & `safir-4.3.0/docs/user-guide/fastapi-errors.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/gafaelfawr.rst` & `safir-4.3.0/docs/user-guide/gafaelfawr.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/gcs.rst` & `safir-4.3.0/docs/user-guide/gcs.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/github-apps/api-resources.rst` & `safir-4.3.0/docs/user-guide/github-apps/api-resources.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/github-apps/create-a-github-client.rst` & `safir-4.3.0/docs/user-guide/github-apps/create-a-github-client.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/github-apps/handling-webhooks.rst` & `safir-4.3.0/docs/user-guide/github-apps/handling-webhooks.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/github-apps/index.rst` & `safir-4.3.0/docs/user-guide/github-apps/index.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/github-apps/webhook-models.rst` & `safir-4.3.0/docs/user-guide/github-apps/webhook-models.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/http-client.rst` & `safir-4.3.0/docs/user-guide/http-client.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/ivoa.rst` & `safir-4.3.0/docs/user-guide/ivoa.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/kubernetes.rst` & `safir-4.3.0/docs/user-guide/kubernetes.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/logging.rst` & `safir-4.3.0/docs/user-guide/logging.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/pydantic-redis.rst` & `safir-4.3.0/docs/user-guide/pydantic-redis.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/pydantic.rst` & `safir-4.3.0/docs/user-guide/pydantic.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/set-up-from-template.rst` & `safir-4.3.0/docs/user-guide/set-up-from-template.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/slack-webhook.rst` & `safir-4.3.0/docs/user-guide/slack-webhook.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/uvicorn.rst` & `safir-4.3.0/docs/user-guide/uvicorn.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/docs/user-guide/x-forwarded.rst` & `safir-4.3.0/docs/user-guide/x-forwarded.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/pyproject.toml` & `safir-4.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/__init__.py` & `safir-4.3.0/src/safir/__init__.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/arq.py` & `safir-4.3.0/src/safir/arq.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/asyncio.py` & `safir-4.3.0/src/safir/asyncio.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/database.py` & `safir-4.3.0/src/safir/database.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/datetime.py` & `safir-4.3.0/src/safir/datetime.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/dependencies/arq.py` & `safir-4.3.0/src/safir/dependencies/arq.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/dependencies/db_session.py` & `safir-4.3.0/src/safir/dependencies/db_session.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/dependencies/gafaelfawr.py` & `safir-4.3.0/src/safir/dependencies/gafaelfawr.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/dependencies/http_client.py` & `safir-4.3.0/src/safir/dependencies/http_client.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/dependencies/logger.py` & `safir-4.3.0/src/safir/dependencies/logger.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/fastapi.py` & `safir-4.3.0/src/safir/fastapi.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/gcs.py` & `safir-4.3.0/src/safir/gcs.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/github/_client.py` & `safir-4.3.0/src/safir/github/_client.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/github/models.py` & `safir-4.3.0/src/safir/github/models.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/github/webhooks.py` & `safir-4.3.0/src/safir/github/webhooks.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/kubernetes.py` & `safir-4.3.0/src/safir/kubernetes.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/logging.py` & `safir-4.3.0/src/safir/logging.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/metadata.py` & `safir-4.3.0/src/safir/metadata.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/middleware/ivoa.py` & `safir-4.3.0/src/safir/middleware/ivoa.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/middleware/x_forwarded.py` & `safir-4.3.0/src/safir/middleware/x_forwarded.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/models.py` & `safir-4.3.0/src/safir/models.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/pydantic.py` & `safir-4.3.0/src/safir/pydantic.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/redis.py` & `safir-4.3.0/src/safir/redis.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/slack/blockkit.py` & `safir-4.3.0/src/safir/slack/blockkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
             if self.method:
                 text = f"{self.method} {self.url}"
             else:
                 text = self.url
             message.blocks.append(SlackTextBlock(heading="URL", text=text))
         if self.body:
             block = SlackCodeBlock(heading="Response", code=self.body)
-            message.blocks.append(block)
+            message.attachments.append(block)
         return message
 
 
 def _format_and_truncate_at_end(string: str, max_length: int) -> str:
     """Format a string for Slack, truncating at the end.
 
     Slack prohibits text blocks longer than a varying number of characters
```

### Comparing `safir-4.2.2/src/safir/slack/webhook.py` & `safir-4.3.0/src/safir/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/testing/gcs.py` & `safir-4.3.0/src/safir/testing/gcs.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/testing/kubernetes.py` & `safir-4.3.0/src/safir/testing/kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from kubernetes_asyncio import client, config
 from kubernetes_asyncio.client import (
     ApiException,
     CoreV1Event,
     CoreV1EventList,
     V1ConfigMap,
+    V1DeleteOptions,
     V1Ingress,
     V1IngressList,
     V1IngressStatus,
     V1Job,
     V1JobList,
     V1JobStatus,
     V1LoadBalancerStatus,
@@ -505,14 +506,17 @@
     async def delete_namespaced_custom_object(
         self,
         group: str,
         version: str,
         namespace: str,
         plural: str,
         name: str,
+        *,
+        grace_period_seconds: int | None = None,
+        body: V1DeleteOptions | None = None,
     ) -> Any:
         """Delete a custom namespaced object.
 
         Parameters
         ----------
         group
             API group for this custom object.
@@ -520,14 +524,18 @@
             API version for this custom object.
         namespace
             Namespace in which to delete the object.
         plural
             API plural for this custom object.
         name
             Custom object to delete.
+        grace_period_seconds
+            Grace period for object deletion (currently ignored).
+        body
+            Delete options (currently ignored).
 
         Returns
         -------
         kubernetes_asyncio.client.V1Status
             Success status if object was deleted.
 
         Raises
@@ -732,24 +740,33 @@
         """
         self._maybe_error("create_namespaced_config_map", namespace, body)
         self._update_metadata(body, "v1", "ConfigMap", namespace)
         name = body.metadata.name
         self._store_object(namespace, "ConfigMap", name, body)
 
     async def delete_namespaced_config_map(
-        self, name: str, namespace: str
+        self,
+        name: str,
+        namespace: str,
+        *,
+        grace_period_seconds: int | None = None,
+        body: V1DeleteOptions | None = None,
     ) -> V1Status:
         """Delete a ``ConfigMap`` object.
 
         Parameters
         ----------
         name
             Name of object.
         namespace
             Namespace of object.
+        grace_period_seconds
+            Grace period for object deletion (currently ignored).
+        body
+            Delete options (currently ignored).
 
         Returns
         -------
         kubernetes_asyncio.client.V1Status
             Success status if object was deleted.
 
         Raises
@@ -898,24 +915,33 @@
             load_balancer=V1LoadBalancerStatus(ingress=[])
         )
         self._store_object(namespace, "Ingress", name, body)
         stream = self._event_streams[namespace]["Ingress"]
         stream.add_event({"type": "ADDED", "object": body.to_dict()})
 
     async def delete_namespaced_ingress(
-        self, name: str, namespace: str
+        self,
+        name: str,
+        namespace: str,
+        *,
+        grace_period_seconds: int | None = None,
+        body: V1DeleteOptions | None = None,
     ) -> V1Status:
         """Delete an ingress object.
 
         Parameters
         ----------
         name
             Name of ingress to delete.
         namespace
             Namespace of ingress to delete.
+        grace_period_seconds
+            Grace period for object deletion (currently ignored).
+        body
+            Delete options (currently ignored).
 
         Returns
         -------
         kubernetes_asyncio.client.V1Status
             Success status.
 
         Raises
@@ -1129,50 +1155,70 @@
         podmd.labels["job-name"] = name
         pod = V1Pod(metadata=podmd, spec=template.spec)
         await self.create_namespaced_pod(namespace, pod)
         if pod.status.phase == "Running":
             body.status = V1JobStatus(active=1)
 
     async def delete_namespaced_job(
-        self, name: str, namespace: str, propagation_policy: str
+        self,
+        name: str,
+        namespace: str,
+        *,
+        grace_period_seconds: int | None = None,
+        propagation_policy: str = "Foreground",
+        body: V1DeleteOptions | None = None,
     ) -> V1Status:
         """Delete a job object.
 
         Will also propagate to pods.
 
         Parameters
         ----------
         name
             Name of job to delete.
         namespace
             Namespace of job to delete.
+        grace_period_seconds
+            Grace period for object deletion (currently ignored).
+        propagation_policy
+            Propagation policy for deletion. Must be ``Foreground`` if
+            specified, and has no effect on the behavior of the mock.
+        body
+            Delete options (currently ignored).
 
         Returns
         -------
         kubernetes_asyncio.client.V1Status
             Success status.
 
         Raises
         ------
+        AssertionError
+            Raised if the propagation policy is not ``Foreground``.
         kubernetes_asyncio.client.ApiException
             Raised with 404 status if the job was not found.
         """
-        assert (
-            propagation_policy == "Foreground"
-        ), "Only 'Foreground' propagation_policy is currently supported"
+        if propagation_policy not in ("Foreground", "Background", "Orphan"):
+            msg = f"Invalid propagation_policy {propagation_policy}"
+            raise AssertionError(msg)
         self._maybe_error("delete_namespaced_job", name, namespace)
-        stream = self._event_streams[namespace]["Job"]
+
+        # This simulates a foreground deletion, where the Job is blocked
+        # from deletion until all its pods are deleted. We also use it for
+        # background deletion for the time being, since it should be close
+        # enough.
         pods = await self.list_namespaced_pod(
             namespace, label_selector=f"job-name=={name}"
         )
-        # This simulates a foreground deletion, where the Job is blocked
-        # from deletion until all its pods are deleted.
-        for pod in pods.items:
-            await self.delete_namespaced_pod(pod.metadata.name, namespace)
+        if propagation_policy != "Orphan":
+            for pod in pods.items:
+                await self.delete_namespaced_pod(pod.metadata.name, namespace)
+
         job = self._get_object(namespace, "Job", name)
+        stream = self._event_streams[namespace]["Job"]
         stream.add_event({"type": "DELETED", "object": job.to_dict()})
         return self._delete_object(namespace, "Job", name)
 
     async def list_namespaced_job(
         self,
         namespace: str,
         *,
@@ -1306,23 +1352,33 @@
         self._update_metadata(body, "v1", "Namespace", None)
         name = body.metadata.name
         if name in self._objects:
             msg = f"Namespace {name} already exists"
             raise ApiException(status=409, reason=msg)
         self._store_object(name, "Namespace", name, body)
 
-    async def delete_namespace(self, name: str) -> None:
+    async def delete_namespace(
+        self,
+        name: str,
+        *,
+        grace_period_seconds: int | None = None,
+        body: V1DeleteOptions | None = None,
+    ) -> None:
         """Delete a namespace.
 
         This also immediately removes all objects in the namespace.
 
         Parameters
         ----------
         name
             Namespace to delete.
+        grace_period_seconds
+            Grace period for object deletion (currently ignored).
+        body
+            Delete options (currently ignored).
 
         Raises
         ------
         kubernetes_asyncio.client.ApiException
             Raised with 404 status if the namespace does not exist.
         """
         self._maybe_error("delete_namespace")
@@ -1482,24 +1538,33 @@
                 involved_object=V1ObjectReference(
                     kind="Pod", name=body.metadata.name, namespace=namespace
                 ),
             )
             await self.create_namespaced_event(namespace, event)
 
     async def delete_namespaced_pod(
-        self, name: str, namespace: str
+        self,
+        name: str,
+        namespace: str,
+        *,
+        grace_period_seconds: int | None = None,
+        body: V1DeleteOptions | None = None,
     ) -> V1Status:
         """Delete a pod object.
 
         Parameters
         ----------
         name
             Name of pod to delete.
         namespace
             Namespace of pod to delete.
+        grace_period_seconds
+            Grace period for object deletion (currently ignored).
+        body
+            Delete options (currently ignored).
 
         Returns
         -------
         kubernetes_asyncio.client.V1Status
             Success status.
 
         Raises
@@ -1871,24 +1936,33 @@
             Raised with 409 status if the object already exists.
         """
         self._maybe_error("create_namespaced_service", namespace, body)
         self._update_metadata(body, "v1", "Service", namespace)
         self._store_object(namespace, "Service", body.metadata.name, body)
 
     async def delete_namespaced_service(
-        self, name: str, namespace: str
+        self,
+        name: str,
+        namespace: str,
+        *,
+        grace_period_seconds: int | None = None,
+        body: V1DeleteOptions | None = None,
     ) -> V1Status:
         """Delete a service object.
 
         Parameters
         ----------
         name
             Name of service to delete.
         namespace
             Namespace of service to delete.
+        grace_period_seconds
+            Grace period for object deletion (currently ignored).
+        body
+            Delete options (currently ignored).
 
         Returns
         -------
         kubernetes_asyncio.client.V1Status
             Success status.
 
         Raises
```

### Comparing `safir-4.2.2/src/safir/testing/slack.py` & `safir-4.3.0/src/safir/testing/slack.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir/testing/uvicorn.py` & `safir-4.3.0/src/safir/testing/uvicorn.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/src/safir.egg-info/PKG-INFO` & `safir-4.3.0/src/safir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 4.2.2
+Version: 4.3.0
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `safir-4.2.2/src/safir.egg-info/SOURCES.txt` & `safir-4.3.0/src/safir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/conftest.py` & `safir-4.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/database_test.py` & `safir-4.3.0/tests/database_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/datetime_test.py` & `safir-4.3.0/tests/datetime_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/dependencies/arq_test.py` & `safir-4.3.0/tests/dependencies/arq_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/dependencies/db_session_test.py` & `safir-4.3.0/tests/dependencies/db_session_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/dependencies/gafaelfawr_test.py` & `safir-4.3.0/tests/dependencies/gafaelfawr_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/dependencies/http_client_test.py` & `safir-4.3.0/tests/dependencies/http_client_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/dependencies/logger_test.py` & `safir-4.3.0/tests/dependencies/logger_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/fastapi_test.py` & `safir-4.3.0/tests/fastapi_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/gcs_test.py` & `safir-4.3.0/tests/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/github/data/webhooks/check_run_created.json` & `safir-4.3.0/tests/github/data/webhooks/check_run_created.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/github/data/webhooks/check_suite_completed.json` & `safir-4.3.0/tests/github/data/webhooks/check_suite_completed.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/github/data/webhooks/installation.json` & `safir-4.3.0/tests/github/data/webhooks/installation.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/github/data/webhooks/installation_repositories.json` & `safir-4.3.0/tests/github/data/webhooks/installation_repositories.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/github/data/webhooks/pull_request_event.json` & `safir-4.3.0/tests/github/data/webhooks/pull_request_event.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/github/data/webhooks/push_event.json` & `safir-4.3.0/tests/github/data/webhooks/push_event.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/github/webhooks_test.py` & `safir-4.3.0/tests/github/webhooks_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/logging_test.py` & `safir-4.3.0/tests/logging_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/metadata_test.py` & `safir-4.3.0/tests/metadata_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/middleware/ivoa_test.py` & `safir-4.3.0/tests/middleware/ivoa_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/middleware/x_forwarded_test.py` & `safir-4.3.0/tests/middleware/x_forwarded_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/pydantic_test.py` & `safir-4.3.0/tests/pydantic_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/redis_test.py` & `safir-4.3.0/tests/redis_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/slack/blockkit_test.py` & `safir-4.3.0/tests/slack/blockkit_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/slack/webhook_test.py` & `safir-4.3.0/tests/slack/webhook_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/testing/conftest.py` & `safir-4.3.0/tests/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/testing/gcs_test.py` & `safir-4.3.0/tests/testing/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.2/tests/testing/kubernetes_test.py` & `safir-4.3.0/tests/testing/kubernetes_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import asyncio
 from typing import Any, Optional
 
 import pytest
 from kubernetes_asyncio.client import (
     CoreV1Event,
     V1Container,
+    V1DeleteOptions,
     V1ObjectMeta,
     V1ObjectReference,
     V1Pod,
     V1PodSpec,
     V1Secret,
 )
 from kubernetes_asyncio.watch import Watch
@@ -276,15 +277,20 @@
     ]
     await asyncio.sleep(0.1)
     await mock_kubernetes.patch_namespaced_pod_status(
         "foo",
         "other",
         [{"op": "replace", "path": "/status/phase", "value": "Running"}],
     )
-    await mock_kubernetes.delete_namespaced_pod("foo", "other")
+    await mock_kubernetes.delete_namespaced_pod(
+        "foo",
+        "other",
+        grace_period_seconds=1,
+        body=V1DeleteOptions(grace_period_seconds=1),
+    )
 
     # All three watches should see the same thing.
     results = await asyncio.gather(*watchers)
     assert len(results) == 3
     assert results[0] == results[1]
     assert results[0] == results[2]
     result = results[0]
```

### Comparing `safir-4.2.2/tox.ini` & `safir-4.3.0/tox.ini`

 * *Files identical despite different names*

