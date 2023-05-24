# Comparing `tmp/vcrpy-4.2.1.tar.gz` & `tmp/vcrpy-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vcrpy-4.2.1.tar", last modified: Wed Aug 31 19:15:46 2022, max compression
+gzip compressed data, was "vcrpy-4.3.0.tar", last modified: Wed May 24 18:50:19 2023, max compression
```

## Comparing `vcrpy-4.2.1.tar` & `vcrpy-4.3.0.tar`

### file list

```diff
@@ -1,104 +1,106 @@
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/
--rw-r--r--   0 kevin      (501) staff       (20)     4479 2022-08-31 19:15:46.000000 vcrpy-4.2.1/PKG-INFO
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/tests/
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/tests/unit/
--rw-r--r--   0 kevin      (501) staff       (20)      798 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     3648 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_response.py
--rw-r--r--   0 kevin      (501) staff       (20)      396 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_vcr_import.py
--rw-r--r--   0 kevin      (501) staff       (20)      610 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_json_serializer.py
--rw-r--r--   0 kevin      (501) staff       (20)     2669 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_errors.py
--rw-r--r--   0 kevin      (501) staff       (20)     2472 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_request.py
--rw-r--r--   0 kevin      (501) staff       (20)    13162 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_cassettes.py
--rw-r--r--   0 kevin      (501) staff       (20)     1587 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_migration.py
--rw-r--r--   0 kevin      (501) staff       (20)     1067 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_persist.py
--rw-r--r--   0 kevin      (501) staff       (20)    10005 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_matchers.py
--rw-r--r--   0 kevin      (501) staff       (20)     4038 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_serialize.py
--rw-r--r--   0 kevin      (501) staff       (20)    11737 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_filters.py
--rw-r--r--   0 kevin      (501) staff       (20)    11853 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/unit/test_vcr.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/tests/integration/
--rw-r--r--   0 kevin      (501) staff       (20)     6263 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_urllib3.py
--rw-r--r--   0 kevin      (501) staff       (20)     1112 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_register_matcher.py
--rw-r--r--   0 kevin      (501) staff       (20)     2766 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_basic.py
--rw-r--r--   0 kevin      (501) staff       (20)     2620 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_ignore.py
--rw-r--r--   0 kevin      (501) staff       (20)      876 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_multiple.py
--rw-r--r--   0 kevin      (501) staff       (20)     1499 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_disksaver.py
--rw-r--r--   0 kevin      (501) staff       (20)     5039 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     1030 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_http
--rw-r--r--   0 kevin      (501) staff       (20)     5072 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_urllib2.py
--rw-r--r--   0 kevin      (501) staff       (20)     5180 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_filter.py
--rw-r--r--   0 kevin      (501) staff       (20)    16104 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_aiohttp.py
--rw-r--r--   0 kevin      (501) staff       (20)     1852 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_register_persister.py
--rw-r--r--   0 kevin      (501) staff       (20)     4467 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_boto3.py
--rw-r--r--   0 kevin      (501) staff       (20)      738 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_request.py
--rw-r--r--   0 kevin      (501) staff       (20)     3434 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_wild.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/tests/integration/cassettes/
--rw-r--r--   0 kevin      (501) staff       (20)     1017 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml
--rw-r--r--   0 kevin      (501) staff       (20)      962 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_register_serializer.py
--rw-r--r--   0 kevin      (501) staff       (20)     1256 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/aiohttp_utils.py
--rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     2948 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_boto.py
--rw-r--r--   0 kevin      (501) staff       (20)     4001 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_matchers.py
--rw-r--r--   0 kevin      (501) staff       (20)     5168 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_record_mode.py
--rw-r--r--   0 kevin      (501) staff       (20)    11634 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_requests.py
--rw-r--r--   0 kevin      (501) staff       (20)     1566 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_tornado_with_decorator_use_cassette.yaml
--rw-r--r--   0 kevin      (501) staff       (20)     1778 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_config.py
--rw-r--r--   0 kevin      (501) staff       (20)    12741 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_tornado.py
--rw-r--r--   0 kevin      (501) staff       (20)     1823 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_proxy.py
--rw-r--r--   0 kevin      (501) staff       (20)    10646 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_httpx.py
--rw-r--r--   0 kevin      (501) staff       (20)     5048 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_httplib2.py
--rw-r--r--   0 kevin      (501) staff       (20)     1387 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/integration/test_tornado_exception_can_be_caught.yaml
--rw-r--r--   0 kevin      (501) staff       (20)      354 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/assertions.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/tests/fixtures/
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/tests/fixtures/wild/
--rw-r--r--   0 kevin      (501) staff       (20)     9705 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/fixtures/wild/domain_redirect.yaml
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/tests/fixtures/migration/
--rw-r--r--   0 kevin      (501) staff       (20)     1115 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/fixtures/migration/new_cassette.json
--rw-r--r--   0 kevin      (501) staff       (20)      599 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/fixtures/migration/new_cassette.yaml
--rw-r--r--   0 kevin      (501) staff       (20)       23 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/fixtures/migration/not_cassette.txt
--rw-r--r--   0 kevin      (501) staff       (20)     1031 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/fixtures/migration/old_cassette.json
--rw-r--r--   0 kevin      (501) staff       (20)      869 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tests/fixtures/migration/old_cassette.yaml
--rw-r--r--   0 kevin      (501) staff       (20)      142 2022-08-31 19:12:36.000000 vcrpy-4.2.1/MANIFEST.in
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/vcr/
--rw-r--r--   0 kevin      (501) staff       (20)     2123 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/serialize.py
--rw-r--r--   0 kevin      (501) staff       (20)    20781 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/patch.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/vcr/stubs/
--rw-r--r--   0 kevin      (501) staff       (20)      507 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/stubs/urllib3_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     1736 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/stubs/boto3_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)      581 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/stubs/compat.py
--rw-r--r--   0 kevin      (501) staff       (20)    12476 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/stubs/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     9973 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/stubs/aiohttp_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     2166 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/stubs/httplib2_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)      688 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/stubs/requests_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     5578 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/stubs/httpx_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     3407 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/stubs/tornado_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)      234 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/stubs/boto_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)    10576 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/config.py
--rw-r--r--   0 kevin      (501) staff       (20)     3882 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/util.py
--rw-r--r--   0 kevin      (501) staff       (20)     3781 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/request.py
--rw-r--r--   0 kevin      (501) staff       (20)      295 2022-08-31 19:14:17.000000 vcrpy-4.2.1/vcr/__init__.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/vcr/persisters/
--rw-r--r--   0 kevin      (501) staff       (20)      793 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/persisters/filesystem.py
--rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/persisters/__init__.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/vcr/serializers/
--rw-r--r--   0 kevin      (501) staff       (20)     2513 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/serializers/compat.py
--rw-r--r--   0 kevin      (501) staff       (20)      343 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/serializers/yamlserializer.py
--rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/serializers/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)      778 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/serializers/jsonserializer.py
--rw-r--r--   0 kevin      (501) staff       (20)    13244 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/cassette.py
--rw-r--r--   0 kevin      (501) staff       (20)     1976 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/errors.py
--rw-r--r--   0 kevin      (501) staff       (20)     4105 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/matchers.py
--rw-r--r--   0 kevin      (501) staff       (20)      630 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/record_mode.py
--rw-r--r--   0 kevin      (501) staff       (20)      125 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/_handle_coroutine.py
--rw-r--r--   0 kevin      (501) staff       (20)     4659 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/migration.py
--rw-r--r--   0 kevin      (501) staff       (20)     6608 2022-08-31 19:12:36.000000 vcrpy-4.2.1/vcr/filters.py
--rw-r--r--   0 kevin      (501) staff       (20)     2560 2022-08-31 19:12:36.000000 vcrpy-4.2.1/setup.py
--rw-r--r--   0 kevin      (501) staff       (20)     3000 2022-08-31 19:12:36.000000 vcrpy-4.2.1/tox.ini
--rw-r--r--   0 kevin      (501) staff       (20)       67 2022-08-31 19:15:46.000000 vcrpy-4.2.1/setup.cfg
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-08-31 19:15:46.000000 vcrpy-4.2.1/vcrpy.egg-info/
--rw-r--r--   0 kevin      (501) staff       (20)     4479 2022-08-31 19:15:46.000000 vcrpy-4.2.1/vcrpy.egg-info/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)     2605 2022-08-31 19:15:46.000000 vcrpy-4.2.1/vcrpy.egg-info/SOURCES.txt
--rw-r--r--   0 kevin      (501) staff       (20)       27 2022-08-31 19:15:46.000000 vcrpy-4.2.1/vcrpy.egg-info/requires.txt
--rw-r--r--   0 kevin      (501) staff       (20)        4 2022-08-31 19:15:46.000000 vcrpy-4.2.1/vcrpy.egg-info/top_level.txt
--rw-r--r--   0 kevin      (501) staff       (20)        1 2022-08-31 19:15:46.000000 vcrpy-4.2.1/vcrpy.egg-info/dependency_links.txt
--rw-r--r--   0 kevin      (501) staff       (20)     2767 2022-08-31 19:12:36.000000 vcrpy-4.2.1/README.rst
--rw-r--r--   0 kevin      (501) staff       (20)     1063 2022-08-31 19:12:36.000000 vcrpy-4.2.1/LICENSE.txt
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.886911 vcrpy-4.3.0/
+-rw-r--r--   0 kevin      (501) staff       (20)     1063 2022-08-31 19:12:36.000000 vcrpy-4.3.0/LICENSE.txt
+-rw-r--r--   0 kevin      (501) staff       (20)      142 2022-08-31 19:12:36.000000 vcrpy-4.3.0/MANIFEST.in
+-rw-r--r--   0 kevin      (501) staff       (20)     3925 2023-05-24 18:50:19.886977 vcrpy-4.3.0/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)     2767 2022-08-31 19:12:36.000000 vcrpy-4.3.0/README.rst
+-rw-r--r--   0 kevin      (501) staff       (20)      164 2023-05-24 18:36:09.000000 vcrpy-4.3.0/pyproject.toml
+-rw-r--r--   0 kevin      (501) staff       (20)       67 2023-05-24 18:50:19.887157 vcrpy-4.3.0/setup.cfg
+-rw-r--r--   0 kevin      (501) staff       (20)     2610 2023-05-24 18:36:09.000000 vcrpy-4.3.0/setup.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.876960 vcrpy-4.3.0/tests/
+-rw-r--r--   0 kevin      (501) staff       (20)      354 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/assertions.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.875477 vcrpy-4.3.0/tests/fixtures/
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.877487 vcrpy-4.3.0/tests/fixtures/migration/
+-rw-r--r--   0 kevin      (501) staff       (20)     1115 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/migration/new_cassette.json
+-rw-r--r--   0 kevin      (501) staff       (20)      599 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/migration/new_cassette.yaml
+-rw-r--r--   0 kevin      (501) staff       (20)       23 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/migration/not_cassette.txt
+-rw-r--r--   0 kevin      (501) staff       (20)     1031 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/migration/old_cassette.json
+-rw-r--r--   0 kevin      (501) staff       (20)      869 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/migration/old_cassette.yaml
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.877589 vcrpy-4.3.0/tests/fixtures/wild/
+-rw-r--r--   0 kevin      (501) staff       (20)     9705 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/wild/domain_redirect.yaml
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.881018 vcrpy-4.3.0/tests/integration/
+-rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1214 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/aiohttp_utils.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.881157 vcrpy-4.3.0/tests/integration/cassettes/
+-rw-r--r--   0 kevin      (501) staff       (20)     1017 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml
+-rw-r--r--   0 kevin      (501) staff       (20)      316 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/conftest.py
+-rw-r--r--   0 kevin      (501) staff       (20)    16008 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_aiohttp.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2766 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_basic.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2951 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_boto.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3589 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_boto3.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2526 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_config.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1563 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_disksaver.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5714 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_filter.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1030 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_http
+-rw-r--r--   0 kevin      (501) staff       (20)     4926 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_httplib2.py
+-rw-r--r--   0 kevin      (501) staff       (20)    10415 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_httpx.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2621 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_ignore.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4000 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_matchers.py
+-rw-r--r--   0 kevin      (501) staff       (20)      878 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_multiple.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1779 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_proxy.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5170 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_record_mode.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1167 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_register_matcher.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1852 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_register_persister.py
+-rw-r--r--   0 kevin      (501) staff       (20)      962 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_register_serializer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      739 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_request.py
+-rw-r--r--   0 kevin      (501) staff       (20)    11635 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_requests.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5040 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)    12599 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_tornado.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1387 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_tornado_exception_can_be_caught.yaml
+-rw-r--r--   0 kevin      (501) staff       (20)     1566 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml
+-rw-r--r--   0 kevin      (501) staff       (20)     5072 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_urllib2.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6264 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_urllib3.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3429 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_wild.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.882800 vcrpy-4.3.0/tests/unit/
+-rw-r--r--   0 kevin      (501) staff       (20)    13163 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_cassettes.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2669 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/unit/test_errors.py
+-rw-r--r--   0 kevin      (501) staff       (20)    11738 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_filters.py
+-rw-r--r--   0 kevin      (501) staff       (20)      611 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_json_serializer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     9990 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_matchers.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1588 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_migration.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1067 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/unit/test_persist.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2471 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_request.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3648 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/unit/test_response.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4038 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_serialize.py
+-rw-r--r--   0 kevin      (501) staff       (20)      798 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)    12080 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_vcr.py
+-rw-r--r--   0 kevin      (501) staff       (20)      395 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_vcr_import.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3111 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tox.ini
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.884471 vcrpy-4.3.0/vcr/
+-rw-r--r--   0 kevin      (501) staff       (20)      296 2023-05-24 18:48:06.000000 vcrpy-4.3.0/vcr/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)      125 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/_handle_coroutine.py
+-rw-r--r--   0 kevin      (501) staff       (20)    13892 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/cassette.py
+-rw-r--r--   0 kevin      (501) staff       (20)    10830 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/config.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1976 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/errors.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6651 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/filters.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4105 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/matchers.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4660 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/migration.py
+-rw-r--r--   0 kevin      (501) staff       (20)    17807 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/patch.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.884676 vcrpy-4.3.0/vcr/persisters/
+-rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/persisters/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1095 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/persisters/filesystem.py
+-rw-r--r--   0 kevin      (501) staff       (20)      630 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/record_mode.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3782 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/request.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2124 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/serialize.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.885112 vcrpy-4.3.0/vcr/serializers/
+-rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/serializers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2513 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/serializers/compat.py
+-rw-r--r--   0 kevin      (501) staff       (20)      778 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/serializers/jsonserializer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      363 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/serializers/yamlserializer.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.886204 vcrpy-4.3.0/vcr/stubs/
+-rw-r--r--   0 kevin      (501) staff       (20)    12461 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     9954 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/aiohttp_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1202 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/boto3_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      235 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/boto_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      578 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/compat.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2166 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/httplib2_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5579 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/httpx_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      562 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/requests_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3407 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/stubs/tornado_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      508 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/urllib3_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3882 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/util.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.886795 vcrpy-4.3.0/vcrpy.egg-info/
+-rw-r--r--   0 kevin      (501) staff       (20)     3925 2023-05-24 18:50:19.000000 vcrpy-4.3.0/vcrpy.egg-info/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)     2650 2023-05-24 18:50:19.000000 vcrpy-4.3.0/vcrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        1 2023-05-24 18:50:19.000000 vcrpy-4.3.0/vcrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       27 2023-05-24 18:50:19.000000 vcrpy-4.3.0/vcrpy.egg-info/requires.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        4 2023-05-24 18:50:19.000000 vcrpy-4.3.0/vcrpy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vcrpy-4.2.1/PKG-INFO` & `vcrpy-4.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,102 +1,103 @@
 Metadata-Version: 2.1
 Name: vcrpy
-Version: 4.2.1
+Version: 4.3.0
 Summary: Automatically mock your HTTP interactions to simplify and speed up testing
 Home-page: https://github.com/kevin1024/vcrpy
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
-Description: 
-        ###########
-        VCR.py 📼
-        ###########
-        
-        
-        |PyPI| |Python versions| |Build Status| |CodeCov| |Gitter| |CodeStyleBlack|
-        
-        ----
-        
-        .. image:: https://vcrpy.readthedocs.io/en/latest/_images/vcr.svg
-           :alt: vcr.py logo
-        
-        
-        This is a Python version of `Ruby's VCR
-        library <https://github.com/vcr/vcr>`__.
-        
-        Source code
-          https://github.com/kevin1024/vcrpy
-        
-        Documentation
-          https://vcrpy.readthedocs.io/
-        
-        Rationale
-        ---------
-        
-        VCR.py simplifies and speeds up tests that make HTTP requests. The
-        first time you run code that is inside a VCR.py context manager or
-        decorated function, VCR.py records all HTTP interactions that take
-        place through the libraries it supports and serializes and writes them
-        to a flat file (in yaml format by default). This flat file is called a
-        cassette. When the relevant piece of code is executed again, VCR.py
-        will read the serialized requests and responses from the
-        aforementioned cassette file, and intercept any HTTP requests that it
-        recognizes from the original test run and return the responses that
-        corresponded to those requests. This means that the requests will not
-        actually result in HTTP traffic, which confers several benefits
-        including:
-        
-        -  The ability to work offline
-        -  Completely deterministic tests
-        -  Increased test execution speed
-        
-        If the server you are testing against ever changes its API, all you need
-        to do is delete your existing cassette files, and run your tests again.
-        VCR.py will detect the absence of a cassette file and once again record
-        all HTTP interactions, which will update them to correspond to the new
-        API.
-        
-        Usage with Pytest
-        -----------------
-        
-        There is a library to provide some pytest fixtures called pytest-recording https://github.com/kiwicom/pytest-recording
-        
-        License
-        -------
-        
-        This library uses the MIT license. See `LICENSE.txt <LICENSE.txt>`__ for
-        more details
-        
-        .. |PyPI| image:: https://img.shields.io/pypi/v/vcrpy.svg
-           :target: https://pypi.python.org/pypi/vcrpy
-        .. |Python versions| image:: https://img.shields.io/pypi/pyversions/vcrpy.svg
-           :target: https://pypi.python.org/pypi/vcrpy
-        .. |Build Status| image:: https://github.com/kevin1024/vcrpy/actions/workflows/main.yml/badge.svg
-           :target: https://github.com/kevin1024/vcrpy/actions
-        .. |Gitter| image:: https://badges.gitter.im/Join%20Chat.svg
-           :alt: Join the chat at https://gitter.im/kevin1024/vcrpy
-           :target: https://gitter.im/kevin1024/vcrpy?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-        .. |CodeCov| image:: https://codecov.io/gh/kevin1024/vcrpy/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/kevin1024/vcrpy
-           :alt: Code Coverage Status
-        .. |CodeStyleBlack| image:: https://img.shields.io/badge/code%20style-black-000000.svg 
-           :target: https://github.com/psf/black
-           :alt: Code Style: black
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+
+###########
+VCR.py 📼
+###########
+
+
+|PyPI| |Python versions| |Build Status| |CodeCov| |Gitter| |CodeStyleBlack|
+
+----
+
+.. image:: https://vcrpy.readthedocs.io/en/latest/_images/vcr.svg
+   :alt: vcr.py logo
+
+
+This is a Python version of `Ruby's VCR
+library <https://github.com/vcr/vcr>`__.
+
+Source code
+  https://github.com/kevin1024/vcrpy
+
+Documentation
+  https://vcrpy.readthedocs.io/
+
+Rationale
+---------
+
+VCR.py simplifies and speeds up tests that make HTTP requests. The
+first time you run code that is inside a VCR.py context manager or
+decorated function, VCR.py records all HTTP interactions that take
+place through the libraries it supports and serializes and writes them
+to a flat file (in yaml format by default). This flat file is called a
+cassette. When the relevant piece of code is executed again, VCR.py
+will read the serialized requests and responses from the
+aforementioned cassette file, and intercept any HTTP requests that it
+recognizes from the original test run and return the responses that
+corresponded to those requests. This means that the requests will not
+actually result in HTTP traffic, which confers several benefits
+including:
+
+-  The ability to work offline
+-  Completely deterministic tests
+-  Increased test execution speed
+
+If the server you are testing against ever changes its API, all you need
+to do is delete your existing cassette files, and run your tests again.
+VCR.py will detect the absence of a cassette file and once again record
+all HTTP interactions, which will update them to correspond to the new
+API.
+
+Usage with Pytest
+-----------------
+
+There is a library to provide some pytest fixtures called pytest-recording https://github.com/kiwicom/pytest-recording
+
+License
+-------
+
+This library uses the MIT license. See `LICENSE.txt <LICENSE.txt>`__ for
+more details
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/vcrpy.svg
+   :target: https://pypi.python.org/pypi/vcrpy
+.. |Python versions| image:: https://img.shields.io/pypi/pyversions/vcrpy.svg
+   :target: https://pypi.python.org/pypi/vcrpy
+.. |Build Status| image:: https://github.com/kevin1024/vcrpy/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/kevin1024/vcrpy/actions
+.. |Gitter| image:: https://badges.gitter.im/Join%20Chat.svg
+   :alt: Join the chat at https://gitter.im/kevin1024/vcrpy
+   :target: https://gitter.im/kevin1024/vcrpy?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+.. |CodeCov| image:: https://codecov.io/gh/kevin1024/vcrpy/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/kevin1024/vcrpy
+   :alt: Code Coverage Status
+.. |CodeStyleBlack| image:: https://img.shields.io/badge/code%20style-black-000000.svg 
+   :target: https://github.com/psf/black
+   :alt: Code Style: black
```

### Comparing `vcrpy-4.2.1/tests/unit/test_stubs.py` & `vcrpy-4.3.0/tests/unit/test_stubs.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import mock
 
 from vcr import mode
-from vcr.stubs import VCRHTTPSConnection
 from vcr.cassette import Cassette
+from vcr.stubs import VCRHTTPSConnection
 
 
 class TestVCRConnection:
     def test_setting_of_attributes_get_propagated_to_real_connection(self):
         vcr_connection = VCRHTTPSConnection("www.examplehost.com")
         vcr_connection.ssl_version = "example_ssl_version"
         assert vcr_connection.real_connection.ssl_version == "example_ssl_version"
```

### Comparing `vcrpy-4.2.1/tests/unit/test_response.py` & `vcrpy-4.3.0/tests/unit/test_response.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/unit/test_json_serializer.py` & `vcrpy-4.3.0/tests/unit/test_json_serializer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
-from vcr.serializers.jsonserializer import serialize
+
 from vcr.request import Request
+from vcr.serializers.jsonserializer import serialize
 
 
 def test_serialize_binary():
     request = Request(method="GET", uri="http://localhost/", body="", headers={})
     cassette = {"requests": [request], "responses": [{"body": b"\x8c"}]}
 
     with pytest.raises(Exception) as e:
```

### Comparing `vcrpy-4.2.1/tests/unit/test_errors.py` & `vcrpy-4.3.0/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/unit/test_request.py` & `vcrpy-4.3.0/tests/unit/test_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from vcr.request import Request, HeadersDict
+from vcr.request import HeadersDict, Request
 
 
 @pytest.mark.parametrize(
     "method, uri, expected_str",
     [
         ("GET", "http://www.google.com/", "<Request (GET) http://www.google.com/>"),
         ("OPTIONS", "*", "<Request (OPTIONS) *>"),
@@ -56,15 +56,14 @@
     ],
 )
 def test_uri(method, uri):
     assert Request(method, uri, "", {}).uri == uri
 
 
 def test_HeadersDict():
-
     # Simple test of CaseInsensitiveDict
     h = HeadersDict()
     assert h == {}
     h["Content-Type"] = "application/json"
     assert h == {"Content-Type": "application/json"}
     assert h["content-type"] == "application/json"
     assert h["CONTENT-TYPE"] == "application/json"
```

### Comparing `vcrpy-4.2.1/tests/unit/test_cassettes.py` & `vcrpy-4.3.0/tests/unit/test_cassettes.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import http.client as httplib
 import inspect
 import os
 from unittest import mock
 
 import pytest
 import yaml
+
 from vcr.cassette import Cassette
 from vcr.errors import UnhandledHTTPRequestError
 from vcr.patch import force_reset
 from vcr.stubs import VCRHTTPSConnection
 
 
 def test_cassette_load(tmpdir):
```

### Comparing `vcrpy-4.2.1/tests/unit/test_migration.py` & `vcrpy-4.3.0/tests/unit/test_migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import filecmp
 import json
 import shutil
+
 import yaml
 
 import vcr.migration
 
 # Use the libYAML versions if possible
 try:
     from yaml import CLoader as Loader
```

### Comparing `vcrpy-4.2.1/tests/unit/test_persist.py` & `vcrpy-4.3.0/tests/unit/test_persist.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/unit/test_matchers.py` & `vcrpy-4.3.0/tests/unit/test_matchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import itertools
 from unittest import mock
 
 import pytest
 
-from vcr import matchers
-from vcr import request
+from vcr import matchers, request
 
 # the dict contains requests with corresponding to its key difference
 # with 'base' request.
 REQUESTS = {
     "base": request.Request("GET", "http://host.com/p?a=b", "", {}),
     "method": request.Request("POST", "http://host.com/p?a=b", "", {}),
     "scheme": request.Request("GET", "https://host.com:80/p?a=b", "", {}),
```

### Comparing `vcrpy-4.2.1/tests/unit/test_serialize.py` & `vcrpy-4.3.0/tests/unit/test_serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- encoding: utf-8 -*-
 from unittest import mock
 
 import pytest
 
 from vcr.request import Request
 from vcr.serialize import deserialize, serialize
-from vcr.serializers import yamlserializer, jsonserializer, compat
+from vcr.serializers import compat, jsonserializer, yamlserializer
 
 
 def test_deserialize_old_yaml_cassette():
     with open("tests/fixtures/migration/old_cassette.yaml", "r") as f:
         with pytest.raises(ValueError):
             deserialize(f.read(), yamlserializer)
```

### Comparing `vcrpy-4.2.1/tests/unit/test_filters.py` & `vcrpy-4.3.0/tests/unit/test_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+import gzip
+import json
+import zlib
 from io import BytesIO
+from unittest import mock
+
 from vcr.filters import (
+    decode_response,
     remove_headers,
-    replace_headers,
-    remove_query_parameters,
-    replace_query_parameters,
     remove_post_data_parameters,
+    remove_query_parameters,
+    replace_headers,
     replace_post_data_parameters,
-    decode_response,
+    replace_query_parameters,
 )
 from vcr.request import Request
-import gzip
-import json
-from unittest import mock
-import zlib
 
 
 def test_replace_headers():
     # This tests all of:
     #   1. keeping a header
     #   2. removing a header
     #   3. replacing a header
```

### Comparing `vcrpy-4.2.1/tests/unit/test_vcr.py` & `vcrpy-4.3.0/tests/unit/test_vcr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from unittest import mock
+import http.client as httplib
 import os
+from pathlib import Path
+from unittest import mock
 
 import pytest
-import http.client as httplib
 
 from vcr import VCR, mode, use_cassette
+from vcr.patch import _HTTPConnection, force_reset
 from vcr.request import Request
 from vcr.stubs import VCRHTTPSConnection
-from vcr.patch import _HTTPConnection, force_reset
 
 
 def test_vcr_use_cassette():
     record_mode = mock.Mock()
     test_vcr = VCR(record_mode=record_mode)
     with mock.patch(
         "vcr.cassette.Cassette.load", return_value=mock.MagicMock(inject=False)
@@ -91,15 +92,14 @@
     # Regression test for #191
 
     request = Request("GET", "/", "", {})
     response = object()  # just can't be None
 
     # Prevent actually saving the cassette
     with mock.patch("vcr.cassette.FilesystemPersister.save_cassette"):
-
         # Baseline: non-iterable before_record_response should work
         mock_filter = mock.Mock()
         vcr = VCR(before_record_response=mock_filter)
         with vcr.use_cassette("test") as cassette:
             assert mock_filter.call_count == 0
             cassette.append(request, response)
             assert mock_filter.call_count == 1
@@ -115,29 +115,27 @@
 
 def test_before_record_response_as_filter():
     request = Request("GET", "/", "", {})
     response = object()  # just can't be None
 
     # Prevent actually saving the cassette
     with mock.patch("vcr.cassette.FilesystemPersister.save_cassette"):
-
         filter_all = mock.Mock(return_value=None)
         vcr = VCR(before_record_response=filter_all)
         with vcr.use_cassette("test") as cassette:
             cassette.append(request, response)
             assert cassette.data == []
             assert not cassette.dirty
 
 
 def test_vcr_path_transformer():
     # Regression test for #199
 
     # Prevent actually saving the cassette
     with mock.patch("vcr.cassette.FilesystemPersister.save_cassette"):
-
         # Baseline: path should be unchanged
         vcr = VCR()
         with vcr.use_cassette("test") as cassette:
             assert cassette._path == "test"
 
         # Regression test: path_transformer=None should do the same.
         vcr = VCR(path_transformer=None)
@@ -356,7 +354,15 @@
 
 def test_dynamically_added(self):
     assert httplib.HTTPConnection != _HTTPConnection
 
 
 TestVCRClass.test_dynamically_added = test_dynamically_added
 del test_dynamically_added
+
+
+def test_path_class_as_cassette():
+    path = Path(__file__).parent.parent.joinpath(
+        "integration/cassettes/test_httpx_test_test_behind_proxy.yml"
+    )
+    with use_cassette(path):
+        pass
```

### Comparing `vcrpy-4.2.1/tests/integration/test_urllib3.py` & `vcrpy-4.3.0/tests/integration/test_urllib3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Integration tests with urllib3"""
 
 # coding=utf-8
 
 import pytest
 import pytest_httpbin
+from assertions import assert_cassette_empty, assert_is_json
+
 import vcr
 from vcr.patch import force_reset
-from assertions import assert_cassette_empty, assert_is_json
 
 urllib3 = pytest.importorskip("urllib3")
 
 
 @pytest.fixture(scope="module")
 def verify_pool_mgr():
     return urllib3.PoolManager(
```

### Comparing `vcrpy-4.2.1/tests/integration/test_register_matcher.py` & `vcrpy-4.3.0/tests/integration/test_multiple.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,22 @@
-import vcr
 from urllib.request import urlopen
 
+import pytest
 
-def true_matcher(r1, r2):
-    return True
-
-
-def false_matcher(r1, r2):
-    return False
-
-
-def test_registered_true_matcher(tmpdir, httpbin):
-    my_vcr = vcr.VCR()
-    my_vcr.register_matcher("true", true_matcher)
-    testfile = str(tmpdir.join("test.yml"))
-    with my_vcr.use_cassette(testfile, match_on=["true"]):
-        # These 2 different urls are stored as the same request
-        urlopen(httpbin.url)
-        urlopen(httpbin.url + "/get")
-
-    with my_vcr.use_cassette(testfile, match_on=["true"]):
-        # I can get the response twice even though I only asked for it once
-        urlopen(httpbin.url + "/get")
-        urlopen(httpbin.url + "/get")
+import vcr
 
 
-def test_registered_false_matcher(tmpdir, httpbin):
-    my_vcr = vcr.VCR()
-    my_vcr.register_matcher("false", false_matcher)
-    testfile = str(tmpdir.join("test.yml"))
-    with my_vcr.use_cassette(testfile, match_on=["false"]) as cass:
-        # These 2 different urls are stored as different requests
-        urlopen(httpbin.url)
-        urlopen(httpbin.url + "/get")
-        assert len(cass) == 2
+def test_making_extra_request_raises_exception(tmpdir, httpbin):
+    # make two requests in the first request that are considered
+    # identical (since the match is based on method)
+    with vcr.use_cassette(str(tmpdir.join("test.json")), match_on=["method"]):
+        urlopen(httpbin.url + "/status/200")
+        urlopen(httpbin.url + "/status/201")
+
+    # Now, try to make three requests.  The first two should return the
+    # correct status codes in order, and the third should raise an
+    # exception.
+    with vcr.use_cassette(str(tmpdir.join("test.json")), match_on=["method"]):
+        assert urlopen(httpbin.url + "/status/200").getcode() == 200
+        assert urlopen(httpbin.url + "/status/201").getcode() == 201
+        with pytest.raises(Exception):
+            urlopen(httpbin.url + "/status/200")
```

### Comparing `vcrpy-4.2.1/tests/integration/test_basic.py` & `vcrpy-4.3.0/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/integration/test_ignore.py` & `vcrpy-4.3.0/tests/integration/test_ignore.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from urllib.request import urlopen
 import socket
 from contextlib import contextmanager
+from urllib.request import urlopen
+
 import vcr
 
 
 @contextmanager
 def overridden_dns(overrides):
     """
     Monkeypatch socket.getaddrinfo() to override DNS lookups (name will resolve
```

### Comparing `vcrpy-4.2.1/tests/integration/test_stubs.py` & `vcrpy-4.3.0/tests/integration/test_stubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import vcr
-import zlib
-import json
 import http.client as httplib
+import json
+import zlib
 
 from assertions import assert_is_json
 
+import vcr
+
 
 def _headers_are_case_insensitive(host, port):
     conn = httplib.HTTPConnection(host, port)
     conn.request("GET", "/cookies/set?k1=v1")
     r1 = conn.getresponse()
     cookie_data1 = r1.getheader("set-cookie")
     conn = httplib.HTTPConnection(host, port)
```

### Comparing `vcrpy-4.2.1/tests/integration/test_http` & `vcrpy-4.3.0/tests/integration/test_http`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/integration/test_urllib2.py` & `vcrpy-4.3.0/tests/integration/test_urllib2.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 """Integration tests with urllib2"""
 
 import ssl
-from urllib.request import urlopen
 from urllib.parse import urlencode
+from urllib.request import urlopen
+
 import pytest_httpbin.certs
+from assertions import assert_cassette_has_one_response
 
 # Internal imports
 import vcr
 
-from assertions import assert_cassette_has_one_response
-
 
 def urlopen_with_cafile(*args, **kwargs):
     context = ssl.create_default_context(cafile=pytest_httpbin.certs.where())
     context.check_hostname = False
     kwargs["context"] = context
     try:
         return urlopen(*args, **kwargs)
```

### Comparing `vcrpy-4.2.1/tests/integration/test_filter.py` & `vcrpy-4.3.0/tests/integration/test_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import base64
-import pytest
-from urllib.request import urlopen, Request
-from urllib.parse import urlencode
-from urllib.error import HTTPError
-import vcr
 import json
+from urllib.error import HTTPError
+from urllib.parse import urlencode
+from urllib.request import Request, urlopen
+
+import pytest
 from assertions import assert_cassette_has_one_response, assert_is_json
 
+import vcr
+
 
 def _request_with_auth(url, username, password):
     request = Request(url)
     base64string = base64.b64encode(username.encode("ascii") + b":" + password.encode("ascii"))
     request.add_header(b"Authorization", b"Basic " + base64string)
     return urlopen(request)
 
@@ -102,14 +104,26 @@
         urlopen(request)
     with vcr.use_cassette(cass_file) as cass:
         decoded_response = urlopen(url).read()
         assert_cassette_has_one_response(cass)
     assert_is_json(decoded_response)
 
 
+def test_decomptess_empty_body(tmpdir, httpbin):
+    url = httpbin.url + "/gzip"
+    request = Request(url, headers={"Accept-Encoding": ["gzip, deflate"]}, method="HEAD")
+    cass_file = str(tmpdir.join("gzip_empty_response.yaml"))
+    with vcr.use_cassette(cass_file, decode_compressed_response=True):
+        response = urlopen(request).read()
+    with vcr.use_cassette(cass_file) as cass:
+        decoded_response = urlopen(request).read()
+        assert_cassette_has_one_response(cass)
+    assert decoded_response == response
+
+
 def test_decompress_deflate(tmpdir, httpbin):
     url = httpbin.url + "/deflate"
     request = Request(url, headers={"Accept-Encoding": ["gzip, deflate"]})
     cass_file = str(tmpdir.join("deflate_response.yaml"))
     with vcr.use_cassette(cass_file, decode_compressed_response=True):
         urlopen(request)
     with vcr.use_cassette(cass_file) as cass:
```

### Comparing `vcrpy-4.2.1/tests/integration/test_aiohttp.py` & `vcrpy-4.3.0/tests/integration/test_aiohttp.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pytest
 
 asyncio = pytest.importorskip("asyncio")
 aiohttp = pytest.importorskip("aiohttp")
 
 import vcr  # noqa: E402
+
 from .aiohttp_utils import aiohttp_app, aiohttp_request  # noqa: E402
 
 
 def run_in_loop(fn):
     with contextlib.closing(asyncio.new_event_loop()) as loop:
         asyncio.set_event_loop(loop)
         task = loop.create_task(fn(loop))
@@ -29,112 +30,109 @@
     return request("GET", url, output=output, **kwargs)
 
 
 def post(url, output="text", **kwargs):
     return request("POST", url, output="text", **kwargs)
 
 
-@pytest.fixture(params=["https", "http"])
-def scheme(request):
-    """Fixture that returns both http and https."""
-    return request.param
-
+def test_status(tmpdir, mockbin_request_url):
+    url = mockbin_request_url
 
-def test_status(tmpdir, scheme):
-    url = scheme + "://httpbin.org"
     with vcr.use_cassette(str(tmpdir.join("status.yaml"))):
         response, _ = get(url)
 
     with vcr.use_cassette(str(tmpdir.join("status.yaml"))) as cassette:
         cassette_response, _ = get(url)
         assert cassette_response.status == response.status
         assert cassette.play_count == 1
 
 
 @pytest.mark.parametrize("auth", [None, aiohttp.BasicAuth("vcrpy", "test")])
-def test_headers(tmpdir, scheme, auth):
-    url = scheme + "://httpbin.org"
+def test_headers(tmpdir, auth, mockbin_request_url):
+    url = mockbin_request_url
     with vcr.use_cassette(str(tmpdir.join("headers.yaml"))):
         response, _ = get(url, auth=auth)
 
     with vcr.use_cassette(str(tmpdir.join("headers.yaml"))) as cassette:
         if auth is not None:
             request = cassette.requests[0]
             assert "AUTHORIZATION" in request.headers
         cassette_response, _ = get(url, auth=auth)
         assert dict(cassette_response.headers) == dict(response.headers)
         assert cassette.play_count == 1
         assert "istr" not in cassette.data[0]
         assert "yarl.URL" not in cassette.data[0]
 
 
-def test_case_insensitive_headers(tmpdir, scheme):
-    url = scheme + "://httpbin.org"
+def test_case_insensitive_headers(tmpdir, mockbin_request_url):
+    url = mockbin_request_url
+
     with vcr.use_cassette(str(tmpdir.join("whatever.yaml"))):
         _, _ = get(url)
 
     with vcr.use_cassette(str(tmpdir.join("whatever.yaml"))) as cassette:
         cassette_response, _ = get(url)
         assert "Content-Type" in cassette_response.headers
         assert "content-type" in cassette_response.headers
         assert cassette.play_count == 1
 
 
-def test_text(tmpdir, scheme):
-    url = scheme + "://httpbin.org"
+def test_text(tmpdir, mockbin_request_url):
+    url = mockbin_request_url
+
     with vcr.use_cassette(str(tmpdir.join("text.yaml"))):
         _, response_text = get(url)
 
     with vcr.use_cassette(str(tmpdir.join("text.yaml"))) as cassette:
         _, cassette_response_text = get(url)
         assert cassette_response_text == response_text
         assert cassette.play_count == 1
 
 
-def test_json(tmpdir, scheme):
-    url = scheme + "://httpbin.org/get"
+def test_json(tmpdir, mockbin_request_url):
+    url = mockbin_request_url
     headers = {"Content-Type": "application/json"}
 
     with vcr.use_cassette(str(tmpdir.join("json.yaml"))):
         _, response_json = get(url, output="json", headers=headers)
 
     with vcr.use_cassette(str(tmpdir.join("json.yaml"))) as cassette:
         _, cassette_response_json = get(url, output="json", headers=headers)
         assert cassette_response_json == response_json
         assert cassette.play_count == 1
 
 
-def test_binary(tmpdir, scheme):
-    url = scheme + "://httpbin.org/image/png"
+def test_binary(tmpdir, mockbin_request_url):
+    url = mockbin_request_url + "/image/png"
     with vcr.use_cassette(str(tmpdir.join("binary.yaml"))):
         _, response_binary = get(url, output="raw")
 
     with vcr.use_cassette(str(tmpdir.join("binary.yaml"))) as cassette:
         _, cassette_response_binary = get(url, output="raw")
         assert cassette_response_binary == response_binary
         assert cassette.play_count == 1
 
 
-def test_stream(tmpdir, scheme):
-    url = scheme + "://httpbin.org/get"
+def test_stream(tmpdir, mockbin_request_url):
+    url = mockbin_request_url
 
     with vcr.use_cassette(str(tmpdir.join("stream.yaml"))):
-        resp, body = get(url, output="raw")  # Do not use stream here, as the stream is exhausted by vcr
+        _, body = get(url, output="raw")  # Do not use stream here, as the stream is exhausted by vcr
 
     with vcr.use_cassette(str(tmpdir.join("stream.yaml"))) as cassette:
-        cassette_resp, cassette_body = get(url, output="stream")
+        _, cassette_body = get(url, output="stream")
         assert cassette_body == body
         assert cassette.play_count == 1
 
 
 @pytest.mark.parametrize("body", ["data", "json"])
-def test_post(tmpdir, scheme, body, caplog):
+def test_post(tmpdir, body, caplog, mockbin_request_url):
     caplog.set_level(logging.INFO)
     data = {"key1": "value1", "key2": "value2"}
-    url = scheme + "://httpbin.org/post"
+    url = mockbin_request_url
     with vcr.use_cassette(str(tmpdir.join("post.yaml"))):
         _, response_json = post(url, **{body: data})
 
     with vcr.use_cassette(str(tmpdir.join("post.yaml"))) as cassette:
         request = cassette.requests[0]
         assert request.body == data
         _, cassette_response_json = post(url, **{body: data})
@@ -147,31 +145,31 @@
             for log in caplog.records
             if log.getMessage() == "<Request (POST) {}> not in cassette, sending to real server".format(url)
         ),
         None,
     ), "Log message not found."
 
 
-def test_params(tmpdir, scheme):
-    url = scheme + "://httpbin.org/get?d=d"
+def test_params(tmpdir, mockbin_request_url):
+    url = mockbin_request_url + "?d=d"
     headers = {"Content-Type": "application/json"}
     params = {"a": 1, "b": 2, "c": "c"}
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         _, response_json = get(url, output="json", params=params, headers=headers)
-        assert response_json["args"] == {"a": "1", "b": "2", "c": "c", "d": "d"}
+        assert response_json["queryString"] == {"a": "1", "b": "2", "c": "c", "d": "d"}
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         _, cassette_response_json = get(url, output="json", params=params, headers=headers)
         assert cassette_response_json == response_json
         assert cassette.play_count == 1
 
 
-def test_params_same_url_distinct_params(tmpdir, scheme):
-    url = scheme + "://httpbin.org/get"
+def test_params_same_url_distinct_params(tmpdir, mockbin_request_url):
+    url = mockbin_request_url
     headers = {"Content-Type": "application/json"}
     params = {"a": 1, "b": 2, "c": "c"}
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         _, response_json = get(url, output="json", params=params, headers=headers)
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
@@ -181,16 +179,16 @@
 
     other_params = {"other": "params"}
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         with pytest.raises(vcr.errors.CannotOverwriteExistingCassetteException):
             get(url, output="text", params=other_params)
 
 
-def test_params_on_url(tmpdir, scheme):
-    url = scheme + "://httpbin.org/get?a=1&b=foo"
+def test_params_on_url(tmpdir, mockbin_request_url):
+    url = mockbin_request_url + "?a=1&b=foo"
     headers = {"Content-Type": "application/json"}
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         _, response_json = get(url, output="json", headers=headers)
         request = cassette.requests[0]
         assert request.url == url
 
@@ -246,16 +244,16 @@
     request = cassette.requests[0]
     assert request.url == str(client.make_url(url))
     response_json = loop.run_until_complete(response.json())
     assert response_json is None
     assert cassette.play_count == 1
 
 
-def test_redirect(aiohttp_client, tmpdir):
-    url = "https://mockbin.org/redirect/302/2"
+def test_redirect(tmpdir, mockbin):
+    url = mockbin + "/redirect/302/2"
 
     with vcr.use_cassette(str(tmpdir.join("redirect.yaml"))):
         response, _ = get(url)
 
     with vcr.use_cassette(str(tmpdir.join("redirect.yaml"))) as cassette:
         cassette_response, _ = get(url)
 
@@ -270,38 +268,38 @@
     assert cassette_response.request_info.method == response.request_info.method
     assert {k: v for k, v in cassette_response.request_info.headers.items()} == {
         k: v for k, v in response.request_info.headers.items()
     }
     assert cassette_response.request_info.real_url == response.request_info.real_url
 
 
-def test_not_modified(aiohttp_client, tmpdir):
+def test_not_modified(tmpdir, mockbin):
     """It doesn't try to redirect on 304"""
-    url = "https://httpbin.org/status/304"
+    url = mockbin + "/status/304"
 
     with vcr.use_cassette(str(tmpdir.join("not_modified.yaml"))):
         response, _ = get(url)
 
     with vcr.use_cassette(str(tmpdir.join("not_modified.yaml"))) as cassette:
         cassette_response, _ = get(url)
 
         assert cassette_response.status == 304
         assert response.status == 304
         assert len(cassette_response.history) == len(response.history)
         assert len(cassette) == 1
         assert cassette.play_count == 1
 
 
-def test_double_requests(tmpdir):
+def test_double_requests(tmpdir, mockbin_request_url):
     """We should capture, record, and replay all requests and response chains,
     even if there are duplicate ones.
 
     We should replay in the order we saw them.
     """
-    url = "https://httpbin.org/get"
+    url = mockbin_request_url
 
     with vcr.use_cassette(str(tmpdir.join("text.yaml"))):
         _, response_text1 = get(url, output="text")
         _, response_text2 = get(url, output="text")
 
     with vcr.use_cassette(str(tmpdir.join("text.yaml"))) as cassette:
         resp, cassette_response_text = get(url, output="text")
@@ -398,16 +396,16 @@
                 assert not cookies_resp.cookies
                 cookies = session.cookie_jar.filter_cookies(cookies_url)
                 assert cookies["Cookie_1"].value == "Val_1"
 
     run_in_loop(run)
 
 
-def test_not_allow_redirects(tmpdir):
-    url = "https://mockbin.org/redirect/308/5"
+def test_not_allow_redirects(tmpdir, mockbin):
+    url = mockbin + "/redirect/308/5"
     path = str(tmpdir.join("redirects.yaml"))
 
     with vcr.use_cassette(path):
         response, _ = get(url, allow_redirects=False)
         assert response.url.path == "/redirect/308/5"
         assert response.status == 308
```

### Comparing `vcrpy-4.2.1/tests/integration/test_register_persister.py` & `vcrpy-4.3.0/tests/integration/test_register_persister.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/integration/test_boto3.py` & `vcrpy-4.3.0/tests/integration/test_boto3.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import pytest
 import os
 
+import pytest
+
 boto3 = pytest.importorskip("boto3")
 
 import boto3  # NOQA
 import botocore  # NOQA
+
 import vcr  # NOQA
 
 try:
     from botocore import awsrequest  # NOQA
 
     botocore_awsrequest = True
 except ImportError:
@@ -51,40 +53,21 @@
             # Default client set with fixture `iam_client`
             client = iam_client()
         return client.get_user(UserName=user_name)
 
     return _get_user
 
 
-@boto3_skip_vendored_requests
-def test_boto_vendored_stubs(tmpdir):
-    with vcr.use_cassette(str(tmpdir.join("boto3-stubs.yml"))):
-        # Perform the imports within the patched context so that
-        # HTTPConnection, VerifiedHTTPSConnection refers to the patched version.
-        from botocore.vendored.requests.packages.urllib3.connectionpool import (
-            HTTPConnection,
-            VerifiedHTTPSConnection,
-        )
-        from vcr.stubs.boto3_stubs import VCRRequestsHTTPConnection, VCRRequestsHTTPSConnection
-
-        # Prove that the class was patched by the stub and that we can instantiate it.
-        assert issubclass(HTTPConnection, VCRRequestsHTTPConnection)
-        assert issubclass(VerifiedHTTPSConnection, VCRRequestsHTTPSConnection)
-        HTTPConnection("hostname.does.not.matter")
-        VerifiedHTTPSConnection("hostname.does.not.matter")
-
-
 @pytest.mark.skipif(
     os.environ.get("TRAVIS_PULL_REQUEST") != "false",
     reason="Encrypted Environment Variables from Travis Repository Settings"
     " are disabled on PRs from forks. "
     "https://docs.travis-ci.com/user/pull-requests/#pull-requests-and-security-restrictions",
 )
 def test_boto_medium_difficulty(tmpdir, get_user):
-
     with vcr.use_cassette(str(tmpdir.join("boto3-medium.yml"))):
         response = get_user()
         assert response["User"]["UserName"] == IAM_USER_NAME
 
     with vcr.use_cassette(str(tmpdir.join("boto3-medium.yml"))) as cass:
         response = get_user()
         assert response["User"]["UserName"] == IAM_USER_NAME
```

### Comparing `vcrpy-4.2.1/tests/integration/test_request.py` & `vcrpy-4.3.0/tests/integration/test_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import vcr
 from urllib.request import urlopen
 
+import vcr
+
 
 def test_recorded_request_uri_with_redirected_request(tmpdir, httpbin):
     with vcr.use_cassette(str(tmpdir.join("test.yml"))) as cass:
         assert len(cass) == 0
         urlopen(httpbin.url + "/redirect/3")
         assert cass.requests[0].uri == httpbin.url + "/redirect/3"
         assert cass.requests[3].uri == httpbin.url + "/get"
```

### Comparing `vcrpy-4.2.1/tests/integration/test_wild.py` & `vcrpy-4.3.0/tests/integration/test_wild.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import http.client as httplib
 import multiprocessing
-import pytest
 from xmlrpc.client import ServerProxy
 from xmlrpc.server import SimpleXMLRPCServer
 
+import pytest
+
 requests = pytest.importorskip("requests")
 
 import vcr  # NOQA
 
 
 def test_domain_redirect():
     """Ensure that redirects across domains are considered unique"""
@@ -79,15 +80,15 @@
 def start_rpc_server(q):
     httpd = SimpleXMLRPCServer(("127.0.0.1", 0))
     httpd.register_function(pow)
     q.put("http://{}:{}".format(*httpd.server_address))
     httpd.serve_forever()
 
 
-@pytest.yield_fixture(scope="session")
+@pytest.fixture(scope="session")
 def rpc_server():
     q = multiprocessing.Queue()
     proxy_process = multiprocessing.Process(target=start_rpc_server, args=(q,))
     try:
         proxy_process.start()
         yield q.get()
     finally:
```

### Comparing `vcrpy-4.2.1/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml` & `vcrpy-4.3.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       connection:
       - keep-alive
       host:
       - httpbin.org
       user-agent:
       - python-httpx/0.12.1
     method: GET
-    uri: https://httpbin.org/headers
+    uri: https://mockbin.org/headers
   response:
     content: "{\n  \"headers\": {\n    \"Accept\": \"*/*\", \n    \"Accept-Encoding\"\
       : \"gzip, deflate, br\", \n    \"Host\": \"httpbin.org\", \n    \"User-Agent\"\
       : \"python-httpx/0.12.1\", \n    \"X-Amzn-Trace-Id\": \"Root=1-5ea778c9-ea76170da792abdbf7614067\"\
       \n  }\n}\n"
     headers:
       access-control-allow-credentials:
```

### Comparing `vcrpy-4.2.1/tests/integration/test_register_serializer.py` & `vcrpy-4.3.0/tests/integration/test_register_serializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/integration/aiohttp_utils.py` & `vcrpy-4.3.0/tests/integration/aiohttp_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # flake8: noqa
 import asyncio
 
 import aiohttp
-from aiohttp.test_utils import TestClient
 
 
 async def aiohttp_request(loop, method, url, output="text", encoding="utf-8", content_type=None, **kwargs):
     session = aiohttp.ClientSession(loop=loop)
     response_ctx = session.request(method, url, **kwargs)
 
     response = await response_ctx.__aenter__()
```

### Comparing `vcrpy-4.2.1/tests/integration/test_boto.py` & `vcrpy-4.3.0/tests/integration/test_boto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import pytest
 
 boto = pytest.importorskip("boto")
 
+from configparser import DuplicateSectionError  # NOQA
+
 import boto  # NOQA
 import boto.iam  # NOQA
 from boto.s3.connection import S3Connection  # NOQA
 from boto.s3.key import Key  # NOQA
-from configparser import DuplicateSectionError  # NOQA
+
 import vcr  # NOQA
 
 
 def test_boto_stubs(tmpdir):
     with vcr.use_cassette(str(tmpdir.join("boto-stubs.yml"))):
         # Perform the imports within the patched context so that
         # CertValidatingHTTPSConnection refers to the patched version.
         from boto.https_connection import CertValidatingHTTPSConnection
+
         from vcr.stubs.boto_stubs import VCRCertValidatingHTTPSConnection
 
         # Prove that the class was patched by the stub and that we can instantiate it.
         assert issubclass(CertValidatingHTTPSConnection, VCRCertValidatingHTTPSConnection)
         CertValidatingHTTPSConnection("hostname.does.not.matter")
```

### Comparing `vcrpy-4.2.1/tests/integration/test_matchers.py` & `vcrpy-4.3.0/tests/integration/test_matchers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import vcr
-import pytest
 from urllib.request import urlopen
 
+import pytest
+
+import vcr
 
 DEFAULT_URI = "http://httpbin.org/get?p1=q1&p2=q2"  # base uri for testing
 
 
 def _replace_httpbin(uri, httpbin, httpbin_secure):
     return uri.replace("http://httpbin.org", httpbin.url).replace("https://httpbin.org", httpbin_secure.url)
 
@@ -31,15 +32,14 @@
         ("scheme", "http://google.com/post?a=b", "https://httpbin.org/get?p1=q1&p2=q2"),
         ("host", "https://httpbin.org/post?a=b", "http://google.com/get?p1=q1&p2=q2"),
         ("path", "https://google.com/get?a=b", "http://httpbin.org/post?p1=q1&p2=q2"),
         ("query", "https://google.com/get?p2=q2&p1=q1", "http://httpbin.org/get?p1=q1&a=b"),
     ],
 )
 def test_matchers(httpbin, httpbin_secure, cassette, matcher, matching_uri, not_matching_uri):
-
     matching_uri = _replace_httpbin(matching_uri, httpbin, httpbin_secure)
     not_matching_uri = _replace_httpbin(not_matching_uri, httpbin, httpbin_secure)
     default_uri = _replace_httpbin(DEFAULT_URI, httpbin, httpbin_secure)
 
     # play cassette with default uri
     with vcr.use_cassette(cassette, match_on=[matcher]) as cass:
         urlopen(default_uri)
@@ -71,15 +71,14 @@
             urlopen(default_uri, data=b"")
 
 
 @pytest.mark.parametrize(
     "uri", [DEFAULT_URI, "http://httpbin.org/get?p2=q2&p1=q1", "http://httpbin.org/get?p2=q2&p1=q1"]
 )
 def test_default_matcher_matches(cassette, uri, httpbin, httpbin_secure):
-
     uri = _replace_httpbin(uri, httpbin, httpbin_secure)
 
     with vcr.use_cassette(cassette) as cass:
         urlopen(uri)
         assert cass.play_count == 1
```

### Comparing `vcrpy-4.2.1/tests/integration/test_record_mode.py` & `vcrpy-4.3.0/tests/integration/test_record_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from urllib.request import urlopen
+
 import pytest
+
 import vcr
-from urllib.request import urlopen
 
 
 def test_once_record_mode(tmpdir, httpbin):
     testfile = str(tmpdir.join("recordmode.yml"))
     with vcr.use_cassette(testfile, record_mode=vcr.mode.ONCE):
         # cassette file doesn't exist, so create.
         urlopen(httpbin.url).read()
```

### Comparing `vcrpy-4.2.1/tests/integration/test_requests.py` & `vcrpy-4.3.0/tests/integration/test_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Test requests' interaction with vcr"""
 import pytest
-import vcr
 from assertions import assert_cassette_empty, assert_is_json
 
+import vcr
+
 requests = pytest.importorskip("requests")
 from requests.exceptions import ConnectionError  # noqa E402
 
 
 def test_status_code(httpbin_both, tmpdir):
     """Ensure that we can read the status code"""
     url = httpbin_both.url + "/"
```

### Comparing `vcrpy-4.2.1/tests/integration/test_tornado_with_decorator_use_cassette.yaml` & `vcrpy-4.3.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/integration/test_config.py` & `vcrpy-4.3.0/tests/integration/test_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,82 @@
-import os
 import json
+import os
+from urllib.request import urlopen
+
 import pytest
+
 import vcr
-from urllib.request import urlopen
 
 
-def test_set_serializer_default_config(tmpdir, httpbin):
+def test_set_serializer_default_config(tmpdir, mockbin_request_url):
     my_vcr = vcr.VCR(serializer="json")
 
     with my_vcr.use_cassette(str(tmpdir.join("test.json"))):
         assert my_vcr.serializer == "json"
-        urlopen(httpbin.url + "/get")
+        urlopen(mockbin_request_url)
 
     with open(str(tmpdir.join("test.json"))) as f:
         file_content = f.read()
         assert file_content.endswith("\n")
         assert json.loads(file_content)
 
 
-def test_default_set_cassette_library_dir(tmpdir, httpbin):
+def test_default_set_cassette_library_dir(tmpdir, mockbin_request_url):
     my_vcr = vcr.VCR(cassette_library_dir=str(tmpdir.join("subdir")))
 
     with my_vcr.use_cassette("test.json"):
-        urlopen(httpbin.url + "/get")
+        urlopen(mockbin_request_url)
 
     assert os.path.exists(str(tmpdir.join("subdir").join("test.json")))
 
 
-def test_override_set_cassette_library_dir(tmpdir, httpbin):
+def test_override_set_cassette_library_dir(tmpdir, mockbin_request_url):
     my_vcr = vcr.VCR(cassette_library_dir=str(tmpdir.join("subdir")))
 
     cld = str(tmpdir.join("subdir2"))
 
     with my_vcr.use_cassette("test.json", cassette_library_dir=cld):
-        urlopen(httpbin.url + "/get")
+        urlopen(mockbin_request_url)
 
     assert os.path.exists(str(tmpdir.join("subdir2").join("test.json")))
     assert not os.path.exists(str(tmpdir.join("subdir").join("test.json")))
 
 
-def test_override_match_on(tmpdir, httpbin):
+def test_override_match_on(tmpdir, mockbin_request_url):
     my_vcr = vcr.VCR(match_on=["method"])
 
     with my_vcr.use_cassette(str(tmpdir.join("test.json"))):
-        urlopen(httpbin.url)
+        urlopen(mockbin_request_url)
 
     with my_vcr.use_cassette(str(tmpdir.join("test.json"))) as cass:
-        urlopen(httpbin.url + "/get")
+        urlopen(mockbin_request_url)
 
     assert len(cass) == 1
     assert cass.play_count == 1
 
 
 def test_missing_matcher():
     my_vcr = vcr.VCR()
     my_vcr.register_matcher("awesome", object)
     with pytest.raises(KeyError):
         with my_vcr.use_cassette("test.yaml", match_on=["notawesome"]):
             pass
+
+
+def test_dont_record_on_exception(tmpdir, mockbin_request_url):
+    my_vcr = vcr.VCR(record_on_exception=False)
+
+    @my_vcr.use_cassette(str(tmpdir.join("dontsave.yml")))
+    def some_test():
+        assert b"Not in content" in urlopen(mockbin_request_url)
+
+    with pytest.raises(AssertionError):
+        some_test()
+
+    assert not os.path.exists(str(tmpdir.join("dontsave.yml")))
+
+    # Make sure context decorator has the same behavior
+    with pytest.raises(AssertionError):
+        with my_vcr.use_cassette(str(tmpdir.join("dontsave2.yml"))):
+            assert b"Not in content" in urlopen(mockbin_request_url).read()
+
+    assert not os.path.exists(str(tmpdir.join("dontsave2.yml")))
```

### Comparing `vcrpy-4.2.1/tests/integration/test_tornado.py` & `vcrpy-4.3.0/tests/integration/test_tornado.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 """Test requests' interaction with vcr"""
 
 import json
 
 import pytest
+from assertions import assert_cassette_empty, assert_is_json
+
 import vcr
 from vcr.errors import CannotOverwriteExistingCassetteException
 
-from assertions import assert_cassette_empty, assert_is_json
-
 tornado = pytest.importorskip("tornado")
 http = pytest.importorskip("tornado.httpclient")
 
 # whether the current version of Tornado supports the raise_error argument for
 # fetch().
 supports_raise_error = tornado.version_info >= (4,)
 
@@ -40,20 +40,14 @@
 
 def post(client, url, data=None, **kwargs):
     if data:
         kwargs["body"] = json.dumps(data)
     return client.fetch(http.HTTPRequest(url, method="POST", **kwargs))
 
 
-@pytest.fixture(params=["https", "http"])
-def scheme(request):
-    """Fixture that returns both http and https."""
-    return request.param
-
-
 @pytest.mark.gen_test
 def test_status_code(get_client, scheme, tmpdir):
     """Ensure that we can read the status code"""
     url = scheme + "://httpbin.org/"
     with vcr.use_cassette(str(tmpdir.join("atts.yaml"))):
         status_code = (yield get(get_client(), url)).code
```

### Comparing `vcrpy-4.2.1/tests/integration/test_proxy.py` & `vcrpy-4.3.0/tests/integration/test_proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # -*- coding: utf-8 -*-
 """Test using a proxy."""
 
-# External imports
-import multiprocessing
-import pytest
-
 import http.server
+import multiprocessing
 import socketserver
 from urllib.request import urlopen
 
-# Internal imports
+import pytest
+
 import vcr
 
 # Conditional imports
 requests = pytest.importorskip("requests")
 
 
 class Proxy(http.server.SimpleHTTPRequestHandler):
@@ -35,15 +33,15 @@
         self.send_response(status, upstream_response.msg)
         for header in headers:
             self.send_header(*header)
         self.end_headers()
         self.copyfile(upstream_response, self.wfile)
 
 
-@pytest.yield_fixture(scope="session")
+@pytest.fixture(scope="session")
 def proxy_server():
     httpd = socketserver.ThreadingTCPServer(("", 0), Proxy)
     proxy_process = multiprocessing.Process(target=httpd.serve_forever)
     proxy_process.start()
     yield "http://{}:{}".format(*httpd.server_address)
     proxy_process.terminate()
```

### Comparing `vcrpy-4.2.1/tests/integration/test_httpx.py` & `vcrpy-4.3.0/tests/integration/test_httpx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import pytest
 import os
 
+import pytest
+
 asyncio = pytest.importorskip("asyncio")
 httpx = pytest.importorskip("httpx")
 
 import vcr  # noqa: E402
 from vcr.stubs.httpx_stubs import HTTPX_REDIRECT_PARAM  # noqa: E402
 
 
@@ -75,72 +76,74 @@
         with self:
             return self(*args, **kwargs)
 
 
 def pytest_generate_tests(metafunc):
     if "do_request" in metafunc.fixturenames:
         metafunc.parametrize("do_request", [DoAsyncRequest, DoSyncRequest])
-    if "scheme" in metafunc.fixturenames:
-        metafunc.parametrize("scheme", ["http", "https"])
 
 
 @pytest.fixture
 def yml(tmpdir, request):
     return str(tmpdir.join(request.function.__name__ + ".yaml"))
 
 
-def test_status(tmpdir, scheme, do_request):
-    url = scheme + "://mockbin.org/request"
+def test_status(tmpdir, mockbin, do_request):
+    url = mockbin
+
     with vcr.use_cassette(str(tmpdir.join("status.yaml"))):
         response = do_request()("GET", url)
 
     with vcr.use_cassette(str(tmpdir.join("status.yaml"))) as cassette:
         cassette_response = do_request()("GET", url)
         assert cassette_response.status_code == response.status_code
         assert cassette.play_count == 1
 
 
-def test_case_insensitive_headers(tmpdir, scheme, do_request):
-    url = scheme + "://mockbin.org/request"
+def test_case_insensitive_headers(tmpdir, mockbin, do_request):
+    url = mockbin
+
     with vcr.use_cassette(str(tmpdir.join("whatever.yaml"))):
         do_request()("GET", url)
 
     with vcr.use_cassette(str(tmpdir.join("whatever.yaml"))) as cassette:
         cassette_response = do_request()("GET", url)
         assert "Content-Type" in cassette_response.headers
         assert "content-type" in cassette_response.headers
         assert cassette.play_count == 1
 
 
-def test_content(tmpdir, scheme, do_request):
-    url = scheme + "://httpbin.org"
+def test_content(tmpdir, mockbin, do_request):
+    url = mockbin
+
     with vcr.use_cassette(str(tmpdir.join("cointent.yaml"))):
         response = do_request()("GET", url)
 
     with vcr.use_cassette(str(tmpdir.join("cointent.yaml"))) as cassette:
         cassette_response = do_request()("GET", url)
         assert cassette_response.content == response.content
         assert cassette.play_count == 1
 
 
-def test_json(tmpdir, scheme, do_request):
-    url = scheme + "://httpbin.org/get"
-    headers = {"Content-Type": "application/json"}
+def test_json(tmpdir, mockbin, do_request):
+    url = mockbin + "/request"
+
+    headers = {"content-type": "application/json"}
 
     with vcr.use_cassette(str(tmpdir.join("json.yaml"))):
         response = do_request(headers=headers)("GET", url)
 
     with vcr.use_cassette(str(tmpdir.join("json.yaml"))) as cassette:
         cassette_response = do_request(headers=headers)("GET", url)
         assert cassette_response.json() == response.json()
         assert cassette.play_count == 1
 
 
-def test_params_same_url_distinct_params(tmpdir, scheme, do_request):
-    url = scheme + "://httpbin.org/get"
+def test_params_same_url_distinct_params(tmpdir, mockbin, do_request):
+    url = mockbin + "/request"
     headers = {"Content-Type": "application/json"}
     params = {"a": 1, "b": False, "c": "c"}
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         response = do_request()("GET", url, params=params, headers=headers)
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
@@ -151,16 +154,16 @@
 
     params = {"other": "params"}
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         with pytest.raises(vcr.errors.CannotOverwriteExistingCassetteException):
             do_request()("GET", url, params=params, headers=headers)
 
 
-def test_redirect(tmpdir, do_request, yml):
-    url = "https://mockbin.org/redirect/303/2"
+def test_redirect(mockbin, yml, do_request):
+    url = mockbin + "/redirect/303/2"
 
     redirect_kwargs = {HTTPX_REDIRECT_PARAM.name: True}
 
     response = do_request()("GET", url, **redirect_kwargs)
     with vcr.use_cassette(yml):
         response = do_request()("GET", url, **redirect_kwargs)
 
@@ -177,43 +180,46 @@
     assert cassette_response.request.url == response.request.url
     assert cassette_response.request.method == response.request.method
     assert {k: v for k, v in cassette_response.request.headers.items()} == {
         k: v for k, v in response.request.headers.items()
     }
 
 
-def test_work_with_gzipped_data(tmpdir, do_request, yml):
+def test_work_with_gzipped_data(mockbin, do_request, yml):
+    url = mockbin + "/gzip?foo=bar"
+    headers = {"accept-encoding": "deflate, gzip"}
+
     with vcr.use_cassette(yml):
-        do_request()("GET", "https://httpbin.org/gzip")
+        do_request(headers=headers)("GET", url)
 
     with vcr.use_cassette(yml) as cassette:
-        cassette_response = do_request()("GET", "https://httpbin.org/gzip")
+        cassette_response = do_request(headers=headers)("GET", url)
 
-        assert "gzip" in cassette_response.json()["headers"]["Accept-Encoding"]
+        assert cassette_response.headers["content-encoding"] == "gzip"
         assert cassette_response.read()
         assert cassette.play_count == 1
 
 
 @pytest.mark.parametrize("url", ["https://github.com/kevin1024/vcrpy/issues/" + str(i) for i in range(3, 6)])
-def test_simple_fetching(tmpdir, do_request, yml, url):
+def test_simple_fetching(do_request, yml, url):
     with vcr.use_cassette(yml):
         do_request()("GET", url)
 
     with vcr.use_cassette(yml) as cassette:
         cassette_response = do_request()("GET", url)
         assert str(cassette_response.request.url) == url
         assert cassette.play_count == 1
 
 
 def test_behind_proxy(do_request):
     # This is recorded because otherwise we should have a live proxy somewhere.
     yml = (
         os.path.dirname(os.path.realpath(__file__)) + "/cassettes/" + "test_httpx_test_test_behind_proxy.yml"
     )
-    url = "https://httpbin.org/headers"
+    url = "https://mockbin.org/headers"
     proxy = "http://localhost:8080"
     proxies = {"http://": proxy, "https://": proxy}
 
     with vcr.use_cassette(yml):
         response = do_request(proxies=proxies, verify=False)("GET", url)
 
     with vcr.use_cassette(yml) as cassette:
@@ -221,70 +227,71 @@
         assert str(cassette_response.request.url) == url
         assert cassette.play_count == 1
 
         assert cassette_response.headers["Via"] == "my_own_proxy", str(cassette_response.headers)
         assert cassette_response.request.url == response.request.url
 
 
-def test_cookies(tmpdir, scheme, do_request):
+def test_cookies(tmpdir, mockbin, do_request):
     def client_cookies(client):
         return [c for c in client.client.cookies]
 
     def response_cookies(response):
         return [c for c in response.cookies]
 
-    with do_request() as client:
+    url = mockbin + "/bin/26148652-fe25-4f21-aaf5-689b5b4bf65f"
+    headers = {"cookie": "k1=v1;k2=v2"}
+
+    with do_request(headers=headers) as client:
         assert client_cookies(client) == []
 
         redirect_kwargs = {HTTPX_REDIRECT_PARAM.name: True}
 
-        url = scheme + "://httpbin.org"
         testfile = str(tmpdir.join("cookies.yml"))
         with vcr.use_cassette(testfile):
-            r1 = client("GET", url + "/cookies/set?k1=v1&k2=v2", **redirect_kwargs)
-            assert response_cookies(r1.history[0]) == ["k1", "k2"]
-            assert response_cookies(r1) == []
+            r1 = client("GET", url, **redirect_kwargs)
+
+            assert response_cookies(r1) == ["k1", "k2"]
 
-            r2 = client("GET", url + "/cookies", **redirect_kwargs)
-            assert len(r2.json()["cookies"]) == 2
+            r2 = client("GET", url, **redirect_kwargs)
 
+            assert response_cookies(r2) == ["k1", "k2"]
             assert client_cookies(client) == ["k1", "k2"]
 
-    with do_request() as new_client:
+    with do_request(headers=headers) as new_client:
         assert client_cookies(new_client) == []
 
         with vcr.use_cassette(testfile) as cassette:
-            cassette_response = new_client("GET", url + "/cookies/set?k1=v1&k2=v2")
-            assert response_cookies(cassette_response.history[0]) == ["k1", "k2"]
-            assert response_cookies(cassette_response) == []
+            cassette_response = new_client("GET", url)
 
-            assert cassette.play_count == 2
+            assert cassette.play_count == 1
+            assert response_cookies(cassette_response) == ["k1", "k2"]
             assert client_cookies(new_client) == ["k1", "k2"]
 
 
-def test_relative_redirects(tmpdir, scheme, do_request):
+def test_relative_redirects(tmpdir, scheme, do_request, mockbin):
     redirect_kwargs = {HTTPX_REDIRECT_PARAM.name: True}
 
-    url = scheme + "://mockbin.com/redirect/301?to=/redirect/301?to=/request"
+    url = mockbin + "/redirect/301?to=/redirect/301?to=/request"
     testfile = str(tmpdir.join("relative_redirects.yml"))
     with vcr.use_cassette(testfile):
         response = do_request()("GET", url, **redirect_kwargs)
         assert len(response.history) == 2, response
         assert response.json()["url"].endswith("request")
 
     with vcr.use_cassette(testfile) as cassette:
         response = do_request()("GET", url, **redirect_kwargs)
         assert len(response.history) == 2
         assert response.json()["url"].endswith("request")
 
         assert cassette.play_count == 3
 
 
-def test_redirect_wo_allow_redirects(do_request, yml):
-    url = "https://mockbin.org/redirect/308/5"
+def test_redirect_wo_allow_redirects(do_request, mockbin, yml):
+    url = mockbin + "/redirect/308/5"
 
     redirect_kwargs = {HTTPX_REDIRECT_PARAM.name: False}
 
     with vcr.use_cassette(yml):
         response = do_request()("GET", url, **redirect_kwargs)
 
         assert str(response.url).endswith("308/5")
```

### Comparing `vcrpy-4.2.1/tests/integration/test_httplib2.py` & `vcrpy-4.3.0/tests/integration/test_httplib2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # -*- coding: utf-8 -*-
 """Integration tests with httplib2"""
-
-import sys
-
 from urllib.parse import urlencode
+
 import pytest
 import pytest_httpbin.certs
+from assertions import assert_cassette_has_one_response
 
 import vcr
 
-from assertions import assert_cassette_has_one_response
-
 httplib2 = pytest.importorskip("httplib2")
 
 
 def http():
     """
     Returns an httplib2 HTTP instance
     with the certificate replaced by the httpbin one.
     """
     kwargs = {"ca_certs": pytest_httpbin.certs.where()}
-    if sys.version_info[:2] in [(2, 7), (3, 7)]:
-        kwargs["disable_ssl_certificate_validation"] = True
     return httplib2.Http(**kwargs)
 
 
 def test_response_code(tmpdir, httpbin_both):
     """Ensure we can read a response code from a fetch"""
     url = httpbin_both.url
     with vcr.use_cassette(str(tmpdir.join("atts.yaml"))):
```

### Comparing `vcrpy-4.2.1/tests/integration/test_tornado_exception_can_be_caught.yaml` & `vcrpy-4.3.0/tests/integration/test_tornado_exception_can_be_caught.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/fixtures/wild/domain_redirect.yaml` & `vcrpy-4.3.0/tests/fixtures/wild/domain_redirect.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/fixtures/migration/new_cassette.json` & `vcrpy-4.3.0/tests/fixtures/migration/new_cassette.json`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/fixtures/migration/new_cassette.yaml` & `vcrpy-4.3.0/tests/fixtures/migration/new_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/fixtures/migration/old_cassette.json` & `vcrpy-4.3.0/tests/fixtures/migration/old_cassette.json`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/tests/fixtures/migration/old_cassette.yaml` & `vcrpy-4.3.0/tests/fixtures/migration/old_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/vcr/serialize.py` & `vcrpy-4.3.0/vcr/serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from vcr.serializers import compat
-from vcr.request import Request
 import yaml
 
+from vcr.request import Request
+from vcr.serializers import compat
+
 # version 1 cassettes started with VCR 1.0.x.
 # Before 1.0.x, there was no versioning.
 CASSETTE_FORMAT_VERSION = 1
 
 """
 Just a general note on the serialization philosophy here:
 I prefer cassettes to be human-readable if possible.  Yaml serializes
```

### Comparing `vcrpy-4.2.1/vcr/patch.py` & `vcrpy-4.3.0/vcr/patch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """Utilities for patching in cassettes"""
 import contextlib
 import functools
+import http.client as httplib
 import itertools
+import logging
 from unittest import mock
 
 from .stubs import VCRHTTPConnection, VCRHTTPSConnection
-import http.client as httplib
-
-import logging
 
 log = logging.getLogger(__name__)
 # Save some of the original types for the purposes of unpatching
 _HTTPConnection = httplib.HTTPConnection
 _HTTPSConnection = httplib.HTTPSConnection
 
 # Try to save the original types for boto3
 try:
-    from botocore.awsrequest import AWSHTTPSConnection, AWSHTTPConnection
-except ImportError:
+    from botocore.awsrequest import AWSHTTPConnection, AWSHTTPSConnection
+except ImportError as e:
     try:
-        import botocore.vendored.requests.packages.urllib3.connectionpool as cpool
+        import botocore.vendored.requests  # noqa: F401
     except ImportError:  # pragma: no cover
         pass
     else:
-        _Boto3VerifiedHTTPSConnection = cpool.VerifiedHTTPSConnection
-        _cpoolBoto3HTTPConnection = cpool.HTTPConnection
-        _cpoolBoto3HTTPSConnection = cpool.HTTPSConnection
+        raise RuntimeError(
+            "vcrpy >=4.2.2 and botocore <1.11.0 are not compatible"
+            "; please upgrade botocore (or downgrade vcrpy)"
+        ) from e
 else:
     _Boto3VerifiedHTTPSConnection = AWSHTTPSConnection
     _cpoolBoto3HTTPConnection = AWSHTTPConnection
     _cpoolBoto3HTTPSConnection = AWSHTTPSConnection
 
 cpool = None
 # Try to save the original types for urllib3
@@ -40,22 +40,24 @@
 else:
     _VerifiedHTTPSConnection = cpool.VerifiedHTTPSConnection
     _cpoolHTTPConnection = cpool.HTTPConnection
     _cpoolHTTPSConnection = cpool.HTTPSConnection
 
 # Try to save the original types for requests
 try:
-    if not cpool:
-        import requests.packages.urllib3.connectionpool as cpool
+    import requests
 except ImportError:  # pragma: no cover
     pass
 else:
-    _VerifiedHTTPSConnection = cpool.VerifiedHTTPSConnection
-    _cpoolHTTPConnection = cpool.HTTPConnection
-    _cpoolHTTPSConnection = cpool.HTTPSConnection
+    if requests.__build__ < 0x021602:
+        raise RuntimeError(
+            "vcrpy >=4.2.2 and requests <2.16.2 are not compatible"
+            "; please upgrade requests (or downgrade vcrpy)"
+        )
+
 
 # Try to save the original types for httplib2
 try:
     import httplib2
 except ImportError:  # pragma: no cover
     pass
 else:
@@ -196,28 +198,19 @@
             from .stubs import requests_stubs
         except ImportError:  # pragma: no cover
             return ()
         return self._urllib3_patchers(cpool, requests_stubs)
 
     @_build_patchers_from_mock_triples_decorator
     def _boto3(self):
-
         try:
             # botocore using awsrequest
             import botocore.awsrequest as cpool
         except ImportError:  # pragma: no cover
-            try:
-                # botocore using vendored requests
-                import botocore.vendored.requests.packages.urllib3.connectionpool as cpool
-            except ImportError:  # pragma: no cover
-                pass
-            else:
-                from .stubs import boto3_stubs
-
-                yield self._urllib3_patchers(cpool, boto3_stubs)
+            pass
         else:
             from .stubs import boto3_stubs
 
             log.debug("Patching boto3 cpool with %s", cpool)
             yield cpool.AWSHTTPConnectionPool, "ConnectionCls", boto3_stubs.VCRRequestsHTTPConnection
             yield cpool.AWSHTTPSConnectionPool, "ConnectionCls", boto3_stubs.VCRRequestsHTTPSConnection
 
@@ -265,16 +258,15 @@
     @_build_patchers_from_mock_triples_decorator
     def _httplib2(self):
         try:
             import httplib2 as cpool
         except ImportError:  # pragma: no cover
             pass
         else:
-            from .stubs.httplib2_stubs import VCRHTTPConnectionWithTimeout
-            from .stubs.httplib2_stubs import VCRHTTPSConnectionWithTimeout
+            from .stubs.httplib2_stubs import VCRHTTPConnectionWithTimeout, VCRHTTPSConnectionWithTimeout
 
             yield cpool, "HTTPConnectionWithTimeout", VCRHTTPConnectionWithTimeout
             yield cpool, "HTTPSConnectionWithTimeout", VCRHTTPSConnectionWithTimeout
             yield cpool, "SCHEME_TO_CONNECTION", {
                 "http": VCRHTTPConnectionWithTimeout,
                 "https": VCRHTTPSConnectionWithTimeout,
             }
@@ -414,44 +406,14 @@
 
 
 def reset_patchers():
     yield mock.patch.object(httplib, "HTTPConnection", _HTTPConnection)
     yield mock.patch.object(httplib, "HTTPSConnection", _HTTPSConnection)
 
     try:
-        import requests
-
-        if requests.__build__ < 0x021603:
-            # Avoid double unmock if requests 2.16.3
-            # First, this is pointless, requests.packages.urllib3 *IS* urllib3 (see packages.py)
-            # Second, this is unmocking twice the same classes with different namespaces
-            # and is creating weird issues and bugs:
-            # > AssertionError: assert <class 'urllib3.connection.HTTPConnection'>
-            # >   is <class 'requests.packages.urllib3.connection.HTTPConnection'>
-            # This assert should work!!!
-            # Note that this also means that now, requests.packages is never imported
-            # if requests 2.16.3 or greater is used with VCRPy.
-            import requests.packages.urllib3.connectionpool as cpool
-        else:
-            raise ImportError("Skip requests not vendored anymore")
-    except ImportError:  # pragma: no cover
-        pass
-    else:
-        # unpatch requests v1.x
-        yield mock.patch.object(cpool, "VerifiedHTTPSConnection", _VerifiedHTTPSConnection)
-        yield mock.patch.object(cpool, "HTTPConnection", _cpoolHTTPConnection)
-        # unpatch requests v2.x
-        if hasattr(cpool.HTTPConnectionPool, "ConnectionCls"):
-            yield mock.patch.object(cpool.HTTPConnectionPool, "ConnectionCls", _cpoolHTTPConnection)
-            yield mock.patch.object(cpool.HTTPSConnectionPool, "ConnectionCls", _cpoolHTTPSConnection)
-
-        if hasattr(cpool, "HTTPSConnection"):
-            yield mock.patch.object(cpool, "HTTPSConnection", _cpoolHTTPSConnection)
-
-    try:
         import urllib3.connectionpool as cpool
     except ImportError:  # pragma: no cover
         pass
     else:
         yield mock.patch.object(cpool, "VerifiedHTTPSConnection", _VerifiedHTTPSConnection)
         yield mock.patch.object(cpool, "HTTPConnection", _cpoolHTTPConnection)
         yield mock.patch.object(cpool, "HTTPSConnection", _cpoolHTTPSConnection)
@@ -459,32 +421,15 @@
             yield mock.patch.object(cpool.HTTPConnectionPool, "ConnectionCls", _cpoolHTTPConnection)
             yield mock.patch.object(cpool.HTTPSConnectionPool, "ConnectionCls", _cpoolHTTPSConnection)
 
     try:
         # unpatch botocore with awsrequest
         import botocore.awsrequest as cpool
     except ImportError:  # pragma: no cover
-        try:
-            # unpatch botocore with vendored requests
-            import botocore.vendored.requests.packages.urllib3.connectionpool as cpool
-        except ImportError:  # pragma: no cover
-            pass
-        else:
-            # unpatch requests v1.x
-            yield mock.patch.object(cpool, "VerifiedHTTPSConnection", _Boto3VerifiedHTTPSConnection)
-            yield mock.patch.object(cpool, "HTTPConnection", _cpoolBoto3HTTPConnection)
-            # unpatch requests v2.x
-            if hasattr(cpool.HTTPConnectionPool, "ConnectionCls"):
-                yield mock.patch.object(cpool.HTTPConnectionPool, "ConnectionCls", _cpoolBoto3HTTPConnection)
-                yield mock.patch.object(
-                    cpool.HTTPSConnectionPool, "ConnectionCls", _cpoolBoto3HTTPSConnection
-                )
-
-            if hasattr(cpool, "HTTPSConnection"):
-                yield mock.patch.object(cpool, "HTTPSConnection", _cpoolBoto3HTTPSConnection)
+        pass
     else:
         if hasattr(cpool.AWSHTTPConnectionPool, "ConnectionCls"):
             yield mock.patch.object(cpool.AWSHTTPConnectionPool, "ConnectionCls", _cpoolBoto3HTTPConnection)
             yield mock.patch.object(cpool.AWSHTTPSConnectionPool, "ConnectionCls", _cpoolBoto3HTTPSConnection)
 
         if hasattr(cpool, "AWSHTTPSConnection"):
             yield mock.patch.object(cpool, "AWSHTTPSConnection", _cpoolBoto3HTTPSConnection)
```

### Comparing `vcrpy-4.2.1/vcr/stubs/compat.py` & `vcrpy-4.3.0/vcr/stubs/compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from io import BytesIO
 import http.client
-
+from io import BytesIO
 
 """
 The python3 http.client api moved some stuff around, so this is an abstraction
 layer that tries to cope with this move.
 """
 
 
 def get_header(message, name):
     return message.getallmatchingheaders(name)
 
 
 def get_header_items(message):
-    for (key, values) in get_headers(message):
+    for key, values in get_headers(message):
         for value in values:
             yield key, value
 
 
 def get_headers(message):
     for key in set(message.keys()):
         yield key, message.get_all(key)
```

### Comparing `vcrpy-4.2.1/vcr/stubs/__init__.py` & `vcrpy-4.3.0/vcr/stubs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Stubs for patching HTTP and HTTPS requests"""
 
 import logging
-from http.client import (
-    HTTPConnection,
-    HTTPSConnection,
-    HTTPResponse,
-)
+from http.client import HTTPConnection, HTTPResponse, HTTPSConnection
 from io import BytesIO
-from vcr.request import Request
+
 from vcr.errors import CannotOverwriteExistingCassetteException
+from vcr.request import Request
+
 from . import compat
 
 log = logging.getLogger(__name__)
 
 
 class VCRFakeSocket:
     """
```

### Comparing `vcrpy-4.2.1/vcr/stubs/aiohttp_stubs.py` & `vcrpy-4.3.0/vcr/stubs/aiohttp_stubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Stubs for aiohttp HTTP clients"""
 import asyncio
 import functools
-import logging
 import json
-
-from aiohttp import ClientConnectionError, ClientResponse, RequestInfo, streams
-from aiohttp import hdrs, CookieJar
+import logging
 from http.cookies import CookieError, Morsel, SimpleCookie
+from typing import Mapping, Union
+
+from aiohttp import ClientConnectionError, ClientResponse, CookieJar, RequestInfo, hdrs, streams
 from aiohttp.helpers import strip_auth_from_url
 from multidict import CIMultiDict, CIMultiDictProxy, MultiDict
-from typing import Union, Mapping
 from yarl import URL
 
 from vcr.errors import CannotOverwriteExistingCassetteException
 from vcr.request import Request
 
 log = logging.getLogger(__name__)
```

### Comparing `vcrpy-4.2.1/vcr/stubs/httplib2_stubs.py` & `vcrpy-4.3.0/vcr/stubs/httplib2_stubs.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Stubs for httplib2"""
 
 from httplib2 import HTTPConnectionWithTimeout, HTTPSConnectionWithTimeout
+
 from ..stubs import VCRHTTPConnection, VCRHTTPSConnection
 
 
 class VCRHTTPConnectionWithTimeout(VCRHTTPConnection, HTTPConnectionWithTimeout):
     _baseclass = HTTPConnectionWithTimeout
 
     def __init__(self, *args, **kwargs):
@@ -23,15 +24,14 @@
         self.sock = self.real_connection.sock
 
 
 class VCRHTTPSConnectionWithTimeout(VCRHTTPSConnection, HTTPSConnectionWithTimeout):
     _baseclass = HTTPSConnectionWithTimeout
 
     def __init__(self, *args, **kwargs):
-
         # Delete the keyword arguments that HTTPSConnection would not recognize
         safe_keys = {
             "host",
             "port",
             "key_file",
             "cert_file",
             "strict",
```

### Comparing `vcrpy-4.2.1/vcr/stubs/requests_stubs.py` & `vcrpy-4.3.0/vcr/stubs/requests_stubs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """Stubs for requests"""
 
-try:
-    from urllib3.connectionpool import HTTPConnection, VerifiedHTTPSConnection
-except ImportError:
-    from requests.packages.urllib3.connectionpool import HTTPConnection, VerifiedHTTPSConnection
+from urllib3.connectionpool import HTTPConnection, VerifiedHTTPSConnection
 
 from ..stubs import VCRHTTPConnection, VCRHTTPSConnection
 
 # urllib3 defines its own HTTPConnection classes, which requests goes ahead and assumes
 # you're using.  It includes some polyfills for newer features missing in older pythons.
```

### Comparing `vcrpy-4.2.1/vcr/stubs/httpx_stubs.py` & `vcrpy-4.3.0/vcr/stubs/httpx_stubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import functools
+import inspect
 import logging
-from unittest.mock import patch, MagicMock
+from unittest.mock import MagicMock, patch
 
 import httpx
-from vcr.request import Request as VcrRequest
+
 from vcr.errors import CannotOverwriteExistingCassetteException
-import inspect
+from vcr.request import Request as VcrRequest
 
 _httpx_signature = inspect.signature(httpx.Client.request)
 
 try:
     HTTPX_REDIRECT_PARAM = _httpx_signature.parameters["follow_redirects"]
 except KeyError:
     HTTPX_REDIRECT_PARAM = _httpx_signature.parameters["allow_redirects"]
```

### Comparing `vcrpy-4.2.1/vcr/stubs/tornado_stubs.py` & `vcrpy-4.3.0/vcr/stubs/tornado_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/vcr/config.py` & `vcrpy-4.3.0/vcr/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import copy
-
-from collections import abc as collections_abc
 import functools
 import inspect
 import os
 import types
+from collections import abc as collections_abc
+from pathlib import Path
 
 import six
 
+from . import filters, matchers
 from .cassette import Cassette
-from .serializers import yamlserializer, jsonserializer
 from .persisters.filesystem import FilesystemPersister
-from .util import compose, auto_decorate
 from .record_mode import RecordMode
-from . import matchers
-from . import filters
+from .serializers import jsonserializer, yamlserializer
+from .util import auto_decorate, compose
 
 
 class VCR:
     @staticmethod
     def is_test_method(method_name, function):
         return method_name.startswith("test") and isinstance(function, types.FunctionType)
 
@@ -46,14 +45,15 @@
         match_on=("method", "scheme", "host", "port", "path", "query"),
         before_record=None,
         inject_cassette=False,
         serializer="yaml",
         cassette_library_dir=None,
         func_path_generator=None,
         decode_compressed_response=False,
+        record_on_exception=True,
     ):
         self.serializer = serializer
         self.match_on = match_on
         self.cassette_library_dir = cassette_library_dir
         self.serializers = {"yaml": yamlserializer, "json": jsonserializer}
         self.matchers = {
             "method": matchers.method,
@@ -77,14 +77,15 @@
         self.before_record_response = before_record_response
         self.ignore_hosts = ignore_hosts
         self.ignore_localhost = ignore_localhost
         self.inject_cassette = inject_cassette
         self.path_transformer = path_transformer
         self.func_path_generator = func_path_generator
         self.decode_compressed_response = decode_compressed_response
+        self.record_on_exception = record_on_exception
         self._custom_patches = tuple(custom_patches)
 
     def _get_serializer(self, serializer_name):
         try:
             serializer = self.serializers[serializer_name]
         except KeyError:
             raise KeyError("Serializer {} doesn't exist or isn't registered".format(serializer_name))
@@ -96,15 +97,15 @@
             for m in matcher_names:
                 matchers.append(self.matchers[m])
         except KeyError:
             raise KeyError("Matcher {} doesn't exist or isn't registered".format(m))
         return matchers
 
     def use_cassette(self, path=None, **kwargs):
-        if path is not None and not isinstance(path, str):
+        if path is not None and not isinstance(path, (str, Path)):
             function = path
             # Assume this is an attempt to decorate a function
             return self._use_cassette(**kwargs)(function)
         return self._use_cassette(path=path, **kwargs)
 
     def _use_cassette(self, with_current_defaults=False, **kwargs):
         if with_current_defaults:
@@ -120,14 +121,15 @@
     def get_merged_config(self, **kwargs):
         serializer_name = kwargs.get("serializer", self.serializer)
         matcher_names = kwargs.get("match_on", self.match_on)
         path_transformer = kwargs.get("path_transformer", self.path_transformer)
         func_path_generator = kwargs.get("func_path_generator", self.func_path_generator)
         cassette_library_dir = kwargs.get("cassette_library_dir", self.cassette_library_dir)
         additional_matchers = kwargs.get("additional_matchers", ())
+        record_on_exception = kwargs.get("record_on_exception", self.record_on_exception)
 
         if cassette_library_dir:
 
             def add_cassette_library_dir(path):
                 if not path.startswith(cassette_library_dir):
                     return os.path.join(cassette_library_dir, path)
                 return path
@@ -146,14 +148,15 @@
             "before_record_request": self._build_before_record_request(kwargs),
             "before_record_response": self._build_before_record_response(kwargs),
             "custom_patches": self._custom_patches + kwargs.get("custom_patches", ()),
             "inject": kwargs.get("inject_cassette", self.inject_cassette),
             "path_transformer": path_transformer,
             "func_path_generator": func_path_generator,
             "allow_playback_repeats": kwargs.get("allow_playback_repeats", False),
+            "record_on_exception": record_on_exception,
         }
         path = kwargs.get("path")
         if path:
             merged_config["path"] = path
         return merged_config
 
     def _build_before_record_response(self, options):
```

### Comparing `vcrpy-4.2.1/vcr/util.py` & `vcrpy-4.3.0/vcr/util.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/vcr/request.py` & `vcrpy-4.3.0/vcr/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import logging
 import warnings
 from io import BytesIO
-from urllib.parse import urlparse, parse_qsl
+from urllib.parse import parse_qsl, urlparse
+
 from .util import CaseInsensitiveDict
-import logging
 
 log = logging.getLogger(__name__)
 
 
 class Request:
     """
     VCR's representation of a request.
```

### Comparing `vcrpy-4.2.1/vcr/serializers/compat.py` & `vcrpy-4.3.0/vcr/serializers/compat.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/vcr/serializers/jsonserializer.py` & `vcrpy-4.3.0/vcr/serializers/jsonserializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/vcr/cassette.py` & `vcrpy-4.3.0/vcr/cassette.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import collections
 import contextlib
 import copy
-import sys
 import inspect
 import logging
+import sys
 
 import wrapt
 
+from ._handle_coroutine import handle_coroutine
 from .errors import UnhandledHTTPRequestError
-from .matchers import requests_match, uri, method, get_matchers_results
+from .matchers import get_matchers_results, method, requests_match, uri
 from .patch import CassettePatcherBuilder
-from .serializers import yamlserializer
 from .persisters.filesystem import FilesystemPersister
-from .util import partition_dict
-from ._handle_coroutine import handle_coroutine
 from .record_mode import RecordMode
+from .serializers import yamlserializer
+from .util import partition_dict
 
 try:
     from asyncio import iscoroutinefunction
 except ImportError:
 
     def iscoroutinefunction(*args, **kwargs):
         return False
@@ -41,36 +41,38 @@
     However, functions that are decorated by
     ``CassetteContextDecorator`` instances ARE reentrant. See the
     implementation of ``__call__`` on this class for more details.
     There is also a guard against attempts to reenter instances of
     this class as a context manager in ``__exit__``.
     """
 
-    _non_cassette_arguments = ("path_transformer", "func_path_generator")
+    _non_cassette_arguments = (
+        "path_transformer",
+        "func_path_generator",
+        "record_on_exception",
+    )
 
     @classmethod
     def from_args(cls, cassette_class, **kwargs):
         return cls(cassette_class, lambda: dict(kwargs))
 
     def __init__(self, cls, args_getter):
         self.cls = cls
         self._args_getter = args_getter
         self.__finish = None
+        self.__cassette = None
 
     def _patch_generator(self, cassette):
         with contextlib.ExitStack() as exit_stack:
             for patcher in CassettePatcherBuilder(cassette).build():
                 exit_stack.enter_context(patcher)
             log_format = "{action} context for cassette at {path}."
             log.debug(log_format.format(action="Entering", path=cassette._path))
             yield cassette
             log.debug(log_format.format(action="Exiting", path=cassette._path))
-            # TODO(@IvanMalison): Hmmm. it kind of feels like this should be
-            # somewhere else.
-            cassette._save()
 
     def __enter__(self):
         # This assertion is here to prevent the dangerous behavior
         # that would result from forgetting about a __finish before
         # completing it.
         # How might this condition be met? Here is an example:
         # context_decorator = Cassette.use('whatever')
@@ -80,18 +82,30 @@
         assert self.__finish is None, "Cassette already open."
         other_kwargs, cassette_kwargs = partition_dict(
             lambda key, _: key in self._non_cassette_arguments, self._args_getter()
         )
         if other_kwargs.get("path_transformer"):
             transformer = other_kwargs["path_transformer"]
             cassette_kwargs["path"] = transformer(cassette_kwargs["path"])
-        self.__finish = self._patch_generator(self.cls.load(**cassette_kwargs))
+        self.__cassette = self.cls.load(**cassette_kwargs)
+        self.__finish = self._patch_generator(self.__cassette)
         return next(self.__finish)
 
-    def __exit__(self, *args):
+    def __exit__(self, *exc_info):
+        exception_was_raised = any(exc_info)
+        record_on_exception = self._args_getter().get("record_on_exception", True)
+        if record_on_exception or not exception_was_raised:
+            self.__cassette._save()
+            self.__cassette = None
+        # Fellow programmer, don't remove this `next`, if `self.__finish` is
+        # not consumed the unpatcher functions accumulated in the `exit_stack`
+        # object created in `_patch_generator` will not be called until
+        # `exit_stack` is not garbage collected.
+        # This works in CPython but not in Pypy, where the unpatchers will not
+        # be called until much later.
         next(self.__finish, None)
         self.__finish = None
 
     @wrapt.decorator
     def __call__(self, function, instance, args, kwargs):
         # This awkward cloning thing is done to ensure that decorated
         # functions are reentrant. This is required for thread
```

### Comparing `vcrpy-4.2.1/vcr/errors.py` & `vcrpy-4.3.0/vcr/errors.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/vcr/matchers.py` & `vcrpy-4.3.0/vcr/matchers.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
+import logging
 import urllib
 import xmlrpc.client
-from .util import read_body
-import logging
 
+from .util import read_body
 
 log = logging.getLogger(__name__)
 
 
 def method(r1, r2):
     assert r1.method == r2.method, "{} != {}".format(r1.method, r2.method)
```

### Comparing `vcrpy-4.2.1/vcr/record_mode.py` & `vcrpy-4.3.0/vcr/record_mode.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/vcr/migration.py` & `vcrpy-4.3.0/vcr/migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 """
 
 import json
 import os
 import shutil
 import sys
 import tempfile
+
 import yaml
 
-from .serializers import yamlserializer, jsonserializer
-from .serialize import serialize
 from . import request
+from .serialize import serialize
+from .serializers import jsonserializer, yamlserializer
 from .stubs.compat import get_httpmessage
 
 # Use the libYAML versions if possible
 try:
     from yaml import CLoader as Loader
 except ImportError:
     from yaml import Loader
```

### Comparing `vcrpy-4.2.1/vcr/filters.py` & `vcrpy-4.3.0/vcr/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from io import BytesIO
-from urllib.parse import urlparse, urlencode, urlunparse
 import copy
 import json
 import zlib
+from io import BytesIO
+from urllib.parse import urlencode, urlparse, urlunparse
 
 from .util import CaseInsensitiveDict
 
 
 def replace_headers(request, replacements):
     """Replace headers in request according to replacements.
     The replacements should be a list of (key, value) pairs where the value can be any of:
@@ -146,14 +146,16 @@
         encoding = headers.get("content-encoding", [])
         return encoding and encoding[0] in ("gzip", "deflate")
 
     def decompress_body(body, encoding):
         """Returns decompressed body according to encoding using zlib.
         to (de-)compress gzip format, use wbits = zlib.MAX_WBITS | 16
         """
+        if not body:
+            return ""
         if encoding == "gzip":
             return zlib.decompress(body, zlib.MAX_WBITS | 16)
         else:  # encoding == 'deflate'
             return zlib.decompress(body)
 
     # Deepcopy here in case `headers` contain objects that could
     # be mutated by a shallow copy and corrupt the real response.
```

### Comparing `vcrpy-4.2.1/setup.py` & `vcrpy-4.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import codecs
 import os
 import re
 import sys
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 from setuptools.command.test import test as TestCommand
 
 long_description = open("README.rst", "r").read()
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 def read(*parts):
@@ -69,14 +69,15 @@
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Testing",
         "Topic :: Internet :: WWW/HTTP",
         "License :: OSI Approved :: MIT License",
     ],
```

### Comparing `vcrpy-4.2.1/tox.ini` & `vcrpy-4.3.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tox]
 skip_missing_interpreters=true
 envlist =
   cov-clean,
   lint,
-  {py37,py38,py39,py310}-{requests,httplib2,urllib3,tornado4,boto3,aiohttp,httpx},
+  {py37,py38,py39,py310,py311}-{requests,httplib2,urllib3,tornado4,boto3,aiohttp,httpx},
   {pypy3}-{requests,httplib2,urllib3,tornado4,boto3},
   {py310}-httpx019,
   cov-report
 
 
 [gh-actions]
 python =
-    3.7: py37, lint
+    3.7: py37
     3.8: py38
     3.9: py39
-    3.10: py310
+    3.10: py310, lint
+    3.11: py311
     pypy-3: pypy3
 
 # Coverage environment tasks: cov-clean and cov-report
 # https://pytest-cov.readthedocs.io/en/latest/tox.html
 [testenv:cov-clean]
 deps = coverage
 skip_install=true
@@ -32,21 +33,24 @@
   coverage report --fail-under=90
 
 [testenv:lint]
 skipsdist = True
 commands =
     black --version
     black --check --diff .
+    isort --version
+    isort . --check --diff
     flake8 --version
-    flake8 --exclude=./docs/conf.py,./.tox/
+    flake8 --exclude=./docs/conf.py,./.tox/,./venv/
     pyflakes ./docs/conf.py
 deps =
   flake8
   black
-basepython = python3.7
+  isort
+basepython = python3.10
 
 [testenv:docs]
 # Running sphinx from inside the "docs" directory
 # ensures it will not pick up any stray files that might
 # get into a virtual environment under the top-level directory
 # or other artifacts under build/
 changedir = docs
@@ -67,39 +71,42 @@
 
 [testenv]
 # Need to use develop install so that paths
 # for aggregate code coverage combine
 usedevelop=true
 commands =
     ./runtests.sh --cov=./vcr --cov-branch --cov-report=xml --cov-append {posargs}
+allowlist_externals =
+    ./runtests.sh
 deps =
     Werkzeug==2.0.3
     pytest
-    git+https://github.com/immerrr/pytest-httpbin@fix-redirect-location-scheme-for-secure-server
+    pytest-httpbin>=1.0.1
     pytest-cov
     PyYAML
     ipaddress
     requests: requests>=2.22.0
+    requests: urllib3<2
     httplib2: httplib2
-    urllib3: urllib3
+    urllib3: urllib3<2
     boto3: boto3
     boto3: urllib3
     aiohttp: aiohttp
     aiohttp: pytest-asyncio
     aiohttp: pytest-aiohttp
     httpx: httpx
     {py37,py38,py39,py310}-{httpx}: httpx
     {py37,py38,py39,py310}-{httpx}: pytest-asyncio
     httpx: httpx>0.19
     # httpx==0.19 is the latest version that supports allow_redirects, newer versions use follow_redirects
     httpx019: httpx==0.19
     {py37,py38,py39,py310}-{httpx}: pytest-asyncio
 depends =
-  lint,{py37,py38,py39,py310,pypy3}-{requests,httplib2,urllib3,tornado4,boto3},{py37,py38,py39,py310}-{aiohttp},{py37,py38,py39,py310}-{httpx}: cov-clean
-  cov-report: lint,{py37,py38,py39,py310,pypy3}-{requests,httplib2,urllib3,tornado4,boto3},{py37,py38,py39,py310}-{aiohttp}
+  lint,{py37,py38,py39,py310,py311,pypy3}-{requests,httplib2,urllib3,tornado4,boto3},{py37,py38,py39,py310,py311}-{aiohttp},{py37,py38,py39,py310,py311}-{httpx}: cov-clean
+  cov-report: lint,{py37,py38,py39,py310,py311,pypy3}-{requests,httplib2,urllib3,tornado4,boto3},{py37,py38,py39,py310,py311}-{aiohttp}
 passenv =
     AWS_ACCESS_KEY_ID
     AWS_DEFAULT_REGION
     AWS_SECRET_ACCESS_KEY
 
 [flake8]
 max_line_length = 110
```

### Comparing `vcrpy-4.2.1/vcrpy.egg-info/PKG-INFO` & `vcrpy-4.3.0/vcrpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,102 +1,103 @@
 Metadata-Version: 2.1
 Name: vcrpy
-Version: 4.2.1
+Version: 4.3.0
 Summary: Automatically mock your HTTP interactions to simplify and speed up testing
 Home-page: https://github.com/kevin1024/vcrpy
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
-Description: 
-        ###########
-        VCR.py 📼
-        ###########
-        
-        
-        |PyPI| |Python versions| |Build Status| |CodeCov| |Gitter| |CodeStyleBlack|
-        
-        ----
-        
-        .. image:: https://vcrpy.readthedocs.io/en/latest/_images/vcr.svg
-           :alt: vcr.py logo
-        
-        
-        This is a Python version of `Ruby's VCR
-        library <https://github.com/vcr/vcr>`__.
-        
-        Source code
-          https://github.com/kevin1024/vcrpy
-        
-        Documentation
-          https://vcrpy.readthedocs.io/
-        
-        Rationale
-        ---------
-        
-        VCR.py simplifies and speeds up tests that make HTTP requests. The
-        first time you run code that is inside a VCR.py context manager or
-        decorated function, VCR.py records all HTTP interactions that take
-        place through the libraries it supports and serializes and writes them
-        to a flat file (in yaml format by default). This flat file is called a
-        cassette. When the relevant piece of code is executed again, VCR.py
-        will read the serialized requests and responses from the
-        aforementioned cassette file, and intercept any HTTP requests that it
-        recognizes from the original test run and return the responses that
-        corresponded to those requests. This means that the requests will not
-        actually result in HTTP traffic, which confers several benefits
-        including:
-        
-        -  The ability to work offline
-        -  Completely deterministic tests
-        -  Increased test execution speed
-        
-        If the server you are testing against ever changes its API, all you need
-        to do is delete your existing cassette files, and run your tests again.
-        VCR.py will detect the absence of a cassette file and once again record
-        all HTTP interactions, which will update them to correspond to the new
-        API.
-        
-        Usage with Pytest
-        -----------------
-        
-        There is a library to provide some pytest fixtures called pytest-recording https://github.com/kiwicom/pytest-recording
-        
-        License
-        -------
-        
-        This library uses the MIT license. See `LICENSE.txt <LICENSE.txt>`__ for
-        more details
-        
-        .. |PyPI| image:: https://img.shields.io/pypi/v/vcrpy.svg
-           :target: https://pypi.python.org/pypi/vcrpy
-        .. |Python versions| image:: https://img.shields.io/pypi/pyversions/vcrpy.svg
-           :target: https://pypi.python.org/pypi/vcrpy
-        .. |Build Status| image:: https://github.com/kevin1024/vcrpy/actions/workflows/main.yml/badge.svg
-           :target: https://github.com/kevin1024/vcrpy/actions
-        .. |Gitter| image:: https://badges.gitter.im/Join%20Chat.svg
-           :alt: Join the chat at https://gitter.im/kevin1024/vcrpy
-           :target: https://gitter.im/kevin1024/vcrpy?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-        .. |CodeCov| image:: https://codecov.io/gh/kevin1024/vcrpy/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/kevin1024/vcrpy
-           :alt: Code Coverage Status
-        .. |CodeStyleBlack| image:: https://img.shields.io/badge/code%20style-black-000000.svg 
-           :target: https://github.com/psf/black
-           :alt: Code Style: black
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+
+###########
+VCR.py 📼
+###########
+
+
+|PyPI| |Python versions| |Build Status| |CodeCov| |Gitter| |CodeStyleBlack|
+
+----
+
+.. image:: https://vcrpy.readthedocs.io/en/latest/_images/vcr.svg
+   :alt: vcr.py logo
+
+
+This is a Python version of `Ruby's VCR
+library <https://github.com/vcr/vcr>`__.
+
+Source code
+  https://github.com/kevin1024/vcrpy
+
+Documentation
+  https://vcrpy.readthedocs.io/
+
+Rationale
+---------
+
+VCR.py simplifies and speeds up tests that make HTTP requests. The
+first time you run code that is inside a VCR.py context manager or
+decorated function, VCR.py records all HTTP interactions that take
+place through the libraries it supports and serializes and writes them
+to a flat file (in yaml format by default). This flat file is called a
+cassette. When the relevant piece of code is executed again, VCR.py
+will read the serialized requests and responses from the
+aforementioned cassette file, and intercept any HTTP requests that it
+recognizes from the original test run and return the responses that
+corresponded to those requests. This means that the requests will not
+actually result in HTTP traffic, which confers several benefits
+including:
+
+-  The ability to work offline
+-  Completely deterministic tests
+-  Increased test execution speed
+
+If the server you are testing against ever changes its API, all you need
+to do is delete your existing cassette files, and run your tests again.
+VCR.py will detect the absence of a cassette file and once again record
+all HTTP interactions, which will update them to correspond to the new
+API.
+
+Usage with Pytest
+-----------------
+
+There is a library to provide some pytest fixtures called pytest-recording https://github.com/kiwicom/pytest-recording
+
+License
+-------
+
+This library uses the MIT license. See `LICENSE.txt <LICENSE.txt>`__ for
+more details
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/vcrpy.svg
+   :target: https://pypi.python.org/pypi/vcrpy
+.. |Python versions| image:: https://img.shields.io/pypi/pyversions/vcrpy.svg
+   :target: https://pypi.python.org/pypi/vcrpy
+.. |Build Status| image:: https://github.com/kevin1024/vcrpy/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/kevin1024/vcrpy/actions
+.. |Gitter| image:: https://badges.gitter.im/Join%20Chat.svg
+   :alt: Join the chat at https://gitter.im/kevin1024/vcrpy
+   :target: https://gitter.im/kevin1024/vcrpy?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+.. |CodeCov| image:: https://codecov.io/gh/kevin1024/vcrpy/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/kevin1024/vcrpy
+   :alt: Code Coverage Status
+.. |CodeStyleBlack| image:: https://img.shields.io/badge/code%20style-black-000000.svg 
+   :target: https://github.com/psf/black
+   :alt: Code Style: black
```

### Comparing `vcrpy-4.2.1/vcrpy.egg-info/SOURCES.txt` & `vcrpy-4.3.0/vcrpy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 tests/assertions.py
 tests/fixtures/migration/new_cassette.json
 tests/fixtures/migration/new_cassette.yaml
 tests/fixtures/migration/not_cassette.txt
 tests/fixtures/migration/old_cassette.json
 tests/fixtures/migration/old_cassette.yaml
 tests/fixtures/wild/domain_redirect.yaml
 tests/integration/__init__.py
 tests/integration/aiohttp_utils.py
+tests/integration/conftest.py
 tests/integration/test_aiohttp.py
 tests/integration/test_basic.py
 tests/integration/test_boto.py
 tests/integration/test_boto3.py
 tests/integration/test_config.py
 tests/integration/test_disksaver.py
 tests/integration/test_filter.py
```

### Comparing `vcrpy-4.2.1/README.rst` & `vcrpy-4.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `vcrpy-4.2.1/LICENSE.txt` & `vcrpy-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

