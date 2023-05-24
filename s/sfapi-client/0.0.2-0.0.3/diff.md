# Comparing `tmp/sfapi_client-0.0.2.tar.gz` & `tmp/sfapi_client-0.0.3.tar.gz`

## Comparing `sfapi_client-0.0.2.tar` & `sfapi_client-0.0.3.tar`

### file list

```diff
@@ -1,83 +1,86 @@
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/pytest.ini
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/requirements-dev.txt
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/.github/workflows/pypi.yml
--rwxr-xr-x   0        0        0     1097 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/gen_examples.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/gen_sync.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/index.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/community/contributing.md
--rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/examples/check_current_and_past_jobs.ipynb
--rw-r--r--   0        0        0    11955 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/examples/run_job_and_check_status.ipynb
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/javascript/apiselector.js
--rw-r--r--   0        0        0    12012 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/quickstart/index.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/SUMMARY.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/client/index.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/compute/index.md
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/exceptions/index.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/groups/index.md
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/jobs/index.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/paths/index.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/projects/index.md
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/resources/index.md
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/users/index.md
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/scripts/run.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_compute.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_jobs.py
--rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_monitor.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/client.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/compute.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/exceptions.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/groups.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/jobs.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/paths.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/projects.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/resources.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/__init__.py
--rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/client.py
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/compute.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/groups.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/jobs.py
--rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/paths.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/projects.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/users.py
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_models/__init__.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_models/job_status_response_sacct.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_models/job_status_response_squeue.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_models/resources.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/__init__.py
--rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/_models.py
--rw-r--r--   0        0        0    15536 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/client.py
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/compute.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/groups.py
--rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/jobs.py
--rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/paths.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/projects.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/users.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_api.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_api_async.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_client.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_client_async.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_compute.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_compute_async.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_groups.py
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_groups_async.py
--rwxr-xr-x   0        0        0     4647 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_jobs.py
--rwxr-xr-x   0        0        0     6378 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_jobs_async.py
--rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_paths.py
--rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_paths_async.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_projects.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_projects_async.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_resources.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_resources_async.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_users.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_users_async.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/.gitignore
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/LICENSE
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/README.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/LEGAL
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/pytest.ini
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/requirements-dev.txt
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/.github/workflows/pytest.yml
+-rwxr-xr-x   0        0        0     1097 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/gen_examples.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/gen_sync.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/index.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/community/contributing.md
+-rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/examples/check_current_and_past_jobs.ipynb
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/examples/getting_bearer_token.ipynb
+-rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/examples/run_job_and_check_status.ipynb
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/javascript/apiselector.js
+-rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/quickstart/index.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/SUMMARY.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/client/index.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/compute/index.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/exceptions/index.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/groups/index.md
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/jobs/index.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/paths/index.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/projects/index.md
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/resources/index.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/docs/reference/async/users/index.md
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/scripts/run.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_compute.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_jobs.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_monitor.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/client.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/compute.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/exceptions.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/groups.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/jobs.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/paths.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/projects.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/resources.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/__init__.py
+-rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/client.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/compute.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/groups.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/jobs.py
+-rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/paths.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/projects.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_async/users.py
+-rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_models/__init__.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_models/job_status_response_sacct.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_models/job_status_response_squeue.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_models/resources.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/__init__.py
+-rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/_models.py
+-rw-r--r--   0        0        0    15536 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/client.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/compute.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/groups.py
+-rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/jobs.py
+-rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/paths.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/projects.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/src/sfapi_client/_sync/users.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_api.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_api_async.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_client.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_client_async.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_compute.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_compute_async.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_groups.py
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_groups_async.py
+-rwxr-xr-x   0        0        0     4647 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_jobs.py
+-rwxr-xr-x   0        0        0     6378 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_jobs_async.py
+-rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_paths.py
+-rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_paths_async.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_projects.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_projects_async.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_resources.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_resources_async.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_users.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/tests/test_users_async.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/.gitignore
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/README.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 sfapi_client-0.0.3/PKG-INFO
```

### Comparing `sfapi_client-0.0.2/mkdocs.yml` & `sfapi_client-0.0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/.github/workflows/mkdocs.yml` & `sfapi_client-0.0.3/.github/workflows/mkdocs.yml`

 * *Files 23% similar despite different names*

```diff
@@ -19,8 +19,9 @@
       - uses: actions/cache@v3
         with:
           key: mkdocs-${{ github.ref }}
           path: .cache
           restore-keys: |
             mkdocs-
       - run: pip install .[docs]
+      - run: mkdocs build
       - run: mkdocs gh-deploy --force
```

### Comparing `sfapi_client-0.0.2/.github/workflows/pypi.yml` & `sfapi_client-0.0.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/docs/gen_examples.py` & `sfapi_client-0.0.3/docs/gen_examples.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/docs/gen_sync.py` & `sfapi_client-0.0.3/docs/gen_sync.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/docs/index.md` & `sfapi_client-0.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/docs/examples/check_current_and_past_jobs.ipynb` & `sfapi_client-0.0.3/docs/examples/check_current_and_past_jobs.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/docs/examples/run_job_and_check_status.ipynb` & `sfapi_client-0.0.3/docs/examples/run_job_and_check_status.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979166666666%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, 'First we make a client to connect connect with the REST "*

 * *            'api. The client will read in a file from the directory `$HOME/.superfacility` in the '*

 * *            "pem format.\\n')], delete: [0]}, 'attachments': OrderedDict()}}"}*

```diff
@@ -23,18 +23,19 @@
                 "user_name = \"elvis\"\n",
                 "\n",
                 "### This gets your home based on your username\n",
                 "user_home = f'/global/homes/{user_name[0]}/{user_name}'"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "First we make a client to connect connect with the REST api. This client will read in a file from the directoy `$HOME/.superfacility` in the pem format.\n",
+                "First we make a client to connect connect with the REST api. The client will read in a file from the directory `$HOME/.superfacility` in the pem format.\n",
                 "\n",
                 "```pem\n",
                 "CLIENT_ID\n",
                 "-----BEGIN RSA PRIVATE KEY-----\n",
                 "...\n",
                 "-----END RSA PRIVATE KEY-----\n",
                 "```\n",
```

### Comparing `sfapi_client-0.0.2/docs/javascript/apiselector.js` & `sfapi_client-0.0.3/docs/javascript/apiselector.js`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/docs/quickstart/index.md` & `sfapi_client-0.0.3/docs/quickstart/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -140,27 +140,27 @@
     ```pycon
     >>> from sfapi_client import AsyncClient
     >>> from sfapi_client.compute import Machine
     >>> from pathlib import Path
     >>>
     >>> key_path = Path("/path/to/secret/key.pem")
     >>>
-    >>> async with AsyncClient(key_name=key_path) as client:
+    >>> async with AsyncClient(key=key_path) as client:
     ...     perlmutter = await client.compute(Machine.perlmutter)
 
     ```
 === "sync"
     ```pycon
     >>> from sfapi_client import Client
     >>> from sfapi_client.compute import Machine
     >>> from pathlib import Path
     >>>
     >>> key_path = Path("/path/to/secret/key.pem")
     >>>
-    >>> with Client(key_name=key_path) as client:
+    >>> with Client(key=key_path) as client:
     ...     perlmutter = client.compute(Machine.perlmutter)
     ```
 
 
 ## Submitting a job
 
 === "async"
```

### Comparing `sfapi_client-0.0.2/docs/reference/SUMMARY.txt` & `sfapi_client-0.0.3/docs/reference/SUMMARY.txt`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/docs/reference/async/compute/index.md` & `sfapi_client-0.0.3/docs/reference/async/compute/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/docs/reference/async/groups/index.md` & `sfapi_client-0.0.3/docs/reference/async/groups/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/docs/reference/async/jobs/index.md` & `sfapi_client-0.0.3/docs/reference/async/jobs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         show_if_no_docstring: yes
         filters:
             - "!^_[^_]"
             - "!^__"
 
 ## `AsyncJobSacct`
 
-Models a job running on a compute resource, the informatio is fetched using `sacct`.
+Models a job running on a compute resource, the information is fetched using `sacct`.
 
 <!-- mkdocsstring doesn't display inherited pydantic members, so we fake
 by include the parent explicitly. -->
 ::: sfapi_client._models.job_status_response_squeue.OutputItem
     options:
         show_bases: false
         inherited_members: true
@@ -34,15 +34,15 @@
         show_if_no_docstring: yes
         filters:
             - "!^_[^_]"
             - "!^__"
 
 ## `AsyncJobSqueue`
 
-Models a job running on a compute resource, the informatio is fetched using `squeue`.
+Models a job running on a compute resource, the information is fetched using `squeue`.
 
 <!-- mkdocsstring doesn't display inherited pydantic members, so we fake
 by include the parent explicitly. -->
 ::: sfapi_client._models.job_status_response_sacct.OutputItem
     options:
         show_bases: false
         inherited_members: true
```

### Comparing `sfapi_client-0.0.2/docs/reference/async/paths/index.md` & `sfapi_client-0.0.3/docs/reference/async/paths/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/docs/reference/async/projects/index.md` & `sfapi_client-0.0.3/docs/reference/async/projects/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/scripts/run.py` & `sfapi_client-0.0.3/scripts/run.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_jobs.py` & `sfapi_client-0.0.3/src/sfapi_client/_jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_monitor.py` & `sfapi_client-0.0.3/src/sfapi_client/_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 #
 class SyncJobMonitor:
     def __init__(self, compute: "Compute"):
         self._compute = compute
         self._requests: Dict[Type, Set[JobRequest]] = {}
         # Lock to protect access to self._requests
         self._requests_lock = Lock()
-        # Lock to prevent multipe server requests concurrently
+        # Lock to prevent multiple server requests concurrently
         self._request_lock = Lock()
 
     def fetch_jobs(
         self, job_type: Union["JobSacct", "JobSqueue"], jobids: List[int]
     ) -> List[Union[JobSqueue, JobSacct]]:
         # First update the jobids and create a request context
         request = None
```

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_async/client.py` & `sfapi_client-0.0.3/src/sfapi_client/_async/client.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_async/compute.py` & `sfapi_client-0.0.3/src/sfapi_client/_async/compute.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union, Callable
 import json
 from enum import Enum
 from pydantic import BaseModel, PrivateAttr
-
+from functools import wraps
 
 from ..exceptions import SfApiError
 from .._utils import _ASYNC_SLEEP
 from .jobs import AsyncJobSacct, AsyncJobSqueue, AsyncJobSqueue, JobCommand
 from .._models import (
     AppRoutersStatusModelsStatus as ComputeBase,
     Task,
@@ -21,22 +21,33 @@
 from .._monitor import AsyncJobMonitor
 from .._compute import CommandResult, SubmitJobResponse, SubmitJobResponseStatus
 
 # Patch to return str names from Enum of py3.11
 Machine.__str__ = lambda self: self.value
 
 
+def check_auth(method: Callable):
+    @wraps(method)
+    def wrapper(self, *args, **kwargs):
+        if self.client._client_id is None:
+            raise SfApiError(
+                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client.")
+        elif self.status in [StatusValue.unavailable]:
+            raise SfApiError(
+                f"Compute resource {self.name} is {self.status.name}, {self.notes}")
+        return method(self, *args, **kwargs)
+    return wrapper
+
+
 class AsyncCompute(ComputeBase):
     client: Optional["AsyncClient"]
     _monitor: AsyncJobMonitor = PrivateAttr()
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        if self.status in [StatusValue.unavailable, StatusValue.other]:
-            raise SfApiError(f"Compute resource {self.name} is {self.status.name}, {self.notes}")
         self._monitor = AsyncJobMonitor(self)
 
     def dict(self, *args, **kwargs) -> Dict:
         if "exclude" not in kwargs:
             kwargs["exclude"] = {"client"}
         return super().dict(*args, **kwargs)
 
@@ -52,18 +63,19 @@
 
             if task.result is None:
                 await _ASYNC_SLEEP(1)
                 continue
 
             return task.result
 
+    @check_auth
     async def submit_job(self, script: Union[str, AsyncRemotePath]) -> AsyncJobSqueue:
         """Submit a job to the compute resource
 
-        :param script: Path to file on the compute system, or script to run begining with `#!`.
+        :param script: Path to file on the compute system, or script to run beginning with `#!`.
         :return: Object containing information about the job, its job id, and status on the system.
         """
 
         is_path: bool = True
 
         # If it's a remote path we've already checked so just continue
         if isinstance(script, AsyncRemotePath):
@@ -103,25 +115,27 @@
             raise SfApiError(f"Unable to extract jobid if for task: {task_id}")
 
         job = AsyncJobSqueue(jobid=jobid)
         job.compute = self
 
         return job
 
+    @check_auth
     async def job(
         self, jobid: int, command: Optional[JobCommand] = JobCommand.sacct
     ) -> Union["AsyncJobSacct", "AsyncJobSqueue"]:
         # Get different job depending on query
         Job = AsyncJobSacct if (command == JobCommand.sacct) else AsyncJobSqueue
         jobs = await self._monitor.fetch_jobs(job_type=Job, jobids=[jobid])
         if len(jobs) == 0:
             raise SfApiError(f"Job not found: ${jobid}")
 
         return jobs[0]
 
+    @check_auth
     async def jobs(
         self,
         jobids: Optional[int] = None,
         user: Optional[str] = None,
         partition: Optional[str] = None,
         command: Optional[JobCommand] = JobCommand.squeue,
     ) -> List[Union[AsyncJobSacct, AsyncJobSqueue]]:
@@ -131,17 +145,19 @@
         if jobids is not None and user is None and partition is None:
             return await self._monitor.fetch_jobs(job_type=Job, jobids=jobids)
         else:
             return await Job._fetch_jobs(
                 self, jobids=jobids, user=user, partition=partition
             )
 
+    @check_auth
     async def ls(self, path, directory=False) -> List[AsyncRemotePath]:
         return await AsyncRemotePath._ls(self, path, directory)
 
+    @check_auth
     async def run(self, args: Union[str, AsyncRemotePath, List[str]]):
         body: RunCommandBody = {
             "executable": args if not isinstance(args, list) else " ".join(args)
         }
 
         r = await self.client.post(f"utilities/command/{self.name}", data=body)
         json_response = r.json()
```

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_async/groups.py` & `sfapi_client-0.0.3/src/sfapi_client/_async/groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,25 @@
-from typing import Optional, Union, List, Any
+from typing import Optional, Union, List, Any, Callable
+from functools import wraps
 from pydantic import ValidationError, Field, BaseModel, validator
 from .._models import BatchGroupAction as GroupAction, UserStats as GroupMemberBase
 from ..exceptions import SfApiError
 from .users import AsyncUser
 
 
+def check_auth(method: Callable):
+    @wraps(method)
+    def wrapper(self, *args, **kwargs):
+        if self._client_id is None:
+            raise SfApiError(
+                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client.")
+        return method(self, *args, **kwargs)
+    return wrapper
+
+
 class AsyncGroupMember(GroupMemberBase):
     client: Optional["AsyncClient"]
 
     async def user(self) -> "AsyncUser":
         """
         Get the user associated with the membership.
         """
@@ -84,14 +95,15 @@
             return m
 
         members = map(_set_client, members)
 
         return list(members)
 
     @staticmethod
+    @check_auth
     async def _fetch_group(client: "AsyncClient", name):
         response = await client.get(f"account/groups/{name}")
         json_response = response.json()
 
         group = AsyncGroup.parse_obj(json_response)
         group.client = client
```

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_async/jobs.py` & `sfapi_client-0.0.3/src/sfapi_client/_async/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         partition: Optional[str] = None,
     ):
         return await _fetch_jobs(cls, compute, jobids, user, partition)
 
 
 class AsyncJobSqueue(AsyncJob, JobSqueueBase):
     """
-    Models a job running on a compute resource, the informatio is
+    Models a job running on a compute resource, the information is
     fetched using `squeue`.
     """
     _command: ClassVar[JobCommand] = JobCommand.squeue
 
     async def _fetch_state(self):
         jobs = await self.compute._monitor.fetch_jobs(
             job_type=self.__class__, jobids=[self.jobid]
```

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_async/paths.py` & `sfapi_client-0.0.3/src/sfapi_client/_async/paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,24 +115,24 @@
     def dict(self, *args, **kwargs) -> Dict:
         if "exclude" not in kwargs:
             kwargs["exclude"] = {"compute"}
         return super().dict(*args, **kwargs)
 
     async def is_dir(self):
         """
-        :return: Returns True if path is a directory, False othewise .
+        :return: Returns True if path is a directory, False otherwise.
         """
         if self.perms is None:
             await self.update()
 
         return self.perms[0] == "d"
 
     async def is_file(self):
         """
-        :return: Returns True if path is a file, False othewise .
+        :return: Returns True if path is a file, False otherwise.
         """
         return not await self.is_dir()
 
     async def download(self, binary=False) -> IO[AnyStr]:
         """
         Download the file contents.
```

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_async/projects.py` & `sfapi_client-0.0.3/src/sfapi_client/_async/projects.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_async/users.py` & `sfapi_client-0.0.3/src/sfapi_client/_async/users.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,33 @@
-from typing import List, Optional
+from typing import List, Optional, Callable
+from functools import wraps
+
 from .._models import (
     UserInfo as UserBase,
     GroupList as GroupsResponse,
 )
 from .projects import AsyncProject
 from ..exceptions import SfApiError
 
 
+def check_auth(method: Callable):
+    @wraps(method)
+    def wrapper(self, *args, **kwargs):
+        if self._client_id is None:
+            raise SfApiError(
+                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client.")
+        return method(self, *args, **kwargs)
+    return wrapper
+
+
 class AsyncUser(UserBase):
     client: Optional["AsyncClient"]
 
     @staticmethod
+    @check_auth
     async def _fetch_user(client: "AsyncClient", username: Optional[str] = None):
         url = "account/"
         if username is not None:
             url = f"{url}?username={username}"
 
         response = await client.get(url)
         json_response = response.json()
```

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_models/__init__.py` & `sfapi_client-0.0.3/src/sfapi_client/_models/__init__.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_models/job_status_response_sacct.py` & `sfapi_client-0.0.3/src/sfapi_client/_models/job_status_response_sacct.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_models/job_status_response_squeue.py` & `sfapi_client-0.0.3/src/sfapi_client/_models/job_status_response_squeue.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_models/resources.py` & `sfapi_client-0.0.3/src/sfapi_client/_models/resources.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_sync/_models.py` & `sfapi_client-0.0.3/src/sfapi_client/_sync/_models.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_sync/client.py` & `sfapi_client-0.0.3/src/sfapi_client/_sync/client.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_sync/compute.py` & `sfapi_client-0.0.3/src/sfapi_client/_sync/compute.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union, Callable
 import json
 from enum import Enum
 from pydantic import BaseModel, PrivateAttr
-
+from functools import wraps
 
 from ..exceptions import SfApiError
 from .._utils import _SLEEP
 from .jobs import JobSacct, JobSqueue, JobSqueue, JobCommand
 from .._models import (
     AppRoutersStatusModelsStatus as ComputeBase,
     Task,
@@ -21,22 +21,33 @@
 from .._monitor import SyncJobMonitor
 from .._compute import CommandResult, SubmitJobResponse, SubmitJobResponseStatus
 
 # Patch to return str names from Enum of py3.11
 Machine.__str__ = lambda self: self.value
 
 
+def check_auth(method: Callable):
+    @wraps(method)
+    def wrapper(self, *args, **kwargs):
+        if self.client._client_id is None:
+            raise SfApiError(
+                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client.")
+        elif self.status in [StatusValue.unavailable]:
+            raise SfApiError(
+                f"Compute resource {self.name} is {self.status.name}, {self.notes}")
+        return method(self, *args, **kwargs)
+    return wrapper
+
+
 class Compute(ComputeBase):
     client: Optional["Client"]
     _monitor: SyncJobMonitor = PrivateAttr()
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        if self.status in [StatusValue.unavailable, StatusValue.other]:
-            raise SfApiError(f"Compute resource {self.name} is {self.status.name}, {self.notes}")
         self._monitor = SyncJobMonitor(self)
 
     def dict(self, *args, **kwargs) -> Dict:
         if "exclude" not in kwargs:
             kwargs["exclude"] = {"client"}
         return super().dict(*args, **kwargs)
 
@@ -52,18 +63,19 @@
 
             if task.result is None:
                 _SLEEP(1)
                 continue
 
             return task.result
 
+    @check_auth
     def submit_job(self, script: Union[str, RemotePath]) -> JobSqueue:
         """Submit a job to the compute resource
 
-        :param script: Path to file on the compute system, or script to run begining with `#!`.
+        :param script: Path to file on the compute system, or script to run beginning with `#!`.
         :return: Object containing information about the job, its job id, and status on the system.
         """
 
         is_path: bool = True
 
         # If it's a remote path we've already checked so just continue
         if isinstance(script, RemotePath):
@@ -103,25 +115,27 @@
             raise SfApiError(f"Unable to extract jobid if for task: {task_id}")
 
         job = JobSqueue(jobid=jobid)
         job.compute = self
 
         return job
 
+    @check_auth
     def job(
         self, jobid: int, command: Optional[JobCommand] = JobCommand.sacct
     ) -> Union["JobSacct", "JobSqueue"]:
         # Get different job depending on query
         Job = JobSacct if (command == JobCommand.sacct) else JobSqueue
         jobs = self._monitor.fetch_jobs(job_type=Job, jobids=[jobid])
         if len(jobs) == 0:
             raise SfApiError(f"Job not found: ${jobid}")
 
         return jobs[0]
 
+    @check_auth
     def jobs(
         self,
         jobids: Optional[int] = None,
         user: Optional[str] = None,
         partition: Optional[str] = None,
         command: Optional[JobCommand] = JobCommand.squeue,
     ) -> List[Union[JobSacct, JobSqueue]]:
@@ -131,17 +145,19 @@
         if jobids is not None and user is None and partition is None:
             return self._monitor.fetch_jobs(job_type=Job, jobids=jobids)
         else:
             return Job._fetch_jobs(
                 self, jobids=jobids, user=user, partition=partition
             )
 
+    @check_auth
     def ls(self, path, directory=False) -> List[RemotePath]:
         return RemotePath._ls(self, path, directory)
 
+    @check_auth
     def run(self, args: Union[str, RemotePath, List[str]]):
         body: RunCommandBody = {
             "executable": args if not isinstance(args, list) else " ".join(args)
         }
 
         r = self.client.post(f"utilities/command/{self.name}", data=body)
         json_response = r.json()
```

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_sync/groups.py` & `sfapi_client-0.0.3/src/sfapi_client/_sync/groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,25 @@
-from typing import Optional, Union, List, Any
+from typing import Optional, Union, List, Any, Callable
+from functools import wraps
 from pydantic import ValidationError, Field, BaseModel, validator
 from .._models import BatchGroupAction as GroupAction, UserStats as GroupMemberBase
 from ..exceptions import SfApiError
 from .users import User
 
 
+def check_auth(method: Callable):
+    @wraps(method)
+    def wrapper(self, *args, **kwargs):
+        if self._client_id is None:
+            raise SfApiError(
+                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client.")
+        return method(self, *args, **kwargs)
+    return wrapper
+
+
 class GroupMember(GroupMemberBase):
     client: Optional["Client"]
 
     def user(self) -> "User":
         """
         Get the user associated with the membership.
         """
@@ -84,14 +95,15 @@
             return m
 
         members = map(_set_client, members)
 
         return list(members)
 
     @staticmethod
+    @check_auth
     def _fetch_group(client: "Client", name):
         response = client.get(f"account/groups/{name}")
         json_response = response.json()
 
         group = Group.parse_obj(json_response)
         group.client = client
```

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_sync/jobs.py` & `sfapi_client-0.0.3/src/sfapi_client/_sync/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         partition: Optional[str] = None,
     ):
         return _fetch_jobs(cls, compute, jobids, user, partition)
 
 
 class JobSqueue(Job, JobSqueueBase):
     """
-    Models a job running on a compute resource, the informatio is
+    Models a job running on a compute resource, the information is
     fetched using `squeue`.
     """
     _command: ClassVar[JobCommand] = JobCommand.squeue
 
     def _fetch_state(self):
         jobs = self.compute._monitor.fetch_jobs(
             job_type=self.__class__, jobids=[self.jobid]
```

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_sync/paths.py` & `sfapi_client-0.0.3/src/sfapi_client/_sync/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,24 +132,24 @@
     def dict(self, *args, **kwargs) -> Dict:
         if "exclude" not in kwargs:
             kwargs["exclude"] = {"compute"}
         return super().dict(*args, **kwargs)
 
     def is_dir(self) -> bool:
         """
-        :return: Returns True if path is a directory, False othewise .
+        :return: Returns True if path is a directory, False otherwise.
         """
         if self.perms is None:
             self.update()
 
         return self.perms[0] == "d"
 
     def is_file(self) -> bool:
         """
-        :return: Returns True if path is a file, False othewise .
+        :return: Returns True if path is a file, False otherwise.
         """
         return not self.is_dir()
 
     def download(self, binary=False) -> IO[AnyStr]:
         """
         Download the file contents.
```

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_sync/projects.py` & `sfapi_client-0.0.3/src/sfapi_client/_sync/projects.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/src/sfapi_client/_sync/users.py` & `sfapi_client-0.0.3/src/sfapi_client/_sync/users.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,33 @@
-from typing import List, Optional
+from typing import List, Optional, Callable
+from functools import wraps
+
 from .._models import (
     UserInfo as UserBase,
     GroupList as GroupsResponse,
 )
 from .projects import Project
 from ..exceptions import SfApiError
 
 
+def check_auth(method: Callable):
+    @wraps(method)
+    def wrapper(self, *args, **kwargs):
+        if self._client_id is None:
+            raise SfApiError(
+                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client.")
+        return method(self, *args, **kwargs)
+    return wrapper
+
+
 class User(UserBase):
     client: Optional["Client"]
 
     @staticmethod
+    @check_auth
     def _fetch_user(client: "Client", username: Optional[str] = None):
         url = "account/"
         if username is not None:
             url = f"{url}?username={username}"
 
         response = client.get(url)
         json_response = response.json()
```

### Comparing `sfapi_client-0.0.2/tests/conftest.py` & `sfapi_client-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_compute.py` & `sfapi_client-0.0.3/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_compute_async.py` & `sfapi_client-0.0.3/tests/test_compute_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_groups.py` & `sfapi_client-0.0.3/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_groups_async.py` & `sfapi_client-0.0.3/tests/test_groups_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_jobs.py` & `sfapi_client-0.0.3/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_jobs_async.py` & `sfapi_client-0.0.3/tests/test_jobs_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_paths.py` & `sfapi_client-0.0.3/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_paths_async.py` & `sfapi_client-0.0.3/tests/test_paths_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_projects.py` & `sfapi_client-0.0.3/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_projects_async.py` & `sfapi_client-0.0.3/tests/test_projects_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_resources.py` & `sfapi_client-0.0.3/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_resources_async.py` & `sfapi_client-0.0.3/tests/test_resources_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_users.py` & `sfapi_client-0.0.3/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/tests/test_users_async.py` & `sfapi_client-0.0.3/tests/test_users_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/README.md` & `sfapi_client-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.2/pyproject.toml` & `sfapi_client-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -44,9 +44,10 @@
   "mkdocs-section-index",
   "mkdocs-jupyter"
 ]
 
 test = [
   "pytest",
   "pydantic[dotenv]",
-  "pytest-mock"
-]
+  "pytest-mock",
+  "pytest-asyncio"
+]
```

### Comparing `sfapi_client-0.0.2/PKG-INFO` & `sfapi_client-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfapi_client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python client for NERSC SF API
 Author-email: Chris Harris <cjh@lbl.gov>, Nicholas Tyler <tylern@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -18,14 +18,15 @@
 Requires-Dist: mkdocs-literate-nav; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocs-section-index; extra == 'docs'
 Requires-Dist: mkdocstrings[python]; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pydantic[dotenv]; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-mock; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Welcome to sfapi_client
 
 sfapi_client is a Python 3 client for NERSC's [Superfacility API](https://docs.nersc.gov/services/sfapi/).
```

