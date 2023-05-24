# Comparing `tmp/spic-0.0.4.tar.gz` & `tmp/spic-0.0.5.tar.gz`

## Comparing `spic-0.0.4.tar` & `spic-0.0.5.tar`

### file list

```diff
@@ -1,60 +1,68 @@
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 spic-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 spic-0.0.4/COVERAGE.md
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 spic-0.0.4/Makefile
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 spic-0.0.4/book.toml
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 spic-0.0.4/test.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spic-0.0.4/.github/workflows/coverage.yaml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 spic-0.0.4/.github/workflows/ruff.yaml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 spic-0.0.4/docs/SUMMARY.md
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 spic-0.0.4/docs/USERGUIDE.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 spic-0.0.4/docs/installation.md
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 spic-0.0.4/docs/intro.md
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 spic-0.0.4/docs/tldr.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 spic-0.0.4/performance/go.mod
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 spic-0.0.4/performance/perf_test.go
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 spic-0.0.4/performance/results.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 spic-0.0.4/performance/run.sh
--rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 spic-0.0.4/scripts/cov.sh
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 spic-0.0.4/scripts/test.sh
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/__about__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/__init__.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/app.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/core_exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/default.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/defaults.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/emit.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/encoders.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/enums.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/exceptions.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/func_handler.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/inspect.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/middleware.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/request.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/responses.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/routing.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/types.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/utils.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/openapi/__init__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/openapi/models.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/openapi/utils.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/params/__init__.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 spic-0.0.4/src/spic/params/params.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 spic-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 spic-0.0.4/tests/methods.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_call.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_dataclass_headers.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_dataclass_mixed.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_dataclass_query.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_hdr_args.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_openapi.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_param_wrapper.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_query_args.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_responses.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_router.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_schema.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 spic-0.0.4/tests/test_start.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 spic-0.0.4/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 spic-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 spic-0.0.4/README.md
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 spic-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 spic-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 spic-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 spic-0.0.5/COVERAGE.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 spic-0.0.5/Makefile
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 spic-0.0.5/book.toml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 spic-0.0.5/test.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spic-0.0.5/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 spic-0.0.5/.github/workflows/ruff.yaml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 spic-0.0.5/docs/SUMMARY.md
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 spic-0.0.5/docs/USERGUIDE.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 spic-0.0.5/docs/installation.md
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 spic-0.0.5/docs/intro.md
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 spic-0.0.5/docs/tldr.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 spic-0.0.5/performance/go.mod
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 spic-0.0.5/performance/perf_test.go
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 spic-0.0.5/performance/results.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 spic-0.0.5/performance/run.sh
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 spic-0.0.5/scripts/cov.sh
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 spic-0.0.5/scripts/test.sh
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/__about__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/__init__.py
+-rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/default.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/defaults.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/emit.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/encoders.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/enums.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/exception_handlers.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/exceptions.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/func_handler.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/inspect.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/middleware.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/request.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/responses.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/routing.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/types.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/utils.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/openapi/__init__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/openapi/models.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/openapi/utils.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/params/__init__.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/params/params.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 spic-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 spic-0.0.5/tests/buf.gen.yaml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 spic-0.0.5/tests/buf.yaml
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 spic-0.0.5/tests/methods.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_call.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_dataclass_headers.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_dataclass_mixed.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_dataclass_query.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_grpc.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_hdr_args.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_openapi.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_param_wrapper.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_query_args.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_responses.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_router.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_schema.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_start.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spic-0.0.5/tests/protos/__init.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 spic-0.0.5/tests/protos/hello.proto
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spic-0.0.5/tests/protos/gen/__init__.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 spic-0.0.5/tests/protos/gen/hello_pb2.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 spic-0.0.5/tests/protos/gen/hello_pb2.pyi
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 spic-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 spic-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 spic-0.0.5/README.md
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 spic-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 spic-0.0.5/PKG-INFO
```

### Comparing `spic-0.0.4/.pre-commit-config.yaml` & `spic-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/COVERAGE.md` & `spic-0.0.5/COVERAGE.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 | Name                             |   Stmts |    Miss |   Cover |                                                                        Missing |
 | -------------------------------- | ------: | ------: | ------: | -----------------------------------------------------------------------------: |
-| src/spic/\_\_init\_\_.py         |       0 |       0 |    100% |                                                                                |
+| src/spic/\_\_init\_\_.py         |       1 |       0 |    100% |                                                                                |
 | src/spic/app.py                  |     128 |      35 |     73% | 58-59, 65-72, 85-92, 100-132, 135, 143, 185, 188, 191, 194, 197, 200, 203, 209 |
-| src/spic/core_exceptions.py      |      11 |       1 |     91% |                                                                             13 |
 | src/spic/defaults.py             |       4 |       0 |    100% |                                                                                |
 | src/spic/emit.py                 |      22 |       3 |     86% |                                                                      39-40, 45 |
-| src/spic/encoders.py             |      54 |      11 |     80% |                                                   37, 45, 54, 61, 63-66, 82-85 |
-| src/spic/enums.py                |       9 |       0 |    100% |                                                                                |
+| src/spic/encoders.py             |      83 |      23 |     72% |                17-18, 21-22, 26-31, 51, 59, 67-68, 73, 89, 96, 98-101, 118-121 |
+| src/spic/enums.py                |      12 |       0 |    100% |                                                                                |
+| src/spic/exception_handlers.py   |      11 |       1 |     91% |                                                                             13 |
 | src/spic/exceptions.py           |      41 |       5 |     88% |                                                                      32-35, 63 |
 | src/spic/func_handler.py         |      97 |      16 |     84% |                34, 49-50, 52, 56-57, 61, 64, 83-86, 90, 129, 138, 140-141, 146 |
 | src/spic/inspect.py              |      50 |       5 |     90% |                                                                  14, 20, 72-74 |
 | src/spic/middleware.py           |      20 |       6 |     70% |                                                                      15, 24-28 |
 | src/spic/openapi/\_\_init\_\_.py |       4 |       0 |    100% |                                                                                |
 | src/spic/openapi/models.py       |     157 |       0 |    100% |                                                                                |
 | src/spic/openapi/utils.py        |       8 |       0 |    100% |                                                                                |
 | src/spic/params/\_\_init\_\_.py  |      11 |       0 |    100% |                                                                                |
 | src/spic/params/params.py        |      88 |      12 |     86% |                                          29-32, 39, 56, 59, 64, 72, 76-77, 101 |
 | src/spic/request.py              |      33 |       0 |    100% |                                                                                |
 | src/spic/responses.py            |      41 |       2 |     95% |                                                                          84-85 |
 | src/spic/routing.py              |     109 |      15 |     86% |                    67-68, 102, 123-133, 146, 167, 170, 173, 176, 179, 182, 185 |
-| src/spic/types.py                |      29 |       8 |     72% |                                                                  29, 33-40, 47 |
+| src/spic/types.py                |      36 |      12 |     67% |                                                       29, 33-40, 47, 52, 56-59 |
 | src/spic/utils.py                |      34 |       2 |     94% |                                                                         37, 65 |
-| **TOTAL**                        | **950** | **121** | **87%** |                                                                                |
+| **TOTAL**                        | **990** | **137** | **86%** |                                                                                |
```

### Comparing `spic-0.0.4/test.py` & `spic-0.0.5/test.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/.github/workflows/coverage.yaml` & `spic-0.0.5/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/docs/intro.md` & `spic-0.0.5/docs/intro.md`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/docs/tldr.md` & `spic-0.0.5/docs/tldr.md`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/performance/perf_test.go` & `spic-0.0.5/performance/perf_test.go`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/app.py` & `spic-0.0.5/src/spic/app.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/emit.py` & `spic-0.0.5/src/spic/emit.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/exceptions.py` & `spic-0.0.5/src/spic/exceptions.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/func_handler.py` & `spic-0.0.5/src/spic/func_handler.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/inspect.py` & `spic-0.0.5/src/spic/inspect.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/middleware.py` & `spic-0.0.5/src/spic/middleware.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/request.py` & `spic-0.0.5/src/spic/request.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/responses.py` & `spic-0.0.5/src/spic/responses.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/routing.py` & `spic-0.0.5/src/spic/routing.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/types.py` & `spic-0.0.5/src/spic/types.py`

 * *Files 27% similar despite different names*

```diff
@@ -41,7 +41,19 @@
 
 
 def get_args(tp: Type[Any]) -> Tuple[Any, ...]:
     if type(tp).__name__ in AnnotatedTypeNames:
         return tp.__args__ + tp.__metadata__
     # the fallback is needed for the same reasons as `get_origin` (see above)
     return _get_args(tp) or getattr(tp, "__args__", ()) or _generic_get_args(tp)
+
+
+class DependencyError(Exception):
+    def __init__(self, pkg: str):
+        self.pkg = pkg
+
+
+def create_raises_dep_error(pkg: str):
+    def handle(*_, **__):
+        raise DependencyError(pkg)
+
+    return handle
```

### Comparing `spic-0.0.4/src/spic/utils.py` & `spic-0.0.5/src/spic/utils.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/openapi/models.py` & `spic-0.0.5/src/spic/openapi/models.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/params/__init__.py` & `spic-0.0.5/src/spic/params/__init__.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/src/spic/params/params.py` & `spic-0.0.5/src/spic/params/params.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/tests/test_call.py` & `spic-0.0.5/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/tests/test_dataclass_headers.py` & `spic-0.0.5/tests/test_dataclass_headers.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/tests/test_dataclass_mixed.py` & `spic-0.0.5/tests/test_dataclass_mixed.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/tests/test_dataclass_query.py` & `spic-0.0.5/tests/test_dataclass_query.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/tests/test_hdr_args.py` & `spic-0.0.5/tests/test_hdr_args.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/tests/test_openapi.py` & `spic-0.0.5/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/tests/test_param_wrapper.py` & `spic-0.0.5/tests/test_param_wrapper.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/tests/test_query_args.py` & `spic-0.0.5/tests/test_query_args.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/tests/test_responses.py` & `spic-0.0.5/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/tests/test_router.py` & `spic-0.0.5/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/LICENSE.txt` & `spic-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/README.md` & `spic-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `spic-0.0.4/pyproject.toml` & `spic-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spic"
 dynamic = ["version"]
-description = "spic-api"
+description = "a little opinionated framework for creating spic & span apis"
 readme = "README.md"
 requires-python = ">=3.9"
 license = "MIT"
 keywords = []
 authors = [
   { name = "joshua-auchincloss", email = "joshua.auchincloss@proton.me" },
 ]
 classifiers = [
+  "Typing :: Typed",
+  "Topic :: Internet :: WWW/HTTP",
+  "Topic :: Software Development",
   "Development Status :: 4 - Beta",
+  "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
+  "Intended Audience :: Information Technology",
+  "Intended Audience :: System Administrators",
+  "Topic :: Software Development :: Libraries",
+  "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
+  "Topic :: Software Development :: Libraries :: Python Modules",
+  "Topic :: Software Development :: Libraries :: Application Frameworks",
+  "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
   "srsly",
   "uvicorn",
   "rich",
   "hypercorn",
   "beartype",
+  "pyserde[json]",
 ]
 
 [project.optional-dependencies]
-core = [
-  "pyserde[json]",
-]
 dev = [
   "coverage",
   "black",
   "isort",
   "ruff",
   "pytest-asyncio",
   "starlette",
@@ -47,14 +54,18 @@
 experimental = [
   "pydantic",
 ]
 msgpack = [
   "msgpack",
   "pyserde[msgpack]"
 ]
+grpc-compat = [
+  "protobuf",
+  "grpcio"
+]
 
 [project.urls]
 Documentation = "https://github.com/joshua-auchincloss/spic#readme"
 Issues = "https://github.com/joshua-auchincloss/spic/issues"
 Source = "https://github.com/joshua-auchincloss/spic"
 
 [tool.hatch.version]
```

### Comparing `spic-0.0.4/PKG-INFO` & `spic-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 Metadata-Version: 2.1
 Name: spic
-Version: 0.0.4
-Summary: spic-api
+Version: 0.0.5
+Summary: a little opinionated framework for creating spic & span apis
 Project-URL: Documentation, https://github.com/joshua-auchincloss/spic#readme
 Project-URL: Issues, https://github.com/joshua-auchincloss/spic/issues
 Project-URL: Source, https://github.com/joshua-auchincloss/spic
 Author-email: joshua-auchincloss <joshua.auchincloss@proton.me>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: beartype
 Requires-Dist: hypercorn
+Requires-Dist: pyserde[json]
 Requires-Dist: rich
 Requires-Dist: srsly
 Requires-Dist: uvicorn
-Provides-Extra: core
-Requires-Dist: pyserde[json]; extra == 'core'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: coverage; extra == 'dev'
 Requires-Dist: httpx; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pytest-asyncio; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: starlette; extra == 'dev'
 Provides-Extra: experimental
 Requires-Dist: pydantic; extra == 'experimental'
+Provides-Extra: grpc-compat
+Requires-Dist: grpcio; extra == 'grpc-compat'
+Requires-Dist: protobuf; extra == 'grpc-compat'
 Provides-Extra: msgpack
 Requires-Dist: msgpack; extra == 'msgpack'
 Requires-Dist: pyserde[msgpack]; extra == 'msgpack'
 Description-Content-Type: text/markdown
 
 # `spic`
```

