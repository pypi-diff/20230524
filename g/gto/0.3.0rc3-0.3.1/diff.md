# Comparing `tmp/gto-0.3.0rc3.tar.gz` & `tmp/gto-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gto-0.3.0rc3.tar", last modified: Fri May 19 15:51:14 2023, max compression
+gzip compressed data, was "gto-0.3.1.tar", last modified: Wed May 24 10:47:07 2023, max compression
```

## Comparing `gto-0.3.0rc3.tar` & `gto-0.3.1.tar`

### file list

```diff
@@ -1,66 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.533838 gto-0.3.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.521838 gto-0.3.0rc3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.525838 gto-0.3.0rc3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.github/ISSUE_TEMPLATE/epic-or-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.525838 gto-0.3.0rc3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.github/workflows/check-test-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-19 15:50:58.000000 gto-0.3.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-19 15:51:14.533838 gto-0.3.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-19 15:50:58.000000 gto-0.3.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.529838 gto-0.3.0rc3/gto/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto/_gto_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29313 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/commit_message_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/ext_dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/ext_mlem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.529838 gto-0.3.0rc3/gto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-19 15:50:58.000000 gto-0.3.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-19 15:50:58.000000 gto-0.3.0rc3/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-19 15:51:14.533838 gto-0.3.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-19 15:50:58.000000 gto-0.3.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.533838 gto-0.3.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.533838 gto-0.3.0rc3/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/resources/sample_remote_repo_expected_history_churn.json
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/resources/sample_remote_repo_expected_registry.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/skip_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    28593 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_showcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.986599 gto-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-24 10:46:54.000000 gto-0.3.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.962599 gto-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.970599 gto-0.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-24 10:46:54.000000 gto-0.3.1/.github/ISSUE_TEMPLATE/epic-or-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.970599 gto-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-24 10:46:54.000000 gto-0.3.1/.github/workflows/check-test-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-24 10:46:54.000000 gto-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-24 10:46:54.000000 gto-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-05-24 10:46:54.000000 gto-0.3.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-24 10:46:54.000000 gto-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-24 10:47:07.986599 gto-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-24 10:46:54.000000 gto-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.978599 gto-0.3.1/gto/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-24 10:46:54.000000 gto-0.3.1/gto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 10:47:07.000000 gto-0.3.1/gto/_gto_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-24 10:46:54.000000 gto-0.3.1/gto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-05-24 10:46:54.000000 gto-0.3.1/gto/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-05-24 10:46:54.000000 gto-0.3.1/gto/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-05-24 10:46:54.000000 gto-0.3.1/gto/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-24 10:46:54.000000 gto-0.3.1/gto/commit_message_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-24 10:46:54.000000 gto-0.3.1/gto/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-24 10:46:54.000000 gto-0.3.1/gto/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-24 10:46:54.000000 gto-0.3.1/gto/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-24 10:46:54.000000 gto-0.3.1/gto/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-24 10:46:54.000000 gto-0.3.1/gto/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-24 10:46:54.000000 gto-0.3.1/gto/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-24 10:46:54.000000 gto-0.3.1/gto/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-05-24 10:46:54.000000 gto-0.3.1/gto/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-24 10:46:54.000000 gto-0.3.1/gto/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-24 10:46:54.000000 gto-0.3.1/gto/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-24 10:46:54.000000 gto-0.3.1/gto/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-24 10:46:54.000000 gto-0.3.1/gto/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.978599 gto-0.3.1/gto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-24 10:46:54.000000 gto-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 10:46:54.000000 gto-0.3.1/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-24 10:47:07.986599 gto-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-24 10:46:54.000000 gto-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.986599 gto-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 10:46:54.000000 gto-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-24 10:46:54.000000 gto-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.986599 gto-0.3.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-24 10:46:54.000000 gto-0.3.1/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-24 10:46:54.000000 gto-0.3.1/tests/resources/sample_remote_repo_expected_history_churn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-24 10:46:54.000000 gto-0.3.1/tests/resources/sample_remote_repo_expected_registry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-24 10:46:54.000000 gto-0.3.1/tests/skip_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-24 10:46:54.000000 gto-0.3.1/tests/utils.py
```

### Comparing `gto-0.3.0rc3/.github/ISSUE_TEMPLATE/epic-or-story.md` & `gto-0.3.1/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/.github/workflows/check-test-release.yml` & `gto-0.3.1/.github/workflows/check-test-release.yml`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/.gitignore` & `gto-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/.pre-commit-config.yaml` & `gto-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/.pylintrc` & `gto-0.3.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/LICENSE` & `gto-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/PKG-INFO` & `gto-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gto
-Version: 0.3.0rc3
+Version: 0.3.1
 Summary: Version and deploy your models following GitOps principles
 Download-URL: https://github.com/iterative/gto
 Author: Alexander Guschin
 Author-email: aguschin@iterative.ai
 License: Apache License 2.0
 Keywords: git repo repository artifact registry developer-tools collaboration
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gto-0.3.0rc3/README.md` & `gto-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/api.py` & `gto-0.3.1/gto/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import OrderedDict
-from typing import Any, List, Optional, Union
+from typing import Optional, Union
 
 from funcy import distinct
 from git import Repo
 
 from gto.constants import (
     ARTIFACT,
     ASSIGNMENTS_PER_VERSION,
@@ -39,67 +39,14 @@
 
 
 def get_stages(repo: Union[str, Repo], allowed: bool = False, used: bool = False):
     with GitRegistry.from_repo(repo=repo) as reg:
         return reg.get_stages(allowed=allowed, used=used)
 
 
-# TODO: make this work the same as CLI version
-def annotate(
-    repo: Union[str, Repo],
-    name: str,
-    type: Optional[str] = None,
-    path: Optional[str] = None,
-    must_exist: bool = False,
-    allow_same_path: bool = False,
-    labels: List[str] = None,
-    description: str = "",
-    custom: Any = None,
-    commit: bool = False,
-    push: bool = False,
-    branch: str = None,
-    stdout: bool = False,
-    # update: bool = False,
-):
-    """Add an artifact to the Index"""
-    with RepoIndexManager.from_repo(repo, branch=branch) as index:
-        return index.add(
-            name,
-            type=type,
-            path=path,
-            must_exist=must_exist,
-            allow_same_path=allow_same_path,
-            labels=labels,
-            description=description,
-            custom=custom,
-            update=True,
-            commit=commit,
-            push=push or is_url_of_remote_repo(repo),
-            stdout=stdout,
-        )
-
-
-def remove(
-    repo: Union[str, Repo],
-    name: str,
-    commit: bool = False,
-    push: bool = False,
-    branch: str = None,
-    stdout: bool = False,
-):
-    """Remove an artifact from the Index"""
-    with RepoIndexManager.from_repo(repo, branch=branch) as index:
-        return index.remove(
-            name,
-            commit=commit,
-            push=push or is_url_of_remote_repo(repo),
-            stdout=stdout,
-        )
-
-
 def describe(
     repo: Union[str, Repo], name: str, rev: Optional[str] = None
 ) -> Optional[Artifact]:
     """Find enrichments for the artifact"""
     shortcut = parse_shortcut(name)
     if shortcut.shortcut:
         if rev:
@@ -325,58 +272,50 @@
     with GitRegistry.from_repo(repo=repo) as reg:
         return reg.check_ref(ref)
 
 
 def show(
     repo: Union[str, Repo],
     name: Optional[str] = None,
-    all_branches=False,
-    all_commits=False,
     truncate_hexsha=False,
     registered_only=False,
     deprecated=False,
     assignments_per_version=ASSIGNMENTS_PER_VERSION,
     versions_per_stage=VERSIONS_PER_STAGE,
     sort=VersionSort.Timestamp,
     table: bool = False,
 ):
     return (
         _show_versions(
             repo,
             name=name,
-            all_branches=all_branches,
-            all_commits=all_commits,
             registered_only=registered_only,
             deprecated=deprecated,
             assignments_per_version=assignments_per_version,
             versions_per_stage=versions_per_stage,
             sort=sort,
             table=table,
             truncate_hexsha=truncate_hexsha,
         )
         if name
         else _show_registry(
             repo,
-            all_branches=all_branches,
-            all_commits=all_commits,
             registered_only=registered_only,
             deprecated=deprecated,
             assignments_per_version=assignments_per_version,
             versions_per_stage=versions_per_stage,
             sort=sort,
             table=table,
             truncate_hexsha=truncate_hexsha,
         )
     )
 
 
 def _show_registry(
     repo: Union[str, Repo],
-    all_branches=False,
-    all_commits=False,
     registered_only=False,
     deprecated=False,
     assignments_per_version: int = None,
     versions_per_stage: int = None,
     sort: VersionSort = None,
     table: bool = False,
     truncate_hexsha: bool = False,
@@ -409,18 +348,15 @@
                     )
                     or None
                     for name in stages
                 },
                 "registered": o.is_registered,
                 "active": o.is_active,
             }
-            for o in reg.get_artifacts(
-                all_branches=all_branches,
-                all_commits=all_commits,
-            ).values()
+            for o in reg.get_artifacts().values()
             if o.is_active or deprecated
         }
 
     if not table:
         return models_state
 
     return [
@@ -438,16 +374,14 @@
     ], "keys"
 
 
 def _show_versions(  # pylint: disable=too-many-locals
     repo: Union[str, Repo],
     name: str,
     raw: bool = False,
-    all_branches=False,
-    all_commits=False,
     registered_only=False,
     deprecated=False,
     assignments_per_version: int = None,
     versions_per_stage: int = None,
     sort: VersionSort = None,
     table: bool = False,
     truncate_hexsha: bool = False,
@@ -459,19 +393,15 @@
 
     shortcut = parse_shortcut(name)
 
     with GitRegistry.from_repo(repo=repo) as reg:
         if raw:
             return reg.find_artifact(shortcut.name).versions
 
-        artifact = reg.find_artifact(
-            shortcut.name,
-            all_branches=all_branches,
-            all_commits=all_commits,
-        )
+        artifact = reg.find_artifact(shortcut.name)
     stages = artifact.get_vstages(
         registered_only=registered_only,
         assignments_per_version=assignments_per_version,
         versions_per_stage=versions_per_stage,
         sort=sort,
     )
     versions = []
@@ -533,25 +463,20 @@
     return versions_, "keys"
 
 
 def history(
     repo: Union[str, Repo],
     artifact: Optional[str] = None,
     # action: str = None,
-    all_branches=False,
-    all_commits=False,
     ascending: bool = False,
     table: bool = False,
     truncate_hexsha: bool = False,
 ):
     with GitRegistry.from_repo(repo=repo) as reg:
-        artifacts = reg.get_artifacts(
-            all_branches=all_branches,
-            all_commits=all_commits,
-        )
+        artifacts = reg.get_artifacts()
 
     def format_hexsha(hexsha):
         return hexsha[:7] if truncate_hexsha and is_hexsha(hexsha) else hexsha
 
     events = [
         OrderedDict(
             timestamp=e.created_at,
@@ -564,14 +489,15 @@
             author=e.author,
             author_email=e.author_email,
             message=e.message,
             ref=format_hexsha(e.ref) if e.ref == e.commit_hexsha else e.ref,
         )
         for o in artifacts.values()
         for e in o.get_events()
+        if type(e).__name__.lower() != "commit"
     ]
 
     events = sorted(
         events,
         key=lambda x: (x["timestamp"], x["priority"]),
     )
     if not ascending:
```

### Comparing `gto-0.3.0rc3/gto/base.py` & `gto-0.3.1/gto/base.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/cli.py` & `gto-0.3.1/gto/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 )
 from gto.exceptions import (
     GTOException,
     NotImplementedInGTO,
     WrongArgs,
     WrongConfig,
 )
-from gto.index import RepoIndexManager
 from gto.ui import (
     EMOJI_FAIL,
     EMOJI_GTO,
     EMOJI_OK,
     bold,
     cli_echo,
     color,
@@ -229,24 +228,14 @@
 option_repo = Option(
     ".",
     "-r",
     "--repo",
     help="Local or remote repository",
     show_default=True,
 )
-option_all_branches = Option(
-    False,
-    "-a",
-    "--all-branches",
-    is_flag=True,
-    help="Read heads from all branches",
-)
-option_all_commits = Option(
-    False, "-A", "--all-commits", is_flag=True, help="Read all commits"
-)
 option_message = Option(
     None, "--message", "-m", help="Message to annotate the Git tag with"
 )
 option_force = Option(
     False,
     "--force",
     is_flag=True,
@@ -416,15 +405,14 @@
     Git Tag Ops. Turn your Git repository into an Artifact Registry:
     * Registry: Track new artifacts and their versions for releases and significant
     changes.
     * Lifecycle Management: Create actionable stages for versions marking status of
     artifact or it's readiness to be consumed by a specific environment.
     * GitOps: Signal CI/CD automation or other downstream systems to act upon these
     new versions and lifecycle updates.
-    * Enrichments: Annotate and query artifact metadata with additional information.
     """
     if ctx.invoked_subcommand is None and show_version:
         with cli_echo():
             echo(f"{EMOJI_GTO} GTO Version: {gto.__version__}")
     if verbose:
         logger = logging.getLogger("gto")
         logger.handlers[0].setLevel(logging.DEBUG)
@@ -491,117 +479,14 @@
                 # send_cli_call(cmd_name, error_msg=error, **res)
 
         return inner
 
     return decorator
 
 
-@gto_command(section=CommandGroups.enriching)
-def annotate(
-    repo: str = option_repo,
-    name: str = arg_name,
-    type: str = Option(None, help="Artifact type"),
-    path: str = Option(None, help="Artifact path"),
-    must_exist: bool = Option(
-        False,
-        "-e",
-        "--must-exist",
-        is_flag=True,
-        help="Verify artifact is committed to Git",
-    ),
-    allow_same_path: bool = Option(
-        False,
-        "--allow-same-path",
-        is_flag=True,
-        help="Allow multiple artifacts use the same path",
-    ),
-    label: List[str] = Option(None, "--label", help="Labels to add to artifact"),
-    description: str = Option("", "-d", "--description", help="Artifact description"),
-    custom: str = Option(
-        None,
-        "-c",
-        "--custom",
-        help="Custom metadata to add to artifact",
-    ),
-    commit: bool = option_commit,
-    push: bool = option_push_commit,
-    branch: str = option_branch,
-    # update: bool = Option(
-    #     False, "-u", "--update", is_flag=True, help="Update artifact if it exists"
-    # ),
-):
-    """Update artifact metadata annotations."""
-    gto.api.annotate(
-        repo,
-        name,
-        type=type,
-        path=path,
-        must_exist=must_exist,
-        allow_same_path=allow_same_path,
-        labels=label,
-        description=description,
-        custom=custom,
-        commit=commit,
-        push=push,
-        branch=branch,
-        stdout=True,
-        # update=update,
-    )
-
-
-@gto_command(section=CommandGroups.enriching)
-def remove(
-    repo: str = option_repo,
-    name: str = arg_name,
-    commit: bool = option_commit,
-    push: bool = option_push_commit,
-    branch: str = option_branch,
-):
-    """Remove the enrichment for given artifact."""
-    gto.api.remove(
-        repo=repo, name=name, commit=commit, push=push, branch=branch, stdout=True
-    )
-
-
-@gto_command(section=CommandGroups.enriching)
-def describe(
-    repo: str = option_repo,
-    name: str = arg_name,
-    rev: str = option_rev,
-    type: Optional[bool] = option_show_type,
-    path: Optional[bool] = option_show_path,
-    description: Optional[bool] = option_show_description,
-    custom: Optional[bool] = option_show_custom,
-):
-    """Display enrichments for an artifact."""
-    assert (
-        sum(bool(i) for i in (type, path, description)) <= 1  # , custom
-    ), "Can output one key only"
-    if type:
-        field = "type"
-    elif path:
-        field = "path"
-    elif description:
-        field = "description"
-    elif custom:
-        field = "custom"
-    else:
-        field = None
-
-    artifact = gto.api.describe(repo=repo, name=name, rev=rev)
-    if not artifact:
-        return
-    annotation = artifact.dict(exclude_defaults=True)
-    if field is None:
-        format_echo(annotation, "json")
-    elif field in annotation:
-        with cli_echo():
-            echo(annotation[field])
-
-
 @gto_command(section=CommandGroups.modifying)
 def register(
     repo: str = option_repo,
     name: str = arg_name,
     ref: str = Argument("HEAD", help="Git reference to use for registration"),
     version: Optional[str] = Option(
         None, "--version", "--ver", help="Version name in SemVer format"
@@ -788,16 +673,14 @@
         echo(f"{EMOJI_OK} {found_event}")
 
 
 @gto_command(section=CommandGroups.querying)
 def show(  # pylint: disable=too-many-locals
     repo: str = option_repo,
     name: str = Argument(None, help="Artifact name to show. If empty, show registry"),
-    all_branches: bool = option_all_branches,
-    all_commits: bool = option_all_commits,
     json: bool = option_json,
     plain: bool = option_plain,
     show_name: bool = option_show_name,
     show_version: bool = option_show_version,
     show_stage: bool = option_show_stage,
     show_ref: bool = option_show_ref,
     registered_only: bool = option_registered_only,
@@ -811,30 +694,26 @@
     assert (
         sum(bool(i) for i in [json, plain] + show_options) <= 1
     ), "Only one output format allowed"
     if json:
         output = gto.api.show(
             repo,
             name=name,
-            all_branches=all_branches,
-            all_commits=all_commits,
             registered_only=registered_only,
             deprecated=deprecated,
             assignments_per_version=assignments_per_version,
             versions_per_stage=versions_per_stage,
             sort=sort,
             table=False,
         )
         format_echo(output, "json")
     else:
         output = gto.api.show(
             repo,
             name=name,
-            all_branches=all_branches,
-            all_commits=all_commits,
             registered_only=registered_only,
             deprecated=deprecated,
             assignments_per_version=assignments_per_version,
             versions_per_stage=versions_per_stage,
             sort=sort,
             table=True,
             truncate_hexsha=True,
@@ -859,41 +738,35 @@
             )
 
 
 @gto_command(section=CommandGroups.querying)
 def history(
     repo: str = option_repo,
     name: str = Argument(None, help="Artifact name to show. If empty, show all."),
-    all_branches: bool = option_all_branches,
-    all_commits: bool = option_all_commits,
     json: bool = option_json,
     plain: bool = option_plain,
     ascending: bool = option_ascending,
 ):
     """Show a journal of registry operations."""
     assert sum(bool(i) for i in (json, plain)) <= 1, "Only one output format allowed"
     if json:
         format_echo(
             gto.api.history(
                 repo,
                 name,
-                all_branches=all_branches,
-                all_commits=all_commits,
                 ascending=ascending,
                 table=False,
             ),
             format="json",
         )
     else:
         format_echo(
             gto.api.history(
                 repo,
                 name,
-                all_branches=all_branches,
-                all_commits=all_commits,
                 ascending=ascending,
                 table=True,
                 truncate_hexsha=True,
             ),
             format="table",
             format_table="plain" if plain else "fancy_outline",
             if_empty="Nothing found in the current workspace",
@@ -932,25 +805,17 @@
     """Technical cmd: Print current registry state."""
     state = make_ready_to_serialize(
         gto.api._get_state(repo).dict()  # pylint: disable=protected-access
     )
     format_echo(state, "json")
 
 
-@gto_command(hidden=True)
-def print_index(repo: str = option_repo):
-    """Technical cmd: Print repo index."""
-    with RepoIndexManager.from_repo(repo) as index:
-        format_echo(index.artifact_centric_representation(), "json")
-
-
 @gto_command(section=CommandGroups.querying)
 def doctor(
     repo: str = option_repo,
-    all_commits: bool = option_all_commits,
 ):
     """Display GTO version and check the registry for problems."""
     with cli_echo():
         echo(f"{EMOJI_GTO} GTO Version: {gto.__version__}")
         echo("---------------------------------")
         try:
             from gto.config import (  # pylint: disable=import-outside-toplevel
@@ -959,16 +824,13 @@
 
             echo(CONFIG.__repr_str__("\n"))
         except WrongConfig:
             echo(f"{EMOJI_FAIL} Fail to parse config")
         echo("---------------------------------")
 
     gto.api._get_state(repo).dict()  # pylint: disable=protected-access
-    if all_commits:
-        with RepoIndexManager.from_repo(repo) as index:
-            index.artifact_centric_representation()
     with cli_echo():
         echo(f"{EMOJI_OK} No issues found")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `gto-0.3.0rc3/gto/config.py` & `gto-0.3.1/gto/config.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/constants.py` & `gto-0.3.1/gto/constants.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/exceptions.py` & `gto-0.3.1/gto/exceptions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/git_utils.py` & `gto-0.3.1/gto/git_utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/index.py` & `gto-0.3.1/gto/index.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/log.py` & `gto-0.3.1/gto/log.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/registry.py` & `gto-0.3.1/gto/registry.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/tag.py` & `gto-0.3.1/gto/tag.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/ui.py` & `gto-0.3.1/gto/ui.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/utils.py` & `gto-0.3.1/gto/utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto/versions.py` & `gto-0.3.1/gto/versions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/gto.egg-info/PKG-INFO` & `gto-0.3.1/gto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gto
-Version: 0.3.0rc3
+Version: 0.3.1
 Summary: Version and deploy your models following GitOps principles
 Download-URL: https://github.com/iterative/gto
 Author: Alexander Guschin
 Author-email: aguschin@iterative.ai
 License: Apache License 2.0
 Keywords: git repo repository artifact registry developer-tools collaboration
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gto-0.3.0rc3/gto.egg-info/SOURCES.txt` & `gto-0.3.1/gto.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 gto/base.py
 gto/cli.py
 gto/commit_message_generator.py
 gto/config.py
 gto/constants.py
 gto/exceptions.py
 gto/ext.py
-gto/ext_dvc.py
-gto/ext_mlem.py
 gto/git_utils.py
 gto/index.py
 gto/log.py
 gto/registry.py
 gto/tag.py
 gto/ui.py
 gto/utils.py
```

### Comparing `gto-0.3.0rc3/setup.cfg` & `gto-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/setup.py` & `gto-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/tests/conftest.py` & `gto-0.3.1/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,34 +66,44 @@
         CONFIG_FILE_NAME,
         "",
     )
 
     return repo, write_file
 
 
+artifacts_yaml = """
+rf:
+  type: model
+  path: models/random-forest.pkl
+  virtual: false
+nn:
+  type: model
+  path: models/neural-network.pkl
+  virtual: false
+features:
+  type: dataset
+  path: datasets/features.csv
+"""
+
+
 @pytest.fixture
 def showcase(
     init_showcase_semver,
 ):  # pylint: disable=too-many-locals, too-many-statements
     repo: git.Repo
     repo, write_file = init_showcase_semver
     path = repo.working_dir
 
     write_file("models/random-forest.pkl", "1st version")
     write_file("models/neural-network.pkl", "1st version")
     repo.index.add(["models"])
     repo.index.commit("Create models")
 
-    gto.api.annotate(
-        path, "rf", type="model", path="models/random-forest.pkl", must_exist=True
-    )
-    gto.api.annotate(
-        path, "nn", type="model", path="models/neural-network.pkl", must_exist=True
-    )
-    gto.api.annotate(path, "features", type="dataset", path="datasets/features.csv")
+    with open(os.path.join(path, "artifacts.yaml"), "w", encoding="utf8") as file:
+        file.write(artifacts_yaml)
 
     repo.index.add(["artifacts.yaml"])
     first_commit = repo.index.commit("Add artifacts")
 
     nn_vname = "v0.0.1"
     rf_vname = "v1.2.3"
     gto.api.register(path, "rf", "HEAD", rf_vname)
```

### Comparing `gto-0.3.0rc3/tests/resources/__init__.py` & `gto-0.3.1/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/tests/resources/sample_remote_repo_expected_registry.json` & `gto-0.3.1/tests/resources/sample_remote_repo_expected_registry.json`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/tests/skip_presets.py` & `gto-0.3.1/tests/skip_presets.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/tests/test_api.py` & `gto-0.3.1/tests/test_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,20 +11,15 @@
 import git
 import pytest
 from freezegun import freeze_time
 
 import gto
 import tests.resources
 from gto.api import show
-from gto.commit_message_generator import (
-    generate_annotate_commit_message,
-    generate_remove_commit_message,
-)
-from gto.exceptions import PathIsUsed, WrongArgs
-from gto.git_utils import git_clone
+from gto.exceptions import WrongArgs
 from gto.index import RepoIndexManager
 from gto.tag import find
 from gto.versions import SemVer
 from tests.skip_presets import skip_for_windows
 from tests.utils import (
     check_obj,
     convert_objects_to_str_in_json_serializable_object,
@@ -46,99 +41,69 @@
 
 def test_api_info_commands_empty_repo(empty_git_repo: Tuple[git.Repo, Callable]):
     repo, write_file = empty_git_repo
     gto.api.show(repo.working_dir)
     gto.api.history(repo.working_dir)
 
 
-def test_add_remove(empty_git_repo: Tuple[git.Repo, Callable]):
-    repo, write_file = empty_git_repo
-    name, type, path, must_exist = "new-artifact", "new-type", "new/path", False
-    gto.api.annotate(
-        repo.working_dir, name, type=type, path=path, must_exist=must_exist
-    )
-    with pytest.raises(PathIsUsed):
-        gto.api.annotate(repo.working_dir, "other-name", path=path)
-    gto.api.annotate(repo.working_dir, "other-name", path=path, allow_same_path=True)
-    with RepoIndexManager.from_repo(repo) as index:
-        index = index.get_index()
-    assert name in index
-    check_obj(
-        index.state[name],
-        dict(
-            type=type,
-            path=path,
-            virtual=not must_exist,
-            labels=[],
-            description="",
-            custom=None,
-        ),
-        [],
-    )
-    gto.api.remove(repo, name)
-    with RepoIndexManager.from_repo(repo) as index:
-        index = index.get_index()
-    assert name not in index
-
-
 @pytest.fixture
 def repo_with_artifact(init_showcase_semver):
     repo: git.Repo
     repo, write_file = init_showcase_semver
-    name, type, path, must_exist = "new-artifact", "new-type", "new/path", False
-    gto.api.annotate(repo, name, type=type, path=path, must_exist=must_exist)
+    with open(
+        os.path.join(repo.working_dir, "artifacts.yaml"), "w", encoding="utf8"
+    ) as f:
+        f.write("rf: \n  type: model\n  path: models/random-forest.pkl\n")
     repo.index.add(["artifacts.yaml"])
     repo.index.commit("Added index")
-    gto.api.annotate(repo, name, type=type, path="path", must_exist=must_exist)
+    with open(
+        os.path.join(repo.working_dir, "artifacts.yaml"), "w", encoding="utf8"
+    ) as f:
+        f.write("rf: \n  type: model\n  path: models/random-forest.pklx\n")
     repo.index.add(["artifacts.yaml"])
     repo.index.commit("Added index")
-    return repo, name
+    return repo, "new-artifact"
 
 
-def test_api_info_commands_repo_with_artifact(
-    repo_with_artifact: Tuple[git.Repo, Callable]
-):
-    repo, write_file = repo_with_artifact
-    gto.api.show(repo)
-    gto.api.show(repo, "new-artifact")
-    gto.api.history(repo)
-
-
-def test_describe(repo_with_artifact: Tuple[git.Repo, Callable]):
-    repo, write_file = repo_with_artifact
-    gto.api.annotate(repo, "new-artifact", path="other-path")
-    check_obj(
-        gto.api.describe(repo, "new-artifact").dict(exclude_defaults=True),  # type: ignore
-        dict(
-            type="new-type",
-            path="other-path",
-        ),
-    )
-    check_obj(
-        gto.api.describe(repo, "new-artifact", rev="HEAD").dict(exclude_defaults=True),  # type: ignore
-        dict(
-            type="new-type",
-            path="path",
-        ),
-    )
+# def test_api_info_commands_repo_with_artifact(
+#     repo_with_artifact: Tuple[git.Repo, Callable]
+# ):
+#     repo, write_file = repo_with_artifact
+#     gto.api.show(repo)
+#     gto.api.show(repo, "new-artifact")
+#     gto.api.history(repo)
+
+
+# def test_describe(repo_with_artifact: Tuple[git.Repo, Callable]):
+#     repo, write_file = repo_with_artifact
+#     gto.api.annotate(repo, "new-artifact", path="other-path")
+#     check_obj(
+#         gto.api.describe(repo, "new-artifact").dict(exclude_defaults=True),  # type: ignore
+#         dict(
+#             type="new-type",
+#             path="other-path",
+#         ),
+#     )
+#     check_obj(
+#         gto.api.describe(repo, "new-artifact", rev="HEAD").dict(exclude_defaults=True),  # type: ignore
+#         dict(
+#             type="new-type",
+#             path="path",
+#         ),
+#     )
 
 
 def test_register_deregister(repo_with_artifact):
     repo, name = repo_with_artifact
     vname1, vname2 = "v1.0.0", "v1.0.1"
     gto.api.register(repo.working_dir, name, "HEAD", vname1)
     latest = gto.api.find_latest_version(repo.working_dir, name)
     assert latest.version == vname1
-    gto.api.annotate(
-        repo.working_dir,
-        "something-irrelevant",
-        "doesnt-matter",
-        "anything",
-        must_exist=False,
-    )
+    with open("tmp.txt", "w", encoding="utf8") as f:
+        f.write("some text")
     repo.index.commit(
         "Irrelevant action to create a git commit to register another version"
     )
     message = "Some message"
     author = "GTO"
     author_email = "gto@iterative.ai"
     gto.api.register(
@@ -655,162 +620,7 @@
             )
             mocked_git_push_tag.assert_called_once_with(
                 repo=Path(tmp_dir.name).as_posix(),
                 tag_name="churn#staging!#3",
                 delete=False,
             )
             tmp_dir.cleanup()
-
-
-def test_if_annotate_with_auto_commit_then_invoke_stash_and_commit(
-    init_showcase_semver,
-):
-    repo, write_file = init_showcase_semver
-    name, type, path, must_exist = "new-artifact", "new-type", "new/path", False
-    repo.index.commit(message="first commit")
-
-    with patch("gto.git_utils.stashed_changes") as mocked_stashed_changes:
-        mocked_stashed_changes.return_value.__enter__.return_value = [], []
-        with patch(
-            "gto.git_utils.git_add_and_commit_all_changes"
-        ) as mocked_git_add_and_commit_all_changes:
-            gto.api.annotate(
-                repo.working_dir,
-                name,
-                type=type,
-                path=path,
-                must_exist=must_exist,
-                commit=True,
-            )
-
-    mocked_stashed_changes.assert_called_once_with(repo=repo, include_untracked=True)
-    mocked_git_add_and_commit_all_changes.assert_called_once_with(
-        repo=repo,
-        message=generate_annotate_commit_message(name=name, type=type, path=path),
-    )
-
-
-def test_if_remove_with_auto_commit_then_invoke_stash_and_commit(
-    init_showcase_semver,
-):
-    repo, write_file = init_showcase_semver
-    name, type, path, must_exist = "new-artifact", "new-type", "new/path", False
-    repo.index.commit(message="first commit")
-    gto.api.annotate(
-        repo.working_dir,
-        name,
-        type=type,
-        path=path,
-        must_exist=must_exist,
-        commit=True,
-    )
-
-    with patch("gto.git_utils.stashed_changes") as mocked_stashed_changes:
-        mocked_stashed_changes.return_value.__enter__.return_value = [], []
-        with patch(
-            "gto.git_utils.git_add_and_commit_all_changes"
-        ) as mocked_git_add_and_commit_all_changes:
-            gto.api.remove(repo=repo.working_dir, name=name, commit=True)
-
-    mocked_stashed_changes.assert_called_once_with(repo=repo, include_untracked=True)
-    mocked_git_add_and_commit_all_changes.assert_called_once_with(
-        repo=git.Repo(repo.working_dir),
-        message=generate_remove_commit_message(name=name),
-    )
-
-
-def test_if_annotate_with_auto_push_then_invoke_commit_and_push(init_showcase_semver):
-    repo, write_file = init_showcase_semver
-    name, type, path, must_exist = "new-artifact", "new-type", "new/path", False
-    repo.index.commit(message="first commit")
-
-    with patch("gto.git_utils.stashed_changes") as mocked_stashed_changes:
-        mocked_stashed_changes.return_value.__enter__.return_value = [], []
-        with patch(
-            "gto.git_utils.git_add_and_commit_all_changes"
-        ) as mocked_git_add_and_commit_all_changes:
-            with patch("gto.git_utils.git_push") as mocked_git_push:
-                gto.api.annotate(
-                    repo.working_dir,
-                    name,
-                    type=type,
-                    path=path,
-                    must_exist=must_exist,
-                    push=True,
-                )
-
-    mocked_stashed_changes.assert_called_once_with(repo=repo, include_untracked=True)
-    mocked_git_add_and_commit_all_changes.assert_called_once_with(
-        repo=repo,
-        message=generate_annotate_commit_message(name=name, type=type, path=path),
-    )
-    mocked_git_push.assert_called_once_with(repo=repo)
-
-
-def test_if_remove_with_auto_push_then_invoke_commit_and_push(
-    init_showcase_semver,
-):
-    repo, write_file = init_showcase_semver
-    name, type, path, must_exist = "new-artifact", "new-type", "new/path", False
-    repo.index.commit(message="first commit")
-    gto.api.annotate(
-        repo.working_dir,
-        name,
-        type=type,
-        path=path,
-        must_exist=must_exist,
-        commit=True,
-    )
-
-    with patch("gto.git_utils.stashed_changes") as mocked_stashed_changes:
-        mocked_stashed_changes.return_value.__enter__.return_value = [], []
-        with patch(
-            "gto.git_utils.git_add_and_commit_all_changes"
-        ) as mocked_git_add_and_commit_all_changes:
-            with patch("gto.git_utils.git_push") as mocked_git_push:
-                gto.api.remove(repo=repo.working_dir, name=name, push=True)
-
-    mocked_stashed_changes.assert_called_once_with(repo=repo, include_untracked=True)
-    mocked_git_add_and_commit_all_changes.assert_called_once_with(
-        repo=repo, message=generate_remove_commit_message(name=name)
-    )
-    mocked_git_push.assert_called_once_with(repo=repo)
-
-
-@skip_for_windows
-def test_if_annotate_with_remote_repo_then_clone_and_push():
-    with patch("gto.git_utils.git_push") as mocked_git_push:
-        with patch("gto.git_utils.git_clone") as mocked_git_clone:
-            mocked_git_clone.side_effect = git_clone
-            with patch("gto.git_utils.TemporaryDirectory") as MockedTemporaryDirectory:
-                MockedTemporaryDirectory.return_value = (
-                    TemporaryDirectory()  # pylint: disable=consider-using-with
-                )
-                gto.api.annotate(
-                    repo=tests.resources.SAMPLE_REMOTE_REPO_URL, name="test-model"
-                )
-
-    mocked_git_push.assert_called_once()
-    mocked_git_clone.assert_called_once_with(
-        repo=tests.resources.SAMPLE_REMOTE_REPO_URL,
-        dir=MockedTemporaryDirectory.return_value.name,
-    )
-
-
-@skip_for_windows
-def test_if_remove_with_remote_repo_then_clone_and_push():
-    with patch("gto.git_utils.git_push") as mocked_git_push:
-        with patch("gto.git_utils.git_clone") as mocked_git_clone:
-            mocked_git_clone.side_effect = git_clone
-            with patch("gto.git_utils.TemporaryDirectory") as MockedTemporaryDirectory:
-                MockedTemporaryDirectory.return_value = (
-                    TemporaryDirectory()  # pylint: disable=consider-using-with
-                )
-                gto.api.remove(
-                    repo=tests.resources.SAMPLE_REMOTE_REPO_URL, name="segment"
-                )
-
-    mocked_git_push.assert_called_once()
-    mocked_git_clone.assert_called_once_with(
-        repo=tests.resources.SAMPLE_REMOTE_REPO_URL,
-        dir=MockedTemporaryDirectory.return_value.name,
-    )
```

### Comparing `gto-0.3.0rc3/tests/test_cli.py` & `gto-0.3.1/tests/test_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 import pytest
 import typer
 from packaging import version
 from typer.main import get_command_from_info
 
 from gto.cli import app
 from gto.exceptions import GTOException
-from gto.index import RepoIndexManager
 from tests.conftest import Runner
 
-from .utils import check_obj
-
 
 def _check_output_contains(output: str, search_value: str) -> bool:
     return search_value in output
 
 
 def _check_output_exact_match(output: str, search_value: str) -> bool:
     return search_value == output
@@ -142,32 +139,14 @@
         "v1.2.4\n",
     )
     _check_successful_cmd(
         "show",
         ["-r", path, "rf#production", "--ref"],
         "rf@v1.2.3\n",
     )
-    _check_successful_cmd("describe", ["-r", path, "artifactnotexist"], "")
-    _check_successful_cmd("describe", ["-r", path, "rf#stagenotexist"], "")
-    _check_successful_cmd("describe", ["-r", path, "rf"], EXPECTED_DESCRIBE_OUTPUT)
-    _check_successful_cmd(
-        "describe", ["-r", path, "rf#production"], EXPECTED_DESCRIBE_OUTPUT
-    )
-    _check_successful_cmd(
-        "describe", ["-r", path, "rf@latest"], EXPECTED_DESCRIBE_OUTPUT
-    )
-    _check_successful_cmd(
-        "describe", ["-r", path, "rf@v1.2.3"], EXPECTED_DESCRIBE_OUTPUT
-    )
-    _check_successful_cmd(
-        "describe", ["-r", path, "rf", "--path"], "models/random-forest.pkl\n"
-    )
-    _check_successful_cmd("describe", ["-r", path, "rf", "--type"], "model\n")
-    _check_successful_cmd("describe", ["-r", path, "rf", "--description"], "")
-    _check_successful_cmd("describe", ["-r", path, "rf", "--custom"], "")
     # None because of random order - fix this
     _check_successful_cmd("stages", ["-r", path], None)
     # None because of output randomness and complexity
     _check_successful_cmd(
         "show",
         ["-r", path],
         None,
@@ -247,83 +226,14 @@
         "some-label"
     ],
     "description": "new description"
 }
 """
 
 
-def test_annotate(empty_git_repo: Tuple[git.Repo, Callable]):
-    repo, write_file = empty_git_repo
-    name = "new-artifact"
-    _check_successful_cmd(
-        "annotate",
-        [
-            "-r",
-            repo.working_dir,
-            "--type",
-            "new-type",
-            name,
-            "--path",
-            "new/path",
-            "--label",
-            "some-label",
-            "--label",
-            "another-label",
-            "--description",
-            "some description",
-        ],
-        "Updated `artifacts.yaml`",
-        _check_output_contains,
-    )
-    _check_successful_cmd(
-        "annotate",
-        [
-            "-r",
-            repo.working_dir,
-            name,
-            "--label",
-            "new-label",
-            "--description",
-            "new description",
-        ],
-        "Updated `artifacts.yaml`",
-        _check_output_contains,
-    )
-    with RepoIndexManager.from_repo(repo.working_dir) as index:
-        artifact = index.get_index().state[name]  # pylint: disable=protected-access
-    check_obj(
-        artifact.dict(exclude_defaults=True),
-        dict(
-            type="new-type",
-            path="new/path",
-            labels=["another-label", "new-label", "some-label"],
-            description="new description",
-        ),
-    )
-    repo.index.add(["artifacts.yaml"])
-    repo.index.commit("Add new artifact")
-
-    _check_successful_cmd(
-        "describe", ["-r", repo.working_dir, name], EXPECTED_DESCRIBE_OUTPUT_2
-    )
-    _check_successful_cmd(
-        "remove",
-        ["-r", repo.working_dir, name],
-        "Updated `artifacts.yaml`",
-        _check_output_contains,
-    )
-    write_file(name, "new-artifact update")
-    repo.index.add(["artifacts.yaml"])
-    repo.index.commit("Remove new artifact")
-
-    _check_successful_cmd(
-        "describe", ["-r", repo.working_dir, "this-artifact-doesnt-exist"], ""
-    )
-
-
 def test_register(repo_with_commit: Tuple[git.Repo, Callable]):
     repo, write_file = repo_with_commit
 
     _check_successful_cmd(
         "register",
         ["-r", repo.working_dir, "a1"],
         "Created git tag 'a1@v0.0.1' that registers version\n"
```

### Comparing `gto-0.3.0rc3/tests/test_constants.py` & `gto-0.3.1/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/tests/test_git_utils.py` & `gto-0.3.1/tests/test_git_utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/tests/test_index.py` & `gto-0.3.1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/tests/test_registry.py` & `gto-0.3.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/tests/test_showcase.py` & `gto-0.3.1/tests/test_showcase.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/tests/test_tag.py` & `gto-0.3.1/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/tests/test_versions.py` & `gto-0.3.1/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc3/tests/utils.py` & `gto-0.3.1/tests/utils.py`

 * *Files identical despite different names*

