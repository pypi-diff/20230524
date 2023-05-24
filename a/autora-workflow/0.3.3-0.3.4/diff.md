# Comparing `tmp/autora-workflow-0.3.3.tar.gz` & `tmp/autora-workflow-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-workflow-0.3.3.tar", last modified: Fri May  5 21:05:47 2023, max compression
+gzip compressed data, was "autora-workflow-0.3.4.tar", last modified: Wed May 24 21:14:09 2023, max compression
```

## Comparing `autora-workflow-0.3.3.tar` & `autora-workflow-0.3.4.tar`

### file list

```diff
@@ -1,104 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.031272 autora-workflow-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.043272 autora-workflow-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.047272 autora-workflow-0.3.3/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/autora-workflow.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.047272 autora-workflow-0.3.3/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.047272 autora-workflow-0.3.3/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.047272 autora-workflow-0.3.3/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/runConfigurations/pytest_in_tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.051272 autora-workflow-0.3.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.051272 autora-workflow-0.3.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.035272 autora-workflow-0.3.3/docs/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.051272 autora-workflow-0.3.3/docs/cli/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)   253372 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/basic-usage/README.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/basic-usage/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.055272 autora-workflow-0.3.3/docs/cli/with-cylc-conda/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.035272 autora-workflow-0.3.3/docs/cli/with-cylc-conda/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.055272 autora-workflow-0.3.3/docs/cli/with-cylc-conda/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/lib/python/controller_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-conda/lib/python/dump_initial_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.055272 autora-workflow-0.3.3/docs/cli/with-cylc-pip/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.035272 autora-workflow-0.3.3/docs/cli/with-cylc-pip/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.055272 autora-workflow-0.3.3/docs/cli/with-cylc-pip/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/lib/python/controller_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/lib/python/dump_initial_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-pip/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.059272 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/global.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.035272 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.059272 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/lib/python/controller_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/lib/python/dump_initial_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/cli/with-cylc-slurm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.063272 autora-workflow-0.3.3/docs/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/interactive/accessing-state-dependent-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/interactive/basic-usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/interactive/passing-static-parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    58276 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/interactive/saving-and-loading-dill.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/docs/interactive/using-alternative-planners-and-executors.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.063272 autora-workflow-0.3.3/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.039272 autora-workflow-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.039272 autora-workflow-0.3.3/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.063272 autora-workflow-0.3.3/src/autora/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.063272 autora-workflow-0.3.3/src/autora/workflow/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/serializer/yaml_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/src/autora/workflow/state/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/state/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/state/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/src/autora/workflow/state/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/src/autora_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-05 21:05:46.000000 autora-workflow-0.3.3/src/autora_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-05 21:05:47.000000 autora-workflow-0.3.3/src/autora_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:05:46.000000 autora-workflow-0.3.3/src/autora_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 21:05:46.000000 autora-workflow-0.3.3/src/autora_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 21:05:46.000000 autora-workflow-0.3.3/src/autora_workflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:47.067272 autora-workflow-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-05 21:05:34.000000 autora-workflow-0.3.3/tests/test_controller_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/autora-workflow.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/runConfigurations/pytest_in_tests.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/docs/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/docs/cli/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)   249249 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/cli/basic-usage/README.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/cli/basic-usage/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/docs/cli/with-cylc/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/cli/with-cylc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/docs/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)    16061 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/interactive/accessing-state-dependent-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/interactive/basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/interactive/passing-static-parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    57339 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/interactive/saving-and-loading-dill.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/docs/interactive/using-alternative-planners-and-executors.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/examples/cylc-conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/examples/cylc-conda/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/examples/cylc-conda/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-conda/lib/python/dump_initial_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/examples/cylc-pip/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/examples/cylc-pip/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/examples/cylc-pip/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/lib/python/dump_initial_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-pip/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.316397 autora-workflow-0.3.4/examples/cylc-slurm-pip/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/global.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/examples/cylc-slurm-pip/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/examples/cylc-slurm-pip/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/lib/python/controller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/lib/python/dump_initial_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/examples/cylc-slurm-pip/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.312397 autora-workflow-0.3.4/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/src/autora/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/src/autora/workflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/serializer/yaml_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/src/autora/workflow/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/state/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/state/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/src/autora/workflow/state/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/src/autora_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-24 21:14:09.000000 autora-workflow-0.3.4/src/autora_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-24 21:14:09.000000 autora-workflow-0.3.4/src/autora_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:14:09.000000 autora-workflow-0.3.4/src/autora_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-24 21:14:09.000000 autora-workflow-0.3.4/src/autora_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 21:14:09.000000 autora-workflow-0.3.4/src/autora_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:14:09.320397 autora-workflow-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-24 21:13:58.000000 autora-workflow-0.3.4/tests/test_controller_plots.py
```

### Comparing `autora-workflow-0.3.3/.github/workflows/python-publish.yml` & `autora-workflow-0.3.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/.github/workflows/test-pytest.yml` & `autora-workflow-0.3.4/.github/workflows/test-pytest.yml`

 * *Files 21% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: "pip"
     - run: pip install ".[dev]"
-    - run: pytest --doctest-modules --ignore docs/cli/
+    - run: pytest --doctest-modules --ignore docs/cli/ --ignore examples/
```

### Comparing `autora-workflow-0.3.3/.gitignore` & `autora-workflow-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/.idea/autora-workflow.iml` & `autora-workflow-0.3.4/.idea/autora-workflow.iml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/.idea/inspectionProfiles/Project_Default.xml` & `autora-workflow-0.3.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/.idea/runConfigurations/pytest_in_tests.xml` & `autora-workflow-0.3.4/.idea/runConfigurations/pytest_in_tests.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/LICENSE.md` & `autora-workflow-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/PKG-INFO` & `autora-workflow-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.3.3
+Version: 0.3.4
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: cylc
 License-File: LICENSE.md
 
-# Workflow
+# AutoRA Workflow
 
 Workflow management tools for AutoRA.
 
 ## Quickstart Guide
 
 You will need:
```

### Comparing `autora-workflow-0.3.3/docs/cli/basic-usage/README.ipynb` & `autora-workflow-0.3.4/docs/cli/basic-usage/README.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990451388888889%*

 * *Differences: {"'cells'": "{1: {'execution_count': 3, 'outputs': {0: {'text': ['import numpy as np\\r\\n', 'from "*

 * *            "autora.experimentalist.pipeline import (\\r\\n', '    make_pipeline as "*

 * *            "make_experimentalist_pipeline,\\r\\n', ')\\r\\n', 'from autora.variable import "*

 * *            "Variable, VariableCollection\\r\\n', 'from sklearn.linear_model import "*

 * *            "LinearRegression\\r\\n', 'from sklearn.model_selection import GridSearchCV\\r\\n', "*

 * *            "'from sklearn.pipeline import make […]*

```diff
@@ -10,84 +10,84 @@
                 "\n",
                 "The command line interface requires us to save and load the state of a Controller from file.\n",
                 "To initialize it, we can define a file `lib.py` with the code for the experiment:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-05-04T21:18:24.377330Z",
-                    "start_time": "2023-05-04T21:18:23.946824Z"
+                    "end_time": "2023-05-24T20:25:32.788587Z",
+                    "start_time": "2023-05-24T20:25:32.643459Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[34mimport\u001b[39;49;00m \u001b[04m\u001b[36mnumpy\u001b[39;49;00m \u001b[34mas\u001b[39;49;00m \u001b[04m\u001b[36mnp\u001b[39;49;00m\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[34mfrom\u001b[39;49;00m \u001b[04m\u001b[36mautora\u001b[39;49;00m\u001b[04m\u001b[36m.\u001b[39;49;00m\u001b[04m\u001b[36mexperimentalist\u001b[39;49;00m\u001b[04m\u001b[36m.\u001b[39;49;00m\u001b[04m\u001b[36mpipeline\u001b[39;49;00m \u001b[34mimport\u001b[39;49;00m (\u001b[37m\u001b[39;49;00m\r\n",
-                        "    make_pipeline \u001b[34mas\u001b[39;49;00m make_experimentalist_pipeline,\u001b[37m\u001b[39;49;00m\r\n",
-                        ")\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[34mfrom\u001b[39;49;00m \u001b[04m\u001b[36mautora\u001b[39;49;00m\u001b[04m\u001b[36m.\u001b[39;49;00m\u001b[04m\u001b[36mvariable\u001b[39;49;00m \u001b[34mimport\u001b[39;49;00m Variable, VariableCollection\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[34mfrom\u001b[39;49;00m \u001b[04m\u001b[36msklearn\u001b[39;49;00m\u001b[04m\u001b[36m.\u001b[39;49;00m\u001b[04m\u001b[36mlinear_model\u001b[39;49;00m \u001b[34mimport\u001b[39;49;00m LinearRegression\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[34mfrom\u001b[39;49;00m \u001b[04m\u001b[36msklearn\u001b[39;49;00m\u001b[04m\u001b[36m.\u001b[39;49;00m\u001b[04m\u001b[36mmodel_selection\u001b[39;49;00m \u001b[34mimport\u001b[39;49;00m GridSearchCV\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[34mfrom\u001b[39;49;00m \u001b[04m\u001b[36msklearn\u001b[39;49;00m\u001b[04m\u001b[36m.\u001b[39;49;00m\u001b[04m\u001b[36mpipeline\u001b[39;49;00m \u001b[34mimport\u001b[39;49;00m make_pipeline \u001b[34mas\u001b[39;49;00m make_theorist_pipeline\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[34mfrom\u001b[39;49;00m \u001b[04m\u001b[36msklearn\u001b[39;49;00m\u001b[04m\u001b[36m.\u001b[39;49;00m\u001b[04m\u001b[36mpreprocessing\u001b[39;49;00m \u001b[34mimport\u001b[39;49;00m PolynomialFeatures\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[34mfrom\u001b[39;49;00m \u001b[04m\u001b[36mautora\u001b[39;49;00m\u001b[04m\u001b[36m.\u001b[39;49;00m\u001b[04m\u001b[36mworkflow\u001b[39;49;00m \u001b[34mimport\u001b[39;49;00m Controller\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[37m\u001b[39;49;00m\r\n",
-                        "rng = np.random.default_rng(\u001b[34m180\u001b[39;49;00m)\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[37m\u001b[39;49;00m\r\n",
-                        "experimentalist = make_experimentalist_pipeline(\u001b[37m\u001b[39;49;00m\r\n",
-                        "    [np.linspace, rng.choice],\u001b[37m\u001b[39;49;00m\r\n",
-                        "    params={\u001b[37m\u001b[39;49;00m\r\n",
-                        "        \u001b[33m\"\u001b[39;49;00m\u001b[33mlinspace\u001b[39;49;00m\u001b[33m\"\u001b[39;49;00m: {\u001b[33m\"\u001b[39;49;00m\u001b[33mstart\u001b[39;49;00m\u001b[33m\"\u001b[39;49;00m: [-\u001b[34m10\u001b[39;49;00m], \u001b[33m\"\u001b[39;49;00m\u001b[33mstop\u001b[39;49;00m\u001b[33m\"\u001b[39;49;00m: [+\u001b[34m10\u001b[39;49;00m], \u001b[33m\"\u001b[39;49;00m\u001b[33mnum\u001b[39;49;00m\u001b[33m\"\u001b[39;49;00m: \u001b[34m1001\u001b[39;49;00m},\u001b[37m\u001b[39;49;00m\r\n",
-                        "        \u001b[33m\"\u001b[39;49;00m\u001b[33mchoice\u001b[39;49;00m\u001b[33m\"\u001b[39;49;00m: {\u001b[33m\"\u001b[39;49;00m\u001b[33msize\u001b[39;49;00m\u001b[33m\"\u001b[39;49;00m: \u001b[34m10\u001b[39;49;00m},\u001b[37m\u001b[39;49;00m\r\n",
-                        "    },\u001b[37m\u001b[39;49;00m\r\n",
-                        ")\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[37m\u001b[39;49;00m\r\n",
-                        "coefs = [\u001b[34m2.0\u001b[39;49;00m, \u001b[34m3.0\u001b[39;49;00m, \u001b[34m1.0\u001b[39;49;00m]\u001b[37m\u001b[39;49;00m\r\n",
-                        "noise_std = \u001b[34m10.0\u001b[39;49;00m\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[34mdef\u001b[39;49;00m \u001b[32mexperiment_runner\u001b[39;49;00m(x, coefs_=coefs, noise_std_=noise_std, rng=rng):\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[37m    \u001b[39;49;00m\u001b[33m\"\"\"Simple experiment.\"\"\"\u001b[39;49;00m\u001b[37m\u001b[39;49;00m\r\n",
-                        "    x_ = np.array(x)  \u001b[37m# assume we've got an array already\u001b[39;49;00m\u001b[37m\u001b[39;49;00m\r\n",
-                        "    y_ = (\u001b[37m\u001b[39;49;00m\r\n",
-                        "        coefs_[\u001b[34m0\u001b[39;49;00m] * x_**\u001b[34m2.0\u001b[39;49;00m\u001b[37m\u001b[39;49;00m\r\n",
-                        "        + coefs_[\u001b[34m1\u001b[39;49;00m] * x_\u001b[37m\u001b[39;49;00m\r\n",
-                        "        + coefs_[\u001b[34m2\u001b[39;49;00m]\u001b[37m\u001b[39;49;00m\r\n",
-                        "        + rng.normal(\u001b[34m0.0\u001b[39;49;00m, noise_std_, size=x_.shape)\u001b[37m\u001b[39;49;00m\r\n",
-                        "    )\u001b[37m\u001b[39;49;00m\r\n",
-                        "    \u001b[34mreturn\u001b[39;49;00m y_\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[37m\u001b[39;49;00m\r\n",
-                        "theorist = GridSearchCV(\u001b[37m\u001b[39;49;00m\r\n",
-                        "    make_theorist_pipeline(PolynomialFeatures(), LinearRegression()),\u001b[37m\u001b[39;49;00m\r\n",
-                        "    param_grid={\u001b[33m\"\u001b[39;49;00m\u001b[33mpolynomialfeatures__degree\u001b[39;49;00m\u001b[33m\"\u001b[39;49;00m: [\u001b[34m0\u001b[39;49;00m, \u001b[34m1\u001b[39;49;00m, \u001b[34m2\u001b[39;49;00m, \u001b[34m3\u001b[39;49;00m, \u001b[34m4\u001b[39;49;00m]},\u001b[37m\u001b[39;49;00m\r\n",
-                        "    scoring=\u001b[33m\"\u001b[39;49;00m\u001b[33mr2\u001b[39;49;00m\u001b[33m\"\u001b[39;49;00m,\u001b[37m\u001b[39;49;00m\r\n",
-                        ")\u001b[37m\u001b[39;49;00m\r\n",
-                        "\u001b[37m\u001b[39;49;00m\r\n",
-                        "controller = Controller(\u001b[37m\u001b[39;49;00m\r\n",
-                        "    variables=VariableCollection(\u001b[37m\u001b[39;49;00m\r\n",
-                        "        independent_variables=[Variable(\u001b[33m\"\u001b[39;49;00m\u001b[33mx\u001b[39;49;00m\u001b[33m\"\u001b[39;49;00m)], dependent_variables=[Variable(\u001b[33m\"\u001b[39;49;00m\u001b[33my\u001b[39;49;00m\u001b[33m\"\u001b[39;49;00m)]\u001b[37m\u001b[39;49;00m\r\n",
-                        "    ),\u001b[37m\u001b[39;49;00m\r\n",
-                        "    experiment_runner=experiment_runner,\u001b[37m\u001b[39;49;00m\r\n",
-                        "    experimentalist=experimentalist,\u001b[37m\u001b[39;49;00m\r\n",
-                        "    theorist=theorist,\u001b[37m\u001b[39;49;00m\r\n",
-                        ")\u001b[37m\u001b[39;49;00m\r\n"
+                        "import numpy as np\r\n",
+                        "from autora.experimentalist.pipeline import (\r\n",
+                        "    make_pipeline as make_experimentalist_pipeline,\r\n",
+                        ")\r\n",
+                        "from autora.variable import Variable, VariableCollection\r\n",
+                        "from sklearn.linear_model import LinearRegression\r\n",
+                        "from sklearn.model_selection import GridSearchCV\r\n",
+                        "from sklearn.pipeline import make_pipeline as make_theorist_pipeline\r\n",
+                        "from sklearn.preprocessing import PolynomialFeatures\r\n",
+                        "\r\n",
+                        "from autora.workflow import Controller\r\n",
+                        "\r\n",
+                        "rng = np.random.default_rng(180)\r\n",
+                        "\r\n",
+                        "experimentalist = make_experimentalist_pipeline(\r\n",
+                        "    [np.linspace, rng.choice],\r\n",
+                        "    params={\r\n",
+                        "        \"linspace\": {\"start\": [-10], \"stop\": [+10], \"num\": 1001},\r\n",
+                        "        \"choice\": {\"size\": 10},\r\n",
+                        "    },\r\n",
+                        ")\r\n",
+                        "\r\n",
+                        "coefs = [2.0, 3.0, 1.0]\r\n",
+                        "noise_std = 10.0\r\n",
+                        "\r\n",
+                        "\r\n",
+                        "def experiment_runner(x, coefs_=coefs, noise_std_=noise_std, rng=rng):\r\n",
+                        "    \"\"\"Simple experiment.\"\"\"\r\n",
+                        "    x_ = np.array(x)  # assume we've got an array already\r\n",
+                        "    y_ = (\r\n",
+                        "        coefs_[0] * x_**2.0\r\n",
+                        "        + coefs_[1] * x_\r\n",
+                        "        + coefs_[2]\r\n",
+                        "        + rng.normal(0.0, noise_std_, size=x_.shape)\r\n",
+                        "    )\r\n",
+                        "    return y_\r\n",
+                        "\r\n",
+                        "\r\n",
+                        "theorist = GridSearchCV(\r\n",
+                        "    make_theorist_pipeline(PolynomialFeatures(), LinearRegression()),\r\n",
+                        "    param_grid={\"polynomialfeatures__degree\": [0, 1, 2, 3, 4]},\r\n",
+                        "    scoring=\"r2\",\r\n",
+                        ")\r\n",
+                        "\r\n",
+                        "controller = Controller(\r\n",
+                        "    variables=VariableCollection(\r\n",
+                        "        independent_variables=[Variable(\"x\")], dependent_variables=[Variable(\"y\")]\r\n",
+                        "    ),\r\n",
+                        "    experiment_runner=experiment_runner,\r\n",
+                        "    experimentalist=experimentalist,\r\n",
+                        "    theorist=theorist,\r\n",
+                        ")\r\n"
                     ]
                 }
             ],
             "source": [
-                "!pygmentize lib.py"
+                "!pygmentize lib.py  # display the lib.py file"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
```

### Comparing `autora-workflow-0.3.3/docs/cli/basic-usage/lib.py` & `autora-workflow-0.3.4/docs/cli/basic-usage/lib.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/docs/cli/with-cylc-conda/README.md` & `autora-workflow-0.3.4/examples/cylc-conda/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-# Usage with Cylc workflow manager and conda
+# Using the Cylc workflow manager and conda
 
 The command line interface can be used with workflow managers like cylc and conda environments.
 
 ## Prerequisites
 
-This example requires a conda environment called `autora-cylc` with the following dependencies:
+This example requires:
 
-- `autora` 3+
-- `cylc-flow`
-
-The conda environment will be cloned during the setup phase of the `cylc` workflow run.
-
-You can initialize the conda environment using the included environment.yml file.
-```shell
-conda env create -f environment.yml
-```
-
-## Workflow
-
-To initialize the workflow, we again define a file with the code for the experiment, this time in the
-`lib/python` directory [(a cylc convention)](https://cylc.github.io/cylc-doc/stable/html/user-guide/writing-workflows/configuration.html#workflow-configuration-directories):
-
-```python title="lib/python/controller_setup.py"
---8<-- "docs/cli/with-cylc-conda/lib/python/controller_setup.py"
-```
+- familiarity with and a working installation of `cylc` (e.g. by going through the
+  [tutorial](https://cylc.github.io/cylc-doc/latest/html/tutorial/index.html))
+- a conda environment called `autora-cylc` with the following dependencies:
+  - `autora` 3+
+  - `cylc-flow`
+  
+  The conda environment will be cloned during the setup phase of the `cylc` workflow run.
+    You can initialize the conda environment using the included environment.yml file.
+    ```shell
+    conda env create -f environment.yml
+    ```
+
+## Setup
+
+To initialize the workflow, we define a file in the`lib/python` directory 
+[(a cylc convention)](https://cylc.github.io/cylc-doc/stable/html/user-guide/writing-workflows/configuration.html#workflow-configuration-directories) with the code for the experiment: 
+[`lib/python/controller_setup.py`](./lib/python/controller_setup.py)
 
 The first step in the workflow will be to:
 - load the controller from the file
 - save its state to a `.dill` file in the share directory.
 
-```python title="lib/python/dump_initial_controller.py"
---8<-- "docs/cli/with-cylc-conda/lib/python/dump_initial_controller.py"
-```
+This is done with the file [`lib/python/dump_initial_controller.py`](./lib/python/dump_initial_controller.py).
 
-The `flow.cylc` file defines the workflow:
-```  title="flow.cylc"
---8<-- "docs/cli/with-cylc-conda/flow.cylc"
-```
+The [`flow.cylc`](./flow.cylc) file defines the workflow.
+
+## Execution
 
 We can call the `cylc` command line interface as follows, in a shell session:
 
 First, we validate the `flow.cylc` file:
 ```shell
 cylc validate .
 ```
@@ -63,15 +59,17 @@
 ```
 
 ... or the text user interface (TUI):
 ```shell
 cylc tui "with-cylc-conda"
 ```
 
-We can load and interrogate the resulting object as follows:
+## Results
+
+We can load and interrogate the resulting object in a python session as follows:
 
 ```python
 import os
 import dill
 import numpy as np
 from matplotlib import pyplot as plt
```

### Comparing `autora-workflow-0.3.3/docs/cli/with-cylc-conda/flow.cylc` & `autora-workflow-0.3.4/examples/cylc-conda/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/docs/cli/with-cylc-conda/lib/python/controller_setup.py` & `autora-workflow-0.3.4/examples/cylc-conda/lib/python/controller_setup.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/docs/cli/with-cylc-pip/README.md` & `autora-workflow-0.3.4/examples/cylc-pip/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,44 +2,36 @@
 
 The command line interface can be used with workflow managers like cylc in virtualenv environments.
 
 ## Prerequisites
 
 This example requires:
 
-- `cylc`
+- familiarity with and a working installation of `cylc` (e.g. by going through the
+  [tutorial](https://cylc.github.io/cylc-doc/latest/html/tutorial/index.html))
 - `virtualenv`
 - `python3.10` (so you can run `virtualenv venv -p python3.10`)
 
 A new environment will be created during the setup phase of the `cylc` workflow run.
 
-## Workflow
+## Setup
 
-To initialize the workflow, we define a file with the code for the experiment, this time in the
-`lib/python` directory [(a cylc convention)](https://cylc.github.io/cylc-doc/stable/html/user-guide/writing-workflows/configuration.html#workflow-configuration-directories):
-
-```python title="lib/python/controller_setup.py"
---8<-- "docs/cli/with-cylc-pip/lib/python/controller_setup.py"
-```
+To initialize the workflow, we define a file in the`lib/python` directory 
+[(a cylc convention)](https://cylc.github.io/cylc-doc/stable/html/user-guide/writing-workflows/configuration.html#workflow-configuration-directories) with the code for the experiment: 
+[`lib/python/controller_setup.py`](./lib/python/controller_setup.py)
 
 The first step in the workflow will be to:
-
 - load the controller from the file
 - save its state to a `.dill` file in the share directory.
 
-This is handled by the initialization.py file:
+This is done with the file [`lib/python/dump_initial_controller.py`](./lib/python/dump_initial_controller.py).
 
-```python title="lib/python/dump_initial_controller.py"
---8<-- "docs/cli/with-cylc-pip/lib/python/dump_initial_controller.py"
-```
+The [`flow.cylc`](./flow.cylc) file defines the workflow.
 
-The `flow.cylc` file defines the workflow:
-```  title="flow.cylc"
---8<-- "docs/cli/with-cylc-pip/flow.cylc"
-```
+## Execution
 
 We can call the `cylc` command line interface as follows, in a shell session:
 
 First, we validate the `flow.cylc` file:
 ```shell
 cylc validate .
 ```
@@ -62,14 +54,16 @@
 ```
 
 ... or the text user interface (TUI):
 ```shell
 cylc tui "with-cylc-pip"
 ```
 
+## Results
+
 We can load and interrogate the resulting object as follows:
 
 ```python
 import os
 import dill
 import numpy as np
 from matplotlib import pyplot as plt
```

### Comparing `autora-workflow-0.3.3/docs/cli/with-cylc-pip/flow.cylc` & `autora-workflow-0.3.4/examples/cylc-pip/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/docs/cli/with-cylc-pip/lib/python/controller_setup.py` & `autora-workflow-0.3.4/examples/cylc-pip/lib/python/controller_setup.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/docs/cli/with-cylc-slurm/README.md` & `autora-workflow-0.3.4/examples/cylc-slurm-pip/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -3,51 +3,40 @@
 The command line interface can be used with cylc in environments which use a scheduler like slurm.
 
 ## Prerequisites
 
 This example requires:
 
 - `slurm`, e.g. on a high performance computing cluster.
-- `cylc`
+- familiarity with and a working installation of `cylc` (e.g. by going through the
+  [tutorial](https://cylc.github.io/cylc-doc/latest/html/tutorial/index.html))
 - `virtualenv`
 - `python` (so you can run `virtualenv venv -p python`)
 
 A new environment will be created during the setup phase of the `cylc` workflow run.
 
 Cylc requires a site-specific setup when using a scheduler like slurm. See the cylc documentation for a guide on setting up cylc on your platform.
-For Oscar at Brown University, we can use the following global configuration:
+For Oscar at Brown University, we can use the following configuration in 
+[`./global.cylc`](./global.cylc)
 
-```python title="global.cylc"
---8<-- "docs/cli/with-cylc-slurm/global.cylc"
-```
-
-## Workflow
+## Setup
 
-To initialize the workflow, we define a file with the code for the experiment, in the
-`lib/python` directory [(a cylc convention)](https://cylc.github.io/cylc-doc/stable/html/user-guide/writing-workflows/configuration.html#workflow-configuration-directories):
-
-```python title="lib/python/controller_setup.py"
---8<-- "docs/cli/with-cylc-slurm/lib/python/controller_setup.py"
-```
+To initialize the workflow, we define a file in the`lib/python` directory 
+[(a cylc convention)](https://cylc.github.io/cylc-doc/stable/html/user-guide/writing-workflows/configuration.html#workflow-configuration-directories) with the code for the experiment: 
+[`lib/python/controller_setup.py`](./lib/python/controller_setup.py)
 
 The first step in the workflow will be to:
-
 - load the controller from the file
 - save its state to a `.dill` file in the share directory.
 
-This is handled by the initialization.py file:
+This is done with the file [`lib/python/dump_initial_controller.py`](./lib/python/dump_initial_controller.py).
 
-```python title="lib/python/dump_initial_controller.py"
---8<-- "docs/cli/with-cylc-slurm/lib/python/dump_initial_controller.py"
-```
+The [`flow.cylc`](./flow.cylc) file defines the workflow.
 
-The `flow.cylc` file defines the workflow, including special directives to use "Oscar" specific settings for the runtime:
-```  title="flow.cylc"
---8<-- "docs/cli/with-cylc-slurm/flow.cylc"
-```
+## Execution
 
 We can call the `cylc` command line interface as follows, in a shell session:
 
 First, we validate the `flow.cylc` file:
 ```shell
 cylc validate .
 ```
@@ -70,14 +59,16 @@
 ```
 
 ... or the text user interface (TUI):
 ```shell
 cylc tui "with-cylc-slurm"
 ```
 
+## Results
+
 We can load and interrogate the resulting object in Python as follows:
 
 ```python
 import os
 import dill
 import numpy as np
 from matplotlib import pyplot as plt
```

### Comparing `autora-workflow-0.3.3/docs/cli/with-cylc-slurm/flow.cylc` & `autora-workflow-0.3.4/examples/cylc-slurm-pip/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/docs/cli/with-cylc-slurm/lib/python/controller_setup.py` & `autora-workflow-0.3.4/examples/cylc-slurm-pip/lib/python/controller_setup.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/docs/interactive/basic-usage.ipynb` & `autora-workflow-0.3.4/docs/interactive/basic-usage.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9711298500881834%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}}, 1: {'execution_count': None, 'metadata': "*

 * *            "{replace: OrderedDict()}}, 2: {'execution_count': None, 'metadata': {replace: "*

 * *            "OrderedDict()}}, 3: {'metadata': {replace: OrderedDict()}}, 4: {'execution_count': "*

 * *            "None, 'source': {insert: [(0, 'variables_0 = VariableCollection(\\n')], delete: [0]}, "*

 * *            "'metadata': {replace: OrderedDict()}}, 5: {'metadata': {replace: OrderedDict()}}, 6: "*

 * *            "{'execu […]*

```diff
@@ -1,135 +1,99 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "# Basic Usage\n",
                 "\n",
                 "Aim: Use the Controller to recover a simple ground truth model from noisy data."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.593823Z",
-                    "start_time": "2023-04-28T16:00:28.742319Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from autora.experimentalist.pipeline import make_pipeline\n",
                 "from autora.variable import VariableCollection, Variable\n",
                 "from sklearn.linear_model import LinearRegression\n",
                 "\n",
                 "from autora.workflow import Cycle\n",
                 "from itertools import takewhile"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.595804Z",
-                    "start_time": "2023-04-28T16:00:29.594123Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "def ground_truth(x):\n",
                 "    return x + 1"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The space of allowed x values is the integers between 0 and 10 inclusive, and we record the allowed output values as well."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.599669Z",
-                    "start_time": "2023-04-28T16:00:29.596722Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
-                "metadata_0 = VariableCollection(\n",
+                "variables_0 = VariableCollection(\n",
                 "   independent_variables=[Variable(name=\"x1\", allowed_values=range(11))],\n",
                 "   dependent_variables=[Variable(name=\"y\", value_range=(-20, 20))],\n",
                 "   )"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The experimentalist is used to propose experiments.\n",
                 "Since the space of values is so restricted, we can just sample them all each time."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.602835Z",
-                    "start_time": "2023-04-28T16:00:29.600797Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "example_experimentalist = make_pipeline(\n",
-                "    [metadata_0.independent_variables[0].allowed_values])"
+                "    [variables_0.independent_variables[0].allowed_values])"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "When we run a synthetic experiment, we get a reproducible noisy result:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.607989Z",
-                    "start_time": "2023-04-28T16:00:29.605654Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "array([2.04339546])"
+                        "text/plain": [
+                            "array([2.04339546])"
+                        ]
                     },
-                    "execution_count": 5,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "def get_example_synthetic_experiment_runner():\n",
                 "    rng = np.random.default_rng(seed=180)\n",
@@ -138,97 +102,75 @@
                 "    return runner\n",
                 "example_synthetic_experiment_runner = get_example_synthetic_experiment_runner()\n",
                 "example_synthetic_experiment_runner(np.array([1]))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The theorist \"tries\" to work out the best model. We use a trivial scikit-learn regressor."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.610805Z",
-                    "start_time": "2023-04-28T16:00:29.608494Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "example_theorist = LinearRegression()"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
-                "    We initialize the Controller with the metadata describing the domain of the model,\n",
+                "    We initialize the Controller with the variables describing the domain of the model,\n",
                 "    the theorist, experimentalist and experiment runner,\n",
                 "    as well as a monitor which will let us know which cycle we're currently on."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.620255Z",
-                    "start_time": "2023-04-28T16:00:29.615491Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "<autora.workflow.cycle.Cycle at 0x14d254910>"
+                        "text/plain": [
+                            "<autora.workflow.cycle.Cycle at 0x157959660>"
+                        ]
                     },
-                    "execution_count": 7,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "cycle = Cycle(\n",
-                "    metadata=metadata_0,\n",
+                "    variables=variables_0,\n",
                 "    theorist=example_theorist,\n",
                 "    experimentalist=example_experimentalist,\n",
                 "    experiment_runner=example_synthetic_experiment_runner,\n",
                 "    monitor=lambda state: print(f\"Generated {len(state.models)} models\"),\n",
                 ")\n",
                 "cycle # doctest: +ELLIPSIS"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "We can run the cycle by calling the run method:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.625412Z",
-                    "start_time": "2023-04-28T16:00:29.618752Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Generated 1 models\n",
                         "Generated 2 models\n",
@@ -238,227 +180,198 @@
             ],
             "source": [
                 "_ = cycle.run(num_cycles=3)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "We can now interrogate the results. The first set of conditions which went into the\n",
                 "experiment runner were:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.627948Z",
-                    "start_time": "2023-04-28T16:00:29.624167Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "array([ 0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10])"
+                        "text/plain": [
+                            "array([ 0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10])"
+                        ]
                     },
-                    "execution_count": 9,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "cycle.data.conditions[0]"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The observations include the conditions and the results:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.631975Z",
-                    "start_time": "2023-04-28T16:00:29.629640Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "array([[ 0.        ,  0.92675345],\n       [ 1.        ,  1.89519928],\n       [ 2.        ,  3.08746571],\n       [ 3.        ,  3.93023943],\n       [ 4.        ,  4.95429102],\n       [ 5.        ,  6.04763988],\n       [ 6.        ,  7.20770574],\n       [ 7.        ,  7.85681519],\n       [ 8.        ,  9.05735823],\n       [ 9.        , 10.18713406],\n       [10.        , 10.88517906]])"
+                        "text/plain": [
+                            "array([[ 0.        ,  0.92675345],\n",
+                            "       [ 1.        ,  1.89519928],\n",
+                            "       [ 2.        ,  3.08746571],\n",
+                            "       [ 3.        ,  3.93023943],\n",
+                            "       [ 4.        ,  4.95429102],\n",
+                            "       [ 5.        ,  6.04763988],\n",
+                            "       [ 6.        ,  7.20770574],\n",
+                            "       [ 7.        ,  7.85681519],\n",
+                            "       [ 8.        ,  9.05735823],\n",
+                            "       [ 9.        , 10.18713406],\n",
+                            "       [10.        , 10.88517906]])"
+                        ]
                     },
-                    "execution_count": 10,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "cycle.data.observations[0]"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "In the third cycle (index = 2) the first and last values are different again:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.635291Z",
-                    "start_time": "2023-04-28T16:00:29.633048Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "array([[ 0.        ,  1.08559827],\n       [10.        , 11.08179553]])"
+                        "text/plain": [
+                            "array([[ 0.        ,  1.08559827],\n",
+                            "       [10.        , 11.08179553]])"
+                        ]
                     },
-                    "execution_count": 11,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "cycle.data.observations[2][[0,-1]]"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The best fit model after the first cycle is:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.638810Z",
-                    "start_time": "2023-04-28T16:00:29.636568Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/html": "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>LinearRegression()</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">LinearRegression</label><div class=\"sk-toggleable__content\"><pre>LinearRegression()</pre></div></div></div></div></div>",
-                        "text/plain": "LinearRegression()"
+                        "text/html": [
+                            "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>LinearRegression()</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">LinearRegression</label><div class=\"sk-toggleable__content\"><pre>LinearRegression()</pre></div></div></div></div></div>"
+                        ],
+                        "text/plain": [
+                            "LinearRegression()"
+                        ]
                     },
-                    "execution_count": 12,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "cycle.data.models[0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.651434Z",
-                    "start_time": "2023-04-28T16:00:29.640123Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "'y = 1.0089 x + 0.9589'"
+                        "text/plain": [
+                            "'y = 1.0089 x + 0.9589'"
+                        ]
                     },
-                    "execution_count": 13,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "def report_linear_fit(m: LinearRegression,  precision=4):\n",
                 "    s = f\"y = {np.round(m.coef_[0].item(), precision)} x \" \\\n",
                 "        f\"+ {np.round(m.intercept_.item(), 4)}\"\n",
                 "    return s\n",
                 "report_linear_fit(cycle.data.models[0])"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The best fit model after all the cycles, including all the data, is:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.651704Z",
-                    "start_time": "2023-04-28T16:00:29.642827Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "'y = 0.9989 x + 1.0292'"
+                        "text/plain": [
+                            "'y = 0.9989 x + 1.0292'"
+                        ]
                     },
-                    "execution_count": 14,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "report_linear_fit(cycle.data.models[-1])"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "This is close to the ground truth model of x -> (x + 1)\n",
                 "We can also run the cycle with more control over the execution flow:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.651855Z",
-                    "start_time": "2023-04-28T16:00:29.644832Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Generated 4 models\n"
                     ]
@@ -466,22 +379,16 @@
             ],
             "source": [
                 "_ = next(cycle)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.651938Z",
-                    "start_time": "2023-04-28T16:00:29.648413Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Generated 5 models\n"
                     ]
@@ -489,22 +396,16 @@
             ],
             "source": [
                 "_ = next(cycle)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.657114Z",
-                    "start_time": "2023-04-28T16:00:29.652804Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Generated 6 models\n"
                     ]
@@ -512,32 +413,24 @@
             ],
             "source": [
                 "_ = next(cycle)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "We can continue to run the cycle as long as we like,\n",
                 "with a simple arbitrary stopping condition like the number of models generated:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.661188Z",
-                    "start_time": "2023-04-28T16:00:29.658078Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Generated 7 models\n",
                         "Generated 8 models\n",
@@ -547,31 +440,23 @@
             ],
             "source": [
                 "_ = list(takewhile(lambda c: len(c.data.models) < 9, cycle))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "... or the precision (here we keep iterating while the difference between the gradients of the second-last and last cycle is larger than 0.001)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.666266Z",
-                    "start_time": "2023-04-28T16:00:29.663336Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Generated 10 models\n",
                         "Generated 11 models\n"
@@ -586,31 +471,23 @@
                 "            cycle\n",
                 "        )\n",
                 "    )\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "... or continue to run as long as we like:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:00:29.711974Z",
-                    "start_time": "2023-04-28T16:00:29.667061Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Generated 12 models\n",
                         "Generated 13 models\n",
@@ -731,14 +608,13 @@
                 "name": "ipython",
                 "version": 2
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython2",
-            "version": "2.7.6"
+            "pygments_lexer": "ipython2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 0
 }
```

### Comparing `autora-workflow-0.3.3/docs/interactive/saving-and-loading-dill.ipynb` & `autora-workflow-0.3.4/docs/interactive/saving-and-loading-dill.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9714732142857143%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}}, 1: {'execution_count': None, 'metadata': "*

 * *            "{replace: OrderedDict()}}, 2: {'metadata': {replace: OrderedDict()}}, 3: "*

 * *            "{'execution_count': None, 'outputs': {0: {'data': {'text/plain': "*

 * *            "['<autora.workflow.controller.Controller at 0x107361420>']}, 'execution_count': "*

 * *            "None}}, 'metadata': {replace: OrderedDict()}}, 4: {'metadata': {replace: "*

 * *            "OrderedDict()}}, 5: {'execution_count': None, 'm […]*

```diff
@@ -1,70 +1,56 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "# Saving and loading controllers using dill\n",
                 "\n",
                 "## Basic usage\n",
                 "\n",
                 "Workflow managers can be saved to and loaded using [dill](https://github.com/uqfoundation/dill).\n",
                 "\n",
                 "For instance, you could generate a basic Controller object in an interactive python session as follows:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-05-04T12:24:43.498320Z",
-                    "start_time": "2023-05-04T12:24:43.494965Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import autora.workflow\n",
                 "import dill\n",
                 "\n",
                 "controller = autora.workflow.Controller()\n",
                 "\n",
                 "with open(\"default-controller.dill\", \"wb\") as file:\n",
                 "    dill.dump(controller, file)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The same Controller state can be loaded in a separate session as follows:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 68,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-05-04T12:48:52.708474Z",
-                    "start_time": "2023-05-04T12:48:52.704595Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "<autora.workflow.controller.Controller at 0x29fd1e010>"
+                        "text/plain": [
+                            "<autora.workflow.controller.Controller at 0x107361420>"
+                        ]
                     },
-                    "execution_count": 68,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import dill\n",
                 "\n",
@@ -72,38 +58,30 @@
                 "    reloaded_controller = dill.load(file)\n",
                 "\n",
                 "reloaded_controller"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## Executors\n",
                 "\n",
                 "A Controller for real use always includes at least one (and usually more than one) Executor.\n",
                 "\n",
                 "In this example, the Controller includes:\n",
                 "- an experimentalist, which suggests a random sample across a particular problem domain,\n",
                 "- an experiment runner, which makes synthetic observations of a polynomial function,\n",
                 "- and a theorist, which is a scikit-learn regressor."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 69,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-05-04T12:48:55.092067Z",
-                    "start_time": "2023-05-04T12:48:55.075258Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from sklearn.model_selection import GridSearchCV\n",
                 "from sklearn.pipeline import make_pipeline as make_theorist_pipeline\n",
                 "from sklearn.preprocessing import PolynomialFeatures\n",
                 "from sklearn.linear_model import LinearRegression\n",
@@ -144,31 +122,23 @@
                 "\n",
                 "with open(\"simple-controller.dill\", \"wb\") as file:\n",
                 "    dill.dump(controller, file)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "Later, we can reload the same Controller and run the cycle:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 70,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-05-04T12:48:56.699666Z",
-                    "start_time": "2023-05-04T12:48:55.776597Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "new_conditions=array([[-5.22],\n",
                         "       [ 1.52],\n",
@@ -510,75 +480,71 @@
                         "       [ 9.4 ],\n",
                         "       [ 0.2 ],\n",
                         "       [ 5.68]]) is an ndarray, so variable confusion is a possibility\n"
                     ]
                 },
                 {
                     "data": {
-                        "text/plain": "<autora.workflow.controller.Controller at 0x29f88f7d0>"
+                        "text/plain": [
+                            "<autora.workflow.controller.Controller at 0x148bf8790>"
+                        ]
                     },
-                    "execution_count": 70,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "with open(\"simple-controller.dill\", \"rb\") as file:\n",
                 "    controller_loaded = dill.load(file)\n",
                 "\n",
                 "controller_loaded.run(num_steps=100)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 71,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-05-04T12:48:59.515261Z",
-                    "start_time": "2023-05-04T12:48:59.511247Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "{'polynomialfeatures__degree': 3}"
+                        "text/plain": [
+                            "{'polynomialfeatures__degree': 3}"
+                        ]
                     },
-                    "execution_count": 71,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "controller_loaded.state.models[-1].best_params_"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 72,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-05-04T12:49:00.139466Z",
-                    "start_time": "2023-05-04T12:48:59.998120Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "<matplotlib.legend.Legend at 0x29efe2290>"
+                        "text/plain": [
+                            "<matplotlib.legend.Legend at 0x298b1c400>"
+                        ]
                     },
-                    "execution_count": 72,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
                         "image/png": "iVBORw0KGgoAAAANSUhEUgAAAigAAAGdCAYAAAA44ojeAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAABy4ElEQVR4nO3deXhTZdoG8Dt7uiVpkrZpSwstWxEBERURHRdQQERRRwUZFQfBBVxxVGYUXAcXFPdl3NBxxwUUBUcRQdkElBFkh+57mzZp2uw53x+d9qNwzmkLTZu09++6eil53nP6puny5F2eVyEIggAiIiKiCKLs6g4QERERHYkJChEREUUcJihEREQUcZigEBERUcRhgkJEREQRhwkKERERRRwmKERERBRxmKAQERFRxFF3dQeORSgUQklJCRISEqBQKLq6O0RERNQGgiCgrq4OaWlpUCrlx0iiMkEpKSlBRkZGV3eDiIiIjkFhYSF69eol2yYqE5SEhAQAjU/QYDB0cW+IiIioLZxOJzIyMpr/jsuJygSlaVrHYDAwQSEiIooybVmewUWyREREFHGYoBAREVHEYYJCREREEScq16C0hSAICAQCCAaDXd0VijAqlQpqtZpb1ImIIli3TFB8Ph9KS0vR0NDQ1V2hCBUbG4vU1FRotdqu7goRUZdraGiAXq9vtTZJZ+p2CUooFEJubi5UKhXS0tKg1Wr5TpmaCYIAn8+HyspK5Obmon///hH1A0lE1NkEQcCBAwcQCoWQmJgIs9ncpm3A4dbtEhSfz4dQKISMjAzExsZ2dXcoAsXExECj0SA/Px8+nw96vb6ru0RE1GWcTif8fj8AoKqqClVVVdBqtTCbzbBYLF32O7LbJShN+K6Y5PD7g4iokd1uP+oxn8+HsrIylJWVITY2FhaLBWazGWp156UN3S5B2bFjBwoLC+F0OqHT6bq6O0dRKpUYOnRoV3eDiIgIwWAQtbW1sm0aGhrQ0NCAoqIiGAwGWCwWGI3GsL/R63YJSigUQigUQjAY5A6eMFuyZAnuuOOOVr+5w2369Omora3FsmXLurQfRETRpra2FqFQqE1tBUGAw+GAw+GASqVC3759w7pWhePcFDZ5eXlQKBTYvn17RN6PiKinq66uPqbrQqEQYmJiOrg3LTFBiWI+n6+ru9AhusvzICKKJj6fD3V1dcd0rdFoDPt6FCYoEaKurg7Tpk1DXFwcUlNTsXjxYpxzzjm44447mtv06dMHjzzyCK699loYDAbMmjULAPDZZ59h8ODB0Ol06NOnD55++ukW91YoFEdNf5hMJixZsgTA/49MfP755zj33HMRGxuLYcOGYePGjS2uWbJkCTIzMxEbG4tLL7201cw7KysLADB8+HAoFAqcc845ABqnZCZPnozHHnsMaWlpGDhwYJv6KXW/JosWLUJqaiosFgtmz57dvCqdiIiOJrY4FgAgCIjfuhUIBCSvtVgsYerV/2OCEiHuuusurF+/Hl9++SW+++47/PTTT/j111+Pardo0SIMGzYMv/32Gx544AFs27YNV155JaZMmYIdO3bgwQcfxAMPPND8R709/vGPf+Duu+/G9u3bMWDAAEydOhWB/32Dbt68GTNmzMCcOXOwfft2nHvuuXj00Udl7/fLL78AAL7//nuUlpbi888/b46tXr0ae/fuxXfffYcVK1a0qX9y91uzZg0OHjyINWvW4J133sGSJUuO6WtARNRTSL3JjN2zBwNvugmGLVtE42q1GkajMZxda/w8Yf8M1Kq6ujq88847+OCDDzBmzBgAwNtvv420tLSj2p533nmYO3du87+nTZuGMWPG4IEHHgAADBgwALt27cJTTz2F6dOnt6sfd999NyZOnAgAeOihhzB48GAcOHAAOTk5eO655zB+/Hjcc889zZ9nw4YNWLVqleT9kpKSADRm2jabrUUsLi4Ob7zxRrsqucrdLzExES+++CJUKhVycnIwceJErF69GjNnzmzz/YmIeoqGhgZ4PB7RmPmbb+C3WOA89VTReGJiYqcUQOUISgQ4dOgQ/H4/TjvttObHjEZj89TH4U455ZQW/969ezdGjx7d4rHRo0dj//797d7FdPj259TUVABARUVF8+cZOXJki/ajRo1q1/0PN2TIkA4tMz948GCoVKrmf6empjb3nYiIWpKcog8EYF61CvZx4wCJNSadMb0DMEGJOnFxce2+RqFQQBCEFo+Jrc/QaDQtrgHQ5u1n7SX2PNraTzGH973pXuHqOxFRNBMEQXL9iWHTJmhqalB94YWicZ1Od0x/h44FE5QIkJ2dDY1Ggy2Hzfc5HA7s27ev1WsHDRqE9evXt3hs/fr1GDBgQPOIQlJSEkpLS5vj+/fvb/dBioMGDcLmzZtbPLZp0ybZa5pGSNo6ktNaP9t7PyIiOprT6WxeX3gky9dfw923L9wiI/hA542eAFyDEhESEhJw3XXX4W9/+xvMZjOSk5OxYMECKJXKVuf55s6di1NPPRWPPPIIrrrqKmzcuBEvvvgiXn755eY25513Hl588UWMGjUKwWAQ995771EjDq257bbbMHr0aCxatAiXXHIJvv32W9n1JwCQnJyMmJgYrFq1Cr169YJer5ddWNVaP9t7PyIiOprU6InS5YJp3TqUzJoFSPztMZvN4exay/502mciWc888wxGjRqFiy66CGPHjsXo0aMxaNCgVg9pOvnkk/HJJ5/go48+woknnoj58+fj4YcfbrFA9umnn0ZGRgbOOussXH311bj77rvbfZDi6aefjtdffx3PPfcchg0bhv/85z+4//77Za9Rq9V4/vnn8dprryEtLQ2XXHKJbPvW+tne+xERUUtype0TV6+GwueDffx40Xh8fHynHiGjEI6c9I8CTqcTRqMRDocDBoOhRWzz5s0oLCxEWlpaRJ7Fo1KpcNJJJ7Xarr6+Hunp6Xj66acxY8aM8Hesh/F4PMjNzUVWVhZPMyaiHqOqqgr5+fmisQGzZkFQq7H/sBH4w2VmZjbvpjxWcn+/j9TtpniUSiWUSiVUKlWLXR2RQupwpd9++w179uzBaaedBofDgYcffhgAOEpAREQdRmp6R1taioRff0Xugw+KxhUKRadO7wDdMEEZMmQI4uPjo/Kd8aJFi7B3715otVqMGDECP/30E6xWa1d3i4iIugG50vbmlSsR0ulQe+65onGj0djpb/q7XYISrYYPH45t27Z1dTeIiKibkittb/7mG9Scdx5CEluIO3P3ThMukiUiIuoBJEvb796NmLw82CVqn3RWafsjMUEhIiLq5urr6yVL21u+/joiStsfiQkKERFRNyc1eqLw+5H47beonjChy0vbH4kJChERUTcmW9p+/XpoamtRfdFFovHOLG1/JCYoRERE3Vhtba3kESGWr79Gw8CB8PTrJx7votETgAkKERFRtyY1vaOqrYXxp58kR08AJijUBfr06YNnn322+d8KhQLLli07rnt2xD2IiKjj+P1+OJ1O0Zj522+hEATYx40TjSckJDQf0toVWAeFAAClpaVITExsU9sHH3wQy5Ytw/bt24/5HkREFH52ux1SJ9pYvv4ajjPOQECiQmxXjp4A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CALmzJmDL774Aj/88AOysrJaxEeMGAGNRoPVq1c3P7Z3714UFBRg1KhRAIBRo0Zhx44dLcrQf/fddzAYDDjhhBNEP69Op4PBYGjxQURE1BNJ1T6J2b8fcbt2SVaOVSqVzWtGo0G71qDMnj0bH3zwAZYvX46EhITmNSNGoxExMTEwGo2YMWMG7rrrLpjNZhgMBtx6660YNWoUTj/9dADABRdcgBNOOAHXXHMNnnzySZSVleH+++/H7NmzodPpOv4ZEhERdRNOpxM+n080Zl22DH6LRfJgwGg7ILVdCcorr7wCADjnnHNaPP72229j+vTpAIDFixdDqVTi8ssvh9frxbhx4/Dyyy83t1WpVFixYgVuvvlmjBo1CnFxcbjuuuvw8MMPH98zISIi6uYkDwb0eGD+5htUXn655MGA0TS9AxxnHZSuwjooRETU0/j9fuzYsQNif7bN33yDrPnzsfOLL+AV2Uii0+mad9x2pU6rg0JERESdo7q6WjQ5ARqnd5ynnCKanADRN3oCMEEhIiKKClLTO7q8PCT8+iuqJk8WjSsUiog/GFAMExQiIqIIV1dX16Jg6eGsy5cjYDSi9txzReNGoxEajSac3QsLJihEREQRTnJxrN8Py4oVqL7wQggSO2GjcXoHYIJCREQU0QKBAGpqakRjxrVroampQdWll4rGtVpt1G4mYYJCREQUwex2u+ziWNfQofBkZ4vGLRZLVBwMKIYJChERUQSTmt7RlpTAsHmz5OgJEL3TOwATFCIioojlcrngdrtFY9blyxGKjUXN2LGicYPBAK1WG87uhRUTFCIiogglNXqCQACWL7+Effx4hCROJ05KSgpjz8KPCQoREVEECgQCsNvtojHjzz9DW1mJyssuE41rNBoYjcZwdi/smKAQERFFILnFsUmff476E06Ae+BA0Xg0L45twgSFiIgoAlVWVoo+ri0pgWHjRsnREyC6F8c2YYJCREQUYVwuFzwej2jMumxZ4+LYceNE4waDATqJom3RhAkKERFRhJEaPUEgAOvy5ai+8ELJxbHdYfQEYIJCREQUUeQqx5rWrYOmuhpVEtM7arUaJpMpjL3rPExQiIiIIkh1dbV05djPP4dryBC4+/cXj1utUb84tgkTFCIioggiWTm2qAjGTZskR0+A7jO9AzBBISIiihh1dXXSi2OXL0cgPh72888XjXeXxbFNmKAQERFFCNnFsV9+CfvEiRD0etEm0V459khMUIiIiCKA3+9HbW2taMz044/QVFejUuJgwO5QOfZITFCIiIgiQFVVlXTl2M8+g2vYMHj69RONd6fFsU2YoBAREXUxQRAkF8fq8vJg2LIFlX/+s+T13WlxbBMmKERERF3M4XDA5/OJxpI++wx+kwk1Y8aIxo1GI7RabTi71yWYoBAREXUxqcWxCo8HlhUrUH3xxRAkkpDutji2CRMUIiKiLuT1euF0OkVj5m+/hcrlkjwYUKvVwmAwhLN7XYYJChERUReS3FqMxukd56hR8PXqJR5PSup2i2ObMEGREQwGJecEiYiIjlcoFEJ1dbVoLHbXLsTt2iW5OFahUMBisYSze11K3dUdiERutxuVlZWorq6GwWBA3759u7pLRETUDdXW1iIQCIjGkj79FF6bDY7Ro0XjJpMJGo0mnN3rUkxQ/kcQBDgcDlRUVKCurq758draWni93m5VPpiIiCJDRUWF6OMqpxPmb79F6V//CqhUom266+LYJj0+QQkEAqiqqkJlZaXkdE5lZSV6Scz/ERERHYuGhgbU19eLxiwrVkARCKDqkktE43q9HgkJCeHsXpfrsQlKQ0MDKioqYLfbJSv3NamqqkJaWhqUSi7ZISKijiG5OFYQkPTZZ6g57zwEJAqwdffRE6CHJSiCIKCmpgYVFRWSWauYYDAIu93eLSv1ERFR5wsEArDb7aKxhF9+gT4/H/nz5onGlUplt14c26RHDQnU1dUhNze3XclJE6l5QiIiovaqrq5GKBQSjSUtXQp3djZcI0aIxs1mM1QS61K6kx6VoBgMBugljqlujdvthsvl6uAeERFRTyMIguT0jqasDKZ161Bx5ZWARH2TnjC9A/SwBAVo/YVVeDxAMCga4ygKEREdL6fTCa/XKxpL+uwzhGJiYL/wQtF4XFwcYmNjw9m9iNHjEhSLxSK52FVTUYGhEyfCuGGDaLy2thZ+vz+c3SMiom5O8twdrxfWL75A1aRJCEkkIcnJyeHsWkTpcQmKSqWSXFzkT0qCNz0dSZ98IhqXG5YjIiJqjdfrhcPhEI0lfv89NLW1kpVj1Wo1EhMTw9m9iNLjEhRAJgNVKFBx5ZUwbtwIXV6eaJPKyspWtyUTERGJkT13Z+lSOEeOhLdPH/F4Nz53R0yPTFDkCtzUnH8+/CYTkj79VDQeCARQU1MTzu4REVE3FAqFUFVVJRqL3bUL8Tt3ouKKK0TjCoWix5W66JEJCiA9iiLodKi69FJYv/oKSontyFwsS0RE7WW32xGU2ISRtHRp47k7Z50lGjeZTNBqteHsXsTpsQmK0WiUfLErL78cSo8Hlm++EY3X19cfUy0VIiLquSTP3amthfnbbxvXnvTQc3fE9NgERaFQSL7gfpsNtWef3bhYVmK9CRfLEhFRW9XV1cHtdovGrMuXAwCqe/C5O2J6bIICAFarVXLLccWVVyImNxcJW7aIxu12u+QR2URERIeTXBoQCCBp6VLUnH8+AhI7dHrS1uLD9egERa1Ww2w2i8ZcI0bA3bcvkj/+WDQuCILkYiciIqImPp8PtbW1ojHTTz9BV1aGiilTROMqlUry71R316MTFEBmXk+hQMVVV8H400/QlpSINqmoqOCWYyIikiW3sSL5o4/gGjYMDYMGicYtFkuPOHdHTI9PUGJjYxEfHy8as0+YgGBcnOSWY7/fL5kVExERyW0tjtm/HwnbtkmOngA9c3Fskx6foADS3wChmBhUX3wxrMuXN57RI6K8vDycXSMioigmu7X444/hS05GzbnnisaP54Db7oAJCoDExERoNBrRWMUVV0DldMKycqVonFuOiYhIitzWYsvKlY1bi9Vq0TY9dXFsEyYokN9y7OvVC44//QnJH34oueWYhduIiOhIsluLly0DBAFVl14qGtfpdDAajWHsXeRjgvI/VqtV8oyD8qlTEXPokOSW45qaGp5yTERELchuLf70U9jHjePWYhlMUP5Ho9FInhLpGjECDf37N46iiOApx0REdDiv1yu9tXjdusatxVddJRpXKpWwWCxh7F10YIJymJSUFPFA05bjn3+GtqhItEllZSVCoVAYe0dERNGita3FdSedBHdOjmjcarX22K3Fh2OCchjZLcfjxyNoMEgWbuMpx0REBADBYBDV1dWisZh9+5Dw66+olBg9AXr21uLDMUE5guQpx3o9Ki+7DNYvv4TS5RJtw8WyRERUXV0tubU4+cMP4UtJkdxabDQae/TW4sMxQTmC3JHWlVdc0XjK8YoVovGGhgbU1dWFs3tERBTBBEGQfLOqrqqCedWqxrUn3FrcKiYoR5A95Tg5GTVjxjRO80isN+EoChFRz+VwOOD1ekVjSZ99BkGlQtXkyaJx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",
-                        "text/plain": "<Figure size 640x480 with 1 Axes>"
+                        "text/plain": [
+                            "<Figure size 640x480 with 1 Axes>"
+                        ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "import matplotlib.pyplot as plt\n",
@@ -604,14 +570,13 @@
                 "name": "ipython",
                 "version": 2
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython2",
-            "version": "2.7.6"
+            "pygments_lexer": "ipython2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 0
 }
```

### Comparing `autora-workflow-0.3.3/docs/interactive/using-alternative-planners-and-executors.ipynb` & `autora-workflow-0.3.4/docs/interactive/using-alternative-planners-and-executors.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722211238662132%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}}, 1: {'execution_count': None, 'metadata': "*

 * *            "{replace: OrderedDict()}}, 2: {'execution_count': None, 'source': {insert: [(2, "*

 * *            "'variables = VariableCollection(\\n'), (7, '    "*

 * *            "[variables.independent_variables[0].allowed_values])\\n'), (24, '    "*

 * *            "variables=variables,\\n')], delete: [24, 7, 2]}, 'metadata': {replace: "*

 * *            "OrderedDict()}}, 3: {'metadata': {replace: OrderedDict()}}, 4: {'execut […]*

```diff
@@ -1,14 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "# Custom Planners and Executors\n",
                 "\n",
                 "By switching out the `executor_collection` and/or the `planner`, we can specify a\n",
                 "different way of running the cycle.\n",
                 "\n",
                 "## Easier Seeding with a Smarter Planner\n",
@@ -16,52 +14,40 @@
                 "In this example, we use the `Controller` which allows much more control over execution\n",
                 "order. It considers the last available result and picks the matching next step. This means\n",
                 "that seeding is relatively simple."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.631186Z",
-                    "start_time": "2023-04-28T16:01:56.933043Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from autora.experimentalist.pipeline import make_pipeline\n",
                 "from autora.variable import VariableCollection, Variable\n",
                 "from sklearn.linear_model import LinearRegression\n",
                 "from autora.workflow import Controller\n",
                 "from itertools import takewhile"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.635379Z",
-                    "start_time": "2023-04-28T16:01:57.633245Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "def ground_truth(x):\n",
                 "    return x + 1\n",
-                "metadata_0 = VariableCollection(\n",
+                "variables = VariableCollection(\n",
                 "   independent_variables=[Variable(name=\"x1\", allowed_values=range(11))],\n",
                 "   dependent_variables=[Variable(name=\"y\", value_range=(-20, 20))],\n",
                 "   )\n",
                 "example_experimentalist = make_pipeline(\n",
-                "    [metadata_0.independent_variables[0].allowed_values])\n",
+                "    [variables.independent_variables[0].allowed_values])\n",
                 "\n",
                 "def get_example_synthetic_experiment_runner():\n",
                 "    rng = np.random.default_rng(seed=180)\n",
                 "    def runner(x):\n",
                 "        return ground_truth(x) + rng.normal(0, 0.1, x.shape)\n",
                 "    return runner\n",
                 "\n",
@@ -70,118 +56,94 @@
                 "example_theorist = LinearRegression()\n",
                 "\n",
                 "def monitor(state):\n",
                 "    print(f\"MONITOR: Generated new {state.history[-1].kind}\")\n",
                 "\n",
                 "cycle_with_last_result_planner = Controller(\n",
                 "    monitor=monitor,\n",
-                "    metadata=metadata_0,\n",
+                "    variables=variables,\n",
                 "    experimentalist=example_experimentalist,\n",
                 "    experiment_runner=example_synthetic_experiment_runner,\n",
                 "    theorist=example_theorist,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "When we run this cycle starting with no data, we generate an experimental condition first:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.641066Z",
-                    "start_time": "2023-04-28T16:01:57.636930Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "MONITOR: Generated new ResultKind.CONDITION\n",
-                        "MONITOR: Generated new ResultKind.OBSERVATION\n",
-                        "MONITOR: Generated new ResultKind.MODEL\n",
-                        "MONITOR: Generated new ResultKind.CONDITION\n",
-                        "MONITOR: Generated new ResultKind.OBSERVATION\n",
-                        "MONITOR: Generated new ResultKind.MODEL\n"
+                        "MONITOR: Generated new CONDITION\n",
+                        "MONITOR: Generated new OBSERVATION\n",
+                        "MONITOR: Generated new MODEL\n",
+                        "MONITOR: Generated new CONDITION\n",
+                        "MONITOR: Generated new OBSERVATION\n",
+                        "MONITOR: Generated new MODEL\n"
                     ]
                 }
             ],
             "source": [
                 "_ = list(takewhile(lambda c: len(c.state.models) < 2, cycle_with_last_result_planner))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "However, if we seed the same cycle with observations, then its first Executor will be the theorist:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.643810Z",
-                    "start_time": "2023-04-28T16:01:57.642246Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "controller_with_seed_observation = Controller(\n",
                 "    monitor=monitor,\n",
-                "    metadata=metadata_0,\n",
+                "    variables=variables,\n",
                 "    theorist=example_theorist,\n",
                 "    experimentalist=example_experimentalist,\n",
                 "    experiment_runner=example_synthetic_experiment_runner,\n",
                 ")\n",
                 "seed_observation = example_synthetic_experiment_runner(np.linspace(0,5,10))\n",
                 "controller_with_seed_observation.seed(observations=[seed_observation])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.648672Z",
-                    "start_time": "2023-04-28T16:01:57.646294Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "MONITOR: Generated new ResultKind.MODEL\n"
+                        "MONITOR: Generated new MODEL\n"
                     ]
                 }
             ],
             "source": [
                 "_ = next(controller_with_seed_observation)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## Arbitrary Execution Order (Toy Example)\n",
                 "\n",
                 "In some cases, we need to change the order of execution of different steps completely. This might be\n",
                 " useful in cases when different experimentalists or theorists are needed at different times in\n",
                 " the cycle, e.g. for initial seeding, or if the _order_ of execution is the subject of the\n",
                 " experiment.\n",
@@ -192,319 +154,257 @@
                 "\n",
                 "This might be useful in cases when different experimentalists or theorists are needed at\n",
                 "different times in the cycle, e.g. for initial seeding."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.650942Z",
-                    "start_time": "2023-04-28T16:01:57.648821Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "from autora.workflow.planner import random_operation_planner\n",
                 "def monitor(state):\n",
                 "    print(f\"MONITOR: Generated new {state.history[-1].kind}\")\n",
                 "controller_with_random_planner = Controller(\n",
                 "    planner=random_operation_planner,\n",
                 "    monitor=monitor,\n",
-                "    metadata=metadata_0,\n",
+                "    variables=variables,\n",
                 "    theorist=example_theorist,\n",
                 "    experimentalist=example_experimentalist,\n",
                 "    experiment_runner=example_synthetic_experiment_runner,\n",
                 ")\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The `random_operation_planner` depends on the python random number generator, so we seed it first:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.682695Z",
-                    "start_time": "2023-04-28T16:01:57.651180Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "from random import seed\n",
                 "seed(42)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "We also want to watch the logging messages from the cycle:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.690905Z",
-                    "start_time": "2023-04-28T16:01:57.653429Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import logging\n",
                 "import sys\n",
                 "logging.basicConfig(format='%(levelname)s: %(message)s', stream=sys.stdout,\n",
                 "    level=logging.INFO)\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "Now we can evaluate the cycle and watch its behaviour:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.691071Z",
-                    "start_time": "2023-04-28T16:01:57.655486Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "def step(controller_):\n",
                 "    try:\n",
                 "        _ = next(controller_)\n",
                 "    except Exception as e:\n",
                 "        print(f\"FAILED: with {e=}\")\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The first step, the theorist is selected as the random Executor, and it fails because it\n",
                 "depends on there being observations to theorize against:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.691280Z",
-                    "start_time": "2023-04-28T16:01:57.659011Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
+                        "INFO: getting step_name='theorist'\n",
+                        "INFO: running next_function=<function from_theorist_estimator.<locals>._executor_theorist at 0x14f594dc0>\n",
                         "FAILED: with e=AssertionError('observations=[] needs at least one entry for model fitting')\n"
                     ]
                 }
             ],
             "source": [
                 "step(controller_with_random_planner) # i = 0"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The second step, a new condition is generated."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.691357Z",
-                    "start_time": "2023-04-28T16:01:57.661419Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "MONITOR: Generated new ResultKind.CONDITION\n"
+                        "INFO: getting step_name='experimentalist'\n",
+                        "INFO: running next_function=<function from_experimentalist_pipeline.<locals>._executor_experimentalist at 0x14f594dc0>\n",
+                        "MONITOR: Generated new CONDITION\n"
                     ]
                 }
             ],
             "source": [
                 "step(controller_with_random_planner) # i = 1"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "... which is repeated on the third step as well:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.691425Z",
-                    "start_time": "2023-04-28T16:01:57.663622Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "MONITOR: Generated new ResultKind.CONDITION\n"
+                        "INFO: getting step_name='experimentalist'\n",
+                        "INFO: running next_function=<function from_experimentalist_pipeline.<locals>._executor_experimentalist at 0x14f595750>\n",
+                        "MONITOR: Generated new CONDITION\n"
                     ]
                 }
             ],
             "source": [
                 "step(controller_with_random_planner) # i = 2"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "On the fourth step, we generate another error when trying to run the theorist:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.691501Z",
-                    "start_time": "2023-04-28T16:01:57.667337Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
+                        "INFO: getting step_name='theorist'\n",
+                        "INFO: running next_function=<function from_theorist_estimator.<locals>._executor_theorist at 0x14f5955a0>\n",
                         "FAILED: with e=AssertionError('observations=[] needs at least one entry for model fitting')\n"
                     ]
                 }
             ],
             "source": [
                 "step(controller_with_random_planner) # i = 3"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "On the fifth step, we generate a first real observation, so that the next time we try to run\n",
                 "a theorist we are successful:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.691583Z",
-                    "start_time": "2023-04-28T16:01:57.669604Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "MONITOR: Generated new ResultKind.OBSERVATION\n"
+                        "INFO: getting step_name='experiment_runner'\n",
+                        "INFO: running next_function=<function from_experiment_runner_callable.<locals>._executor_experiment_runner at 0x107119630>\n",
+                        "MONITOR: Generated new OBSERVATION\n"
                     ]
                 }
             ],
             "source": [
                 "step(controller_with_random_planner) # i = 4"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "By the ninth iteration, there are observations which the theorist can use, and it succeeds."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.691641Z",
-                    "start_time": "2023-04-28T16:01:57.671841Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "MONITOR: Generated new ResultKind.CONDITION\n",
-                        "MONITOR: Generated new ResultKind.CONDITION\n",
-                        "MONITOR: Generated new ResultKind.CONDITION\n",
-                        "MONITOR: Generated new ResultKind.MODEL\n"
+                        "INFO: getting step_name='experimentalist'\n",
+                        "INFO: running next_function=<function from_experimentalist_pipeline.<locals>._executor_experimentalist at 0x14f596200>\n",
+                        "MONITOR: Generated new CONDITION\n",
+                        "INFO: getting step_name='experimentalist'\n",
+                        "INFO: running next_function=<function from_experimentalist_pipeline.<locals>._executor_experimentalist at 0x1071195a0>\n",
+                        "MONITOR: Generated new CONDITION\n",
+                        "INFO: getting step_name='experimentalist'\n",
+                        "INFO: running next_function=<function from_experimentalist_pipeline.<locals>._executor_experimentalist at 0x14f5964d0>\n",
+                        "MONITOR: Generated new CONDITION\n",
+                        "INFO: getting step_name='theorist'\n",
+                        "INFO: running next_function=<function from_theorist_estimator.<locals>._executor_theorist at 0x14f596830>\n",
+                        "MONITOR: Generated new MODEL\n"
                     ]
                 }
             ],
             "source": [
                 "_ = list(takewhile(lambda c: len(c.state.models) < 1, controller_with_random_planner))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## Arbitrary Executors and Planners\n",
                 "\n",
                 "In some cases, we need to go beyond adding different orders of planning the three\n",
                 "`experimentalist`, `experiment_runner` and `theorist` and build more complex cycles with\n",
                 "different Executors for different states.\n",
                 "\n",
@@ -516,80 +416,58 @@
                 "\n",
                 "In these cases, we need full control over (and have full responsibility for) the planners and\n",
                 "executors.\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The model we'll try to discover is:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.691699Z",
-                    "start_time": "2023-04-28T16:01:57.675535Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "def ground_truth(x, m=3.5, c=1):\n",
                 "    return m * x + c\n",
                 "rng = np.random.default_rng(seed=180)\n",
                 "def experiment_runner(x):\n",
                 "    return ground_truth(x) + rng.normal(0, 0.1)\n",
-                "metadata_2 = VariableCollection(\n",
+                "variables = VariableCollection(\n",
                 "   independent_variables=[Variable(name=\"x1\", value_range=(-10, 10))],\n",
                 "   dependent_variables=[Variable(name=\"y\", value_range=(-100, 100))],\n",
                 "   )"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "We now define a planner which chooses a different experimentalist when supplied with no data\n",
                 "versus some data."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.700515Z",
-                    "start_time": "2023-04-28T16:01:57.677699Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "from autora.workflow.planner import last_result_kind_planner\n",
                 "from autora.workflow.state import History"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.707520Z",
-                    "start_time": "2023-04-28T16:01:57.679940Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "def seeding_planner(state):\n",
                 "    # We're going to reuse the \"last_result_kind_planner\" planner, and modify its output.\n",
                 "    next_function = last_result_kind_planner(state)\n",
                 "    if next_function == \"experimentalist\":\n",
                 "        if len(state.models) >= 2:\n",
@@ -598,540 +476,526 @@
                 "            return \"seed_experimentalist\"\n",
                 "    else:\n",
                 "        return next_function\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "Now we can see what would happen with a particular state. If there are no results, then we get the seed experimentalist:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.707878Z",
-                    "start_time": "2023-04-28T16:01:57.683044Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "'seed_experimentalist'"
+                        "text/plain": [
+                            "'seed_experimentalist'"
+                        ]
                     },
-                    "execution_count": 19,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "seeding_planner(History())"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "... and we also get the seed experimentalist if the last result was a model and there are less than two models:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.708090Z",
-                    "start_time": "2023-04-28T16:01:57.685631Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "'seed_experimentalist'"
+                        "text/plain": [
+                            "'seed_experimentalist'"
+                        ]
                     },
-                    "execution_count": 20,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "seeding_planner(History(models=['a single model']))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "whereas if we have at least two models to work on, we get the main experimentalist:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.708246Z",
-                    "start_time": "2023-04-28T16:01:57.688533Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "'main_experimentalist'"
+                        "text/plain": [
+                            "'main_experimentalist'"
+                        ]
                     },
-                    "execution_count": 21,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "seeding_planner(History(models=['a model', 'another model']))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "If we had a condition last, we choose the experiment runner next:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.708731Z",
-                    "start_time": "2023-04-28T16:01:57.691768Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "'experiment_runner'"
+                        "text/plain": [
+                            "'experiment_runner'"
+                        ]
                     },
-                    "execution_count": 22,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "seeding_planner(History(conditions=['a condition']))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "If we had an observation last, we choose the theorist next:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.708804Z",
-                    "start_time": "2023-04-28T16:01:57.694315Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "'theorist'"
+                        "text/plain": [
+                            "'theorist'"
+                        ]
                     },
-                    "execution_count": 23,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "seeding_planner(History(observations=['an observation']))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "Now we need to define an executor collection to handle the actual execution steps."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.708840Z",
-                    "start_time": "2023-04-28T16:01:57.696837Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "from autora.experimentalist.pipeline import make_pipeline, Pipeline\n",
                 "from autora.experimentalist.sampler.random_sampler import random_sampler\n",
                 "from functools import partial"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "Wen can run the seed pipeline with no data:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-28T16:01:57.708934Z",
-                    "start_time": "2023-04-28T16:01:57.700468Z"
-                },
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "array([ 6.71671672, -0.73073073, -5.05505506,  6.13613614,  0.03003003,\n        4.59459459,  2.79279279,  5.43543544, -1.65165165,  8.0980981 ])"
+                        "text/plain": [
+                            "array([ 6.71671672, -0.73073073, -5.05505506,  6.13613614,  0.03003003,\n",
+                            "        4.59459459,  2.79279279,  5.43543544, -1.65165165,  8.0980981 ])"
+                        ]
                     },
-                    "execution_count": 25,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "experimentalist_which_needs_no_data = make_pipeline([\n",
-                "    np.linspace(*metadata_2.independent_variables[0].value_range, 1_000),\n",
+                "    np.linspace(*variables.independent_variables[0].value_range, 1_000),\n",
                 "    partial(random_sampler, n=10)]\n",
                 ")\n",
                 "np.array(experimentalist_which_needs_no_data())"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "... whereas we need some model for this sampler:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
-            "metadata": {
-                "collapsed": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "ename": "TypeError",
                     "evalue": "model_disagreement_sampler() missing 1 required positional argument: 'models'",
                     "output_type": "error",
                     "traceback": [
                         "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
                         "\u001b[0;31mTypeError\u001b[0m                                 Traceback (most recent call last)",
-                        "Cell \u001b[0;32mIn[26], line 5\u001b[0m\n\u001b[1;32m      1\u001b[0m \u001b[38;5;28;01mfrom\u001b[39;00m \u001b[38;5;21;01mautora\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mexperimentalist\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01msampler\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mmodel_disagreement\u001b[39;00m \u001b[38;5;28;01mimport\u001b[39;00m model_disagreement_sampler\n\u001b[1;32m      2\u001b[0m experimentalist_which_needs_a_model \u001b[38;5;241m=\u001b[39m Pipeline([\n\u001b[1;32m      3\u001b[0m     (\u001b[38;5;124m'\u001b[39m\u001b[38;5;124mpool\u001b[39m\u001b[38;5;124m'\u001b[39m, np\u001b[38;5;241m.\u001b[39mlinspace(\u001b[38;5;241m*\u001b[39mvariables_2\u001b[38;5;241m.\u001b[39mindependent_variables[\u001b[38;5;241m0\u001b[39m]\u001b[38;5;241m.\u001b[39mvalue_range, \u001b[38;5;241m1_000\u001b[39m)),\n\u001b[1;32m      4\u001b[0m     (\u001b[38;5;124m'\u001b[39m\u001b[38;5;124msampler\u001b[39m\u001b[38;5;124m'\u001b[39m, partial(model_disagreement_sampler, num_samples\u001b[38;5;241m=\u001b[39m\u001b[38;5;241m5\u001b[39m)),])\n\u001b[0;32m----> 5\u001b[0m \u001b[43mexperimentalist_which_needs_a_model\u001b[49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m\n",
-                        "File \u001b[0;32m~/Developer/autora-core/src/autora/experimentalist/pipeline.py:171\u001b[0m, in \u001b[0;36mPipeline.__call__\u001b[0;34m(self, ex, **params)\u001b[0m\n\u001b[1;32m    169\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m \u001b[38;5;28misinstance\u001b[39m(pipe, Pipe)\n\u001b[1;32m    170\u001b[0m     all_params_for_pipe \u001b[38;5;241m=\u001b[39m merged_params\u001b[38;5;241m.\u001b[39mget(name, \u001b[38;5;28mdict\u001b[39m())\n\u001b[0;32m--> 171\u001b[0m     results\u001b[38;5;241m.\u001b[39mappend(\u001b[43mpipe\u001b[49m\u001b[43m(\u001b[49m\u001b[43mresults\u001b[49m\u001b[43m[\u001b[49m\u001b[38;5;241;43m-\u001b[39;49m\u001b[38;5;241;43m1\u001b[39;49m\u001b[43m]\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[43mall_params_for_pipe\u001b[49m\u001b[43m)\u001b[49m)\n\u001b[1;32m    173\u001b[0m \u001b[38;5;28;01mreturn\u001b[39;00m results[\u001b[38;5;241m-\u001b[39m\u001b[38;5;241m1\u001b[39m]\n",
+                        "Cell \u001b[0;32mIn[26], line 5\u001b[0m\n\u001b[1;32m      1\u001b[0m \u001b[38;5;28;01mfrom\u001b[39;00m \u001b[38;5;21;01mautora\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mexperimentalist\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01msampler\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mmodel_disagreement\u001b[39;00m \u001b[38;5;28;01mimport\u001b[39;00m model_disagreement_sampler\n\u001b[1;32m      2\u001b[0m experimentalist_which_needs_a_model \u001b[38;5;241m=\u001b[39m Pipeline([\n\u001b[1;32m      3\u001b[0m     (\u001b[38;5;124m'\u001b[39m\u001b[38;5;124mpool\u001b[39m\u001b[38;5;124m'\u001b[39m, np\u001b[38;5;241m.\u001b[39mlinspace(\u001b[38;5;241m*\u001b[39mvariables\u001b[38;5;241m.\u001b[39mindependent_variables[\u001b[38;5;241m0\u001b[39m]\u001b[38;5;241m.\u001b[39mvalue_range, \u001b[38;5;241m1_000\u001b[39m)),\n\u001b[1;32m      4\u001b[0m     (\u001b[38;5;124m'\u001b[39m\u001b[38;5;124msampler\u001b[39m\u001b[38;5;124m'\u001b[39m, partial(model_disagreement_sampler, num_samples\u001b[38;5;241m=\u001b[39m\u001b[38;5;241m5\u001b[39m)),])\n\u001b[0;32m----> 5\u001b[0m \u001b[43mexperimentalist_which_needs_a_model\u001b[49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m\n",
+                        "File \u001b[0;32m~/Developer/autora-workflow/venv/lib/python3.10/site-packages/autora/experimentalist/pipeline.py:171\u001b[0m, in \u001b[0;36mPipeline.__call__\u001b[0;34m(self, ex, **params)\u001b[0m\n\u001b[1;32m    169\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m \u001b[38;5;28misinstance\u001b[39m(pipe, Pipe)\n\u001b[1;32m    170\u001b[0m     all_params_for_pipe \u001b[38;5;241m=\u001b[39m merged_params\u001b[38;5;241m.\u001b[39mget(name, \u001b[38;5;28mdict\u001b[39m())\n\u001b[0;32m--> 171\u001b[0m     results\u001b[38;5;241m.\u001b[39mappend(\u001b[43mpipe\u001b[49m\u001b[43m(\u001b[49m\u001b[43mresults\u001b[49m\u001b[43m[\u001b[49m\u001b[38;5;241;43m-\u001b[39;49m\u001b[38;5;241;43m1\u001b[39;49m\u001b[43m]\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[43mall_params_for_pipe\u001b[49m\u001b[43m)\u001b[49m)\n\u001b[1;32m    173\u001b[0m \u001b[38;5;28;01mreturn\u001b[39;00m results[\u001b[38;5;241m-\u001b[39m\u001b[38;5;241m1\u001b[39m]\n",
                         "\u001b[0;31mTypeError\u001b[0m: model_disagreement_sampler() missing 1 required positional argument: 'models'"
                     ]
                 }
             ],
             "source": [
                 "from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler\n",
                 "experimentalist_which_needs_a_model = Pipeline([\n",
-                "    ('pool', np.linspace(*metadata_2.independent_variables[0].value_range, 1_000)),\n",
+                "    ('pool', np.linspace(*variables.independent_variables[0].value_range, 1_000)),\n",
                 "    ('sampler', partial(model_disagreement_sampler, num_samples=5)),])\n",
                 "experimentalist_which_needs_a_model()"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "We'll have to provide the models during the cycle run.\n",
                 "\n",
                 "We need a reasonable theorist for this situation. For this problem, a linear regressor will suffice."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:16.580114Z",
-                    "start_time": "2023-04-27T18:59:16.569889Z"
-                },
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "t = LinearRegression()"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "Let's test the theorist for the ideal case \u2013 lots of data:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:17.816552Z",
-                    "start_time": "2023-04-27T18:59:17.807609Z"
-                },
-                "collapsed": false
-            },
-            "outputs": [],
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "'m = 3.50, c = 1.04'"
+                        ]
+                    },
+                    "execution_count": null,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "X = np.linspace(*metadata_2.independent_variables[0].value_range, 1_000).reshape(-1, 1)\n",
+                "X = np.linspace(*variables.independent_variables[0].value_range, 1_000).reshape(-1, 1)\n",
                 "tfitted = t.fit(X, experiment_runner(X))\n",
                 "f\"m = {tfitted.coef_[0][0]:.2f}, c = {tfitted.intercept_[0]:.2f}\""
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "This seems to work fine.\n",
                 "\n",
-                "Now we can define the executor component. We'll use a factory method to generate the collection:"
+                "Now we can define the executor component. We'll use a factory method to generate the\n",
+                "    collection:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:18.179154Z",
-                    "start_time": "2023-04-27T18:59:18.170109Z"
-                },
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "from autora.workflow.executor import make_online_executor_collection\n",
-                "executor_collection = make_online_executor_collection([\n",
-                "    (\"seed_experimentalist\", \"experimentalist\", experimentalist_which_needs_no_data),\n",
-                "    (\"main_experimentalist\", \"experimentalist\", experimentalist_which_needs_a_model),\n",
-                "    (\"theorist\", \"theorist\", LinearRegression()),\n",
-                "    (\"experiment_runner\", \"experiment_runner\", experiment_runner),\n",
-                "])\n"
+                "from autora.workflow.executor import (ChainedFunctionMapping, from_experimentalist_pipeline,\n",
+                "    from_experiment_runner_callable, from_theorist_estimator)\n",
+                "executor_collection = ChainedFunctionMapping(\n",
+                "    seed_experimentalist=\n",
+                "        [from_experimentalist_pipeline, experimentalist_which_needs_no_data],\n",
+                "    main_experimentalist=\n",
+                "        [from_experimentalist_pipeline, experimentalist_which_needs_a_model],\n",
+                "    experiment_runner=[from_experiment_runner_callable, experiment_runner],\n",
+                "    theorist=[from_theorist_estimator, LinearRegression()],\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "We need some special parameters to handle the main experimentalist, so we specify those:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:18.528215Z",
-                    "start_time": "2023-04-27T18:59:18.518548Z"
-                },
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "params = {\"main_experimentalist\": {\"sampler\": {\"models\": \"%models%\"}}}"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "We now instantiate the controller:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:18.930882Z",
-                    "start_time": "2023-04-27T18:59:18.926964Z"
-                },
-                "collapsed": false
-            },
-            "outputs": [],
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<autora.workflow.base.BaseController at 0x14f8ed570>"
+                        ]
+                    },
+                    "execution_count": null,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "from autora.workflow.base import BaseController\n",
                 "from autora.workflow.state import History\n",
                 "c = BaseController(\n",
-                "        state=History(metadata=metadata_2, params=params),\n",
+                "        state=History(variables=variables, params=params),\n",
                 "        planner=seeding_planner,\n",
                 "        executor_collection=executor_collection\n",
                 ")\n",
                 "c"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:19.257785Z",
-                    "start_time": "2023-04-27T18:59:19.249578Z"
-                },
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "class PrintHandler(logging.Handler):\n",
                 "    def emit(self, record):\n",
                 "        print(self.format(record))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "On the first step, we generate a condition sampled randomly across the whole domain (as we\n",
                 "expected):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:19.747720Z",
-                    "start_time": "2023-04-27T18:59:19.737183Z"
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "INFO: getting step_name='seed_experimentalist'\n",
+                        "INFO: running next_function=<function from_experimentalist_pipeline.<locals>._executor_experimentalist at 0x14f85feb0>\n"
+                    ]
                 },
-                "collapsed": false
-            },
-            "outputs": [],
+                {
+                    "data": {
+                        "text/plain": [
+                            "Result(data=array([ 9.4994995 , -8.17817818, -1.19119119,  8.6986987 ,  7.45745746,\n",
+                            "       -6.93693694,  8.05805806, -1.45145145, -5.97597598,  1.57157157]), kind=ResultKind.CONDITION)"
+                        ]
+                    },
+                    "execution_count": null,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "next(c).state.history[-1]"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "After three more steps, we generate a new condition, which again is sampled across the whole domain. Here we iterate\n",
                 "the controller until we've got two sets of conditions:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:20.145376Z",
-                    "start_time": "2023-04-27T18:59:20.137931Z"
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "INFO: getting step_name='experiment_runner'\n",
+                        "INFO: running next_function=<function from_experiment_runner_callable.<locals>._executor_experiment_runner at 0x14f85fe20>\n",
+                        "INFO: getting step_name='theorist'\n",
+                        "INFO: running next_function=<function from_theorist_estimator.<locals>._executor_theorist at 0x107118b80>\n",
+                        "INFO: getting step_name='seed_experimentalist'\n",
+                        "INFO: running next_function=<function from_experimentalist_pipeline.<locals>._executor_experimentalist at 0x14f85fe20>\n"
+                    ]
                 },
-                "collapsed": false
-            },
-            "outputs": [],
+                {
+                    "data": {
+                        "text/plain": [
+                            "Result(data=array([ 1.57157157, -3.93393393, -0.47047047, -4.47447447,  8.43843844,\n",
+                            "        6.17617618, -3.49349349, -8.998999  ,  4.93493493,  2.25225225]), kind=ResultKind.CONDITION)"
+                        ]
+                    },
+                    "execution_count": null,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "_ = list(takewhile(lambda c: len(c.state.conditions) < 2, c))\n",
                 "c.state.history[-1]"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "Once we have two models:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:21.060733Z",
-                    "start_time": "2023-04-27T18:59:21.040079Z"
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "INFO: getting step_name='experiment_runner'\n",
+                        "INFO: running next_function=<function from_experiment_runner_callable.<locals>._executor_experiment_runner at 0x14f85f9a0>\n",
+                        "INFO: getting step_name='theorist'\n",
+                        "INFO: running next_function=<function from_theorist_estimator.<locals>._executor_theorist at 0x107118b80>\n"
+                    ]
                 },
-                "collapsed": false
-            },
-            "outputs": [],
+                {
+                    "data": {
+                        "text/plain": [
+                            "[LinearRegression(), LinearRegression()]"
+                        ]
+                    },
+                    "execution_count": null,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "_ = list(takewhile(lambda c: len(c.state.models) < 2, c))\n",
                 "c.state.models"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "... when we run the next step, we'll get the main experimentalist. This samples five points from the extreme\n",
                 "parts  of the problem domain where the disagreement between the two models is the greatest:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:23.445789Z",
-                    "start_time": "2023-04-27T18:59:23.419106Z"
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "INFO: getting step_name='main_experimentalist'\n",
+                        "INFO: running next_function=<function from_experimentalist_pipeline.<locals>._executor_experimentalist at 0x14f85f9a0>\n",
+                        "WARNING: new_conditions=array([-10.        ,  -9.97997998,  -9.95995996,  -9.93993994,\n",
+                        "        -9.91991992]) is an ndarray, so variable confusion is a possibility\n"
+                    ]
                 },
-                "collapsed": false
-            },
-            "outputs": [],
+                {
+                    "data": {
+                        "text/plain": [
+                            "Result(data=array([-10.        ,  -9.97997998,  -9.95995996,  -9.93993994,\n",
+                            "        -9.91991992]), kind=ResultKind.CONDITION)"
+                        ]
+                    },
+                    "execution_count": null,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "next(c).state.history[-1]\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
@@ -1143,14 +1007,13 @@
                 "name": "ipython",
                 "version": 2
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython2",
-            "version": "2.7.6"
+            "pygments_lexer": "ipython2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 0
 }
```

### Comparing `autora-workflow-0.3.3/mkdocs/base.yml` & `autora-workflow-0.3.4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/mkdocs.yml` & `autora-workflow-0.3.4/mkdocs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -9,11 +9,9 @@
     - 'interactive/basic-usage.ipynb'
     - 'interactive/passing-static-parameters.ipynb'
     - "interactive/accessing-state-dependent-properties.ipynb"
     - "interactive/using-alternative-planners-and-executors.ipynb"
     - "interactive/saving-and-loading-dill.ipynb"
 - Command line:
     - "Basic Usage": "cli/basic-usage/README.ipynb"
-    - "With Cylc, Virtualenv and Pip": "cli/with-cylc-pip/README.md"
-    - "With Cylc and Conda": "cli/with-cylc-conda/README.md"
-    - "With Cylc and Slurm": "cli/with-cylc-slurm/README.md"
+    - "Using Cylc": "cli/with-cylc/README.md"
```

### Comparing `autora-workflow-0.3.3/pyproject.toml` & `autora-workflow-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/__init__.py` & `autora-workflow-0.3.4/src/autora/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/__main__.py` & `autora-workflow-0.3.4/src/autora/workflow/__main__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/base.py` & `autora-workflow-0.3.4/src/autora/workflow/base.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/controller.py` & `autora-workflow-0.3.4/src/autora/workflow/controller.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/cycle.py` & `autora-workflow-0.3.4/src/autora/workflow/cycle.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/executor.py` & `autora-workflow-0.3.4/src/autora/workflow/executor.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/planner.py` & `autora-workflow-0.3.4/src/autora/workflow/planner.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/plotting.py` & `autora-workflow-0.3.4/src/autora/workflow/plotting.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/protocol.py` & `autora-workflow-0.3.4/src/autora/workflow/protocol.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/serializer/__init__.py` & `autora-workflow-0.3.4/src/autora/workflow/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/state/history.py` & `autora-workflow-0.3.4/src/autora/workflow/state/history.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/state/param.py` & `autora-workflow-0.3.4/src/autora/workflow/state/param.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora/workflow/state/snapshot.py` & `autora-workflow-0.3.4/src/autora/workflow/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.3.3/src/autora_workflow.egg-info/PKG-INFO` & `autora-workflow-0.3.4/src/autora_workflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.3.3
+Version: 0.3.4
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: cylc
 License-File: LICENSE.md
 
-# Workflow
+# AutoRA Workflow
 
 Workflow management tools for AutoRA.
 
 ## Quickstart Guide
 
 You will need:
```

### Comparing `autora-workflow-0.3.3/tests/test_controller_plots.py` & `autora-workflow-0.3.4/tests/test_controller_plots.py`

 * *Files identical despite different names*

