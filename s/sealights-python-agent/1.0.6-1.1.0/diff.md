# Comparing `tmp/sealights-python-agent-1.0.6.tar.gz` & `tmp/sealights-python-agent-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sealights-python-agent-1.0.6.tar", last modified: Tue Aug 30 13:30:03 2022, max compression
+gzip compressed data, was "dist/sealights-python-agent-1.1.0.tar", last modified: Wed May 24 07:26:19 2023, max compression
```

## Comparing `sealights-python-agent-1.0.6.tar` & `sealights-python-agent-1.1.0.tar`

### file list

```diff
@@ -1,306 +1,321 @@
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    13769 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/admin.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/bootstrap/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1171 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/bootstrap/sitecustomize.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/bootstrap/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8417 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/configuration_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1787 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/environment_variables_resolver.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2740 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/config_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2767 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/constants.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/autoupgrade/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3132 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/autoupgrade/autoupgrade_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/autoupgrade/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/token/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      353 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/token/token_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1328 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/token/token_parser.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/token/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/http/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7672 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/http/backend_proxy.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2422 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/http/sl_routes.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1838 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/http/requests_wrapper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/http/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/build_session/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      343 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/build_session/build_session_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/build_session/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/log/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2923 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/log/sealights_logging.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/log/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5183 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/utils.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/queues/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      821 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/queues/events_queue.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/queues/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      940 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/queues/footprints_queue.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1280 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/bottle_framework.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1260 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/flask_framework.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       51 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/coloring/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1396 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/coloring/requests_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2218 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/coloring/selenium_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      682 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/coloring/urllib2_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       68 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/coloring/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4000 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/tia_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4899 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/code_coverage_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2989 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/agent_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7483 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/footprints_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2791 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/events_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      453 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/footprints_collector.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2551 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/sealights_api.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/services/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6000 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/services/footprints_service.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1200 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/services/events_service.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/services/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1026 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/line_footprints_collector.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      744 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3654 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/method_footprints_collector.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      560 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/freezegun_patcher.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2806 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/multiprocessing_patcher.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      779 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/pytest_xdist_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4928 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/unittest_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4371 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/nose_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6774 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/pytest_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      239 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/upload_reports_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      130 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/footprint_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      308 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/footprints_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      417 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/events_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      410 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/start_execution_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      388 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/logs_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      608 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/upload_reports_metadata.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/test_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      197 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/file_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/app_data.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1402 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/agent_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1958 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/pytest_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1135 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/unittest_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1200 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/nose_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2175 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/upload_reports.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      395 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/end_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      836 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/start_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2068 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/run.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/send_footprints.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      523 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/anonymous_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1604 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/state_tracker.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3113 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/scm/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7711 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/scm/git_integration.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2517 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/scm/scm_info.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/scm/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1581 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/file_scanner.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2419 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/visitors.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5864 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/app.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2281 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/ast_utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3794 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/method_hasher.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2327 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/environment_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      263 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/build_mapping_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      620 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/method_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       91 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/code_element_with_hash.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      625 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/file_data.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/executors/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      652 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/executors/build.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1836 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/executors/config.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/executors/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      632 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/init.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/blinker/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4479 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/blinker/_utilities.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    16341 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/blinker/base.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9223 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/blinker/_saferef.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      322 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/blinker/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    22041 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/adapters.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3456 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1003 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/packages.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    35166 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/models.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      441 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/__version__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      475 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/certs.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6402 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/api.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      757 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/hooks.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18430 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/cookies.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    10207 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/auth.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    33321 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4071 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/help.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1096 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/_internal_utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5039 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4188 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/status_codes.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3005 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/structures.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2081 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/compat.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    29835 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/sessions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    32452 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/six.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/certifi/
--rw-r--r--   0 jenkins    (498) jenkins    (497)   276001 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/certifi/cacert.pem
--rw-r--r--   0 jenkins    (498) jenkins    (497)      243 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/certifi/__main__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       96 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/certifi/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2537 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/certifi/core.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9186 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jws.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      963 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1914 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/jwks_client.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8025 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jwt.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    22392 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/algorithms.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3114 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jwk.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3993 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/help.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1548 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1222 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/__main__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20121 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser36.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1435 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/printer.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    26742 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      466 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20676 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser37.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2917 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/string_repr.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    32032 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/code_gen.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        6 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/VERSION
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3268 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/file_util.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7373 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/source_repr.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6542 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/node_util.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2291 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6741 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/rtrip.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6020 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/tree_walk.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3191 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/op_util.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      204 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/codegen.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)   107685 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/typing_extensions.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1862 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_adapters.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2166 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_text.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      743 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_collections.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1826 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_compat.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2895 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_functools.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1154 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_meta.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/py.typed
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2068 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_itertools.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    30533 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8425 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/zipp.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/click/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1353 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/_textwrap.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9167 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    16063 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/testing.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    35114 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/types.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    23451 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/_termui_impl.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18810 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/_compat.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3201 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/_unicodefun.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7860 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/_winconsole.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1983 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/globals.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18956 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    19066 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/parser.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3243 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)   111454 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/core.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    14901 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/decorators.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9706 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/formatting.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18003 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/shell_completion.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    28873 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/termui.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    11076 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cd.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3384 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/legacy.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    13303 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/models.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/assets/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    25485 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/assets/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cli/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9364 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cli/normalizer.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cli/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20303 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/api.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/py.typed
--rw-r--r--   0 jenkins    (498) jenkins    (497)       80 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/version.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18191 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/md.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9308 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1790 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    19449 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/constant.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/semantic_version/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    48115 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/semantic_version/base.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      546 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/semantic_version/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/semantic_version/django_fields.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3374 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/codec.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1881 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/intranges.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)   204400 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/uts46data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       21 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/package_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    44025 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/idnadata.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    12795 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/core.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      321 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/compat.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8217 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    28276 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/response.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8579 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/fields.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    39013 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/connectionpool.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       63 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/_version.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    19786 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/poolmanager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    10811 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/_collections.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2440 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/filepost.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20070 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/connection.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5758 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6895 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssltransport.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/response.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/proxy.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    17165 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssl_.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5404 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/wait.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    10003 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/timeout.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4901 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/connection.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      498 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/queue.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4225 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    22001 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/retry.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1155 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    14057 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/url.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5985 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/request.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4538 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/ntlmpool.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    13922 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    17632 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    34433 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/securetransport.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    16901 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      957 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    11010 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/appengine.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7097 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/socks.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2763 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    34666 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/six.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/backports/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1417 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/backports/makefile.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/backports/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/freezegun/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    25911 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/freezegun/api.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      421 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/freezegun/_async.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      302 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/freezegun/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2305 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/LICENSE.txt
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/
--rw-r--r--   0 jenkins    (498) jenkins    (497)        1 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)       95 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)    11869 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)      386 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/requires.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)       13 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3717 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (498) jenkins    (497)      433 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/requirements.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1992 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/CHANGES.rst
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1004 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/README.rst
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3717 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/PKG-INFO
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3808 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/setup.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       67 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/setup.cfg
--rw-r--r--   0 jenkins    (498) jenkins    (497)      138 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/MANIFEST.in
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    17323 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/admin.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/bootstrap/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1171 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/bootstrap/sitecustomize.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/bootstrap/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/common/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8417 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/configuration_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1795 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/environment_variables_resolver.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2772 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/config_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2973 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/constants.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/common/autoupgrade/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3132 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/autoupgrade/autoupgrade_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/autoupgrade/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/common/token/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      353 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/token/token_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1328 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/token/token_parser.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/token/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/common/http/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8527 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/http/backend_proxy.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3041 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/http/sl_routes.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1838 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/http/requests_wrapper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/http/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/common/build_session/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      343 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/build_session/build_session_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/build_session/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4935 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/agent_events_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5448 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/env_vars.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/entites/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      644 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/entites/agent_heartbeat_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      643 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/entites/agent_footprints_submission_error_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      467 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/entites/agent_stop_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1761 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/entites/agent_start_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      618 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/entites/agent_build_scan_error_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/entites/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      626 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/entites/agent_tests_submission_error_event.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      120 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/agent_events/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/common/log/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2923 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/log/sealights_logging.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/common/log/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5356 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/utils.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/test_listener/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/test_listener/queues/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      821 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/queues/events_queue.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/queues/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      940 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/queues/footprints_queue.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/test_listener/web_frameworks/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1280 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/web_frameworks/bottle_framework.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1260 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/web_frameworks/flask_framework.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       51 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/web_frameworks/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/test_listener/coloring/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1396 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/coloring/requests_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2218 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/coloring/selenium_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      682 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/coloring/urllib2_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       68 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/coloring/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/test_listener/managers/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4000 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/managers/tia_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4883 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/managers/code_coverage_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3556 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/managers/agent_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7679 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/managers/footprints_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2986 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/managers/events_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/managers/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      453 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/footprints_collector.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2551 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/sealights_api.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/test_listener/services/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6000 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/services/footprints_service.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1200 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/services/events_service.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/services/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1026 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/line_footprints_collector.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      744 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3654 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/method_footprints_collector.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/test_listener/integrations/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      560 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/integrations/freezegun_patcher.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2806 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/integrations/multiprocessing_patcher.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      779 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/integrations/pytest_xdist_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5391 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/integrations/unittest_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4996 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/integrations/nose_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6774 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/integrations/pytest_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/integrations/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      239 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/upload_reports_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      130 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/footprint_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      308 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/footprints_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      417 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/events_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      461 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/start_execution_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      388 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/logs_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      608 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/upload_reports_metadata.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/test_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      197 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/file_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/entities/app_data.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/test_frameworks/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1473 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/test_frameworks/agent_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2002 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/test_frameworks/pytest_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1179 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/test_frameworks/unittest_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/test_frameworks/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1244 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/test_frameworks/nose_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2175 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/upload_reports.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      466 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/end_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      918 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/start_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2173 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/run.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/send_footprints.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      523 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/executors/anonymous_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1604 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/test_listener/state_tracker.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3113 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/scm/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7711 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/scm/git_integration.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2517 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/scm/scm_info.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/scm/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1537 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/file_scanner.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2419 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/visitors.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5735 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/app.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1363 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/ast_utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3782 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/method_hasher.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/entities/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2327 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/entities/environment_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/entities/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/entities/v3/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      263 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/entities/v3/build_mapping_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      620 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/entities/v3/method_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       91 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/entities/v3/code_element_with_hash.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/entities/v3/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      680 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/entities/v3/file_data.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/executors/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1404 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/executors/build.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1835 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/executors/config.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/build_scanner/executors/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      632 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/init.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/blinker/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4479 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/blinker/_utilities.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    16341 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/blinker/base.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9223 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/blinker/_saferef.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      322 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/blinker/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    22041 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/adapters.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3456 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1003 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/packages.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    35166 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/models.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      441 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/__version__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      475 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/certs.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6402 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/api.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      757 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/hooks.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18430 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/cookies.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    10207 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/auth.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    33321 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4071 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/help.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1096 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/_internal_utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5039 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4188 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/status_codes.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3005 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/structures.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2081 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/compat.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    29835 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/requests/sessions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    32452 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/six.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/certifi/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   276001 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/certifi/cacert.pem
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      243 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/certifi/__main__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       96 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/certifi/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2537 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/certifi/core.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/jwt/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9186 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/jwt/api_jws.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      963 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/jwt/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1914 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/jwt/jwks_client.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8025 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/jwt/api_jwt.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    22392 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/jwt/algorithms.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3114 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/jwt/api_jwk.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3993 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/jwt/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/jwt/help.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1548 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/jwt/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/astunparse/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1222 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astunparse/__main__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20121 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astunparse/unparser36.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20690 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astunparse/unparser38.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1435 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astunparse/printer.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    26742 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astunparse/unparser.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3197 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astunparse/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20676 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astunparse/unparser37.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2917 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/string_repr.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    32032 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/code_gen.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        6 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/VERSION
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3268 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/file_util.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7373 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/source_repr.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6542 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/node_util.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2291 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6741 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/rtrip.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6020 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/tree_walk.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3191 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/op_util.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      204 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/astor/codegen.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   107685 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/typing_extensions.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1862 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_adapters.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2166 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_text.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      743 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_collections.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1826 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_compat.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2895 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_functools.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1154 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_meta.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/py.typed
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2068 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_itertools.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    30533 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8425 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/zipp.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/click/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1353 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/_textwrap.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9167 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    16063 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/testing.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    35805 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/types.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    23451 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/_termui_impl.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18810 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/_compat.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3201 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/_unicodefun.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/py.typed
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7860 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/_winconsole.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1961 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/globals.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18682 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    19044 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/parser.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3138 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   112782 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/core.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    16350 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/decorators.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9706 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/formatting.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18018 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/shell_completion.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    28355 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/click/termui.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    11076 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/cd.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3384 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/legacy.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    13303 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/models.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/assets/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    25485 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/assets/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/cli/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9364 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/cli/normalizer.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/cli/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20303 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/api.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/py.typed
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       80 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/version.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18191 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/md.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9308 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1790 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    19449 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/constant.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/semantic_version/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    48115 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/semantic_version/base.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      546 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/semantic_version/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/semantic_version/django_fields.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/idna/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3374 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/idna/codec.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1881 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/idna/intranges.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   204400 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/idna/uts46data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       21 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/idna/package_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    44025 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/idna/idnadata.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/idna/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    12795 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/idna/core.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      321 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/idna/compat.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8217 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    28276 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/response.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8579 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/fields.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    39013 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/connectionpool.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       63 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/_version.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    19786 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/poolmanager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    10811 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/_collections.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2440 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/filepost.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20070 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/connection.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5758 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6895 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/ssltransport.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/response.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/proxy.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    17165 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/ssl_.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5404 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/wait.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    10003 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/timeout.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4901 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/connection.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      498 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/queue.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4225 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    22001 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/retry.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1155 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    14057 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/url.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5985 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/request.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4538 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/ntlmpool.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/_securetransport/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    13922 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    17632 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    34433 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/securetransport.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    16901 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      957 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    11010 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/appengine.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7097 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/socks.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2763 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/packages/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    34666 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/packages/six.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/packages/backports/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1417 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/urllib3/packages/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/python_agent/packages/freezegun/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    25911 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/freezegun/api.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      421 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/freezegun/_async.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      302 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/python_agent/packages/freezegun/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2305 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/LICENSE.txt
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/sealights_python_agent.egg-info/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        1 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/sealights_python_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       95 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/sealights_python_agent.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    12620 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/sealights_python_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      586 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/sealights_python_agent.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       13 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/sealights_python_agent.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4043 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/sealights_python_agent.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      585 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/requirements.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2076 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/CHANGES.rst
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1044 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/README.rst
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4043 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/PKG-INFO
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3846 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/setup.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       67 2023-05-24 07:26:19.000000 sealights-python-agent-1.1.0/setup.cfg
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      138 2023-05-24 07:26:17.000000 sealights-python-agent-1.1.0/MANIFEST.in
```

### Comparing `sealights-python-agent-1.0.6/python_agent/admin.py` & `sealights-python-agent-1.1.0/python_agent/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import logging
 import sys
 from distutils.util import strtobool
-
+from python_agent import __version__ as AGENT_VERSION
 from coverage.cmdline import Opts, unshell_list
 
 from python_agent.build_scanner.executors.build import Build
 from python_agent.build_scanner.executors.config import Config
 from python_agent.common import constants
-from python_agent.common.constants import TOKEN_FILE, BUILD_SESSION_ID_FILE, TEST_RECOMMENDATION
+from python_agent.common.constants import TOKEN_FILE, BUILD_SESSION_ID_FILE, TEST_RECOMMENDATION, DEFAULT_BRANCH_NAME
 from python_agent.common.config_data import ScmConfigArgs
 from python_agent.common.configuration_manager import ConfigurationManager
 from python_agent.common.constants import DEFAULT_WORKSPACEPATH
 from python_agent.packages import click
 from python_agent.test_listener.executors.end_execution import EndAnonymousExecution
 from python_agent.test_listener.executors.run import Run
 from python_agent.test_listener.executors.send_footprints import SendFootprintsAnonymousExecution
 from python_agent.test_listener.executors.start_execution import StartAnonymousExecution
 from python_agent.test_listener.executors.test_frameworks.agent_execution import AgentExecution
 from python_agent.test_listener.executors.test_frameworks.nose_execution import NoseAgentExecution
 from python_agent.test_listener.executors.test_frameworks.pytest_execution import PytestAgentExecution
 from python_agent.test_listener.executors.test_frameworks.unittest_execution import UnittestAgentExecution
 from python_agent.test_listener.executors.upload_reports import UploadReports
-from python_agent.utils import CommandType
+from python_agent.utils import CommandType, generate_random_build_name
 
 log = logging.getLogger(__name__)
 
 CONTEXT_SETTINGS = dict(token_normalize_func=lambda x: x.lower(), ignore_unknown_options=True, allow_extra_args=True)
 
 _common_options = [
     click.option("--token", help="Token (mandatory. Can also be provided by 'tokenfile' argument). Case-sensitive."),
-    click.option("--tokenfile", default=TOKEN_FILE, help="A path to a file where the program can find the token. Case-sensitive."),
+    click.option("--tokenfile", default=TOKEN_FILE,
+                 help="A path to a file where the program can find the token. Case-sensitive."),
     click.option("--proxy", help="Proxy. Must be of the form: http[s]://<server>")
 ]
 
 _build_session_options = [
     click.option("--buildsessionid", help="Provide build session id manually, case-sensitive."),
     click.option("--buildsessionidfile", default=BUILD_SESSION_ID_FILE,
                  help="Path to a file to save the build session id in (default: <user.dir>/buildSessionId.txt)."),
@@ -63,123 +64,178 @@
         f = option(f)
     return f
 
 
 def get_config_data(ctx, token, tokenfile, buildsessionid, buildsessionidfile, proxy, labid, scm_args=None):
     configuration_manager = ConfigurationManager()
     command_type = getattr(ctx, "command_type", CommandType.OTHER)
-    config_data = configuration_manager.init_configuration(command_type, token, buildsessionid, labid, tokenfile, buildsessionidfile, proxy, scm_args)
+    config_data = configuration_manager.init_configuration(command_type, token, buildsessionid, labid, tokenfile,
+                                                           buildsessionidfile, proxy, scm_args)
     return config_data
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
+@click.version_option(version=AGENT_VERSION, prog_name='SeaLights Python Agent')
 def cli():
     # entry point for the CLI. Reference from below and from setup.py -> console_scripts
     pass
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS)
 @common_options
 @click.option("--appname", required=True, help="Application name, case-sensitive.")
-@click.option("--branchname", required=True, help="Branch name, case-sensitive.")
-@click.option("--buildname", required=True, help="Build id, case-sensitive. Should be unique between builds.")
+@click.option("--branchname", help="Branch name, case-sensitive.", default=DEFAULT_BRANCH_NAME)
+@click.option("--buildname", help="Build id, case-sensitive. Should be unique between builds.",
+              default=generate_random_build_name())
 @click.option("--buildsessionid", required=False, help="Provide build session id manually, case-sensitive.")
-@click.option("--workspacepath", help="Path to the workspace where the source code exists", default=DEFAULT_WORKSPACEPATH)
+@click.option("--workspacepath", help="Path to the workspace where the source code exists",
+              default=DEFAULT_WORKSPACEPATH)
 @click.option("--include", help=Opts.include.help, default=None, type=unshell_list)
-@click.option("--exclude", help=Opts.omit.help, default=None, type=unshell_list)
+@click.option("--exclude", help=Opts.omit.help, default='*venv*', type=unshell_list)
 @click.pass_context
-def config(ctx, token, tokenfile, proxy, appname, branchname, buildname, buildsessionid, workspacepath, include, exclude):
+def config(ctx, token, tokenfile, proxy, appname, branchname, buildname, buildsessionid, workspacepath, include,
+           exclude):
     ctx.command_type = CommandType.CONFIG
     config_data = get_config_data(ctx, token, tokenfile, None, None, proxy, None)
     Config(config_data, appname, branchname, buildname, buildsessionid, workspacepath, include, exclude).execute()
+    log.info("Configuration completed successfully")
 
 
-@cli.command(context_settings=CONTEXT_SETTINGS)
+@cli.command(hidden=True, context_settings=CONTEXT_SETTINGS)
 @common_options
 @click.option(_scm_options_defs[0][0], required=False, help=_scm_options_defs[0][1])
 @click.option(_scm_options_defs[1][0], required=False, help=_scm_options_defs[1][1])
 @click.option(_scm_options_defs[2][0], required=False, help=_scm_options_defs[2][1])
 @click.option(_scm_options_defs[3][0], required=False, help=_scm_options_defs[3][1])
 @click.pass_context
 def build(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, scmprovider, scmversion, scmbaseurl, scm):
+    print("The build command is deprecated. Please use 'scan' command instead.")
     scm_args = ScmConfigArgs(scmprovider, scmversion, scmbaseurl, scm)
-    config_data = get_config_data(ctx, token, tokenfile, buildsessionid, buildsessionidfile, proxy, None, scm_args=scm_args)
+    config_data = get_config_data(ctx, token, tokenfile, buildsessionid, buildsessionidfile, proxy, None,
+                                  scm_args=scm_args)
+    Build(config_data).execute()
+
+
+@cli.command(context_settings=CONTEXT_SETTINGS)
+@common_options
+@click.option(_scm_options_defs[0][0], required=False, help=_scm_options_defs[0][1])
+@click.option(_scm_options_defs[1][0], required=False, help=_scm_options_defs[1][1])
+@click.option(_scm_options_defs[2][0], required=False, help=_scm_options_defs[2][1])
+@click.option(_scm_options_defs[3][0], required=False, help=_scm_options_defs[3][1])
+@click.pass_context
+def scan(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, scmprovider, scmversion, scmbaseurl, scm):
+    scm_args = ScmConfigArgs(scmprovider, scmversion, scmbaseurl, scm)
+    config_data = get_config_data(ctx, token, tokenfile, buildsessionid, buildsessionidfile, proxy, None,
+                                  scm_args=scm_args)
     Build(config_data).execute()
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS)
 @common_options
 @click.option("--labid", help="Lab Id, case-sensitive.")
-@click.option("--teststage", required=True, default=constants.DEFAULT_ENV, help="The tests stage (e.g 'integration tests', 'regression'). The default will be 'Unit Tests'")
+@click.option("--teststage", required=True, default=constants.DEFAULT_ENV,
+              help="The tests stage (e.g 'integration tests', 'regression'). The default will be 'Unit Tests'")
 @click.option("--cov-report", type=click.Path(writable=True), help="generate xml coverage report")
 @click.option("--per-test", default="true", type=strtobool, help="collect coverage per test")
-@click.option("--interval", default=constants.INTERVAL_IN_MILLISECONDS, type=int, help="interval in milliseconds to send data")
-@click.option("-tsd", "--test-selection-disable", is_flag=True, help='A flag to disable the test selection otherwise enable')
-@click.option("-tsri", "--test-selection-retry-interval", default=TEST_RECOMMENDATION.interval_sec, help='Test recommendation retry interval in sec')
-@click.option("-tsrt", "--test-selection-retry-timeout", default=TEST_RECOMMENDATION.timeout_sec, help='Test recommendation retry timeout in sec')
+@click.option("--interval", default=constants.INTERVAL_IN_MILLISECONDS, type=int,
+              help="interval in milliseconds to send data")
+@click.option("-tsd", "--test-selection-disable", is_flag=True,
+              help='A flag to disable the test selection otherwise enable')
+@click.option("-tsri", "--test-selection-retry-interval", default=TEST_RECOMMENDATION.interval_sec,
+              help='Test recommendation retry interval in sec')
+@click.option("-tsrt", "--test-selection-retry-timeout", default=TEST_RECOMMENDATION.timeout_sec,
+              help='Test recommendation retry timeout in sec')
+@click.option("--testgroupid", required=False, default="", help="The Test Group Id")
 @click.argument('args', nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
-def pytest(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, labid, teststage, cov_report, per_test, interval,
-           test_selection_disable, test_selection_retry_interval, test_selection_retry_timeout, args):
+def pytest(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, labid, teststage, cov_report, per_test,
+           interval,
+           test_selection_disable, test_selection_retry_interval, test_selection_retry_timeout, testgroupid, args):
     config_data = get_config_data(ctx, token, tokenfile, buildsessionid, buildsessionidfile, proxy, labid)
     config_data.testSelection.update({"enable": not test_selection_disable, "interval": test_selection_retry_interval,
-                                     "timeout": test_selection_retry_timeout})
-    PytestAgentExecution(config_data, labid, teststage, cov_report, per_test, interval, args).execute()
+                                      "timeout": test_selection_retry_timeout})
+    PytestAgentExecution(config_data, labid, teststage, cov_report, per_test, interval, testgroupid, args).execute()
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS)
 @common_options
 @click.option("--labid", help="Lab Id, case-sensitive.")
-@click.option("--teststage", required=True, default=constants.DEFAULT_ENV, help="The tests stage (e.g 'integration tests', 'regression'). The default will be 'Unit Tests'")
+@click.option("--teststage", required=True, default=constants.DEFAULT_ENV,
+              help="The tests stage (e.g 'integration tests', 'regression'). The default will be 'Unit Tests'")
 @click.option("--cov-report", type=click.Path(writable=True), help="generate xml coverage report")
 @click.option("--per-test", default="true", type=strtobool, help="collect coverage per test")
-@click.option("--interval", default=constants.INTERVAL_IN_MILLISECONDS, type=int, help="interval in milliseconds to send data")
+@click.option("--interval", default=constants.INTERVAL_IN_MILLISECONDS, type=int,
+              help="interval in milliseconds to send data")
+@click.option("-tsd", "--test-selection-disable", is_flag=True,
+              help='A flag to disable the test selection otherwise enable')
+@click.option("-tsri", "--test-selection-retry-interval", default=TEST_RECOMMENDATION.interval_sec,
+              help='Test recommendation retry interval in sec')
+@click.option("-tsrt", "--test-selection-retry-timeout", default=TEST_RECOMMENDATION.timeout_sec,
+              help='Test recommendation retry timeout in sec')
+@click.option("--testgroupid", required=False, default="", help="The Test Group Id")
 @click.argument('args', nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
-def nose(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, labid, teststage, cov_report, per_test, interval, args):
+def nose(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, labid, teststage, cov_report, per_test,
+         interval, test_selection_disable, test_selection_retry_interval, test_selection_retry_timeout, testgroupid, args):
     # click framework make the args a tuple
     # This creates an error in the parser since it expects a list.
     args = list(args)
     config_data = get_config_data(ctx, token, tokenfile, buildsessionid, buildsessionidfile, proxy, labid)
-    NoseAgentExecution(config_data, labid, teststage, cov_report, per_test, interval, args).execute()
+    config_data.testSelection.update({"enable": not test_selection_disable, "interval": test_selection_retry_interval,
+                                      "timeout": test_selection_retry_timeout})
+    NoseAgentExecution(config_data, labid, teststage, cov_report, per_test, interval, testgroupid, args).execute()
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS)
 @common_options
 @click.option("--labid", help="Lab Id, case-sensitive.")
-@click.option("--teststage", required=True, default=constants.DEFAULT_ENV, help="The tests stage (e.g 'integration tests', 'regression'). The default will be 'Unit Tests'")
+@click.option("--teststage", required=True, default=constants.DEFAULT_ENV,
+              help="The tests stage (e.g 'integration tests', 'regression'). The default will be 'Unit Tests'")
 @click.option("--cov-report", type=click.Path(writable=True), help="generate xml coverage report")
 @click.option("--per-test", default="true", type=strtobool, help="collect coverage per test")
-@click.option("--interval", default=constants.INTERVAL_IN_MILLISECONDS, type=int, help="interval in milliseconds to send data")
+@click.option("--interval", default=constants.INTERVAL_IN_MILLISECONDS, type=int,
+              help="interval in milliseconds to send data")
+@click.option("-tsd", "--test-selection-disable", is_flag=True,
+              help='A flag to disable the test selection otherwise enable')
+@click.option("-tsri", "--test-selection-retry-interval", default=TEST_RECOMMENDATION.interval_sec,
+              help='Test recommendation retry interval in sec')
+@click.option("-tsrt", "--test-selection-retry-timeout", default=TEST_RECOMMENDATION.timeout_sec,
+              help='Test recommendation retry timeout in sec')
+@click.option("--testgroupid", required=False, default="", help="The Test Group Id")
 @click.argument('args', nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
-def unittest(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, labid, teststage, cov_report, per_test, interval, args):
+def unittest(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, labid, teststage, cov_report, per_test,
+             interval, test_selection_disable, test_selection_retry_interval, test_selection_retry_timeout, testgroupid, args):
     config_data = get_config_data(ctx, token, tokenfile, buildsessionid, buildsessionidfile, proxy, labid)
-    UnittestAgentExecution(config_data, labid, teststage, cov_report, per_test, interval, args).execute()
+    config_data.testSelection.update({"enable": not test_selection_disable, "interval": test_selection_retry_interval,
+                                      "timeout": test_selection_retry_timeout})
+    UnittestAgentExecution(config_data, labid, teststage, cov_report, per_test, interval, testgroupid, args).execute()
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS)
 @common_options
 @click.option("--teststage", required=True, default=constants.DEFAULT_ENV,
               help="The tests stage (e.g 'integration tests', 'regression'). The default will be 'Unit Tests'")
 @click.option("--labid", help="Lab Id, case-sensitive.")
+@click.option("--testgroupid", required=False, default="", help="The Test Group Id")
 @click.pass_context
-def start(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, teststage, labid):
+def start(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, teststage, labid, testgroupid):
     ctx.command_type = CommandType.START
     config_data = get_config_data(ctx, token, tokenfile, buildsessionid, buildsessionidfile, proxy, labid)
-    StartAnonymousExecution(config_data, teststage, labid).execute()
+    StartAnonymousExecution(config_data, teststage, labid, testgroupid).execute()
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS)
 @common_options
 @click.option("--labid", help="Lab Id, case-sensitive.")
+@click.option("--testgroupid", required=False, default="", help="The Test Group Id")
 @click.pass_context
-def end(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, labid):
+def end(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, labid, testgroupid):
     config_data = get_config_data(ctx, token, tokenfile, buildsessionid, buildsessionidfile, proxy, labid)
-    EndAnonymousExecution(config_data, labid).execute()
+    EndAnonymousExecution(config_data, labid, testgroupid).execute()
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS)
 @common_options
 @click.option("--labid", help="Lab Id, case-sensitive.")
 @click.option("--reportfile", type=unshell_list,
               help="Report files. This argument can be declared multiple times in order to upload multiple files.")
@@ -198,15 +254,16 @@
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS)
 @common_options
 @click.option("--labid", help="Lab Id, case-sensitive.")
 @click.option("--cov-report", type=click.Path(writable=True), help="generate xml coverage report")
 @click.option("--per-test", default="true", type=strtobool, help="collect coverage per test")
-@click.option("--interval", default=constants.INTERVAL_IN_MILLISECONDS, type=int, help="interval in milliseconds to send data")
+@click.option("--interval", default=constants.INTERVAL_IN_MILLISECONDS, type=int,
+              help="interval in milliseconds to send data")
 @click.argument('args', nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
 def run(ctx, token, tokenfile, proxy, buildsessionid, buildsessionidfile, labid, cov_report, per_test, interval, args):
     config_data = get_config_data(ctx, token, tokenfile, buildsessionid, buildsessionidfile, proxy, None)
     config_data.args = sys.argv
     Run(config_data, labid, cov_report, per_test, interval).execute(args)
```

### Comparing `sealights-python-agent-1.0.6/python_agent/bootstrap/sitecustomize.py` & `sealights-python-agent-1.1.0/python_agent/bootstrap/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/common/configuration_manager.py` & `sealights-python-agent-1.1.0/python_agent/common/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/common/environment_variables_resolver.py` & `sealights-python-agent-1.1.0/python_agent/common/environment_variables_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         for prefix in PREFIXES:
             result.update(self.resolve_with_prefix(prefix))
         return result
 
     def resolve_with_prefix(self, prefix):
         result = {}
         for key in os.environ.keys():
-            if key.lower().startswith(prefix):
+            if key.lower().startswith(prefix.lower()):
                 value = os.environ[key]
                 uppercase_key = key[len(prefix):].upper()
                 if not self.key_to_case_sensitive_key.get(uppercase_key):
                     # could be an external environment variable that isn't in the target object
                     continue
                 case_sensitive_key = self.key_to_case_sensitive_key[uppercase_key]
                 if case_sensitive_key in self.int_properties:
```

### Comparing `sealights-python-agent-1.0.6/python_agent/common/config_data.py` & `sealights-python-agent-1.1.0/python_agent/common/config_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         self.perTest = True
         self.interval = constants.INTERVAL_IN_MILLISECONDS
         self.intervalSeconds = constants.INTERVAL_IN_SECONDS
         self.testSelection = {"enable": True, "interval": constants.TEST_RECOMMENDATION.interval_sec, "timeout": constants.TEST_RECOMMENDATION.timeout_sec}
         self.testSelectionStatus = None
         self.test_selection_enable = True
         self.isDisabled = False
+        self.testGroupId = None
 
     def apply_scm_args(self, scm_args):
         """
         Overrides scm properties by not None values of scm_args
         None scm_args are ignored
         :param scm_args:
         :return:
```

### Comparing `sealights-python-agent-1.0.6/python_agent/common/constants.py` & `sealights-python-agent-1.1.0/python_agent/common/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,80 +3,90 @@
 import os
 import sys
 
 PREFIXES = ["sl.", "sl_", "SL.", "SL_"]
 TOKEN_FILE = "sltoken.txt"
 BUILD_SESSION_ID_FILE = "buildSessionId.txt"
 CONFIG_ENV_VARIABLE = "sl_configuration"
-
+AGENT_EVENT_BUILD_SCAN_ERROR = 4005
+AGENT_EVENT_FOOTPRINTS_SUBMIT_ERROR = 4006
+AGENT_EVENT_TEST_SUBMIT_ERROR = 4007
+AGENT_EVENT_HEARTBEAT = 1003
+AGENT_EVENT_HEARTBEAT_INTERVAL = 120
+AGENT_EVENT_START = 1001
+AGENT_EVENT_STOP = 1002
 TECHNOLOGY = "python"
 DEFAULT_ENV = "Unit Tests"
 DEFAULT_LAB_ID = "DefaultLabId"
 TEST_IDENTIFIER = "x-sl-testid"
 PYTHON_FILES_REG = r"^[^.#~!$@%^&*()+=,]+\.pyw?$"  # regex taken from coverage.py for finding python files
 INIT_TEST_NAME = "__init"
 INITIAL_COLOR = "00000000-0000-0000-0000-000000000000/__init"
 MAX_ITEMS_IN_QUEUE = 5000
 INTERVAL_IN_MILLISECONDS = 10000
 INTERVAL_IN_SECONDS = INTERVAL_IN_MILLISECONDS / 1000
-ACTIVE_EXECUTION_INTERVAL_IN_MILLISECONDS = 30000
+ACTIVE_EXECUTION_INTERVAL_IN_MILLISECONDS = 5000
 WINDOWS = sys.platform.startswith('win')
 LINUX = sys.platform.startswith("linux")
 IN_TEST = os.environ.get("SL_TEST")
 DEFAULT_WORKSPACEPATH = os.path.relpath(os.getcwd())
+DEFAULT_BRANCH_NAME = "main"
 DEFAULT_COMMIT_LOG_SIZE = 100
 NONE_SCM = 'none'
 GIT_SCM = 'git'
 GITHUB = 'Github'
 WAIT_TIMEOUT = 120.0
 XDIST_EXIT_TIMEOUT_IN_SECONDS = 60
-
+AGENT_TYPE_TEST_LISTENER = "TestListener"
+AGENT_TYPE_BUILD_SCANNER = "BuildScanner"
 FUTURE_STATEMENTS = {
-    "generators"      :       0,
-    "nested_scopes"   :  0x0010,
-    "division"        :  0x2000,
-    "absolute_import" :  0x4000,
-    "with_statement"  :  0x8000,
-    "print_function"  : 0x10000,
+    "generators": 0,
+    "nested_scopes": 0x0010,
+    "division": 0x2000,
+    "absolute_import": 0x4000,
+    "with_statement": 0x8000,
+    "print_function": 0x10000,
     "unicode_literals": 0x20000,
 }
 
 MESSAGES_CANNOT_BE_NONE = " cannot be 'None'."
 
 
 class MetadataKeys(object):
-    APP_NAME       = "appName"
-    BUILD          = "build"
-    BRANCH         = "branch"
-    CUSTOMER_ID    = "customerId"
-    GENERATED      = "generated"
-    TECHNOLOGY     = "technology"
-    SCM_PROVIDER   = "scmProvider"
-    SCM_VERSION    = "scmVersion"
-    SCM_BASE_URL   = "scmBaseUrl"
-    SCM            = "scm"
-    COMMIT         = "commit"
-    HISTORY        = "history"
-    COMMIT_LOG     = "commitLog"
-    CONTRIBUTORS   = "contributors"
+    APP_NAME = "appName"
+    BUILD = "build"
+    BRANCH = "branch"
+    CUSTOMER_ID = "customerId"
+    GENERATED = "generated"
+    TECHNOLOGY = "technology"
+    SCM_PROVIDER = "scmProvider"
+    SCM_VERSION = "scmVersion"
+    SCM_BASE_URL = "scmBaseUrl"
+    SCM = "scm"
+    COMMIT = "commit"
+    HISTORY = "history"
+    COMMIT_LOG = "commitLog"
+    CONTRIBUTORS = "contributors"
     REPOSITORY_URL = "repositoryUrl"
 
 
 # https://greentreesnakes.readthedocs.io/en/latest/nodes.html#arguments
 AST_ARGUMENTS_EMPTY_VALUES = {
-    "args"            : [],
-    "vararg"          : None,
-    "kwarg"           : None,
-    "defaults"        : [],
-    "kw_defaults"     : [],
-    "kwonlyargs"      : [],
+    "args": [],
+    "vararg": None,
+    "kwarg": None,
+    "defaults": [],
+    "kw_defaults": [],
+    "kwonlyargs": [],
+    "posonlyargs": [],
     "varargannotation": None,
-    "kwargannotation" : None
+    "kwargannotation": None
 }
 
+
 class TEST_RECOMMENDATION(object):
     timeout_sec = 60
     interval_sec = 5
     RSS = 'recommendationSetStatus'
     RSS_NOT_READY = 'notReady'
     RSS_NO_HISTORY = 'noHistory'
     RSS_READY = 'ready'
```

### Comparing `sealights-python-agent-1.0.6/python_agent/common/autoupgrade/autoupgrade_manager.py` & `sealights-python-agent-1.1.0/python_agent/common/autoupgrade/autoupgrade_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/common/token/token_parser.py` & `sealights-python-agent-1.1.0/python_agent/common/token/token_parser.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/common/http/backend_proxy.py` & `sealights-python-agent-1.1.0/python_agent/common/http/backend_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,54 +32,64 @@
         except Exception as e:
             log.exception("Failed getting Build Session Id. Error: %s" % str(e))
 
         return None
 
     def create_build_session_id(self, build_session_data):
         try:
-            response = self.requests.post(SLRoutes.build_session_v2(), data=json.dumps(build_session_data, default=lambda m: m.__dict__))
+            response = self.requests.post(SLRoutes.build_session_v2(),
+                                          data=json.dumps(build_session_data, default=lambda m: m.__dict__))
             response.raise_for_status()
             build_session_id = response.json()
             return build_session_id
         except Exception as e:
             log.exception("Failed Creating Build Session Id. Error: %s" % str(e))
             return None
 
     def submit_build_mapping(self, build_mapping):
-        response = self.requests.post(SLRoutes.build_mapping_v3(), data=json.dumps(build_mapping, default=lambda m: m.__dict__))
+        response = self.requests.post(SLRoutes.build_mapping_v5(),
+                                      data=json.dumps(build_mapping, default=lambda m: m.__dict__))
         response.raise_for_status()
 
     def send_footprints(self, footprints):
-        response = self.requests.post(SLRoutes.footprints_v5(), data=json.dumps(footprints, default=lambda m: m.__dict__))
+        response = self.requests.post(SLRoutes.footprints_v5(),
+                                      data=json.dumps(footprints, default=lambda m: m.__dict__))
         response.raise_for_status()
 
     def send_events(self, events):
         response = self.requests.post(SLRoutes.events_v2(), data=json.dumps(events, default=lambda m: m.__dict__))
         response.raise_for_status()
 
     def start_execution(self, start_execution_request):
-        response = self.requests.post(SLRoutes.test_execution_v3(), data=json.dumps(start_execution_request, default=lambda m: m.__dict__))
+        response = self.requests.post(SLRoutes.test_execution_v3(),
+                                      data=json.dumps(start_execution_request, default=lambda m: m.__dict__))
         response.raise_for_status()
 
-    def end_execution(self, labid):
-        response = self.requests.delete(SLRoutes.test_execution_v3(), params={"environment": labid})
+    def end_execution(self, labid, testgroupid):
+        if testgroupid is None or testgroupid == "":
+            response = self.requests.delete(SLRoutes.test_execution_v3(), params={"labId": labid})
+        else:
+            response = self.requests.delete(SLRoutes.test_execution_v3(),
+                                            params={"labId": labid, "testGroupId": testgroupid})
         response.raise_for_status()
 
     def upload_reports(self, upload_reports_request):
-        response = self.requests.post(SLRoutes.external_data_v3(), files=upload_reports_request.__dict__, patch_content_type=False)
+        response = self.requests.post(SLRoutes.external_data_v3(), files=upload_reports_request.__dict__,
+                                      patch_content_type=False)
         response.raise_for_status()
 
     def has_active_execution(self, customer_id, labid):
         params = {
             "customerId": customer_id,
             "labId": labid,
             "environment": labid
         }
         try:
-            log.info("[TO TST] - send TestExecutionRequest. Request url: %s. params: %s" % (SLRoutes.test_execution_v3(), params))
+            log.info("[TO TST] - send TestExecutionRequest. Request url: %s. params: %s" % (
+            SLRoutes.test_execution_v3(), params))
             response = self.requests.get(SLRoutes.test_execution_v3(), params=params)
             parsed_response = {}
             if response.content:
                 parsed_response = response.json()
             log.info("[FROM TST] - received TestExecutionResponse. Response: %s" % parsed_response)
 
             status = parsed_response.get("status")
@@ -89,15 +99,16 @@
                 log.info("[FROM TST] - Couldn't find any mapping for the specified parameters.")
                 return False
         except Exception as e:
             log.exception("[FROM TST] - Error while trying to send request. Error: %s" % str(e))
             return False
 
     def submit_logs(self, logs_request):
-        response = self.requests.post(SLRoutes.logsubmission_v2(), data=json.dumps(logs_request, default=lambda m: m.__dict__))
+        response = self.requests.post(SLRoutes.logsubmission_v2(),
+                                      data=json.dumps(logs_request, default=lambda m: m.__dict__))
         response.raise_for_status()
 
     def get_recommended_version(self):
         status_code = None
         try:
             response = self.requests.get(SLRoutes.recommended_v2())
             status_code = response.status_code
@@ -118,15 +129,17 @@
             return True
         except Exception as e:
             log.warning("Version: %s Doesn't exist. URL: %s. Error: %s" % (version, url, str(e)))
             return False
 
     def get_remote_configuration(self):
         try:
-            url = SLRoutes.configuration_v2(self.config_data.customerId, self.config_data.appName, self.config_data.branchName, self.config_data.testStage, PACKAGE_NAME, VERSION)
+            url = SLRoutes.configuration_v2(self.config_data.customerId, self.config_data.appName,
+                                            self.config_data.branchName, self.config_data.testStage, PACKAGE_NAME,
+                                            VERSION)
             response = self.requests.get(url)
             response.raise_for_status()
             response = response.json()
             config_as_json = response["config"]
             if ((config_as_json != None) and (config_as_json != "")):
                 log.info("Server returned The following configuration: '%s'" % config_as_json)
                 config = json.loads(config_as_json)
@@ -138,15 +151,15 @@
                 log.warning("Failed getting remote configuration. Error: %s" % str(e))
         except Exception as e:
             log.warning("Failed getting remote configuration. Error: %s" % str(e))
 
         return {}
 
     def try_get_recommendations(self, build_session_id):
-        url = SLRoutes.test_exclusions_v3(build_session_id, self.config_data.testStage)
+        url = SLRoutes.test_exclusions(build_session_id, self.config_data.testStage, self.config_data.testGroupId)
         try:
             response = self.requests.get(url)
             response.raise_for_status()
             return response.json()
 
         except Exception as e:
             log.warning("failed get recommendation tests from server URL: %s. Error: %s" % (url, str(e)))
@@ -163,7 +176,12 @@
             log.warning("Failed getting active build session from lab id: %s. Error: %s" % (labid, str(e)))
             return None
 
     def _create_build_session_data(self, build_session_dict):
         return BuildSessionData(build_session_dict["appName"], build_session_dict["buildName"],
                                 build_session_dict["branchName"], build_session_dict["buildSessionId"],
                                 additional_params=build_session_dict.get("additionalParams"))
+
+    def send_agent_event(self, agent_event):
+        response = self.requests.post(SLRoutes.agent_events_v3(),
+                                      data=json.dumps(agent_event, default=lambda m: m.__dict__))
+        response.raise_for_status()
```

### Comparing `sealights-python-agent-1.0.6/python_agent/common/http/sl_routes.py` & `sealights-python-agent-1.1.0/python_agent/common/http/sl_routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,18 @@
     LAB_IDS = "lab-ids"
 
     @staticmethod
     def build_session_v2(build_session_id=""):
         return "/v2/agents/%s/%s" % SLRoutes.quote_value_or_empty([SLRoutes.BUILD_SESSION, build_session_id])
 
     @staticmethod
+    def build_mapping_v5():
+        return "/v5/agents/buildmapping"
+
+    @staticmethod
     def build_mapping_v3():
         return "/v3/agents/buildmapping"
 
     @staticmethod
     def build_mapping_v2():
         return "/v2/agents/buildmapping"
 
@@ -55,16 +59,25 @@
         return "/v2/agents/%s/%s" % (PACKAGE_NAME, SLRoutes.RECOMMENDED)
 
     @staticmethod
     def test_exclusions_v3(build_session_id, test_stage):
         return "/v3/%s/%s/%s" % SLRoutes.quote_value_or_null([SLRoutes.EXCLUSIONS, build_session_id, test_stage])
 
     @staticmethod
+    def test_exclusions(build_session_id, test_stage, test_group_id):
+        if test_group_id is None or test_group_id == "":
+            return "/v3/%s/%s/%s" % SLRoutes.quote_value_or_null([SLRoutes.EXCLUSIONS, build_session_id, test_stage])
+        else:
+            return "/v4/%s/%s/%s/%s" % SLRoutes.quote_value_or_null(
+                [SLRoutes.EXCLUSIONS, build_session_id, test_stage, test_group_id])
+
+    @staticmethod
     def configuration_v2(customer_id, app_name, branch_name, test_stage, agent_name, agent_version):
-        return "/v2/config/%s/%s/%s/%s/%s/%s" % SLRoutes.quote_value_or_null([customer_id, app_name, branch_name, test_stage, agent_name, agent_version])
+        return "/v2/config/%s/%s/%s/%s/%s/%s" % SLRoutes.quote_value_or_null(
+            [customer_id, app_name, branch_name, test_stage, agent_name, agent_version])
 
     @staticmethod
     def lab_ids_active_build_session_v1(labid):
         return "/v1/%s/%s/build-sessions/active" % SLRoutes.quote_value_or_null([SLRoutes.LAB_IDS, labid])
 
     @staticmethod
     def get_value_or_null(value):
@@ -77,7 +90,11 @@
     @staticmethod
     def quote_value_or_null(params):
         return tuple(map(lambda p: SLRoutes.get_value_or_null(p), params))
 
     @staticmethod
     def quote_value_or_empty(params):
         return tuple(map(lambda p: SLRoutes.get_value_or_empty(p), params))
+
+    @staticmethod
+    def agent_events_v3():
+        return "/v3/agents/agent-events"
```

### Comparing `sealights-python-agent-1.0.6/python_agent/common/http/requests_wrapper.py` & `sealights-python-agent-1.1.0/python_agent/common/http/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/common/log/sealights_logging.py` & `sealights-python-agent-1.1.0/python_agent/common/log/sealights_logging.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/utils.py` & `sealights-python-agent-1.1.0/python_agent/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from enum import Enum
 
 import functools
 import logging
 import os
 import sys
 import time
-
+import random
+import string
 import threading
 from threading import _DummyThread
 from python_agent import bootstrap
 
 log = logging.getLogger(__name__)
 
 
@@ -18,15 +19,15 @@
         @functools.wraps(f)
         def inner_args(*args, **kwargs):
             for i in range(tries):
                 try:
                     return f(*args, **kwargs)
                 except Exception as e:
                     logger.warning("failed try #%s running function %s. args: %s exception: %s"
-                                % (str(i + 1), f.__name__, str(args), str(e)), exc_info=True)
+                                   % (str(i + 1), f.__name__, str(args), str(e)), exc_info=True)
                     time.sleep(2 * i)
             if quiet:
                 return
             raise
 
         return inner_args
 
@@ -121,54 +122,62 @@
     ctr = 0
     to_str = title
 
     if len(obj_dict) == 0:
         to_str += ': empty'
     else:
         line_format = '\t[%d]:\t%s->%s'
-        to_str += ':\n' + '\n'.join(line_format % (index, key, obj_dict[key]) for index, key in enumerate(obj_dict.keys()))
+        to_str += ':\n' + '\n'.join(
+            line_format % (index, key, obj_dict[key]) for index, key in enumerate(obj_dict.keys()))
 
     return to_str
 
 
 def trace(f, trace_function):
     @functools.wraps(f)
     def inner_trace(*args, **kwargs):
         value = f(*args, **kwargs)
         if type(value) == _DummyThread:
             sys.settrace(trace_function)
             threading.settrace(trace_function)
         return value
+
     return inner_trace
 
 
+def generate_random_build_name():
+    return ''.join(random.choice(string.ascii_letters + string.digits) for _ in range(10))
+
+
 class disableable:
     """
     This decorator skips method execution if config_data.isDisabled is true.
     This means that the agent failed to be configured correctly.
     This decorator should only be used inside a class as it assumes that the first arg is 'self'
     Args:
         config_data_name: the name of the config data member to check isDisabled against
         fail_silently: if True exits with exit code = 1 (unsuccessful)
     Returns: the wrapped function
     """
+
     def __init__(self, config_data_name="config_data", fail_silently=False):
         self.config_data_name = config_data_name
         self.fail_silently = fail_silently
 
     def __call__(self, function):
         def wrapper(*args, **kwargs):
             instance = args[0] if args and len(args) > 0 else object()
             config_data = getattr(instance, self.config_data_name)
             if config_data and not config_data.isDisabled:
                 return function(*args, **kwargs)
             # if config_data doesn't exist, the developer used the decorator wrong, do not run the function
             elif self.fail_silently:
                 return
             sys.exit(1)
+
         return wrapper
 
 
 class CommandType(Enum):
     TEST = 1
     CONFIG = 2
     BUILD = 3
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/queues/events_queue.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/queues/events_queue.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/queues/footprints_queue.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/queues/footprints_queue.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/bottle_framework.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/web_frameworks/bottle_framework.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/flask_framework.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/web_frameworks/flask_framework.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/coloring/requests_helper.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/coloring/requests_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/coloring/selenium_helper.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/coloring/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/coloring/urllib2_helper.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/coloring/urllib2_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/managers/tia_manager.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/managers/tia_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/managers/code_coverage_manager.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/managers/code_coverage_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.config_data.include = self.config_data.include or []
         self.config_data.include.append("*%s*" % os.path.abspath(self.config_data.workspacepath))
         if constants.IN_TEST:
             # coverage.py ignores "include" if source is given so, in order to include python agent coverage
             # we move workspacepath to include, include python_agent, remove exclude and add "data_suffix=True" so
             # coverage files will be saved each time with a unique suffix so we won't loose coverage after each reset
             self.config_data.include.append("*%s*" % python_agent.__name__)
-            coverage = Coverage(source=None, include=self.config_data.include, omit=None, data_suffix=True, branch=False, data_file=None)
+            coverage = Coverage(source=None, include=self.config_data.include, omit=None, data_suffix=True, branch=False)
         else:
             coverage = Coverage(source=None, include=self.config_data.include, omit=self.config_data.exclude, data_suffix=True, branch=False, data_file=None)
         if getattr(coverage, "_warn_no_data", False):
             coverage._warn_no_data = False
         if self.config_data.isOfflineMode:
             # no actual tracing is done here
             # we're loading the raw coverage data from the .coverage file
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/managers/agent_manager.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/managers/agent_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 import atexit
 import logging
 import os
 import sys
 import uuid
 import time
 
+from python_agent.common.agent_events.agent_events_manager import AgentEventsManager
+from python_agent.common.constants import AGENT_TYPE_TEST_LISTENER
 from python_agent.common.http.backend_proxy import BackendProxy
 from python_agent.packages.six import add_metaclass
 from python_agent.test_listener.integrations.freezegun_patcher import FreezeGunPatcher
 from python_agent.test_listener.integrations.pytest_xdist_helper import override_xdist_exit_timeout
 from python_agent.test_listener.managers.events_manager import EventsManager
 from python_agent.test_listener.managers.footprints_manager import FootprintsManager
 from python_agent.test_listener.managers.tia_manager import TIAManager
 from python_agent.test_listener.state_tracker import StateTracker
 from python_agent.test_listener.utils import Singleton
 
 log = logging.getLogger(__name__)
 
+
 @add_metaclass(Singleton)
 class AgentManager(object):
 
     def __init__(self, config_data=None, is_master=True):
         log.info("Initializing... Is Master? %s" % is_master)
         if not config_data:
             raise Exception("'config_data' must be provided")
         self.config_data = config_data
         self.is_master = is_master
         self.pid = os.getpid()
         self.backend_proxy = BackendProxy(config_data)
         self.state_tracker = StateTracker(config_data)
-        self.footprints_manager = FootprintsManager(config_data, self.backend_proxy)
-        self.events_manager = EventsManager(config_data, self.backend_proxy)
+        self.agents_events_manager = AgentEventsManager(config_data=config_data, agent_type=AGENT_TYPE_TEST_LISTENER,
+                                                        agent_id=None)
+        self.agents_events_manager.send_agent_start(lab_id=config_data.labId, test_stage=config_data.testStage)
+        self.footprints_manager = FootprintsManager(config_data, self.backend_proxy, self.agents_events_manager)
+        self.events_manager = EventsManager(config_data, self.backend_proxy, self.agents_events_manager)
         self.tia_manager = TIAManager(config_data)
         self.footprints_manager.start()
         self.events_manager.start()
+
         atexit.register(self.shutdown)
         self.agent_started()
         self.register_integrations()
         # self.register_uwsgi_at_exit()
 
     def get_excluded_tests(self):
         return self.tia_manager.get_excluded_tests()
@@ -53,14 +60,15 @@
         self.events_manager.send_all()
         self.footprints_manager.send_all()
 
     def shutdown(self):
         if self.pid == os.getpid():
             self.events_manager.shutdown()
             self.footprints_manager.shutdown(self.is_master)
+            self.agents_events_manager.send_agent_stop()
             log.info("Finished Shutting Down Agent Manager")
 
     def get_trace_function(self):
         return self.footprints_manager.get_trace_function()
 
     def agent_started(self):
         self.push_event({
@@ -77,8 +85,7 @@
 
             def uwsgi_atexit_callback():
                 self.shutdown()
                 if uwsgi_original_atexit_callback:
                     uwsgi_original_atexit_callback()
 
             uwsgi.atexit = uwsgi_atexit_callback
-
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/managers/footprints_manager.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/managers/footprints_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,31 @@
     "executors": {'processpool': ProcessPoolExecutor(3)}
 }
 
 log = logging.getLogger(__name__)
 
 
 class FootprintsManager(object):
-    def __init__(self, config_data, backend_proxy):
+    def __init__(self, config_data, backend_proxy, agent_events_manager):
         self.config_data = config_data
         self.backend_proxy = backend_proxy
         self.footprints_service = FootprintsService(self.config_data, backend_proxy)
         self.footprints_queue = FootprintsQueue(maxsize=constants.MAX_ITEMS_IN_QUEUE)
         self.code_coverage_manager = CodeCoverageManager(config_data)
         self.watchdog = scheduler_class(**kwargs)
         self.watchdog.add_job(self.send_all, interval.IntervalTrigger(seconds=self.config_data.intervalSeconds))
         self.watchdog.add_job(self.send_current_partial_footprints,
                               interval.IntervalTrigger(seconds=self.config_data.intervalSeconds))
         self.watchdog.add_job(self.get_active_execution, interval.IntervalTrigger(
             seconds=constants.ACTIVE_EXECUTION_INTERVAL_IN_MILLISECONDS / 1000))
         self._is_sending_lock = threading.Lock()
         self.is_getting_footprints_lock = threading.Lock()
         self.has_active_execution = False
+        self.agent_events_manager = agent_events_manager
+
 
     def test_identifier_changing(self, sender, **kwargs):
         old_test_identifier = kwargs.get("old_test_identifier")
         new_test_identifier = kwargs.get("new_test_identifier")
         log.info("Test Identifier Changed. Old: %s. New: %s" % (old_test_identifier, new_test_identifier))
         self.get_and_enqueue_coverage(old_test_identifier)
 
@@ -76,27 +78,30 @@
             except Exception as e:
                 log.exception("Failed Enqueuing Coverage. Test: %s. Error: %s" % (test_identifier, str(e)))
 
         with self.is_getting_footprints_lock:
             enqueue_coverage(test_identifier)
 
     def send_all(self, *args, **kwargs):
+
         self._is_sending_lock.acquire()
         footprint_items = []
         try:
             if not self.should_send_footprints():
                 return
             footprint_items = self.footprints_queue.get_all()
             if footprint_items:
                 self.footprints_service.send_footprints(footprint_items)
             else:
                 log.info("No Footprint Items. Nothing To Send")
         except Exception as e:
             log.exception("Failed Sending All Footprints. Error: %s" % str(e))
             self.footprints_queue.put_all(footprint_items)
+            if self.agent_events_manager:
+                self.agent_events_manager.send_agent_test_event_error(e)
         finally:
             self._is_sending_lock.release()
 
     def start(self):
         log.info("Starting Footprints Manager")
         try:
             self.watchdog.start()
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/managers/events_manager.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/managers/events_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,22 @@
     "executors": {'processpool': ProcessPoolExecutor(1)}
 }
 
 log = logging.getLogger(__name__)
 
 
 class EventsManager(object):
-    def __init__(self, config_data, backend_proxy):
+    def __init__(self, config_data, backend_proxy, agent_events_manager):
         self.config_data = config_data
         self.events_service = EventsService(config_data, backend_proxy)
         self.events_queue = EventsQueue(maxsize=constants.MAX_ITEMS_IN_QUEUE)
         self.watchdog = scheduler_class(**kwargs)
         self.watchdog.add_job(self.send_all, interval.IntervalTrigger(seconds=self.config_data.intervalSeconds))
         self._is_sending_lock = threading.Lock()
+        self.agent_events_manager = agent_events_manager
 
     def push_event(self, event):
         try:
             if not event:
                 return
             self.events_queue.put(event)
             log.info("Pushed Event. Event: %s" % event)
@@ -43,14 +44,17 @@
             if not events:
                 return
             log.info("Dequeued Events From Events Queue. Number Of Events: %s" % len(events))
             self.events_service.send_events(events)
         except Exception as e:
             log.exception("Failed Sending All Events. Number Of Events: %s. Error: %s " % (len(events), str(e)))
             self.events_queue.put_all(events)
+            if self.agent_events_manager:
+                self.agent_events_manager.send_agent_test_event_error(e)
+
         finally:
             self._is_sending_lock.release()
 
     def start(self):
         log.info("Starting Events Manager")
         try:
             self.watchdog.start()
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/sealights_api.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/sealights_api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/services/footprints_service.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/services/footprints_service.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/services/events_service.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/services/events_service.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/line_footprints_collector.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/line_footprints_collector.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/utils.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/method_footprints_collector.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/method_footprints_collector.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/freezegun_patcher.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/integrations/freezegun_patcher.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/multiprocessing_patcher.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/integrations/multiprocessing_patcher.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/pytest_xdist_helper.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/integrations/pytest_xdist_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/unittest_helper.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/integrations/unittest_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,22 @@
 class SealightsTestResult(unittest.TextTestResult):
 
     def __init__(self, stream, descriptions, verbosity):
         super(SealightsTestResult, self).__init__(stream, descriptions, verbosity)
         self.skipped_tests = {}
         self.error_tests = {}
         self.execution_id = SeaLightsAPI.create_execution_id()
+        self.excluded_set = {}
+        self.setTestExcludeSet()
 
+    def setTestExcludeSet(self):
+        try:
+            self.excluded_set = set([t.get("name", "") for t in SeaLightsAPI.get_excluded_tests()])
+        except Exception as e:
+            log.exception("failed getting excluded tests. error: %s" % str(e))
     def startTestRun(self):
         try:
             # startTestRun is called even when there are no tests found. We avoid it here.
             if is_has_tests:
                 SeaLightsAPI.notify_execution_start(self.execution_id)
         except Exception as e:
             log.exception("failed sending execution start. error: %s" % str(e))
@@ -35,15 +42,18 @@
             if is_has_tests:
                 SeaLightsAPI.notify_execution_end(self.execution_id)
         except Exception as e:
             log.exception("failed sending execution end. error: %s" % str(e))
         super(SealightsTestResult, self).stopTestRun()
 
     def startTest(self, test):
+
         try:
+            if test.id() in self.excluded_set:
+                setattr(test, 'setUp', lambda: test.skipTest('test skipped by SeaLights TIA'))
             test.start_time = time.time()
             SeaLightsAPI.notify_test_start(self.execution_id, test.id())
         except Exception as e:
             log.exception("failed sending test start. error: %s" % str(e))
         super(SealightsTestResult, self).startTest(test)
 
     def stopTest(self, test):
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/nose_helper.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/integrations/nose_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging.config
 import os
 import time
 from nose.plugins import Plugin
 from python_agent.test_listener.sealights_api import SeaLightsAPI
 
 log = logging.getLogger(__name__)
@@ -15,14 +16,23 @@
         self.execution_id = SeaLightsAPI.create_execution_id()
         self.error_tests = {}
         self.skipped_tests = {}
         # the nose plugin needs these 3 attributes:
         self.name = self.__class__.__name__
         self.score = 0
         self.enableOpt = 'enable_plugin_sealights'
+        self.excluded_set = {}
+        self.setTestExcludeSet()
+
+
+    def setTestExcludeSet(self):
+        try:
+            self.excluded_set = set([t.get("name", "") for t in SeaLightsAPI.get_excluded_tests()])
+        except Exception as e:
+            log.exception("failed getting excluded tests. error: %s" % str(e))
 
     def options(self, parser, env=os.environ):
         """
         Add command line options here.
         :param parser:
         :param env:
         :return:
@@ -48,14 +58,21 @@
         :param result: test result object
         """
         try:
             SeaLightsAPI.notify_execution_end(self.execution_id)
         except Exception as e:
             log.exception("failed sending execution end from nose. error: %s" % str(e))
 
+    def beforeTest(self, test):
+        if test.id() in self.excluded_set:
+            SeaLightsAPI.notify_test_start(self.execution_id, test.id())
+            SeaLightsAPI.notify_test_end(self.execution_id, test.id(), 1, "skipped")
+            test.skipTest('test skipped by SeaLights TIA')
+
+
     def startTest(self, test):
         """
         Called before test run (after beforeTest)
             :param test:
             :type test: :class:`nose.case.Test`
             see: http://nose.readthedocs.io/en/latest/api/test_cases.html#nose.case.Test:
         """
@@ -87,34 +104,31 @@
         :param test:
         :param err:
         :return:
         """
         try:
             test.end_time = time.time()
             test.duration = test.end_time = test.start_time
-
             # The error tuple holds the the type in index 0 and the exception object in index 1
             # We use the type to discover if the test is skipped.
             if str(err[0]) == "<class 'unittest.case.SkipTest'>":
                 self.skipped_tests[test.id()] = test.id()
                 SeaLightsAPI.notify_test_end(self.execution_id, test.id(), test.duration, "skipped")
             else:
                 self.error_tests[test.id()] = test.id()
                 SeaLightsAPI.notify_test_end(self.execution_id, test.id(), test.duration, "failed")
         except Exception as e:
             log.exception("failed sending test end on from nose addError. error: %s" % str(e))
 
-
     def addFailure(self, test, err):
         """
         Called when test fails (assert error)
         :param test:
         :param err:
         """
         try:
             test.end_time = time.time()
             test.duration = test.end_time - test.start_time
             self.error_tests[test.id()] = test.id()
             SeaLightsAPI.notify_test_end(self.execution_id, test.id(), test.duration, "failed")
         except Exception as e:
             log.exception("failed sending test end from nose addFailure. error: %s" % str(e))
-
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/pytest_helper.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/integrations/pytest_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/entities/upload_reports_metadata.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/entities/upload_reports_metadata.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/agent_execution.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/executors/test_frameworks/agent_execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from python_agent.common import constants
 from python_agent.test_listener.managers.agent_manager import AgentManager
 from python_agent.utils import disableable
 
 
 class AgentExecution(object):
 
-    def __init__(self, config_data, labid, test_stage=None, cov_report=None, per_test=True, interval=constants.INTERVAL_IN_MILLISECONDS, init_agent=True):
+    def __init__(self, config_data, labid, test_stage=None, cov_report=None, per_test=True, interval=constants.INTERVAL_IN_MILLISECONDS, init_agent=True, test_group_id=""):
         self.config_data = config_data
         self.test_stage = test_stage
         self.labid = self.resolve_lab_id(labid)
         self.config_data.covReport = cov_report
         self.config_data.testStage = test_stage or constants.DEFAULT_ENV
+        self.config_data.testGroupId = test_group_id
         self.config_data.labId = self.labid
         self.config_data.workspacepath = self.config_data.additionalParams.get("workspacepath", constants.DEFAULT_WORKSPACEPATH)
         self.config_data.include = self.config_data.additionalParams.get("include")
         self.config_data.exclude = self.config_data.additionalParams.get("exclude")
         self.config_data.perTest = per_test
         self.config_data.interval = interval
         self.config_data.intervalSeconds = interval / 1000
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/pytest_execution.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/executors/test_frameworks/pytest_execution.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from python_agent.utils import disableable
 
 log = logging.getLogger(__name__)
 
 
 class PytestAgentExecution(AgentExecution):
 
-    def __init__(self, config_data, labid, test_stage, cov_report, per_test, interval, args):
+    def __init__(self, config_data, labid, test_stage, cov_report, per_test, interval, test_group_id, args):
         config_data.isInitialColor = False
-        super(PytestAgentExecution, self).__init__(config_data, labid, test_stage=test_stage, cov_report=cov_report, per_test=per_test, interval=interval)
+        super(PytestAgentExecution, self).__init__(config_data, labid, test_stage=test_stage, cov_report=cov_report, per_test=per_test, interval=interval, test_group_id=test_group_id)
         self.args = args
 
     def execute(self):
         try:
             args = list(self.args)
             import pytest
             # we're appending the current working directory for customers running pytest using: "python -m pytest"
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/unittest_execution.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/executors/test_frameworks/unittest_execution.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from python_agent.test_listener.integrations.unittest_helper import unittest
 
 log = logging.getLogger(__name__)
 
 
 class UnittestAgentExecution(AgentExecution):
 
-    def __init__(self, config_data, labid, test_stage, cov_report, per_test, interval, args):
+    def __init__(self, config_data, labid, test_stage, cov_report, per_test, interval, test_group_id, args):
         config_data.isInitialColor = False
-        super(UnittestAgentExecution, self).__init__(config_data, labid, test_stage=test_stage, cov_report=cov_report, per_test=per_test, interval=interval)
+        super(UnittestAgentExecution, self).__init__(config_data, labid, test_stage=test_stage, cov_report=cov_report, per_test=per_test, interval=interval, test_group_id=test_group_id)
         self.args = args
 
     def execute(self):
         # we're appending the current working directory for customers running unittest using: "python -m unittest"
         # since running it like that adds current working directory to sys.path
         sys.path.insert(0, os.getcwd())
         if self.config_data.isDisabled:
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/nose_execution.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/executors/test_frameworks/nose_execution.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from python_agent.test_listener.executors.test_frameworks.agent_execution import AgentExecution
 from python_agent.utils import disableable
 
 log = logging.getLogger(__name__)
 
 
 class NoseAgentExecution(AgentExecution):
-    def __init__(self, config_data, labid, test_stage, cov_report, per_test, interval, args):
+    def __init__(self, config_data, labid, test_stage, cov_report, per_test, interval, test_group_id, args):
         config_data.isInitialColor = False
-        super(NoseAgentExecution, self).__init__(config_data, labid, test_stage, cov_report=cov_report, per_test=per_test, interval=interval)
+        super(NoseAgentExecution, self).__init__(config_data, labid, test_stage, cov_report=cov_report, per_test=per_test, interval=interval, test_group_id=test_group_id)
         self.args = args
 
     def execute(self):
         sys.path.insert(0, os.getcwd())
         try:
             import nose
             # first arg is ignored on parsing because it's the program name
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/executors/upload_reports.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/executors/upload_reports.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/executors/start_execution.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/executors/start_execution.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from python_agent.test_listener.entities.start_execution_request import StartExecutionRequest
 from python_agent.test_listener.executors.anonymous_execution import AnonymousExecution
 from python_agent.utils import disableable
 
 
 class StartAnonymousExecution(AnonymousExecution):
 
-    def __init__(self, config_data, test_stage, labid):
+    def __init__(self, config_data, test_stage, labid, testgroupid):
         super(StartAnonymousExecution, self).__init__(config_data, labid)
         self.test_stage = test_stage
+        self.testgroupid = testgroupid
 
     @disableable()
     def execute(self):
         start_execution_request = StartExecutionRequest(
             self.config_data.customerId,
             self.config_data.appName,
             self.config_data.branchName,
             self.config_data.buildName,
             self.labid,
-            self.test_stage
+            self.test_stage,
+            self.testgroupid
         )
         self.backend_proxy.start_execution(start_execution_request)
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/executors/run.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/executors/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import json
 import os
 
 from python_agent.common import constants
 from python_agent.test_listener.executors.test_frameworks.agent_execution import AgentExecution
 from python_agent.utils import disableable
-
+import logging
+log = logging.getLogger(__name__)
 
 class Run(AgentExecution):
     def __init__(self, config_data, labid, cov_report, per_test, interval):
         super(Run, self).__init__(config_data, labid, cov_report=cov_report, per_test=per_test, interval=interval, init_agent=False)
 
     @disableable()
     def execute(self, args):
+        log.info("Running program: %s" % ' '.join(args))
         self.inject_bootstrap_dir_to_python_path()
         program_exe_path = self.find_program_exe_path(args)
         self.save_config_as_env_variable()
         self.run_program(program_exe_path, args)
 
     def inject_bootstrap_dir_to_python_path(self):
         from python_agent import __file__ as root_directory
```

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/executors/send_footprints.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/executors/send_footprints.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/executors/anonymous_execution.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/executors/anonymous_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/test_listener/state_tracker.py` & `sealights-python-agent-1.1.0/python_agent/test_listener/state_tracker.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/__init__.py` & `sealights-python-agent-1.1.0/python_agent/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from python_agent.packages import urllib3
 from python_agent.packages.urllib3.exceptions import InsecureRequestWarning
 from logging.config import dictConfig
 
 urllib3.disable_warnings(InsecureRequestWarning)
 
-__version__ = "1.0.6"
+__version__ = "1.1.0"
 __package_name__ = "sealights-python-agent"
 
 
 LOG_CONF = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
```

### Comparing `sealights-python-agent-1.0.6/python_agent/build_scanner/scm/git_integration.py` & `sealights-python-agent-1.1.0/python_agent/build_scanner/scm/git_integration.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/build_scanner/scm/scm_info.py` & `sealights-python-agent-1.1.0/python_agent/build_scanner/scm/scm_info.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/build_scanner/file_scanner.py` & `sealights-python-agent-1.1.0/python_agent/build_scanner/file_scanner.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,34 +2,34 @@
     file_scanner module is part of the build scan process.
     For a given full python file path and its relative path:
         - Parse the code to ast
         - Traverse the tree
         - Calculate method hash for functions and lambdas
         - Calculate file hash
 """
+import ast
 import hashlib
 import logging
 import traceback
 
-from python_agent.build_scanner import ast_utils
 from python_agent.build_scanner.entities.v3.file_data import FileData
 from python_agent.build_scanner.visitors import SealightsVisitor
 from python_agent.packages import astunparse
 
 log = logging.getLogger(__name__)
 
 
 class FileScanner(object):
 
     def calculate_file_signature(self, full_path, rel_path):
         file_data = FileData(rel_path)
         try:
             with open(full_path, 'r') as f:
                 code = f.read()
-            tree = ast_utils.parse(code)
+            tree = ast.parse(code)
             file_data.hash = self.calculate_file_hash(tree)
             SealightsVisitor(file_data).visit(tree)
         except SyntaxError as e:
             file_data.error = traceback.format_exc()
             log.error("File ignored due to syntax error. %s. problematic code: (%s)" % (full_path, e.text.strip()))
         except Exception as e:
             file_data.error = traceback.format_exc()
```

### Comparing `sealights-python-agent-1.0.6/python_agent/build_scanner/visitors.py` & `sealights-python-agent-1.1.0/python_agent/build_scanner/visitors.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/build_scanner/app.py` & `sealights-python-agent-1.1.0/python_agent/build_scanner/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,16 +125,15 @@
     if len(scanned_files) != len(files):
         log.warning("Number of scanned files differs from total files: scanned=%s, total=%s"
                     % (len(scanned_files), len(files)))
     return scanned_files
 
 
 def main(config_data=None, workspacepath=None, include=None, exclude=None):
-    try:
-        scanned_files = scan_files(workspacepath, include, exclude)
-        if not scanned_files or len(scanned_files) == 0:
-            log.warning("Total scanned files is 0. Skip sending build to server")
-            return
-        body = prepare_build_request(scanned_files, config_data)
-        send_build(body, config_data)
-    except Exception as e:
-        log.exception("Failed Running Build Scan. Error: %s" % str(e))
+    scanned_files = scan_files(workspacepath, include, exclude)
+    if not scanned_files or len(scanned_files) == 0:
+        log.warning("Total scanned files is 0. Skip sending build to server")
+        return
+    body = prepare_build_request(scanned_files, config_data)
+    send_build(body, config_data)
+
+
```

### Comparing `sealights-python-agent-1.0.6/python_agent/build_scanner/method_hasher.py` & `sealights-python-agent-1.1.0/python_agent/build_scanner/method_hasher.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,14 @@
     def copy_node(self, node):
         # astunparse is not maintained anymore and creates 'wrong' code.
         # So we're using astor which creates the right code.
         # we use it in case there is an exception and not always since we do not want
         # to change hashes for all customers -> meaning, quality risks
         try:
             code = astunparse.unparse(node)
-            copied_node = ast_utils.parse(code)
+            copied_node = ast.parse(code)
             return copied_node
         except SyntaxError as e:
             log.warning("coping node using astor")
             code = astor.to_source(node)
-            copied_node = ast_utils.parse(code)
+            copied_node = ast.parse(code)
             return copied_node
```

### Comparing `sealights-python-agent-1.0.6/python_agent/build_scanner/entities/environment_data.py` & `sealights-python-agent-1.1.0/python_agent/build_scanner/entities/environment_data.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/method_data.py` & `sealights-python-agent-1.1.0/python_agent/build_scanner/entities/v3/method_data.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/file_data.py` & `sealights-python-agent-1.1.0/python_agent/build_scanner/entities/v3/file_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 
 class FileData(object):
     def __init__(self, logical_path):
+        logical_path = logical_path.replace("\\", "/")
         self.logicalPath = logical_path
         self.physicalPath = logical_path
         self.filename = self.get_filename(logical_path)
         self.hash = ''
         self.methods = []
         self.commitIndexes = []
         self.lines = []
```

### Comparing `sealights-python-agent-1.0.6/python_agent/build_scanner/executors/config.py` & `sealights-python-agent-1.1.0/python_agent/build_scanner/executors/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
 from python_agent.common.build_session.build_session_data import BuildSessionData
 from python_agent.common.constants import BUILD_SESSION_ID_FILE
 from python_agent.common.http.backend_proxy import BackendProxy
 from python_agent.utils import disableable
-
 log = logging.getLogger(__name__)
 
 
 class Config(object):
 
     def __init__(self, config_data, app_name, branch_name, build_name, build_session_id, workspacepath, include, exclude):
         self.config_data = config_data
```

### Comparing `sealights-python-agent-1.0.6/python_agent/init.py` & `sealights-python-agent-1.1.0/python_agent/init.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/blinker/_utilities.py` & `sealights-python-agent-1.1.0/python_agent/packages/blinker/_utilities.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/blinker/base.py` & `sealights-python-agent-1.1.0/python_agent/packages/blinker/base.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/blinker/_saferef.py` & `sealights-python-agent-1.1.0/python_agent/packages/blinker/_saferef.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/adapters.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/exceptions.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/packages.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/packages.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/models.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/api.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/hooks.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/cookies.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/auth.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/utils.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/help.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/help.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/_internal_utils.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/__init__.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/status_codes.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/structures.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/compat.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/requests/sessions.py` & `sealights-python-agent-1.1.0/python_agent/packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/six.py` & `sealights-python-agent-1.1.0/python_agent/packages/six.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/certifi/cacert.pem` & `sealights-python-agent-1.1.0/python_agent/packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/certifi/core.py` & `sealights-python-agent-1.1.0/python_agent/packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jws.py` & `sealights-python-agent-1.1.0/python_agent/packages/jwt/api_jws.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/jwt/exceptions.py` & `sealights-python-agent-1.1.0/python_agent/packages/jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/jwt/jwks_client.py` & `sealights-python-agent-1.1.0/python_agent/packages/jwt/jwks_client.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jwt.py` & `sealights-python-agent-1.1.0/python_agent/packages/jwt/api_jwt.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/jwt/algorithms.py` & `sealights-python-agent-1.1.0/python_agent/packages/jwt/algorithms.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jwk.py` & `sealights-python-agent-1.1.0/python_agent/packages/jwt/api_jwk.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/jwt/utils.py` & `sealights-python-agent-1.1.0/python_agent/packages/jwt/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/jwt/help.py` & `sealights-python-agent-1.1.0/python_agent/packages/jwt/help.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/jwt/__init__.py` & `sealights-python-agent-1.1.0/python_agent/packages/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astunparse/__main__.py` & `sealights-python-agent-1.1.0/python_agent/packages/astunparse/__main__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser36.py` & `sealights-python-agent-1.1.0/python_agent/packages/astunparse/unparser36.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astunparse/printer.py` & `sealights-python-agent-1.1.0/python_agent/packages/astunparse/printer.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser.py` & `sealights-python-agent-1.1.0/python_agent/packages/astunparse/unparser.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser37.py` & `sealights-python-agent-1.1.0/python_agent/packages/astunparse/unparser37.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astor/string_repr.py` & `sealights-python-agent-1.1.0/python_agent/packages/astor/string_repr.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astor/code_gen.py` & `sealights-python-agent-1.1.0/python_agent/packages/astor/code_gen.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astor/file_util.py` & `sealights-python-agent-1.1.0/python_agent/packages/astor/file_util.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astor/source_repr.py` & `sealights-python-agent-1.1.0/python_agent/packages/astor/source_repr.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astor/node_util.py` & `sealights-python-agent-1.1.0/python_agent/packages/astor/node_util.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astor/__init__.py` & `sealights-python-agent-1.1.0/python_agent/packages/astor/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astor/rtrip.py` & `sealights-python-agent-1.1.0/python_agent/packages/astor/rtrip.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astor/tree_walk.py` & `sealights-python-agent-1.1.0/python_agent/packages/astor/tree_walk.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/astor/op_util.py` & `sealights-python-agent-1.1.0/python_agent/packages/astor/op_util.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/typing_extensions.py` & `sealights-python-agent-1.1.0/python_agent/packages/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_adapters.py` & `sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_text.py` & `sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_collections.py` & `sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_compat.py` & `sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_functools.py` & `sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_meta.py` & `sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_itertools.py` & `sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/__init__.py` & `sealights-python-agent-1.1.0/python_agent/packages/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/zipp.py` & `sealights-python-agent-1.1.0/python_agent/packages/zipp.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/_textwrap.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/exceptions.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/testing.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/testing.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/types.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ._compat import get_filesystem_encoding
 from ._compat import open_stream
 from .exceptions import BadParameter
 from .utils import LazyFile
 from .utils import safecall
 
 if t.TYPE_CHECKING:
-    import python_agent.packages.typing_extensions as te
+    import typing_extensions as te
     from .core import Context
     from .core import Parameter
     from .shell_completion import CompletionItem
 
 
 class ParamType:
     """Represents the type of a parameter. Validates and converts values
@@ -59,15 +59,22 @@
         CLI structure.
 
         .. versionadded:: 8.0
         """
         # The class name without the "ParamType" suffix.
         param_type = type(self).__name__.partition("ParamType")[0]
         param_type = param_type.partition("ParameterType")[0]
-        return {"param_type": param_type, "name": self.name}
+
+        # Custom subclasses might not remember to set a name.
+        if hasattr(self, "name"):
+            name = self.name
+        else:
+            name = param_type
+
+        return {"param_type": param_type, "name": name}
 
     def __call__(
         self,
         value: t.Any,
         param: t.Optional["Parameter"] = None,
         ctx: t.Optional["Context"] = None,
     ) -> t.Any:
@@ -720,15 +727,15 @@
                 if should_close:
                     ctx.call_on_close(safecall(f.close))
                 else:
                     ctx.call_on_close(safecall(f.flush))
 
             return f
         except OSError as e:  # noqa: B014
-            self.fail(f"{os.fsdecode(value)!r}: {e.strerror}", param, ctx)
+            self.fail(f"'{os.fsdecode(value)}': {e.strerror}", param, ctx)
 
     def shell_complete(
         self, ctx: "Context", param: "Parameter", incomplete: str
     ) -> t.List["CompletionItem"]:
         """Return a special completion marker that tells the completion
         system to use the shell to provide file path completions.
 
@@ -749,26 +756,30 @@
     enabled to validate the type of file and permissions.
 
     :param exists: The file or directory needs to exist for the value to
         be valid. If this is not set to ``True``, and the file does not
         exist, then all further checks are silently skipped.
     :param file_okay: Allow a file as a value.
     :param dir_okay: Allow a directory as a value.
-    :param writable: The file or directory must be writable.
-    :param readable: The file or directory must be readable.
+    :param readable: if true, a readable check is performed.
+    :param writable: if true, a writable check is performed.
+    :param executable: if true, an executable check is performed.
     :param resolve_path: Make the value absolute and resolve any
         symlinks. A ``~`` is not expanded, as this is supposed to be
         done by the shell only.
     :param allow_dash: Allow a single dash as a value, which indicates
         a standard stream (but does not open it). Use
         :func:`~click.open_file` to handle opening this value.
     :param path_type: Convert the incoming path value to this type. If
         ``None``, keep Python's default, which is ``str``. Useful to
         convert to :class:`pathlib.Path`.
 
+    .. versionchanged:: 8.1
+        Added the ``executable`` parameter.
+
     .. versionchanged:: 8.0
         Allow passing ``type=pathlib.Path``.
 
     .. versionchanged:: 6.0
         Added the ``allow_dash`` parameter.
     """
 
@@ -780,20 +791,22 @@
         file_okay: bool = True,
         dir_okay: bool = True,
         writable: bool = False,
         readable: bool = True,
         resolve_path: bool = False,
         allow_dash: bool = False,
         path_type: t.Optional[t.Type] = None,
+        executable: bool = False,
     ):
         self.exists = exists
         self.file_okay = file_okay
         self.dir_okay = dir_okay
-        self.writable = writable
         self.readable = readable
+        self.writable = writable
+        self.executable = executable
         self.resolve_path = resolve_path
         self.allow_dash = allow_dash
         self.type = path_type
 
         if self.file_okay and not self.dir_okay:
             self.name = _("file")
         elif self.dir_okay and not self.file_okay:
@@ -858,31 +871,42 @@
                         name=self.name.title(), filename=os.fsdecode(value)
                     ),
                     param,
                     ctx,
                 )
             if not self.dir_okay and stat.S_ISDIR(st.st_mode):
                 self.fail(
-                    _("{name} {filename!r} is a directory.").format(
+                    _("{name} '{filename}' is a directory.").format(
                         name=self.name.title(), filename=os.fsdecode(value)
                     ),
                     param,
                     ctx,
                 )
+
+            if self.readable and not os.access(rv, os.R_OK):
+                self.fail(
+                    _("{name} {filename!r} is not readable.").format(
+                        name=self.name.title(), filename=os.fsdecode(value)
+                    ),
+                    param,
+                    ctx,
+                )
+
             if self.writable and not os.access(rv, os.W_OK):
                 self.fail(
                     _("{name} {filename!r} is not writable.").format(
                         name=self.name.title(), filename=os.fsdecode(value)
                     ),
                     param,
                     ctx,
                 )
-            if self.readable and not os.access(rv, os.R_OK):
+
+            if self.executable and not os.access(value, os.X_OK):
                 self.fail(
-                    _("{name} {filename!r} is not readable.").format(
+                    _("{name} {filename!r} is not executable.").format(
                         name=self.name.title(), filename=os.fsdecode(value)
                     ),
                     param,
                     ctx,
                 )
 
         return self.coerce_path_result(rv)
```

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/_termui_impl.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/_compat.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/_compat.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/_unicodefun.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/_winconsole.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/globals.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/globals.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as t
 from threading import local
 
 if t.TYPE_CHECKING:
-    import python_agent.packages.typing_extensions as te
+    import typing_extensions as te
     from .core import Context
 
 _local = local()
 
 
 @t.overload
 def get_current_context(silent: "te.Literal[False]" = False) -> "Context":
```

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/utils.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import re
 import sys
 import typing as t
 from functools import update_wrapper
 from types import ModuleType
 
 from ._compat import _default_text_stderr
 from ._compat import _default_text_stdout
@@ -14,15 +15,15 @@
 from ._compat import should_strip_ansi
 from ._compat import strip_ansi
 from ._compat import text_streams
 from ._compat import WIN
 from .globals import resolve_color_default
 
 if t.TYPE_CHECKING:
-    import python_agent.packages.typing_extensions as te
+    import typing_extensions as te
 
 F = t.TypeVar("F", bound=t.Callable[..., t.Any])
 
 
 def _posixify(name: str) -> str:
     return "-".join(name.split()).lower()
 
@@ -375,33 +376,14 @@
 
     if not should_close:
         f = t.cast(t.IO, KeepOpenFile(f))
 
     return f
 
 
-def get_os_args() -> t.Sequence[str]:
-    """Returns the argument part of ``sys.argv``, removing the first
-    value which is the name of the script.
-
-    .. deprecated:: 8.0
-        Will be removed in Click 8.1. Access ``sys.argv[1:]`` directly
-        instead.
-    """
-    import warnings
-
-    warnings.warn(
-        "'get_os_args' is deprecated and will be removed in Click 8.1."
-        " Access 'sys.argv[1:]' directly instead.",
-        DeprecationWarning,
-        stacklevel=2,
-    )
-    return sys.argv[1:]
-
-
 def format_filename(
     filename: t.Union[str, bytes, os.PathLike], shorten: bool = False
 ) -> str:
     """Formats a filename for user display.  The main purpose of this
     function is to ensure that the filename can be displayed at all.  This
     will decode the filename to unicode if necessary in a way that it will
     not fail.  Optionally, it can shorten the filename to not include the
@@ -489,15 +471,15 @@
                 raise
 
     def __getattr__(self, attr: str) -> t.Any:
         return getattr(self.wrapped, attr)
 
 
 def _detect_program_name(
-    path: t.Optional[str] = None, _main: ModuleType = sys.modules["__main__"]
+    path: t.Optional[str] = None, _main: t.Optional[ModuleType] = None
 ) -> str:
     """Determine the command used to run the program, for use in help
     text. If a file or entry point was executed, the file name is
     returned. If ``python -m`` was used to execute a module or package,
     ``python -m name`` is returned.
 
     This doesn't try to be too precise, the goal is to give a concise
@@ -511,14 +493,17 @@
         during internal testing.
 
     .. versionadded:: 8.0
         Based on command args detection in the Werkzeug reloader.
 
     :meta private:
     """
+    if _main is None:
+        _main = sys.modules["__main__"]
+
     if not path:
         path = sys.argv[0]
 
     # The value of __package__ indicates how Python was called. It may
     # not exist if a setuptools script is installed as an egg. It may be
     # set incorrectly for entry points created with pip on Windows.
     if getattr(_main, "__package__", None) is None or (
@@ -551,22 +536,26 @@
     glob_recursive: bool = True,
 ) -> t.List[str]:
     """Simulate Unix shell expansion with Python functions.
 
     See :func:`glob.glob`, :func:`os.path.expanduser`, and
     :func:`os.path.expandvars`.
 
-    This intended for use on Windows, where the shell does not do any
+    This is intended for use on Windows, where the shell does not do any
     expansion. It may not exactly match what a Unix shell would do.
 
     :param args: List of command line arguments to expand.
     :param user: Expand user home directory.
     :param env: Expand environment variables.
     :param glob_recursive: ``**`` matches directories recursively.
 
+    .. versionchanged:: 8.1
+        Invalid glob patterns are treated as empty expansions rather
+        than raising an error.
+
     .. versionadded:: 8.0
 
     :meta private:
     """
     from glob import glob
 
     out = []
@@ -574,15 +563,18 @@
     for arg in args:
         if user:
             arg = os.path.expanduser(arg)
 
         if env:
             arg = os.path.expandvars(arg)
 
-        matches = glob(arg, recursive=glob_recursive)
+        try:
+            matches = glob(arg, recursive=glob_recursive)
+        except re.error:
+            matches = []
 
         if not matches:
             out.append(arg)
         else:
             out.extend(matches)
 
     return out
```

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/parser.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from .exceptions import BadArgumentUsage
 from .exceptions import BadOptionUsage
 from .exceptions import NoSuchOption
 from .exceptions import UsageError
 
 if t.TYPE_CHECKING:
-    import python_agent.packages.typing_extensions as te
+    import typing_extensions as te
     from .core import Argument as CoreArgument
     from .core import Context
     from .core import Option as CoreOption
     from .core import Parameter as CoreParameter
 
 V = t.TypeVar("V")
```

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/__init__.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 from .formatting import wrap_text as wrap_text
 from .globals import get_current_context as get_current_context
 from .parser import OptionParser as OptionParser
 from .termui import clear as clear
 from .termui import confirm as confirm
 from .termui import echo_via_pager as echo_via_pager
 from .termui import edit as edit
-from .termui import get_terminal_size as get_terminal_size
 from .termui import getchar as getchar
 from .termui import launch as launch
 from .termui import pause as pause
 from .termui import progressbar as progressbar
 from .termui import prompt as prompt
 from .termui import secho as secho
 from .termui import style as style
@@ -64,12 +63,11 @@
 from .types import Tuple as Tuple
 from .types import UNPROCESSED as UNPROCESSED
 from .types import UUID as UUID
 from .utils import echo as echo
 from .utils import format_filename as format_filename
 from .utils import get_app_dir as get_app_dir
 from .utils import get_binary_stream as get_binary_stream
-from .utils import get_os_args as get_os_args
 from .utils import get_text_stream as get_text_stream
 from .utils import open_file as open_file
 
-__version__ = "8.0.4"
+__version__ = "8.1.3"
```

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/core.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from functools import partial
 from functools import update_wrapper
 from gettext import gettext as _
 from gettext import ngettext
 from itertools import repeat
 
 from . import types
-from ._unicodefun import _verify_python_env
 from .exceptions import Abort
 from .exceptions import BadParameter
 from .exceptions import ClickException
 from .exceptions import Exit
 from .exceptions import MissingParameter
 from .exceptions import UsageError
 from .formatting import HelpFormatter
@@ -35,15 +34,15 @@
 from .utils import _expand_args
 from .utils import echo
 from .utils import make_default_short_help
 from .utils import make_str
 from .utils import PacifyFlushWrapper
 
 if t.TYPE_CHECKING:
-    import python_agent.packages.typing_extensions as te
+    import typing_extensions as te
     from .shell_completion import CompletionItem
 
 F = t.TypeVar("F", bound=t.Callable[..., t.Any])
 V = t.TypeVar("V")
 
 
 def _complete_visible_commands(
@@ -220,17 +219,22 @@
                                  etc.).  This for instance can be used to
                                  implement case insensitive behavior.
     :param color: controls if the terminal supports ANSI colors or not.  The
                   default is autodetection.  This is only needed if ANSI
                   codes are used in texts that Click prints which is by
                   default not the case.  This for instance would affect
                   help output.
-    :param show_default: Show defaults for all options. If not set,
-        defaults to the value from a parent context. Overrides an
-        option's ``show_default`` argument.
+    :param show_default: Show the default value for commands. If this
+        value is not set, it defaults to the value from the parent
+        context. ``Command.show_default`` overrides this default for the
+        specific command.
+
+    .. versionchanged:: 8.1
+        The ``show_default`` parameter is overridden by
+        ``Command.show_default``, instead of the other way around.
 
     .. versionchanged:: 8.0
         The ``show_default`` parameter defaults to the value from the
         parent context.
 
     .. versionchanged:: 7.1
        Added the ``show_default`` parameter.
@@ -284,14 +288,16 @@
         #: the leftover arguments.
         self.args: t.List[str] = []
         #: protected arguments.  These are arguments that are prepended
         #: to `args` when certain parsing scenarios are encountered but
         #: must be never propagated to another arguments.  This is used
         #: to implement nested parsing.
         self.protected_args: t.List[str] = []
+        #: the collected prefixes of the command's options.
+        self._opt_prefixes: t.Set[str] = set(parent._opt_prefixes) if parent else set()
 
         if obj is None and parent is not None:
             obj = parent.obj
 
         #: the user object stored.
         self.obj: t.Any = obj
         self._meta: t.Dict[str, t.Any] = getattr(parent, "meta", {})
@@ -1025,18 +1031,14 @@
         .. versionchanged:: 8.0
             When taking arguments from ``sys.argv`` on Windows, glob
             patterns, user dir, and env vars are expanded.
 
         .. versionchanged:: 3.0
            Added the ``standalone_mode`` parameter.
         """
-        # Verify that the environment is configured correctly, or reject
-        # further execution to avoid a broken script.
-        _verify_python_env()
-
         if args is None:
             args = sys.argv[1:]
 
             if os.name == "nt" and windows_expand_args:
                 args = _expand_args(args)
         else:
             args = list(args)
@@ -1129,21 +1131,14 @@
 
 
 class Command(BaseCommand):
     """Commands are the basic building block of command line interfaces in
     Click.  A basic command handles command line parsing and might dispatch
     more parsing to commands nested below it.
 
-    .. versionchanged:: 2.0
-       Added the `context_settings` parameter.
-    .. versionchanged:: 8.0
-       Added repr showing the command name
-    .. versionchanged:: 7.1
-       Added the `no_args_is_help` parameter.
-
     :param name: the name of the command to use unless a group overrides it.
     :param context_settings: an optional dictionary with defaults that are
                              passed to the context object.
     :param callback: the callback to invoke.  This is optional.
     :param params: the parameters to register with this command.  This can
                    be either :class:`Option` or :class:`Argument` objects.
     :param help: the help string to use for this command.
@@ -1157,14 +1152,28 @@
                             provided.  This option is disabled by default.
                             If enabled this will add ``--help`` as argument
                             if no arguments are passed
     :param hidden: hide this command from help outputs.
 
     :param deprecated: issues a message indicating that
                              the command is deprecated.
+
+    .. versionchanged:: 8.1
+        ``help``, ``epilog``, and ``short_help`` are stored unprocessed,
+        all formatting is done when outputting help text, not at init,
+        and is done even if not using the ``@command`` decorator.
+
+    .. versionchanged:: 8.0
+        Added a ``repr`` showing the command name.
+
+    .. versionchanged:: 7.1
+        Added the ``no_args_is_help`` parameter.
+
+    .. versionchanged:: 2.0
+        Added the ``context_settings`` parameter.
     """
 
     def __init__(
         self,
         name: t.Optional[str],
         context_settings: t.Optional[t.Dict[str, t.Any]] = None,
         callback: t.Optional[t.Callable[..., t.Any]] = None,
@@ -1182,20 +1191,14 @@
         #: the callback to execute when the command fires.  This might be
         #: `None` in which case nothing happens.
         self.callback = callback
         #: the list of parameters for this command in the order they
         #: should show up in the help page and execute.  Eager parameters
         #: will automatically be handled before non eager ones.
         self.params: t.List["Parameter"] = params or []
-
-        # if a form feed (page break) is found in the help text, truncate help
-        # text to the content preceding the first form feed
-        if help and "\f" in help:
-            help = help.split("\f", 1)[0]
-
         self.help = help
         self.epilog = epilog
         self.options_metavar = options_metavar
         self.short_help = short_help
         self.add_help_option = add_help_option
         self.no_args_is_help = no_args_is_help
         self.hidden = hidden
@@ -1295,18 +1298,20 @@
         self.format_help(ctx, formatter)
         return formatter.getvalue().rstrip("\n")
 
     def get_short_help_str(self, limit: int = 45) -> str:
         """Gets short help for the command or makes it by shortening the
         long help string.
         """
-        text = self.short_help or ""
-
-        if not text and self.help:
+        if self.short_help:
+            text = inspect.cleandoc(self.short_help)
+        elif self.help:
             text = make_default_short_help(self.help, limit)
+        else:
+            text = ""
 
         if self.deprecated:
             text = _("(Deprecated) {text}").format(text=text)
 
         return text.strip()
 
     def format_help(self, ctx: Context, formatter: HelpFormatter) -> None:
@@ -1324,20 +1329,21 @@
         self.format_usage(ctx, formatter)
         self.format_help_text(ctx, formatter)
         self.format_options(ctx, formatter)
         self.format_epilog(ctx, formatter)
 
     def format_help_text(self, ctx: Context, formatter: HelpFormatter) -> None:
         """Writes the help text to the formatter if it exists."""
-        text = self.help or ""
+        text = self.help if self.help is not None else ""
 
         if self.deprecated:
             text = _("(Deprecated) {text}").format(text=text)
 
         if text:
+            text = inspect.cleandoc(text).partition("\f")[0]
             formatter.write_paragraph()
 
             with formatter.indentation():
                 formatter.write_text(text)
 
     def format_options(self, ctx: Context, formatter: HelpFormatter) -> None:
         """Writes all the options into the formatter if they exist."""
@@ -1350,17 +1356,19 @@
         if opts:
             with formatter.section(_("Options")):
                 formatter.write_dl(opts)
 
     def format_epilog(self, ctx: Context, formatter: HelpFormatter) -> None:
         """Writes the epilog into the formatter if it exists."""
         if self.epilog:
+            epilog = inspect.cleandoc(self.epilog)
             formatter.write_paragraph()
+
             with formatter.indentation():
-                formatter.write_text(self.epilog)
+                formatter.write_text(epilog)
 
     def parse_args(self, ctx: Context, args: t.List[str]) -> t.List[str]:
         if not args and self.no_args_is_help and not ctx.resilient_parsing:
             echo(ctx.get_help(), color=ctx.color)
             ctx.exit()
 
         parser = self.make_parser(ctx)
@@ -1375,14 +1383,15 @@
                     "Got unexpected extra argument ({args})",
                     "Got unexpected extra arguments ({args})",
                     len(args),
                 ).format(args=" ".join(map(str, args)))
             )
 
         ctx.args = args
+        ctx._opt_prefixes.update(parser._opt_prefixes)
         return args
 
     def invoke(self, ctx: Context) -> t.Any:
         """Given a context, this invokes the attached callback (if it exists)
         in the right way.
         """
         if self.deprecated:
@@ -1564,25 +1573,14 @@
                 return f(inner, *args, **kwargs)
 
             self._result_callback = rv = update_wrapper(t.cast(F, function), f)
             return rv
 
         return decorator
 
-    def resultcallback(self, replace: bool = False) -> t.Callable[[F], F]:
-        import warnings
-
-        warnings.warn(
-            "'resultcallback' has been renamed to 'result_callback'."
-            " The old name will be removed in Click 8.1.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.result_callback(replace=replace)
-
     def format_commands(self, ctx: Context, formatter: HelpFormatter) -> None:
         """Extra format methods for multi methods that adds all the commands
         after the options.
         """
         commands = []
         for subcommand in self.list_commands(ctx):
             cmd = self.get_command(ctx, subcommand)
@@ -1627,19 +1625,19 @@
             if self._result_callback is not None:
                 value = ctx.invoke(self._result_callback, value, **ctx.params)
             return value
 
         if not ctx.protected_args:
             if self.invoke_without_command:
                 # No subcommand was invoked, so the result callback is
-                # invoked with None for regular groups, or an empty list
-                # for chained groups.
+                # invoked with the group return value for regular
+                # groups, or an empty list for chained groups.
                 with ctx:
-                    super().invoke(ctx)
-                    return _process_result([] if self.chain else None)
+                    rv = super().invoke(ctx)
+                    return _process_result([] if self.chain else rv)
             ctx.fail(_("Missing command."))
 
         # Fetch args back out
         args = [*ctx.protected_args, *ctx.args]
         ctx.args = []
         ctx.protected_args = []
 
@@ -1807,67 +1805,117 @@
         """
         name = name or cmd.name
         if name is None:
             raise TypeError("Command has no name.")
         _check_multicommand(self, name, cmd, register=True)
         self.commands[name] = cmd
 
+    @t.overload
+    def command(self, __func: t.Callable[..., t.Any]) -> Command:
+        ...
+
+    @t.overload
     def command(
         self, *args: t.Any, **kwargs: t.Any
     ) -> t.Callable[[t.Callable[..., t.Any]], Command]:
+        ...
+
+    def command(
+        self, *args: t.Any, **kwargs: t.Any
+    ) -> t.Union[t.Callable[[t.Callable[..., t.Any]], Command], Command]:
         """A shortcut decorator for declaring and attaching a command to
         the group. This takes the same arguments as :func:`command` and
         immediately registers the created command with this group by
         calling :meth:`add_command`.
 
         To customize the command class used, set the
         :attr:`command_class` attribute.
 
+        .. versionchanged:: 8.1
+            This decorator can be applied without parentheses.
+
         .. versionchanged:: 8.0
             Added the :attr:`command_class` attribute.
         """
         from .decorators import command
 
-        if self.command_class is not None and "cls" not in kwargs:
+        if self.command_class and kwargs.get("cls") is None:
             kwargs["cls"] = self.command_class
 
+        func: t.Optional[t.Callable] = None
+
+        if args and callable(args[0]):
+            assert (
+                len(args) == 1 and not kwargs
+            ), "Use 'command(**kwargs)(callable)' to provide arguments."
+            (func,) = args
+            args = ()
+
         def decorator(f: t.Callable[..., t.Any]) -> Command:
-            cmd = command(*args, **kwargs)(f)
+            cmd: Command = command(*args, **kwargs)(f)
             self.add_command(cmd)
             return cmd
 
+        if func is not None:
+            return decorator(func)
+
         return decorator
 
+    @t.overload
+    def group(self, __func: t.Callable[..., t.Any]) -> "Group":
+        ...
+
+    @t.overload
     def group(
         self, *args: t.Any, **kwargs: t.Any
     ) -> t.Callable[[t.Callable[..., t.Any]], "Group"]:
+        ...
+
+    def group(
+        self, *args: t.Any, **kwargs: t.Any
+    ) -> t.Union[t.Callable[[t.Callable[..., t.Any]], "Group"], "Group"]:
         """A shortcut decorator for declaring and attaching a group to
         the group. This takes the same arguments as :func:`group` and
         immediately registers the created group with this group by
         calling :meth:`add_command`.
 
         To customize the group class used, set the :attr:`group_class`
         attribute.
 
+        .. versionchanged:: 8.1
+            This decorator can be applied without parentheses.
+
         .. versionchanged:: 8.0
             Added the :attr:`group_class` attribute.
         """
         from .decorators import group
 
-        if self.group_class is not None and "cls" not in kwargs:
+        func: t.Optional[t.Callable] = None
+
+        if args and callable(args[0]):
+            assert (
+                len(args) == 1 and not kwargs
+            ), "Use 'group(**kwargs)(callable)' to provide arguments."
+            (func,) = args
+            args = ()
+
+        if self.group_class is not None and kwargs.get("cls") is None:
             if self.group_class is type:
                 kwargs["cls"] = type(self)
             else:
                 kwargs["cls"] = self.group_class
 
         def decorator(f: t.Callable[..., t.Any]) -> "Group":
-            cmd = group(*args, **kwargs)(f)
+            cmd: Group = group(*args, **kwargs)(f)
             self.add_command(cmd)
             return cmd
 
+        if func is not None:
+            return decorator(func)
+
         return decorator
 
     def get_command(self, ctx: Context, cmd_name: str) -> t.Optional[Command]:
         return self.commands.get(cmd_name)
 
     def list_commands(self, ctx: Context) -> t.List[str]:
         return sorted(self.commands)
@@ -2016,19 +2064,14 @@
         envvar: t.Optional[t.Union[str, t.Sequence[str]]] = None,
         shell_complete: t.Optional[
             t.Callable[
                 [Context, "Parameter", str],
                 t.Union[t.List["CompletionItem"], t.List[str]],
             ]
         ] = None,
-        autocompletion: t.Optional[
-            t.Callable[
-                [Context, t.List[str], str], t.List[t.Union[t.Tuple[str, str], str]]
-            ]
-        ] = None,
     ) -> None:
         self.name, self.opts, self.secondary_opts = self._parse_decls(
             param_decls or (), expose_value
         )
         self.type = types.convert_type(type, default)
 
         # Default nargs to what the type tells us if we have that
@@ -2044,44 +2087,14 @@
         self.nargs = nargs
         self.multiple = multiple
         self.expose_value = expose_value
         self.default = default
         self.is_eager = is_eager
         self.metavar = metavar
         self.envvar = envvar
-
-        if autocompletion is not None:
-            import warnings
-
-            warnings.warn(
-                "'autocompletion' is renamed to 'shell_complete'. The old name is"
-                " deprecated and will be removed in Click 8.1. See the docs about"
-                " 'Parameter' for information about new behavior.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-
-            def shell_complete(
-                ctx: Context, param: "Parameter", incomplete: str
-            ) -> t.List["CompletionItem"]:
-                from click.shell_completion import CompletionItem
-
-                out = []
-
-                for c in autocompletion(ctx, [], incomplete):  # type: ignore
-                    if isinstance(c, tuple):
-                        c = CompletionItem(c[0], help=c[1])
-                    elif isinstance(c, str):
-                        c = CompletionItem(c)
-
-                    if c.value.startswith(incomplete):
-                        out.append(c)
-
-                return out
-
         self._custom_shell_complete = shell_complete
 
         if __debug__:
             if self.type.is_composite and nargs != self.type.arity:
                 raise ValueError(
                     f"'nargs' must be {self.type.arity} (or None) for"
                     f" type {self.type!r}, but it was {nargs}."
@@ -2395,33 +2408,35 @@
 
 class Option(Parameter):
     """Options are usually optional values on the command line and
     have some extra features that arguments don't have.
 
     All other parameters are passed onwards to the parameter constructor.
 
-    :param show_default: controls if the default value should be shown on the
-                         help page. Normally, defaults are not shown. If this
-                         value is a string, it shows the string instead of the
-                         value. This is particularly useful for dynamic options.
-    :param show_envvar: controls if an environment variable should be shown on
-                        the help page.  Normally, environment variables
-                        are not shown.
-    :param prompt: if set to `True` or a non empty string then the user will be
-                   prompted for input.  If set to `True` the prompt will be the
-                   option name capitalized.
+    :param show_default: Show the default value for this option in its
+        help text. Values are not shown by default, unless
+        :attr:`Context.show_default` is ``True``. If this value is a
+        string, it shows that string in parentheses instead of the
+        actual value. This is particularly useful for dynamic options.
+        For single option boolean flags, the default remains hidden if
+        its value is ``False``.
+    :param show_envvar: Controls if an environment variable should be
+        shown on the help page. Normally, environment variables are not
+        shown.
+    :param prompt: If set to ``True`` or a non empty string then the
+        user will be prompted for input. If set to ``True`` the prompt
+        will be the option name capitalized.
     :param confirmation_prompt: Prompt a second time to confirm the
         value if it was prompted for. Can be set to a string instead of
         ``True`` to customize the message.
     :param prompt_required: If set to ``False``, the user will be
         prompted for input only when the option was specified as a flag
         without a value.
-    :param hide_input: if this is `True` then the input on the prompt will be
-                       hidden from the user.  This is useful for password
-                       input.
+    :param hide_input: If this is ``True`` then the input on the prompt
+        will be hidden from the user. This is useful for password input.
     :param is_flag: forces this option to act as a flag.  The default is
                     auto detection.
     :param flag_value: which value should be used for this flag if it's
                        enabled.  This is set to a boolean automatically if
                        the option string contains a slash to mark two options.
     :param multiple: if this is set to `True` then the argument is accepted
                      multiple times and recorded.  This is similar to ``nargs``
@@ -2431,24 +2446,36 @@
     :param allow_from_autoenv: if this is enabled then the value of this
                                parameter will be pulled from an environment
                                variable in case a prefix is defined on the
                                context.
     :param help: the help string.
     :param hidden: hide this option from help outputs.
 
+    .. versionchanged:: 8.1.0
+        Help text indentation is cleaned here instead of only in the
+        ``@option`` decorator.
+
+    .. versionchanged:: 8.1.0
+        The ``show_default`` parameter overrides
+        ``Context.show_default``.
+
+    .. versionchanged:: 8.1.0
+        The default of a single option boolean flag is not shown if the
+        default value is ``False``.
+
     .. versionchanged:: 8.0.1
         ``type`` is detected from ``flag_value`` if given.
     """
 
     param_type_name = "option"
 
     def __init__(
         self,
         param_decls: t.Optional[t.Sequence[str]] = None,
-        show_default: t.Union[bool, str] = False,
+        show_default: t.Union[bool, str, None] = None,
         prompt: t.Union[bool, str] = False,
         confirmation_prompt: t.Union[bool, str] = False,
         prompt_required: bool = True,
         hide_input: bool = False,
         is_flag: t.Optional[bool] = None,
         flag_value: t.Optional[t.Any] = None,
         multiple: bool = False,
@@ -2457,14 +2484,17 @@
         type: t.Optional[t.Union[types.ParamType, t.Any]] = None,
         help: t.Optional[str] = None,
         hidden: bool = False,
         show_choices: bool = True,
         show_envvar: bool = False,
         **attrs: t.Any,
     ) -> None:
+        if help:
+            help = inspect.cleandoc(help)
+
         default_is_missing = "default" not in attrs
         super().__init__(param_decls, type=type, multiple=multiple, **attrs)
 
         if prompt is True:
             if self.name is None:
                 raise TypeError("'name' is required with 'prompt=True'.")
 
@@ -2495,15 +2525,15 @@
                 # Implicitly a flag because flag options were given.
                 is_flag = bool(self.secondary_opts)
         elif is_flag is False and not self._flag_needs_value:
             # Not a flag, and prompt is not enabled, can be used as a
             # flag if flag_value is set.
             self._flag_needs_value = flag_value is not None
 
-        if is_flag and default_is_missing:
+        if is_flag and default_is_missing and not self.required:
             self.default: t.Union[t.Any, t.Callable[[], t.Any]] = False
 
         if flag_value is None:
             flag_value = not self.default
 
         if is_flag and type is None:
             # Re-guess the type from the flag value instead of the
@@ -2546,14 +2576,17 @@
             if self.count:
                 if self.multiple:
                     raise TypeError("'count' is not valid with 'multiple'.")
 
                 if self.is_flag:
                     raise TypeError("'count' is not valid with 'is_flag'.")
 
+            if self.multiple and self.is_flag:
+                raise TypeError("'multiple' is not valid with 'is_flag', use 'count'.")
+
     def to_info_dict(self) -> t.Dict[str, t.Any]:
         info_dict = super().to_info_dict()
         info_dict.update(
             help=self.help,
             prompt=self.prompt,
             is_flag=self.is_flag,
             flag_value=self.flag_value,
@@ -2707,31 +2740,40 @@
         ctx.resilient_parsing = True
 
         try:
             default_value = self.get_default(ctx, call=False)
         finally:
             ctx.resilient_parsing = resilient
 
-        show_default_is_str = isinstance(self.show_default, str)
+        show_default = False
+        show_default_is_str = False
 
-        if show_default_is_str or (
-            default_value is not None and (self.show_default or ctx.show_default)
-        ):
+        if self.show_default is not None:
+            if isinstance(self.show_default, str):
+                show_default_is_str = show_default = True
+            else:
+                show_default = self.show_default
+        elif ctx.show_default is not None:
+            show_default = ctx.show_default
+
+        if show_default_is_str or (show_default and (default_value is not None)):
             if show_default_is_str:
                 default_string = f"({self.show_default})"
             elif isinstance(default_value, (list, tuple)):
                 default_string = ", ".join(str(d) for d in default_value)
             elif inspect.isfunction(default_value):
                 default_string = _("(dynamic)")
             elif self.is_bool_flag and self.secondary_opts:
                 # For boolean flags that have distinct True/False opts,
                 # use the opt without prefix instead of the value.
                 default_string = split_opt(
                     (self.opts if self.default else self.secondary_opts)[0]
                 )[1]
+            elif self.is_bool_flag and not self.secondary_opts and not default_value:
+                default_string = ""
             else:
                 default_string = str(default_value)
 
             if default_string:
                 extra.append(_("default: {default}").format(default=default_string))
 
         if (
@@ -2817,15 +2859,18 @@
             self.allow_from_autoenv
             and ctx.auto_envvar_prefix is not None
             and self.name is not None
         ):
             envvar = f"{ctx.auto_envvar_prefix}_{self.name.upper()}"
             rv = os.environ.get(envvar)
 
-        return rv
+            if rv:
+                return rv
+
+        return None
 
     def value_from_envvar(self, ctx: Context) -> t.Optional[t.Any]:
         rv: t.Optional[t.Any] = self.resolve_envvar_value(ctx)
 
         if rv is None:
             return None
```

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/decorators.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,87 +117,151 @@
     decorator.__doc__ = (
         f"Decorator that passes {doc_description} as the first argument"
         " to the decorated function."
     )
     return decorator
 
 
-def _make_command(
-    f: F,
-    name: t.Optional[str],
-    attrs: t.MutableMapping[str, t.Any],
-    cls: t.Type[Command],
-) -> Command:
-    if isinstance(f, Command):
-        raise TypeError("Attempted to convert a callback into a command twice.")
+CmdType = t.TypeVar("CmdType", bound=Command)
 
-    try:
-        params = f.__click_params__  # type: ignore
-        params.reverse()
-        del f.__click_params__  # type: ignore
-    except AttributeError:
-        params = []
 
-    help = attrs.get("help")
+@t.overload
+def command(
+    __func: t.Callable[..., t.Any],
+) -> Command:
+    ...
 
-    if help is None:
-        help = inspect.getdoc(f)
-    else:
-        help = inspect.cleandoc(help)
 
-    attrs["help"] = help
-    return cls(
-        name=name or f.__name__.lower().replace("_", "-"),
-        callback=f,
-        params=params,
-        **attrs,
-    )
+@t.overload
+def command(
+    name: t.Optional[str] = None,
+    **attrs: t.Any,
+) -> t.Callable[..., Command]:
+    ...
 
 
+@t.overload
 def command(
     name: t.Optional[str] = None,
+    cls: t.Type[CmdType] = ...,
+    **attrs: t.Any,
+) -> t.Callable[..., CmdType]:
+    ...
+
+
+def command(
+    name: t.Union[str, t.Callable[..., t.Any], None] = None,
     cls: t.Optional[t.Type[Command]] = None,
     **attrs: t.Any,
-) -> t.Callable[[F], Command]:
+) -> t.Union[Command, t.Callable[..., Command]]:
     r"""Creates a new :class:`Command` and uses the decorated function as
     callback.  This will also automatically attach all decorated
     :func:`option`\s and :func:`argument`\s as parameters to the command.
 
     The name of the command defaults to the name of the function with
     underscores replaced by dashes.  If you want to change that, you can
     pass the intended name as the first argument.
 
     All keyword arguments are forwarded to the underlying command class.
+    For the ``params`` argument, any decorated params are appended to
+    the end of the list.
 
     Once decorated the function turns into a :class:`Command` instance
     that can be invoked as a command line utility or be attached to a
     command :class:`Group`.
 
     :param name: the name of the command.  This defaults to the function
                  name with underscores replaced by dashes.
     :param cls: the command class to instantiate.  This defaults to
                 :class:`Command`.
+
+    .. versionchanged:: 8.1
+        This decorator can be applied without parentheses.
+
+    .. versionchanged:: 8.1
+        The ``params`` argument can be used. Decorated params are
+        appended to the end of the list.
     """
+
+    func: t.Optional[t.Callable[..., t.Any]] = None
+
+    if callable(name):
+        func = name
+        name = None
+        assert cls is None, "Use 'command(cls=cls)(callable)' to specify a class."
+        assert not attrs, "Use 'command(**kwargs)(callable)' to provide arguments."
+
     if cls is None:
         cls = Command
 
     def decorator(f: t.Callable[..., t.Any]) -> Command:
-        cmd = _make_command(f, name, attrs, cls)  # type: ignore
+        if isinstance(f, Command):
+            raise TypeError("Attempted to convert a callback into a command twice.")
+
+        attr_params = attrs.pop("params", None)
+        params = attr_params if attr_params is not None else []
+
+        try:
+            decorator_params = f.__click_params__  # type: ignore
+        except AttributeError:
+            pass
+        else:
+            del f.__click_params__  # type: ignore
+            params.extend(reversed(decorator_params))
+
+        if attrs.get("help") is None:
+            attrs["help"] = f.__doc__
+
+        cmd = cls(  # type: ignore[misc]
+            name=name or f.__name__.lower().replace("_", "-"),  # type: ignore[arg-type]
+            callback=f,
+            params=params,
+            **attrs,
+        )
         cmd.__doc__ = f.__doc__
         return cmd
 
+    if func is not None:
+        return decorator(func)
+
     return decorator
 
 
-def group(name: t.Optional[str] = None, **attrs: t.Any) -> t.Callable[[F], Group]:
+@t.overload
+def group(
+    __func: t.Callable[..., t.Any],
+) -> Group:
+    ...
+
+
+@t.overload
+def group(
+    name: t.Optional[str] = None,
+    **attrs: t.Any,
+) -> t.Callable[[F], Group]:
+    ...
+
+
+def group(
+    name: t.Union[str, t.Callable[..., t.Any], None] = None, **attrs: t.Any
+) -> t.Union[Group, t.Callable[[F], Group]]:
     """Creates a new :class:`Group` with a function as callback.  This
     works otherwise the same as :func:`command` just that the `cls`
     parameter is set to :class:`Group`.
+
+    .. versionchanged:: 8.1
+        This decorator can be applied without parentheses.
     """
-    attrs.setdefault("cls", Group)
+    if attrs.get("cls") is None:
+        attrs["cls"] = Group
+
+    if callable(name):
+        grp: t.Callable[[F], Group] = t.cast(Group, command(**attrs))
+        return grp(name)
+
     return t.cast(Group, command(name, **attrs))
 
 
 def _param_memo(f: FC, param: Parameter) -> None:
     if isinstance(f, Command):
         f.params.append(param)
     else:
@@ -215,15 +279,15 @@
     and attaching it to the :attr:`Command.params` list.
 
     :param cls: the argument class to instantiate.  This defaults to
                 :class:`Argument`.
     """
 
     def decorator(f: FC) -> FC:
-        ArgumentClass = attrs.pop("cls", Argument)
+        ArgumentClass = attrs.pop("cls", None) or Argument
         _param_memo(f, ArgumentClass(param_decls, **attrs))
         return f
 
     return decorator
 
 
 def option(*param_decls: str, **attrs: t.Any) -> t.Callable[[FC], FC]:
@@ -236,18 +300,15 @@
     :param cls: the option class to instantiate.  This defaults to
                 :class:`Option`.
     """
 
     def decorator(f: FC) -> FC:
         # Issue 926, copy attrs, so pre-defined options can re-use the same cls=
         option_attrs = attrs.copy()
-
-        if "help" in option_attrs:
-            option_attrs["help"] = inspect.cleandoc(option_attrs["help"])
-        OptionClass = option_attrs.pop("cls", Option)
+        OptionClass = option_attrs.pop("cls", None) or Option
         _param_memo(f, OptionClass(param_decls, **option_attrs))
         return f
 
     return decorator
 
 
 def confirmation_option(*param_decls: str, **kwargs: t.Any) -> t.Callable[[FC], FC]:
@@ -368,15 +429,15 @@
         if version is None and package_name is not None:
             metadata: t.Optional[types.ModuleType]
 
             try:
                 from importlib import metadata  # type: ignore
             except ImportError:
                 # Python < 3.8
-                import python_agent.packages.importlib_metadata as metadata  # type: ignore
+                import importlib_metadata as metadata  # type: ignore
 
             try:
                 version = metadata.version(package_name)  # type: ignore
             except metadata.PackageNotFoundError:  # type: ignore
                 raise RuntimeError(
                     f"{package_name!r} is not installed. Try passing"
                     " 'package_name' instead."
```

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/formatting.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/formatting.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/shell_completion.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/shell_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,43 +444,42 @@
             param.nargs > 1
             and isinstance(value, (tuple, list))
             and len(value) < param.nargs
         )
     )
 
 
-def _start_of_option(value: str) -> bool:
+def _start_of_option(ctx: Context, value: str) -> bool:
     """Check if the value looks like the start of an option."""
     if not value:
         return False
 
     c = value[0]
-    # Allow "/" since that starts a path.
-    return not c.isalnum() and c != "/"
+    return c in ctx._opt_prefixes
 
 
-def _is_incomplete_option(args: t.List[str], param: Parameter) -> bool:
+def _is_incomplete_option(ctx: Context, args: t.List[str], param: Parameter) -> bool:
     """Determine if the given parameter is an option that needs a value.
 
     :param args: List of complete args before the incomplete value.
     :param param: Option object being checked.
     """
     if not isinstance(param, Option):
         return False
 
-    if param.is_flag:
+    if param.is_flag or param.count:
         return False
 
     last_option = None
 
     for index, arg in enumerate(reversed(args)):
         if index + 1 > param.nargs:
             break
 
-        if _start_of_option(arg):
+        if _start_of_option(ctx, arg):
             last_option = arg
 
     return last_option is not None and last_option in param.opts
 
 
 def _resolve_context(
     cli: BaseCommand, ctx_args: t.Dict[str, t.Any], prog_name: str, args: t.List[str]
@@ -547,31 +546,31 @@
     """
     # Different shells treat an "=" between a long option name and
     # value differently. Might keep the value joined, return the "="
     # as a separate item, or return the split name and value. Always
     # split and discard the "=" to make completion easier.
     if incomplete == "=":
         incomplete = ""
-    elif "=" in incomplete and _start_of_option(incomplete):
+    elif "=" in incomplete and _start_of_option(ctx, incomplete):
         name, _, incomplete = incomplete.partition("=")
         args.append(name)
 
     # The "--" marker tells Click to stop treating values as options
     # even if they start with the option character. If it hasn't been
     # given and the incomplete arg looks like an option, the current
     # command will provide option name completions.
-    if "--" not in args and _start_of_option(incomplete):
+    if "--" not in args and _start_of_option(ctx, incomplete):
         return ctx.command, incomplete
 
     params = ctx.command.get_params(ctx)
 
     # If the last complete arg is an option name with an incomplete
     # value, the option will provide value completions.
     for param in params:
-        if _is_incomplete_option(args, param):
+        if _is_incomplete_option(ctx, args, param):
             return param, incomplete
 
     # It's not an option name or value. The first argument without a
     # parsed value will provide value completions.
     for param in params:
         if _is_incomplete_argument(ctx, param):
             return param, incomplete
```

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/click/termui.py` & `sealights-python-agent-1.1.0/python_agent/packages/click/termui.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,16 @@
             else:
                 echo(_("Error: {e.message}").format(e=e), err=err)  # noqa: B306
             continue
         if not confirmation_prompt:
             return result
         while True:
             value2 = prompt_func(confirmation_prompt)
-            if value2:
+            is_empty = not value and not value2
+            if value2 or is_empty:
                 break
         if value == value2:
             return result
         echo(_("Error: The two entered values do not match."), err=err)
 
 
 def confirm(
@@ -245,34 +246,14 @@
             continue
         break
     if abort and not rv:
         raise Abort()
     return rv
 
 
-def get_terminal_size() -> os.terminal_size:
-    """Returns the current size of the terminal as tuple in the form
-    ``(width, height)`` in columns and rows.
-
-    .. deprecated:: 8.0
-        Will be removed in Click 8.1. Use
-        :func:`shutil.get_terminal_size` instead.
-    """
-    import shutil
-    import warnings
-
-    warnings.warn(
-        "'click.get_terminal_size()' is deprecated and will be removed"
-        " in Click 8.1. Use 'shutil.get_terminal_size()' instead.",
-        DeprecationWarning,
-        stacklevel=2,
-    )
-    return shutil.get_terminal_size()
-
-
 def echo_via_pager(
     text_or_generator: t.Union[t.Iterable[str], t.Callable[[], t.Iterable[str]], str],
     color: t.Optional[bool] = None,
 ) -> None:
     """This function takes a text and shows it via an environment specific
     pager on stdout.
```

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cd.py` & `sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/cd.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/legacy.py` & `sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/legacy.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/models.py` & `sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/models.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/assets/__init__.py` & `sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cli/normalizer.py` & `sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/cli/normalizer.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/api.py` & `sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/md.py` & `sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/md.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/utils.py` & `sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/__init__.py` & `sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/constant.py` & `sealights-python-agent-1.1.0/python_agent/packages/charset_normalizer/constant.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/semantic_version/base.py` & `sealights-python-agent-1.1.0/python_agent/packages/semantic_version/base.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/semantic_version/__init__.py` & `sealights-python-agent-1.1.0/python_agent/packages/semantic_version/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/semantic_version/django_fields.py` & `sealights-python-agent-1.1.0/python_agent/packages/semantic_version/django_fields.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/idna/codec.py` & `sealights-python-agent-1.1.0/python_agent/packages/idna/codec.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/idna/intranges.py` & `sealights-python-agent-1.1.0/python_agent/packages/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/idna/uts46data.py` & `sealights-python-agent-1.1.0/python_agent/packages/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/idna/idnadata.py` & `sealights-python-agent-1.1.0/python_agent/packages/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/idna/__init__.py` & `sealights-python-agent-1.1.0/python_agent/packages/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/idna/core.py` & `sealights-python-agent-1.1.0/python_agent/packages/idna/core.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/exceptions.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/response.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/fields.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/connectionpool.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/poolmanager.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/_collections.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/filepost.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/connection.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssl_match_hostname.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssltransport.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/response.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/proxy.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssl_.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/wait.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/timeout.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/connection.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/request.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/retry.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/__init__.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/url.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/request.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/ntlmpool.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/low_level.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/bindings.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/securetransport.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/pyopenssl.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_appengine_environ.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/appengine.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/socks.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/__init__.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/six.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/backports/makefile.py` & `sealights-python-agent-1.1.0/python_agent/packages/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/python_agent/packages/freezegun/api.py` & `sealights-python-agent-1.1.0/python_agent/packages/freezegun/api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/LICENSE.txt` & `sealights-python-agent-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.6/sealights_python_agent.egg-info/SOURCES.txt` & `sealights-python-agent-1.1.0/sealights_python_agent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,25 @@
 python_agent/build_scanner/scm/git_integration.py
 python_agent/build_scanner/scm/scm_info.py
 python_agent/common/__init__.py
 python_agent/common/config_data.py
 python_agent/common/configuration_manager.py
 python_agent/common/constants.py
 python_agent/common/environment_variables_resolver.py
+python_agent/common/agent_events/__init__.py
+python_agent/common/agent_events/agent_events_manager.py
+python_agent/common/agent_events/env_vars.py
+python_agent/common/agent_events/utils.py
+python_agent/common/agent_events/entites/__init__.py
+python_agent/common/agent_events/entites/agent_build_scan_error_event.py
+python_agent/common/agent_events/entites/agent_footprints_submission_error_event.py
+python_agent/common/agent_events/entites/agent_heartbeat_event.py
+python_agent/common/agent_events/entites/agent_start_event.py
+python_agent/common/agent_events/entites/agent_stop_event.py
+python_agent/common/agent_events/entites/agent_tests_submission_error_event.py
 python_agent/common/autoupgrade/__init__.py
 python_agent/common/autoupgrade/autoupgrade_manager.py
 python_agent/common/build_session/__init__.py
 python_agent/common/build_session/build_session_data.py
 python_agent/common/http/__init__.py
 python_agent/common/http/backend_proxy.py
 python_agent/common/http/requests_wrapper.py
@@ -65,14 +76,15 @@
 python_agent/packages/astor/tree_walk.py
 python_agent/packages/astunparse/__init__.py
 python_agent/packages/astunparse/__main__.py
 python_agent/packages/astunparse/printer.py
 python_agent/packages/astunparse/unparser.py
 python_agent/packages/astunparse/unparser36.py
 python_agent/packages/astunparse/unparser37.py
+python_agent/packages/astunparse/unparser38.py
 python_agent/packages/blinker/__init__.py
 python_agent/packages/blinker/_saferef.py
 python_agent/packages/blinker/_utilities.py
 python_agent/packages/blinker/base.py
 python_agent/packages/certifi/__init__.py
 python_agent/packages/certifi/__main__.py
 python_agent/packages/certifi/cacert.pem
@@ -98,14 +110,15 @@
 python_agent/packages/click/_winconsole.py
 python_agent/packages/click/core.py
 python_agent/packages/click/decorators.py
 python_agent/packages/click/exceptions.py
 python_agent/packages/click/formatting.py
 python_agent/packages/click/globals.py
 python_agent/packages/click/parser.py
+python_agent/packages/click/py.typed
 python_agent/packages/click/shell_completion.py
 python_agent/packages/click/termui.py
 python_agent/packages/click/testing.py
 python_agent/packages/click/types.py
 python_agent/packages/click/utils.py
 python_agent/packages/freezegun/__init__.py
 python_agent/packages/freezegun/_async.py
```

### Comparing `sealights-python-agent-1.0.6/sealights_python_agent.egg-info/PKG-INFO` & `sealights-python-agent-1.1.0/sealights_python_agent.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: sealights-python-agent
-Version: 1.0.6
+Version: 1.1.0
 Summary: Python Agent
 Home-page: https://github.com/Sealights/SL.OnPremise.Agents.Python
 Author: Shai Cantor
 Author-email: shai@sealights.io
 License: Other/Proprietary License
 Keywords: sealights python agent setuptools development
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6, <4
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
 ======================
 sealights-python-agent
@@ -27,14 +31,17 @@
 
 
 ****************
 Language Support
 ****************
 * Python 3.6
 * Python 3.7
+* Python 3.8
+* Python 3.9
+* Python 3.10
 
 
 ************
 Installation
 ************
 .. code-block::
 
@@ -77,14 +84,18 @@
 
         $ sl-python unit2 --teststage "Unit Tests" <your args...>
 
 
 Changes
 =======
 
+1.0.14 (2022-11-20)
+--------------------
+* Added support for Python 3.8, 3.9, 3.10
+
 1.0.6 (2022-08-30)
 --------------------
 * Fixed "TIA Not Supported" Indicator for Test Optimization
 
 1.0.5 (2022-07-05)
 --------------------
 * Dropped support for Python 2.7, 3.4 and 3.5.
```

### Comparing `sealights-python-agent-1.0.6/CHANGES.rst` & `sealights-python-agent-1.1.0/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changes
 =======
 
+1.0.14 (2022-11-20)
+--------------------
+* Added support for Python 3.8, 3.9, 3.10
+
 1.0.6 (2022-08-30)
 --------------------
 * Fixed "TIA Not Supported" Indicator for Test Optimization
 
 1.0.5 (2022-07-05)
 --------------------
 * Dropped support for Python 2.7, 3.4 and 3.5.
```

### Comparing `sealights-python-agent-1.0.6/README.rst` & `sealights-python-agent-1.1.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 
 ****************
 Language Support
 ****************
 * Python 3.6
 * Python 3.7
+* Python 3.8
+* Python 3.9
+* Python 3.10
 
 
 ************
 Installation
 ************
 .. code-block::
```

### Comparing `sealights-python-agent-1.0.6/PKG-INFO` & `sealights-python-agent-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: sealights-python-agent
-Version: 1.0.6
+Version: 1.1.0
 Summary: Python Agent
 Home-page: https://github.com/Sealights/SL.OnPremise.Agents.Python
 Author: Shai Cantor
 Author-email: shai@sealights.io
 License: Other/Proprietary License
 Keywords: sealights python agent setuptools development
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6, <4
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
 ======================
 sealights-python-agent
@@ -27,14 +31,17 @@
 
 
 ****************
 Language Support
 ****************
 * Python 3.6
 * Python 3.7
+* Python 3.8
+* Python 3.9
+* Python 3.10
 
 
 ************
 Installation
 ************
 .. code-block::
 
@@ -77,14 +84,18 @@
 
         $ sl-python unit2 --teststage "Unit Tests" <your args...>
 
 
 Changes
 =======
 
+1.0.14 (2022-11-20)
+--------------------
+* Added support for Python 3.8, 3.9, 3.10
+
 1.0.6 (2022-08-30)
 --------------------
 * Fixed "TIA Not Supported" Indicator for Test Optimization
 
 1.0.5 (2022-07-05)
 --------------------
 * Dropped support for Python 2.7, 3.4 and 3.5.
```

### Comparing `sealights-python-agent-1.0.6/setup.py` & `sealights-python-agent-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,14 @@
     changes = f.read()
 
 with open(path.join(here, 'requirements.txt')) as f:
     requirements = f.read().splitlines()
     # python 3.3 use case where dependencies are read as bytes of the form b'APScheduler==3.0.6'
     requirements = [requirement.decode() if isinstance(requirement, bytes) else requirement for requirement in requirements]
 
-if tuple(sys.version_info) >= (3, 7):
-    install_requires = requirements + ["coverage==6.4"]
-else:
-    install_requires = requirements + ["coverage==6.2"]
 
 setup(
     name=python_agent.__package_name__,
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
@@ -54,14 +50,18 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         "License :: Other/Proprietary License",
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     python_requires='>=3.6, <4',
 
     # What does your project relate to?
     keywords='sealights python agent setuptools development',
 
@@ -73,15 +73,15 @@
     # this:
     #   py_modules=["my_module"],
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=install_requires,
+    install_requires=requirements,
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={
         'dev': ['check-manifest'],
```

