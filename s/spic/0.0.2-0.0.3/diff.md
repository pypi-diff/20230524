# Comparing `tmp/spic-0.0.2.tar.gz` & `tmp/spic-0.0.3.tar.gz`

## Comparing `spic-0.0.2.tar` & `spic-0.0.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 spic-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 spic-0.0.2/COVERAGE.md
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 spic-0.0.2/Makefile
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 spic-0.0.2/book.toml
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 spic-0.0.2/test.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spic-0.0.2/.github/workflows/coverage.yaml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 spic-0.0.2/.github/workflows/ruff.yaml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 spic-0.0.2/docs/SUMMARY.md
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 spic-0.0.2/docs/USERGUIDE.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 spic-0.0.2/docs/installation.md
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 spic-0.0.2/docs/intro.md
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 spic-0.0.2/docs/tldr.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 spic-0.0.2/performance/go.mod
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 spic-0.0.2/performance/perf_test.go
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 spic-0.0.2/performance/results.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 spic-0.0.2/performance/run.sh
--rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 spic-0.0.2/scripts/cov.sh
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 spic-0.0.2/scripts/test.sh
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/__about__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/__init__.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/app.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/core_exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/default.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/defaults.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/emit.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/encoders.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/enums.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/exceptions.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/func_handler.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/inspect.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/middleware.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/request.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/responses.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/routing.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/types.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/utils.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/openapi/__init__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/openapi/models.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/openapi/utils.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/params/__init__.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 spic-0.0.2/src/spic/params/params.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 spic-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 spic-0.0.2/tests/methods.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_call.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_dataclass_headers.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_dataclass_mixed.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_dataclass_query.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_hdr_args.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_openapi.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_param_wrapper.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_query_args.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_responses.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_router.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_schema.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 spic-0.0.2/tests/test_start.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 spic-0.0.2/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 spic-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 spic-0.0.2/README.md
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 spic-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 spic-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 spic-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 spic-0.0.3/COVERAGE.md
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 spic-0.0.3/Makefile
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 spic-0.0.3/book.toml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 spic-0.0.3/test.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spic-0.0.3/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 spic-0.0.3/.github/workflows/ruff.yaml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 spic-0.0.3/docs/SUMMARY.md
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 spic-0.0.3/docs/USERGUIDE.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 spic-0.0.3/docs/installation.md
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 spic-0.0.3/docs/intro.md
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 spic-0.0.3/docs/tldr.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 spic-0.0.3/performance/go.mod
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 spic-0.0.3/performance/perf_test.go
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 spic-0.0.3/performance/results.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 spic-0.0.3/performance/run.sh
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 spic-0.0.3/scripts/cov.sh
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 spic-0.0.3/scripts/test.sh
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/__about__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/__init__.py
+-rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/app.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/core_exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/default.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/defaults.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/emit.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/encoders.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/enums.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/exceptions.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/func_handler.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/inspect.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/middleware.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/request.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/responses.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/routing.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/types.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/utils.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/openapi/__init__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/openapi/models.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/openapi/utils.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/params/__init__.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 spic-0.0.3/src/spic/params/params.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 spic-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 spic-0.0.3/tests/methods.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_call.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_dataclass_headers.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_dataclass_mixed.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_dataclass_query.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_hdr_args.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_openapi.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_param_wrapper.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_query_args.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_responses.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_router.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_schema.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 spic-0.0.3/tests/test_start.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 spic-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 spic-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 spic-0.0.3/README.md
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 spic-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 spic-0.0.3/PKG-INFO
```

### Comparing `spic-0.0.2/.pre-commit-config.yaml` & `spic-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/COVERAGE.md` & `spic-0.0.3/COVERAGE.md`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/test.py` & `spic-0.0.3/test.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/.github/workflows/coverage.yaml` & `spic-0.0.3/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/docs/intro.md` & `spic-0.0.3/docs/intro.md`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/docs/tldr.md` & `spic-0.0.3/docs/tldr.md`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/performance/perf_test.go` & `spic-0.0.3/performance/perf_test.go`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/app.py` & `spic-0.0.3/src/spic/app.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/emit.py` & `spic-0.0.3/src/spic/emit.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/encoders.py` & `spic-0.0.3/src/spic/encoders.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/exceptions.py` & `spic-0.0.3/src/spic/exceptions.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/func_handler.py` & `spic-0.0.3/src/spic/func_handler.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/inspect.py` & `spic-0.0.3/src/spic/inspect.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/middleware.py` & `spic-0.0.3/src/spic/middleware.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/request.py` & `spic-0.0.3/src/spic/request.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/responses.py` & `spic-0.0.3/src/spic/responses.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/routing.py` & `spic-0.0.3/src/spic/routing.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/types.py` & `spic-0.0.3/src/spic/types.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/utils.py` & `spic-0.0.3/src/spic/utils.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/openapi/models.py` & `spic-0.0.3/src/spic/openapi/models.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/params/__init__.py` & `spic-0.0.3/src/spic/params/__init__.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/src/spic/params/params.py` & `spic-0.0.3/src/spic/params/params.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/tests/test_call.py` & `spic-0.0.3/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/tests/test_dataclass_headers.py` & `spic-0.0.3/tests/test_dataclass_headers.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/tests/test_dataclass_mixed.py` & `spic-0.0.3/tests/test_dataclass_mixed.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/tests/test_dataclass_query.py` & `spic-0.0.3/tests/test_dataclass_query.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/tests/test_hdr_args.py` & `spic-0.0.3/tests/test_hdr_args.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/tests/test_openapi.py` & `spic-0.0.3/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/tests/test_param_wrapper.py` & `spic-0.0.3/tests/test_param_wrapper.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/tests/test_query_args.py` & `spic-0.0.3/tests/test_query_args.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/tests/test_responses.py` & `spic-0.0.3/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/tests/test_router.py` & `spic-0.0.3/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/LICENSE.txt` & `spic-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/README.md` & `spic-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spic-0.0.2/pyproject.toml` & `spic-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "spic"
 dynamic = ["version"]
 description = ''
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 license = "MIT"
 keywords = []
 authors = [
   { name = "joshua-auchincloss", email = "joshua.auchincloss@proton.me" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
```

### Comparing `spic-0.0.2/PKG-INFO` & `spic-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: spic
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/joshua-auchincloss/spic#readme
 Project-URL: Issues, https://github.com/joshua-auchincloss/spic/issues
 Project-URL: Source, https://github.com/joshua-auchincloss/spic
 Author-email: joshua-auchincloss <joshua.auchincloss@proton.me>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Requires-Dist: beartype
 Requires-Dist: hypercorn
 Requires-Dist: rich
 Requires-Dist: srsly
 Requires-Dist: uvicorn
 Provides-Extra: core
 Requires-Dist: pyserde[json]; extra == 'core'
```

