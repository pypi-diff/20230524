# Comparing `tmp/envoy.code.check-0.5.0.tar.gz` & `tmp/envoy.code.check-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.code.check-0.5.0.tar", last modified: Tue May 16 14:33:12 2023, max compression
+gzip compressed data, was "envoy.code.check-0.5.1.tar", last modified: Wed May 24 11:58:22 2023, max compression
```

## Comparing `envoy.code.check-0.5.0.tar` & `envoy.code.check-0.5.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/envoy/code/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/envoy/code/check/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/envoy/code/check/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/flake8.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/glint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/gofmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/runtime_guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/shellcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/yamllint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/yapf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/envoy.code.check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.449051 envoy.code.check-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 11:58:22.449051 envoy.code.check-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.445051 envoy.code.check-0.5.1/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.445051 envoy.code.check-0.5.1/envoy/code/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.445051 envoy.code.check-0.5.1/envoy/code/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.449051 envoy.code.check-0.5.1/envoy/code/check/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/flake8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/glint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/gofmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/runtime_guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/shellcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/yamllint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/yapf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.445051 envoy.code.check-0.5.1/envoy.code.check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:58:22.449051 envoy.code.check-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/setup.py
```

### Comparing `envoy.code.check-0.5.0/backend_shim.py` & `envoy.code.check-0.5.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/__init__.py` & `envoy.code.check-0.5.1/envoy/code/check/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/__init__.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/base.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/base.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/changelog.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/changelog.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/checker.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     "\n"
     "      - no trailing whitespace\n"
     "      - no preceding mixed tabs/spaces\n"
     "      - all files end with a newline")
 
 NO_EXTENSIONS_ERROR_MSG = (
     "`--extensions_build_config` not provided, disabling extensions checks")
+NO_EXTENSIONS_FUZZ_ERROR_MSG = (
+    "`--extensions_fuzzed_count` not provided, "
+    "disabling extensions fuzz checks")
 
 
 class CodeCheckerSummary(checker.CheckerSummary):
 
     def print_summary(self) -> None:
         """Write summary to stderr."""
         super().print_summary()
@@ -78,14 +81,16 @@
     @cached_property
     def disabled_checks(self):
         disabled = {}
         if not self.args.extensions_build_config:
             disabled["extensions_fuzzed"] = NO_EXTENSIONS_ERROR_MSG
             disabled["extensions_metadata"] = NO_EXTENSIONS_ERROR_MSG
             disabled["extensions_registered"] = NO_EXTENSIONS_ERROR_MSG
+        elif self.args.extensions_fuzzed_count is None:
+            disabled["extensions_fuzzed"] = NO_EXTENSIONS_FUZZ_ERROR_MSG
         return disabled
 
     @property
     def changed_since(self) -> Optional[str]:
         return self.args.since
 
     @cached_property
@@ -251,14 +256,15 @@
         super().add_arguments(parser)
         parser.add_argument("-a", "--all_files", action="store_true")
         parser.add_argument("-m", "--matching", action="append")
         parser.add_argument("-x", "--excluding", action="append")
         parser.add_argument("-b", "--binary", action="append")
         parser.add_argument("-s", "--since")
         parser.add_argument("--extensions_build_config")
+        parser.add_argument("--extensions_fuzzed_count")
 
     async def check_changelog(self):
         for changelog in self.changelog:
             if errors := await changelog.errors:
                 self.error("changelog", errors)
             else:
                 self.succeed(
```

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/extensions.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/extensions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 
 import asyncio
 import itertools
 import json
 import logging
 import pathlib
-import re
 from functools import cached_property
-from typing import Any, cast, Dict, List, Pattern, Set, Tuple, Type, Union
+from typing import (
+    Any, cast, Dict, List,
+    Optional, Set, Tuple, Type, Union)
 
 import yaml as _yaml
 
 import abstracts
 
 from aio.core import functional, utils
 from aio.core.functional import async_property
 
 from envoy.code.check import abstract, exceptions, interface, typing
 
 
 logger = logging.getLogger(__name__)
 
-
-FILTER_NAMES_PATTERN = "envoy\\.filters\\.network"
 FUZZ_TEST_PATH = (
     "test/extensions/filters/network/common/fuzz/BUILD")
 METADATA_PATH = "source/extensions/extensions_metadata.yaml"
 METADATA_ONLY_EXTENSIONS = (
     "envoy.filters.network.envoy_mobile_http_connection_manager", )
 CONTRIB_METADATA_PATH = "contrib/extensions_metadata.yaml"
 EXTENSIONS_SCHEMA = "tools/extensions/extensions_schema.yaml"
@@ -36,24 +35,28 @@
     """Extensions check."""
 
     def __init__(
             self,
             *args,
             **kwargs) -> None:
         self.extensions_build_config = kwargs.pop("extensions_build_config")
+        self._fuzzed_count = kwargs.pop("extensions_fuzzed_count", None)
         super().__init__(*args, **kwargs)
 
     @cached_property
     def all_extensions(self) -> Set[str]:
         return (
             set(self.configured_extensions)
             | set(self.builtin_extensions))
 
     @async_property
     async def all_fuzzed(self) -> bool:
+        if self.fuzzed_count is None:
+            logger.warning("Fuzz check called but fuzz count not set.")
+            return True
         return (
             await self.robust_to_downstream_count
             == self.fuzzed_count)
 
     @property
     def builtin_extensions(self) -> typing.ExtensionsSchemaBuiltinList:
         return self.extensions_schema["builtin"]
@@ -103,24 +106,16 @@
             in self.extensions_schema["status_values"]]
 
     @property
     def fuzz_test_path(self) -> pathlib.Path:
         return self.directory.path.joinpath(FUZZ_TEST_PATH)
 
     @property
-    def fuzzed_count(self) -> int:
-        # Hack-ish! We only search the first 60 lines to capture the filters
-        # in `READFILTER_FUZZ_FILTERS`.
-        return len(
-            self.fuzzed_filter_names_re.findall(
-                "".join(self.fuzz_test_path.read_text().splitlines()[:60])))
-
-    @cached_property
-    def fuzzed_filter_names_re(self) -> Pattern:
-        return re.compile(FILTER_NAMES_PATTERN)
+    def fuzzed_count(self) -> Optional[int]:
+        return self._fuzzed_count
 
     @async_property(cache=True)
     async def metadata(self) -> typing.ExtensionsMetadataDict:
         return dict(**await self.metadata_core, **await self.metadata_contrib)
 
     @async_property
     async def metadata_contrib(self) -> typing.ExtensionsMetadataDict:
```

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/flake8.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/flake8.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/glint.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/glint.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/gofmt.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/gofmt.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/rst.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/rst.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/runtime_guards.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/runtime_guards.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/shellcheck.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/shellcheck.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/yamllint.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/yamllint.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/abstract/yapf.py` & `envoy.code.check-0.5.1/envoy/code/check/abstract/yapf.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/checker.py` & `envoy.code.check-0.5.1/envoy/code/check/checker.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/interface.py` & `envoy.code.check-0.5.1/envoy/code/check/interface.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy/code/check/typing.py` & `envoy.code.check-0.5.1/envoy/code/check/typing.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/envoy.code.check.egg-info/SOURCES.txt` & `envoy.code.check-0.5.1/envoy.code.check.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.0/setup.py` & `envoy.code.check-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,9 +42,9 @@
     },
     'packages': (
         'envoy.code.check',
         'envoy.code.check.abstract',
     ),
     'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/toolshed/tree/main/envoy.code.check',
-    'version': '0.5.0',
+    'version': '0.5.1',
 })
```

