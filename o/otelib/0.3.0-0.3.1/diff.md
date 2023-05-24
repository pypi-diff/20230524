# Comparing `tmp/otelib-0.3.0.tar.gz` & `tmp/otelib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otelib-0.3.0.tar", last modified: Wed Apr 19 07:44:55 2023, max compression
+gzip compressed data, was "otelib-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `otelib-0.3.0.tar` & `otelib-0.3.1.tar`

### file list

```diff
@@ -1,56 +1,58 @@
--rw-r--r--   0        0        0      184 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0      637 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/pull_request_template.md
--rwxr-xr-x   0        0        0     3658 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/utils/wait_for_it.sh
--rw-r--r--   0        0        0      675 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/cd_release.yml
--rw-r--r--   0        0        0      437 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/ci_automerge_dependabot.yml
--rw-r--r--   0        0        0      479 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/ci_cd_updated_master.yml
--rw-r--r--   0        0        0      544 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/ci_check_dependencies.yml
--rw-r--r--   0        0        0      920 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/ci_dependabot.yml
--rw-r--r--   0        0        0     3537 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/ci_tests.yml
--rw-r--r--   0        0        0     3152 2023-04-19 07:44:10.777655 otelib-0.3.0/.gitignore
--rw-r--r--   0        0        0     1731 2023-04-19 07:44:10.777655 otelib-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8745 2023-04-19 07:44:52.569902 otelib-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1050 2023-04-19 07:44:10.777655 otelib-0.3.0/LICENSE
--rw-r--r--   0        0        0     8173 2023-04-19 07:44:10.777655 otelib-0.3.0/README.md
--rw-r--r--   0        0        0     2438 2023-04-19 07:44:10.777655 otelib-0.3.0/docs/demo-notebooks/execute.ipynb
--rw-r--r--   0        0        0    11095 2023-04-19 07:44:10.777655 otelib-0.3.0/docs/img/classes.svg
--rw-r--r--   0        0        0     5473 2023-04-19 07:44:10.777655 otelib-0.3.0/docs/img/filters.drawio
--rw-r--r--   0        0        0     6814 2023-04-19 07:44:10.781656 otelib-0.3.0/docs/img/generic-pipeline.svg
--rw-r--r--   0        0        0    43501 2023-04-19 07:44:10.781656 otelib-0.3.0/docs/img/otelib-overview.png
--rw-r--r--   0        0        0    22053 2023-04-19 07:44:10.781656 otelib-0.3.0/docs/img/pipeline.jpg
--rw-r--r--   0        0        0      226 2023-04-19 07:44:53.029904 otelib-0.3.0/otelib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/__init__.py
--rw-r--r--   0        0        0     2189 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/client.py
--rw-r--r--   0        0        0     1960 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/factories.py
--rw-r--r--   0        0        0      354 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/__init__.py
--rw-r--r--   0        0        0     4911 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/base.py
--rw-r--r--   0        0        0     1856 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/client.py
--rw-r--r--   0        0        0     2678 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/dataresource.py
--rw-r--r--   0        0        0      438 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/filter.py
--rw-r--r--   0        0        0      461 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/function.py
--rw-r--r--   0        0        0      445 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/mapping.py
--rw-r--r--   0        0        0      487 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/transformation.py
--rw-r--r--   0        0        0      354 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/__init__.py
--rw-r--r--   0        0        0     4038 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/base.py
--rw-r--r--   0        0        0      899 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/client.py
--rw-r--r--   0        0        0      388 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/dataresource.py
--rw-r--r--   0        0        0      288 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/filter.py
--rw-r--r--   0        0        0      300 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/function.py
--rw-r--r--   0        0        0      294 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/mapping.py
--rw-r--r--   0        0        0      328 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/transformation.py
--rw-r--r--   0        0        0     3827 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/strategies.py
--rw-r--r--   0        0        0      582 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/utils.py
--rw-r--r--   0        0        0     2932 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/client.py
--rw-r--r--   0        0        0     1260 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/exceptions.py
--rw-r--r--   0        0        0      562 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/pipe.py
--rw-r--r--   0        0        0      484 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/settings.py
--rw-r--r--   0        0        0     1865 2023-04-19 07:44:10.781656 otelib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    11856 2023-04-19 07:44:10.781656 otelib-0.3.0/test_pythonbackend.ipynb
--rw-r--r--   0        0        0     8762 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1504 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/strategies/conftest.py
--rw-r--r--   0        0        0     7010 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/strategies/test_abc.py
--rw-r--r--   0        0        0     9783 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/strategies/test_all_strategies.py
--rw-r--r--   0        0        0     5021 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/test_oteclient.py
--rw-r--r--   0        0        0    10937 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/test_pipe.py
--rw-r--r--   0        0        0     3904 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/utils.py
--rw-r--r--   0        0        0     9440 1970-01-01 00:00:00.000000 otelib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      184 2023-05-24 13:56:13.254460 otelib-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      637 2023-05-24 13:56:13.254460 otelib-0.3.1/.github/pull_request_template.md
+-rwxr-xr-x   0        0        0     3658 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/utils/wait_for_it.sh
+-rw-r--r--   0        0        0      675 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/cd_release.yml
+-rw-r--r--   0        0        0      437 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/ci_automerge_dependabot.yml
+-rw-r--r--   0        0        0      479 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/ci_cd_updated_master.yml
+-rw-r--r--   0        0        0      544 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/ci_check_dependencies.yml
+-rw-r--r--   0        0        0      920 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/ci_dependabot.yml
+-rw-r--r--   0        0        0     3537 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/ci_tests.yml
+-rw-r--r--   0        0        0     3152 2023-05-24 13:56:13.258460 otelib-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1731 2023-05-24 13:56:13.258460 otelib-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9185 2023-05-24 13:57:09.989290 otelib-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1050 2023-05-24 13:56:13.258460 otelib-0.3.1/LICENSE
+-rw-r--r--   0        0        0     8173 2023-05-24 13:56:13.258460 otelib-0.3.1/README.md
+-rw-r--r--   0        0        0     2438 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/demo-notebooks/execute.ipynb
+-rw-r--r--   0        0        0    11095 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/img/classes.svg
+-rw-r--r--   0        0        0     5473 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/img/filters.drawio
+-rw-r--r--   0        0        0     6814 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/img/generic-pipeline.svg
+-rw-r--r--   0        0        0    43501 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/img/otelib-overview.png
+-rw-r--r--   0        0        0    22053 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/img/pipeline.jpg
+-rw-r--r--   0        0        0      226 2023-05-24 13:57:10.553318 otelib-0.3.1/otelib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/__init__.py
+-rw-r--r--   0        0        0     2638 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/client.py
+-rw-r--r--   0        0        0     1960 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/factories.py
+-rw-r--r--   0        0        0      354 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/__init__.py
+-rw-r--r--   0        0        0     4911 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/base.py
+-rw-r--r--   0        0        0     1876 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/client.py
+-rw-r--r--   0        0        0     2678 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/dataresource.py
+-rw-r--r--   0        0        0      438 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/filter.py
+-rw-r--r--   0        0        0      461 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/function.py
+-rw-r--r--   0        0        0      445 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/mapping.py
+-rw-r--r--   0        0        0      487 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/transformation.py
+-rw-r--r--   0        0        0      354 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/__init__.py
+-rw-r--r--   0        0        0     4755 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/base.py
+-rw-r--r--   0        0        0     1719 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/client.py
+-rw-r--r--   0        0        0      388 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/dataresource.py
+-rw-r--r--   0        0        0      288 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/filter.py
+-rw-r--r--   0        0        0      300 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/function.py
+-rw-r--r--   0        0        0      294 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/mapping.py
+-rw-r--r--   0        0        0      328 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/transformation.py
+-rw-r--r--   0        0        0     3827 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/strategies.py
+-rw-r--r--   0        0        0      582 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/utils.py
+-rw-r--r--   0        0        0     3012 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/client.py
+-rw-r--r--   0        0        0     1260 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/exceptions.py
+-rw-r--r--   0        0        0      562 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/pipe.py
+-rw-r--r--   0        0        0      484 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/settings.py
+-rw-r--r--   0        0        0      218 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/warnings.py
+-rw-r--r--   0        0        0     1865 2023-05-24 13:56:13.258460 otelib-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    11856 2023-05-24 13:56:13.258460 otelib-0.3.1/test_pythonbackend.ipynb
+-rw-r--r--   0        0        0     8762 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1504 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/strategies/conftest.py
+-rw-r--r--   0        0        0     7010 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/strategies/test_abc.py
+-rw-r--r--   0        0        0     9783 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/strategies/test_all_strategies.py
+-rw-r--r--   0        0        0     1061 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/test_config.py
+-rw-r--r--   0        0        0     5021 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/test_oteclient.py
+-rw-r--r--   0        0        0    10937 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/test_pipe.py
+-rw-r--r--   0        0        0     3904 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/utils.py
+-rw-r--r--   0        0        0     9440 1970-01-01 00:00:00.000000 otelib-0.3.1/PKG-INFO
```

### Comparing `otelib-0.3.0/.github/pull_request_template.md` & `otelib-0.3.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/.github/utils/wait_for_it.sh` & `otelib-0.3.1/.github/utils/wait_for_it.sh`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/.github/workflows/cd_release.yml` & `otelib-0.3.1/.github/workflows/cd_release.yml`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/.github/workflows/ci_check_dependencies.yml` & `otelib-0.3.1/.github/workflows/ci_check_dependencies.yml`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/.github/workflows/ci_dependabot.yml` & `otelib-0.3.1/.github/workflows/ci_dependabot.yml`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/.github/workflows/ci_tests.yml` & `otelib-0.3.1/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/.gitignore` & `otelib-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/.pre-commit-config.yaml` & `otelib-0.3.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     rev: 1.7.5
     hooks:
     - id: bandit
       args: ["-r"]
       files: ^otelib/.*$
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
     - id: mypy
       exclude: ^tests/.*$
       additional_dependencies:
         - "types-requests"
         - "pydantic"
```

### Comparing `otelib-0.3.0/CHANGELOG.md` & `otelib-0.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 # Changelog
 
-## [v0.3.0](https://github.com/EMMC-ASBL/otelib/tree/v0.3.0) (2023-04-13)
+## [v0.3.1](https://github.com/EMMC-ASBL/otelib/tree/v0.3.1) (2023-05-23)
+
+[Full Changelog](https://github.com/EMMC-ASBL/otelib/compare/v0.3.0...v0.3.1)
+
+**Merged pull requests:**
+
+- \[Auto-generated\] Update dependencies [\#113](https://github.com/EMMC-ASBL/otelib/pull/113) ([TEAM4-0](https://github.com/TEAM4-0))
+- Enh/add auth [\#96](https://github.com/EMMC-ASBL/otelib/pull/96) ([MBueschelberger](https://github.com/MBueschelberger))
+
+## [v0.3.0](https://github.com/EMMC-ASBL/otelib/tree/v0.3.0) (2023-04-19)
 
 [Full Changelog](https://github.com/EMMC-ASBL/otelib/compare/v0.2.0...v0.3.0)
 
 **Implemented enhancements:**
 
 - Use flit instead of setuptools [\#76](https://github.com/EMMC-ASBL/otelib/issues/76)
 - Use SINTEF/ci-cd [\#74](https://github.com/EMMC-ASBL/otelib/issues/74)
```

### Comparing `otelib-0.3.0/LICENSE` & `otelib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/README.md` & `otelib-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/docs/demo-notebooks/execute.ipynb` & `otelib-0.3.1/docs/demo-notebooks/execute.ipynb`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/docs/img/classes.svg` & `otelib-0.3.1/docs/img/classes.svg`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/docs/img/filters.drawio` & `otelib-0.3.1/docs/img/filters.drawio`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/docs/img/generic-pipeline.svg` & `otelib-0.3.1/docs/img/generic-pipeline.svg`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/docs/img/otelib-overview.png` & `otelib-0.3.1/docs/img/otelib-overview.png`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/docs/img/pipeline.jpg` & `otelib-0.3.1/docs/img/pipeline.jpg`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/otelib/backends/client.py` & `otelib-0.3.1/otelib/backends/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """Base API for backend client."""
+import warnings
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 from otelib.backends.factories import strategy_factory
 from otelib.backends.utils import Backend, StrategyType
+from otelib.warnings import IgnoringConfigOptions
 
 if TYPE_CHECKING:  # pragma: no cover
-    from typing import Type, Union
+    from typing import Any, Dict, Type, Union
 
     from otelib.backends.strategies import AbstractBaseStrategy
 
 
 class AbstractBaseClient(ABC):
     """The abstract base class defining the API for a backend client."""
 
     _backend: "Union[Backend, str]"
 
-    def __init__(self, source: str) -> None:
+    def __init__(self, source: str, **config) -> None:
         """Initiates a client."""
         if not source:
             raise ValueError("source must be provided.")
 
         self._source = ""
         self._backend = Backend(self._backend)
 
         self._validate_source(source)
+        self._set_config(config)
 
     @property
     def source(self) -> str:
         """The backend/source the client is using.
 
         This may be an OTE Services base URL or a Python interpreter.
         """
@@ -42,14 +45,23 @@
         """
         if self.source:
             raise RuntimeError(
                 "'source' should not be set prior to calling '_validate_source()'."
             )
         self._source = source
 
+    def _set_config(self, config: "Dict[str, Any]") -> None:
+        """Set the custom client configuration options."""
+        if config:
+            warnings.warn(
+                f"The given configuration option(s) for {tuple(config)} is/are "
+                "ignored.",
+                IgnoringConfigOptions,
+            )
+
     @abstractmethod
     def _create_strategy(
         self, strategy_cls: "Type[AbstractBaseStrategy]", **config
     ) -> "AbstractBaseStrategy":
         """Create a strategy.
 
         This method should not be run by a user, hence it is "private".
```

### Comparing `otelib-0.3.0/otelib/backends/factories.py` & `otelib-0.3.1/otelib/backends/factories.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/otelib/backends/python/base.py` & `otelib-0.3.1/otelib/backends/python/base.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/otelib/backends/python/client.py` & `otelib-0.3.1/otelib/backends/python/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     Attributes:
         interpreter (str): Interpreter for the python backend.
 
     """
 
     _backend = "python"
 
-    def __init__(self, source: str) -> None:
+    def __init__(self, source: str, **config) -> None:
         """Initiates an OTEAPI Python client."""
-        super().__init__(source)
+        super().__init__(source, **config)
 
         self._cache = CACHE
 
         load_strategies()
 
     @property
     def interpreter(self) -> str:
```

### Comparing `otelib-0.3.0/otelib/backends/python/dataresource.py` & `otelib-0.3.1/otelib/backends/python/dataresource.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/otelib/backends/services/base.py` & `otelib-0.3.1/otelib/backends/services/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import requests
 
 from otelib.backends.strategies import AbstractBaseStrategy
 from otelib.exceptions import ApiError
 from otelib.settings import Settings
 
 if TYPE_CHECKING:  # pragma: no cover
-    from typing import Optional
+    from typing import Any, Dict, Optional
 
 
 class BaseServicesStrategy(AbstractBaseStrategy):
     """Abstract class for strategies.
 
     Parameters:
         source (str): The base URL of the OTEAPI Service.
@@ -25,26 +25,42 @@
 
     """
 
     def __init__(self, source: str) -> None:
         super().__init__(source)
 
         self.url: "Optional[str]" = source
+        self._headers: "Optional[Dict[str, Any]]" = None
         self.settings = Settings()
 
+    @property
+    def headers(self) -> "Dict[str, Any]":
+        """URL headers to use for all requests to the OTEAPI Service."""
+        value = self._headers or {}
+        if "Content-Type" not in value:
+            value["Content-Type"] = "application/json"
+        return value
+
+    @headers.setter
+    def headers(self, value: "Dict[str, Any]") -> None:
+        """Set the URL headers to use for all requests to the OTEAPI Service."""
+        if not isinstance(value, dict):
+            raise TypeError("headers must be a dictionary")
+        self._headers = value
+
     def create(self, **config) -> None:
         session_id = config.pop("session_id", None)
         data = self.strategy_config(**config)
 
         response = requests.post(
             f"{self.url}{self.settings.prefix}/{self.strategy_name}",
             data=data.json(),
             params={"session_id": session_id} if session_id else {},
             timeout=self.settings.timeout,
-            headers={"Content-Type": "application/json"},
+            headers=self.headers,
         )
         if not response.ok:
             raise ApiError(
                 f"Cannot create {self.strategy_name}: {data!r}"
                 f"{' content=' + str(response.content) if self.debug else ''}",
                 status=response.status_code,
             )
@@ -57,14 +73,15 @@
         )
 
     def fetch(self, session_id: str) -> bytes:
         response = requests.get(
             f"{self.url}{self.settings.prefix}/{self.strategy_name}/{self.strategy_id}",
             params={"session_id": session_id},
             timeout=self.settings.timeout,
+            headers=self.headers,
         )
         if response.ok:
             return response.content
         strategy_name = (
             self.strategy_name[len("data") :]
             if self.strategy_name.startswith("data")
             else self.strategy_name
@@ -81,14 +98,15 @@
             f"{self.url}{self.settings.prefix}"
             f"/{self.strategy_name}/{self.strategy_id}/initialize"
         )
         response = requests.post(
             post_path,
             params={"session_id": session_id},
             timeout=self.settings.timeout,
+            headers=self.headers,
         )
         if response.ok:
             return response.content
         strategy_name = (
             self.strategy_name[len("data") :]
             if self.strategy_name.startswith("data")
             else self.strategy_name
@@ -100,14 +118,15 @@
             status=response.status_code,
         )
 
     def _create_session(self) -> str:
         response = requests.post(
             f"{self.url}{self.settings.prefix}/session",
             json={},
+            headers=self.headers,
             timeout=self.settings.timeout,
         )
         if not response.ok:
             raise ApiError(
                 f"Cannot create session: {response.status_code} "
                 f"{' content=' + str(response.content) if self.debug else ''}",
                 status=response.status_code,
```

### Comparing `otelib-0.3.0/otelib/backends/strategies.py` & `otelib-0.3.1/otelib/backends/strategies.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/otelib/backends/utils.py` & `otelib-0.3.1/otelib/backends/utils.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/otelib/client.py` & `otelib-0.3.1/otelib/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,30 +17,31 @@
         url (str): The base URL of the OTEAPI Service.
 
     Attributes:
         url (str): The base URL of the OTEAPI Service.
 
     """
 
-    def __init__(self, url: str) -> None:
+    def __init__(self, url: str, **config) -> None:
         """Initialize an OTE Client.
 
         Parameters:
             url: The base URL of the OTE Service (or Python interpreter for local
                 OTEAPI Core usage).
+            config: Custom client configuration properties.
 
         """
         try:
             parse_obj_as(AnyHttpUrl, url)
         except ValidationError:
             backend = Backend.PYTHON
         else:
             backend = Backend.SERVICES
 
-        self._impl = client_factory(backend)(url)
+        self._impl = client_factory(backend)(url, **config)
 
     @property
     def url(self) -> str:
         """The base URL of the OTE Service.
 
         This may also be the Python interpreter for local OTEAPI Core usage.
         """
```

### Comparing `otelib-0.3.0/otelib/exceptions.py` & `otelib-0.3.1/otelib/exceptions.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/otelib/pipe.py` & `otelib-0.3.1/otelib/pipe.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/pyproject.toml` & `otelib-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     "Operating System :: OS Independent",
 ]
 keywords = ["OTE", "OTE-API"]
 requires-python = "~=3.9"
 dynamic = ["version"]
 
 dependencies = [
-    "oteapi-core >=0.4.1,<1",
+    "oteapi-core >=0.4.2,<1",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "pre-commit ~=3.2",
+    "pre-commit ~=3.3",
     "pylint ~=2.17",
     "pytest ~=7.3",
     "pytest-cov ~=4.0",
     "requests-mock ~=1.10",
 ]
 
 [project.urls]
```

### Comparing `otelib-0.3.0/test_pythonbackend.ipynb` & `otelib-0.3.1/test_pythonbackend.ipynb`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/tests/conftest.py` & `otelib-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/tests/strategies/conftest.py` & `otelib-0.3.1/tests/strategies/conftest.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/tests/strategies/test_abc.py` & `otelib-0.3.1/tests/strategies/test_abc.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/tests/strategies/test_all_strategies.py` & `otelib-0.3.1/tests/strategies/test_all_strategies.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/tests/test_oteclient.py` & `otelib-0.3.1/tests/test_oteclient.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/tests/test_pipe.py` & `otelib-0.3.1/tests/test_pipe.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/tests/utils.py` & `otelib-0.3.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.0/PKG-INFO` & `otelib-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: otelib
-Version: 0.3.0
+Version: 0.3.1
 Summary: Open Translation Environment (OTE) REST API client library.
 Keywords: OTE,OTE-API
 Author-email: SINTEF <TEAM4.0@SINTEF.no>
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Dist: oteapi-core >=0.4.1,<1
-Requires-Dist: pre-commit ~=3.2 ; extra == "dev"
+Requires-Dist: oteapi-core >=0.4.2,<1
+Requires-Dist: pre-commit ~=3.3 ; extra == "dev"
 Requires-Dist: pylint ~=2.17 ; extra == "dev"
 Requires-Dist: pytest ~=7.3 ; extra == "dev"
 Requires-Dist: pytest-cov ~=4.0 ; extra == "dev"
 Requires-Dist: requests-mock ~=1.10 ; extra == "dev"
 Project-URL: Changelog, https://github.com/EMMC-ASBL/otelib/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://EMMC-ASBL.github.io/otelib
 Project-URL: Home, https://github.com/EMMC-ASBL/otelib
```

