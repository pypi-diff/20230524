# Comparing `tmp/tripper-0.2.4.tar.gz` & `tmp/tripper-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tripper-0.2.4.tar", last modified: Sun Apr 30 20:08:04 2023, max compression
+gzip compressed data, was "tripper-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tripper-0.2.4.tar` & `tripper-0.2.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      205 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/dependabot.yml
--rw-r--r--   0        0        0      637 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/pull_request_template.md
--rw-r--r--   0        0        0      916 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/cd_release.yml
--rw-r--r--   0        0        0      545 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/ci_automerge_dependency_prs.yml
--rw-r--r--   0        0        0      656 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/ci_cd_updated_main.yml
--rw-r--r--   0        0        0      602 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/ci_check_dependencies.yml
--rw-r--r--   0        0        0     2420 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/ci_tests.yml
--rw-r--r--   0        0        0      838 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/ci_update_dependencies.yml
--rw-r--r--   0        0        0      137 2023-04-30 20:07:11.412130 tripper-0.2.4/.gitignore
--rw-r--r--   0        0        0     1819 2023-04-30 20:07:11.412130 tripper-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       42 2023-04-30 20:07:11.412130 tripper-0.2.4/.pylintrc
--rw-r--r--   0        0        0     9917 2023-04-30 20:08:01.428129 tripper-0.2.4/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2023-04-30 20:07:11.412130 tripper-0.2.4/LICENSE
--rw-r--r--   0        0        0     2496 2023-04-30 20:07:11.412130 tripper-0.2.4/README.md
-lrwxr-xr-x   0        0        0        0 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/CHANGELOG.md -> ../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/LICENSE.md -> ../LICENSE
--rw-r--r--   0        0        0       23 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/.pages
--rw-r--r--   0        0        0       18 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/backends/.pages
--rw-r--r--   0        0        0       46 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/backends/collection.md
--rw-r--r--   0        0        0       38 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/backends/ontopy.md
--rw-r--r--   0        0        0       38 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/backends/rdflib.md
--rw-r--r--   0        0        0       52 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/backends/sparqlwrapper.md
--rw-r--r--   0        0        0       29 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/errors.md
--rw-r--r--   0        0        0       35 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/interface.md
--rw-r--r--   0        0        0       31 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/literal.md
--rw-r--r--   0        0        0       18 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/mappings/.pages
--rw-r--r--   0        0        0       42 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/mappings/mappings.md
--rw-r--r--   0        0        0       35 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/namespace.md
--rw-r--r--   0        0        0       39 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/triplestore.md
--rw-r--r--   0        0        0       27 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/utils.md
--rw-r--r--   0        0        0     2909 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/backend_discovery.md
--rw-r--r--   0        0        0      183 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/css/reference.css
--rw-r--r--   0        0        0     2489 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/index.md
--rw-r--r--   0        0        0    12710 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/mappings/figs/function_emmo.svg
--rw-r--r--   0        0        0      228 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/planned-backends.md
--rw-r--r--   0        0        0     3963 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/tutorial.md
--rw-r--r--   0        0        0     1188 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/README.md
--rw-r--r--   0        0        0    18333 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/knowledge-base.svg
--rw-r--r--   0        0        0     8546 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/route.svg
--rw-r--r--   0        0        0     7117 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/workflow.svg
--rw-r--r--   0        0        0      894 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/workflow_mappings.py
--rw-r--r--   0        0        0    14169 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/workflow_w_pipes.svg
--rw-r--r--   0        0        0     1943 2023-04-30 20:07:11.416130 tripper-0.2.4/mkdocs.yml
--rw-r--r--   0        0        0     2713 2023-04-30 20:07:11.416130 tripper-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3444 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0      959 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/mappings/test_function.py
--rw-r--r--   0        0        0     1455 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/mappings/test_mappings.py
--rw-r--r--   0        0        0     5701 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/ontologies/family.ttl
--rw-r--r--   0        0        0     6753 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/ontologies/food.ttl
--rw-r--r--   0        0        0     3166 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_add_function.py
--rw-r--r--   0        0        0      880 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_collection.py
--rw-r--r--   0        0        0     2451 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_get_data.py
--rw-r--r--   0        0        0     3943 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_literals.py
--rw-r--r--   0        0        0     1993 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_namespace.py
--rw-r--r--   0        0        0     7802 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_triplestore.py
--rw-r--r--   0        0        0     6062 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_utils.py
--rw-r--r--   0        0        0      705 2023-04-30 20:08:01.744129 tripper-0.2.4/tripper/__init__.py
--rw-r--r--   0        0        0     1330 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/backends/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/backends/collection.py
--rw-r--r--   0        0        0     9100 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/backends/ontopy.py
--rw-r--r--   0        0        0     7363 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/backends/rdflib.py
--rw-r--r--   0        0        0     4112 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/backends/sparqlwrapper.py
--rw-r--r--   0        0        0      362 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/errors.py
--rw-r--r--   0        0        0     5379 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/interface.py
--rw-r--r--   0        0        0     5510 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/literal.py
--rw-r--r--   0        0        0      102 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/mappings/__init__.py
--rw-r--r--   0        0        0    35281 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/mappings/mappings.py
--rw-r--r--   0        0        0     6901 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/namespace.py
--rw-r--r--   0        0        0    43718 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/triplestore.py
--rw-r--r--   0        0        0     8237 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/utils.py
--rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 tripper-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      205 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      637 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/pull_request_template.md
+-rw-r--r--   0        0        0      916 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/cd_release.yml
+-rw-r--r--   0        0        0      545 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/ci_automerge_dependency_prs.yml
+-rw-r--r--   0        0        0      656 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/ci_cd_updated_main.yml
+-rw-r--r--   0        0        0      602 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/ci_check_dependencies.yml
+-rw-r--r--   0        0        0     2420 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/ci_tests.yml
+-rw-r--r--   0        0        0      838 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/ci_update_dependencies.yml
+-rw-r--r--   0        0        0      137 2023-05-24 14:00:35.357635 tripper-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1819 2023-05-24 14:00:35.357635 tripper-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       42 2023-05-24 14:00:35.357635 tripper-0.2.5/.pylintrc
+-rw-r--r--   0        0        0    10073 2023-05-24 14:01:27.094360 tripper-0.2.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-05-24 14:00:35.361635 tripper-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2496 2023-05-24 14:00:35.361635 tripper-0.2.5/README.md
+lrwxr-xr-x   0        0        0        0 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/CHANGELOG.md -> ../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/LICENSE.md -> ../LICENSE
+-rw-r--r--   0        0        0       23 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/.pages
+-rw-r--r--   0        0        0       18 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/backends/.pages
+-rw-r--r--   0        0        0       46 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/backends/collection.md
+-rw-r--r--   0        0        0       38 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/backends/ontopy.md
+-rw-r--r--   0        0        0       38 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/backends/rdflib.md
+-rw-r--r--   0        0        0       52 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/backends/sparqlwrapper.md
+-rw-r--r--   0        0        0       29 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/errors.md
+-rw-r--r--   0        0        0       35 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/interface.md
+-rw-r--r--   0        0        0       31 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/literal.md
+-rw-r--r--   0        0        0       18 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/mappings/.pages
+-rw-r--r--   0        0        0       42 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/mappings/mappings.md
+-rw-r--r--   0        0        0       35 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/namespace.md
+-rw-r--r--   0        0        0       39 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/triplestore.md
+-rw-r--r--   0        0        0       27 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/utils.md
+-rw-r--r--   0        0        0     2909 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/backend_discovery.md
+-rw-r--r--   0        0        0      183 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/css/reference.css
+-rw-r--r--   0        0        0     2489 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/index.md
+-rw-r--r--   0        0        0    12710 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/mappings/figs/function_emmo.svg
+-rw-r--r--   0        0        0      228 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/planned-backends.md
+-rw-r--r--   0        0        0     3963 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/tutorial.md
+-rw-r--r--   0        0        0     1188 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/README.md
+-rw-r--r--   0        0        0    18333 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/knowledge-base.svg
+-rw-r--r--   0        0        0     8546 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/route.svg
+-rw-r--r--   0        0        0     7117 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/workflow.svg
+-rw-r--r--   0        0        0      894 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/workflow_mappings.py
+-rw-r--r--   0        0        0    14169 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/workflow_w_pipes.svg
+-rw-r--r--   0        0        0     1943 2023-05-24 14:00:35.361635 tripper-0.2.5/mkdocs.yml
+-rw-r--r--   0        0        0     2713 2023-05-24 14:00:35.361635 tripper-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3444 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0      959 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/mappings/test_function.py
+-rw-r--r--   0        0        0     1455 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/mappings/test_mappings.py
+-rw-r--r--   0        0        0     5701 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/ontologies/family.ttl
+-rw-r--r--   0        0        0     6753 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/ontologies/food.ttl
+-rw-r--r--   0        0        0     3166 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_add_function.py
+-rw-r--r--   0        0        0      880 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_collection.py
+-rw-r--r--   0        0        0     2451 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_get_data.py
+-rw-r--r--   0        0        0     3943 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_literals.py
+-rw-r--r--   0        0        0     1993 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_namespace.py
+-rw-r--r--   0        0        0     7802 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_triplestore.py
+-rw-r--r--   0        0        0     6062 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_utils.py
+-rw-r--r--   0        0        0      705 2023-05-24 14:01:27.594367 tripper-0.2.5/tripper/__init__.py
+-rw-r--r--   0        0        0     1330 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/backends/__init__.py
+-rw-r--r--   0        0        0     2482 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/backends/collection.py
+-rw-r--r--   0        0        0     9100 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/backends/ontopy.py
+-rw-r--r--   0        0        0     7363 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/backends/rdflib.py
+-rw-r--r--   0        0        0     4112 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/backends/sparqlwrapper.py
+-rw-r--r--   0        0        0      362 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/errors.py
+-rw-r--r--   0        0        0     5379 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/interface.py
+-rw-r--r--   0        0        0     5510 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/literal.py
+-rw-r--r--   0        0        0      102 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/mappings/__init__.py
+-rw-r--r--   0        0        0    35281 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/mappings/mappings.py
+-rw-r--r--   0        0        0     6901 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/namespace.py
+-rw-r--r--   0        0        0    43718 2023-05-24 14:00:35.365635 tripper-0.2.5/tripper/triplestore.py
+-rw-r--r--   0        0        0     8237 2023-05-24 14:00:35.365635 tripper-0.2.5/tripper/utils.py
+-rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 tripper-0.2.5/PKG-INFO
```

### Comparing `tripper-0.2.4/.github/pull_request_template.md` & `tripper-0.2.5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/.github/workflows/cd_release.yml` & `tripper-0.2.5/.github/workflows/cd_release.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/.github/workflows/ci_automerge_dependency_prs.yml` & `tripper-0.2.5/.github/workflows/ci_automerge_dependency_prs.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/.github/workflows/ci_cd_updated_main.yml` & `tripper-0.2.5/.github/workflows/ci_cd_updated_main.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/.github/workflows/ci_check_dependencies.yml` & `tripper-0.2.5/.github/workflows/ci_check_dependencies.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/.github/workflows/ci_tests.yml` & `tripper-0.2.5/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/.github/workflows/ci_update_dependencies.yml` & `tripper-0.2.5/.github/workflows/ci_update_dependencies.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/.pre-commit-config.yaml` & `tripper-0.2.5/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -34,24 +34,24 @@
     rev: 1.7.5
     hooks:
     - id: bandit
       args: ["-r"]
       files: ^tripper/.*$
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.3.0
     hooks:
     - id: mypy
       exclude: ^tests/.*$
       additional_dependencies:
         - "types-requests"
         - "pydantic"
 
   - repo: https://github.com/SINTEF/ci-cd
-    rev: v2.3.0
+    rev: v2.4.0
     hooks:
     - id: docs-api-reference
       args:
       - --package-dir=tripper
     - id: docs-landing-page
 
   - repo: local
```

### Comparing `tripper-0.2.4/CHANGELOG.md` & `tripper-0.2.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## [v0.2.5](https://github.com/EMMC-ASBL/tripper/tree/v0.2.5) (2023-05-23)
+
+[Full Changelog](https://github.com/EMMC-ASBL/tripper/compare/v0.2.4...v0.2.5)
+
 ## [v0.2.4](https://github.com/EMMC-ASBL/tripper/tree/v0.2.4) (2023-04-30)
 
 [Full Changelog](https://github.com/EMMC-ASBL/tripper/compare/v0.2.3...v0.2.4)
 
 **Implemented enhancements:**
 
 - Add entrypoint system to link external backend implementation [\#63](https://github.com/EMMC-ASBL/tripper/issues/63)
```

### Comparing `tripper-0.2.4/LICENSE` & `tripper-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/README.md` & `tripper-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/docs/backend_discovery.md` & `tripper-0.2.5/docs/backend_discovery.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/docs/index.md` & `tripper-0.2.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/docs/mappings/figs/function_emmo.svg` & `tripper-0.2.5/docs/mappings/figs/function_emmo.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/docs/tutorial.md` & `tripper-0.2.5/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/examples/workflow-mappings/README.md` & `tripper-0.2.5/examples/workflow-mappings/README.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/examples/workflow-mappings/knowledge-base.svg` & `tripper-0.2.5/examples/workflow-mappings/knowledge-base.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/examples/workflow-mappings/route.svg` & `tripper-0.2.5/examples/workflow-mappings/route.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/examples/workflow-mappings/workflow.svg` & `tripper-0.2.5/examples/workflow-mappings/workflow.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/examples/workflow-mappings/workflow_mappings.py` & `tripper-0.2.5/examples/workflow-mappings/workflow_mappings.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/examples/workflow-mappings/workflow_w_pipes.svg` & `tripper-0.2.5/examples/workflow-mappings/workflow_w_pipes.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/mkdocs.yml` & `tripper-0.2.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/pyproject.toml` & `tripper-0.2.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -23,55 +23,55 @@
     "Operating System :: OS Independent",
 ]
 keywords = ["triplestore", "ontology", "RDF"]
 requires-python = "~=3.7"
 dynamic = ["version"]
 
 dependencies = [
-    "typing-extensions ~=4.5; python_version<'3.8'",
+    "typing-extensions ~=4.6; python_version<'3.8'",
 ]
 
 [project.optional-dependencies]
 docs = [
     "mike ~=1.1",
     "mkdocs ~=1.4",
-    "mkdocs-awesome-pages-plugin ~=2.8",
+    "mkdocs-awesome-pages-plugin ~=2.9",
     "mkdocs-material ~=9.1",
-    "mkdocstrings[python-legacy] ~=0.20.0",
+    "mkdocstrings[python-legacy] ~=0.21.2",
     "EMMOntoPy ~=0.5",
     "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.18,<1",
+    "DLite-Python >=0.3.19,<1",
 ]
 pre-commit = [
     "pre-commit ~=2.21",
     "pylint ~=2.13",
 ]
 testing = [
-    "pytest ~=7.2",
+    "pytest ~=7.3",
     "pytest-cov ~=4.0",
     "EMMOntoPy ~=0.5",
     "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.18,<1",
+    "DLite-Python >=0.3.19,<1",
 ]
 dev = [
     "mike ~=1.1",
     "mkdocs ~=1.4",
-    "mkdocs-awesome-pages-plugin ~=2.8",
+    "mkdocs-awesome-pages-plugin ~=2.9",
     "mkdocs-material ~=9.1",
-    "mkdocstrings[python-legacy] ~=0.20.0",
+    "mkdocstrings[python-legacy] ~=0.21.2",
     "pre-commit ~=2.21",
     "pylint ~=2.13",
-    "pytest ~=7.2",
+    "pytest ~=7.3",
     "pytest-cov ~=4.0",
     "EMMOntoPy ~=0.5",
     "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.18,<1",
+    "DLite-Python >=0.3.19,<1",
 ]
 
 [project.urls]
 Home = "https://github.com/EMMC-ASBL/tripper"
 Documentation = "https://EMMC-ASBL.github.io/tripper"
 Source = "https://github.com/EMMC-ASBL/tripper"
 "Issue Tracker" = "https://github.com/EMMC-ASBL/tripper/issues"
```

### Comparing `tripper-0.2.4/tests/conftest.py` & `tripper-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tests/mappings/test_function.py` & `tripper-0.2.5/tests/mappings/test_function.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tests/mappings/test_mappings.py` & `tripper-0.2.5/tests/mappings/test_mappings.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tests/ontologies/family.ttl` & `tripper-0.2.5/tests/ontologies/family.ttl`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tests/ontologies/food.ttl` & `tripper-0.2.5/tests/ontologies/food.ttl`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tests/test_add_function.py` & `tripper-0.2.5/tests/test_add_function.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tests/test_collection.py` & `tripper-0.2.5/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tests/test_get_data.py` & `tripper-0.2.5/tests/test_get_data.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tests/test_literals.py` & `tripper-0.2.5/tests/test_literals.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tests/test_namespace.py` & `tripper-0.2.5/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tests/test_triplestore.py` & `tripper-0.2.5/tests/test_triplestore.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tests/test_utils.py` & `tripper-0.2.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tripper/__init__.py` & `tripper-0.2.5/tripper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     SKOS,
     XML,
     XSD,
     Namespace,
 )
 from .triplestore import Triplestore, backend_packages
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 __all__ = (
     "Literal",
     #
     "DC",
     "DCTERMS",
     "DM",
```

### Comparing `tripper-0.2.4/tripper/backends/__init__.py` & `tripper-0.2.5/tripper/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tripper/backends/collection.py` & `tripper-0.2.5/tripper/backends/collection.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tripper/backends/ontopy.py` & `tripper-0.2.5/tripper/backends/ontopy.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tripper/backends/rdflib.py` & `tripper-0.2.5/tripper/backends/rdflib.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tripper/backends/sparqlwrapper.py` & `tripper-0.2.5/tripper/backends/sparqlwrapper.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tripper/interface.py` & `tripper-0.2.5/tripper/interface.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tripper/literal.py` & `tripper-0.2.5/tripper/literal.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tripper/mappings/mappings.py` & `tripper-0.2.5/tripper/mappings/mappings.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tripper/namespace.py` & `tripper-0.2.5/tripper/namespace.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tripper/triplestore.py` & `tripper-0.2.5/tripper/triplestore.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/tripper/utils.py` & `tripper-0.2.5/tripper/utils.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.4/PKG-INFO` & `tripper-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tripper
-Version: 0.2.4
+Version: 0.2.5
 Summary: A triplestore wrapper for Python.
 Keywords: triplestore,ontology,RDF
 Author-email: SINTEF <TEAM4.0@sintef.no>
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -12,45 +12,45 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Environment :: Plugins
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Dist: typing-extensions ~=4.5; python_version<'3.8'
+Requires-Dist: typing-extensions ~=4.6; python_version<'3.8'
 Requires-Dist: mike ~=1.1 ; extra == "dev"
 Requires-Dist: mkdocs ~=1.4 ; extra == "dev"
-Requires-Dist: mkdocs-awesome-pages-plugin ~=2.8 ; extra == "dev"
+Requires-Dist: mkdocs-awesome-pages-plugin ~=2.9 ; extra == "dev"
 Requires-Dist: mkdocs-material ~=9.1 ; extra == "dev"
-Requires-Dist: mkdocstrings[python-legacy] ~=0.20.0 ; extra == "dev"
+Requires-Dist: mkdocstrings[python-legacy] ~=0.21.2 ; extra == "dev"
 Requires-Dist: pre-commit ~=2.21 ; extra == "dev"
 Requires-Dist: pylint ~=2.13 ; extra == "dev"
-Requires-Dist: pytest ~=7.2 ; extra == "dev"
+Requires-Dist: pytest ~=7.3 ; extra == "dev"
 Requires-Dist: pytest-cov ~=4.0 ; extra == "dev"
 Requires-Dist: EMMOntoPy ~=0.5 ; extra == "dev"
 Requires-Dist: rdflib ~=6.3 ; extra == "dev"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "dev"
-Requires-Dist: DLite-Python >=0.3.18,<1 ; extra == "dev"
+Requires-Dist: DLite-Python >=0.3.19,<1 ; extra == "dev"
 Requires-Dist: mike ~=1.1 ; extra == "docs"
 Requires-Dist: mkdocs ~=1.4 ; extra == "docs"
-Requires-Dist: mkdocs-awesome-pages-plugin ~=2.8 ; extra == "docs"
+Requires-Dist: mkdocs-awesome-pages-plugin ~=2.9 ; extra == "docs"
 Requires-Dist: mkdocs-material ~=9.1 ; extra == "docs"
-Requires-Dist: mkdocstrings[python-legacy] ~=0.20.0 ; extra == "docs"
+Requires-Dist: mkdocstrings[python-legacy] ~=0.21.2 ; extra == "docs"
 Requires-Dist: EMMOntoPy ~=0.5 ; extra == "docs"
 Requires-Dist: rdflib ~=6.3 ; extra == "docs"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "docs"
-Requires-Dist: DLite-Python >=0.3.18,<1 ; extra == "docs"
+Requires-Dist: DLite-Python >=0.3.19,<1 ; extra == "docs"
 Requires-Dist: pre-commit ~=2.21 ; extra == "pre-commit"
 Requires-Dist: pylint ~=2.13 ; extra == "pre-commit"
-Requires-Dist: pytest ~=7.2 ; extra == "testing"
+Requires-Dist: pytest ~=7.3 ; extra == "testing"
 Requires-Dist: pytest-cov ~=4.0 ; extra == "testing"
 Requires-Dist: EMMOntoPy ~=0.5 ; extra == "testing"
 Requires-Dist: rdflib ~=6.3 ; extra == "testing"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "testing"
-Requires-Dist: DLite-Python >=0.3.18,<1 ; extra == "testing"
+Requires-Dist: DLite-Python >=0.3.19,<1 ; extra == "testing"
 Project-URL: Changelog, https://github.com/EMMC-ASBL/tripper/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://EMMC-ASBL.github.io/tripper
 Project-URL: Home, https://github.com/EMMC-ASBL/tripper
 Project-URL: Issue Tracker, https://github.com/EMMC-ASBL/tripper/issues
 Project-URL: Package, https://pypi.org/project/tripper
 Project-URL: Source, https://github.com/EMMC-ASBL/tripper
 Provides-Extra: dev
```

