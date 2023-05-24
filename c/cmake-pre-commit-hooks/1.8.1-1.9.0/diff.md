# Comparing `tmp/cmake_pre_commit_hooks-1.8.1.tar.gz` & `tmp/cmake_pre_commit_hooks-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake_pre_commit_hooks-1.8.1.tar", last modified: Thu Apr 20 21:59:21 2023, max compression
+gzip compressed data, was "cmake_pre_commit_hooks-1.9.0.tar", last modified: Wed May 24 18:52:10 2023, max compression
```

## Comparing `cmake_pre_commit_hooks-1.8.1.tar` & `cmake_pre_commit_hooks-1.9.0.tar`

### file list

```diff
@@ -1,57 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.codespell.allow
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.417322 cmake_pre_commit_hooks-1.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/draft_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/publish_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19785 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/clang_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/clang_tidy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/cppcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/cpplint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/include_what_you_use.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/lizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/misc/license_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/.pre-commit-win.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/bad.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/tests/cmake_good/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_good/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_good/.pre-commit-win.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_good/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_good/good.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/run_tests.ps1
--rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/run_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.codespell.allow
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.421768 cmake_pre_commit_hooks-1.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.421768 cmake_pre_commit_hooks-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/draft_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/publish_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16323 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_call_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17426 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_cmake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/clang_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/clang_tidy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/cppcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/cpplint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/include_what_you_use.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1738 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/lizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16323 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/misc/license_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 18:52:10.429768 cmake_pre_commit_hooks-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/.pre-commit-win.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/bad.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/tests/cmake_good/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_good/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_good/.pre-commit-win.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_good/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_good/good.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/_argparse_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/_call_process_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/_cmake_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/clang_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/clang_tidy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/cppcheck_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/cpplint_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/iwyu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/lizard_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/run_tests.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/run_tests.sh
```

### Comparing `cmake_pre_commit_hooks-1.8.1/.github/workflows/codeql-analysis.yml` & `cmake_pre_commit_hooks-1.9.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.1/.github/workflows/draft_release.yml` & `cmake_pre_commit_hooks-1.9.0/.github/workflows/draft_release.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.1/.github/workflows/format.yml` & `cmake_pre_commit_hooks-1.9.0/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.1/.github/workflows/publish_release.yml` & `cmake_pre_commit_hooks-1.9.0/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.1/.gitignore` & `cmake_pre_commit_hooks-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.1/.pre-commit-hooks.yaml` & `cmake_pre_commit_hooks-1.9.0/.pre-commit-hooks.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -15,21 +15,25 @@
   description: Find warnings/errors in C/CPP code
   files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cxx|cxxm|h|hpp|hxx|ixx|m|mxx)$
   language: python
 - id: cppcheck
   name: cppcheck (system)
   entry: cmake-pc-cppcheck-hook
   description: Find warnings/errors in C/CPP code
-  files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cxx|cxxm|h|hpp|hxx|ixx|m|mxx)$
+  # NB: no h|hpp|hxx here since we are calling cppcheck with --project=/path/to/compile_commands.json which does not
+  # contain header files
+  files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cxx|cxxm|ixx|m|mxx)$
   language: python
 - id: cppcheck-conda
   name: cppcheck (conda)
   entry: cmake-pc-cppcheck-hook
   description: Find warnings/errors in C/CPP code
-  files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cxx|cxxm|h|hpp|hxx|ixx|m|mxx)$
+  # NB: no h|hpp|hxx here since we are calling cppcheck with --project=/path/to/compile_commands.json which does not
+  # contain header files
+  files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cxx|cxxm|ixx|m|mxx)$
   language: conda
 - id: cpplint
   name: cpplint
   entry: cmake-pc-cpplint-hook
   description: Find warnings/errors in C/CPP code
   files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cuh|cxx|cxxm|h|hh|hpp|hxx|ixx|mxx)$
   language: python
```

### Comparing `cmake_pre_commit_hooks-1.8.1/CHANGELOG.md` & `cmake_pre_commit_hooks-1.9.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,42 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v1.9.0] - 2023-05-24
+
+### Added
+
+-   Added Python tests using PyTest
+-   Added support for parsing hook parameters from TOML configuration files
+-   Added option to dump the current configuration as TOML-formatted output on the standard output (`--dump-toml`)
+-   Added option to parse CMake trace output to detect files generated using `configure_file(...)`
+
+### Fixed
+
+-   Fixed potential issue with CppCheck hook always running on all files in compile database
+
+### Changed
+
+-   CppCheck hook will now exclude C++ header files by default since those are not present within the compilatioon databasebecauzse
+-   Make default logging level `INFO` instead of `WARNING`
+-   Move all CMake handling code into dedicated sub-module
+-   Minor adjustments to logging output format
+-   Update README
+
+### Repository
+
+-   Use [ruff](https://beta.ruff.rs/docs/) for linting over other Python linters
+-   System tests now run using LOGLEVEL=DEBUG
+-   Improved configuration for external linters (e.g. SonarCloud, Codacy)
+-   Update `yamllint` hook to v1.32.0
+
 ## [v1.8.1] - 2023-04-20
 
 ### Added
 
 -   Added support for C++ module files by default
 
 ### Fixed
@@ -260,15 +288,17 @@
 
 Initial release with support for:
 
 -   clang-format
 -   clang-tidy
 -   cppcheck
 
-[Unreleased]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.1...HEAD
+[Unreleased]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.0...HEAD
+
+[v1.9.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.1...v1.9.0
 
 [v1.8.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.0...v1.8.1
 
 [v1.8.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.7.0...v1.8.0
 
 [v1.7.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.6.0...v1.7.0
```

### Comparing `cmake_pre_commit_hooks-1.8.1/LICENSE` & `cmake_pre_commit_hooks-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.1/PKG-INFO` & `cmake_pre_commit_hooks-1.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,163 +1,164 @@
-Metadata-Version: 2.1
-Name: cmake_pre_commit_hooks
-Version: 1.8.1
-Summary: pre-commit hooks for CMake based projects
-Home-page: https://github.com/Takishima/cmake-pre-commit-hooks
-Author: Damien Nguyen
-Author-email: ngn.damien@gmail.com
-License: Apache2
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: clang-format
-Provides-Extra: lizard
-License-File: LICENSE
-
 # pre-commit hooks
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cmake-pre-commit-hooks?label=Python) [![PyPI version](https://badge.fury.io/py/cmake-pre-commit-hooks.svg)](https://badge.fury.io/py/cmake-pre-commit-hooks) [![CI Build](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml) [![CodeQL](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Takishima/cmake-pre-commit-hooks/main.svg)](https://results.pre-commit.ci/latest/github/Takishima/cmake-pre-commit-hooks/main) [![CodeFactor](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks/badge)](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Takishima_cmake-pre-commit-hooks&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Takishima_cmake-pre-commit-hooks)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cmake-pre-commit-hooks?label=Python) [![PyPI version](https://badge.fury.io/py/cmake-pre-commit-hooks.svg)](https://badge.fury.io/py/cmake-pre-commit-hooks) [![CI Build](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml) [![CodeQL](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Takishima/cmake-pre-commit-hooks/main.svg)](https://results.pre-commit.ci/latest/github/Takishima/cmake-pre-commit-hooks/main) [![CodeFactor](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks/badge)](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Takishima_cmake-pre-commit-hooks\&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Takishima_cmake-pre-commit-hooks)[![Codacy Badge](https://api.codacy.com/project/badge/Grade/a3a1139e4bed4d4694bb12991b7df775)](https://app.codacy.com/gh/Takishima/cmake-pre-commit-hooks?utm_source=github.com\&utm_medium=referral\&utm_content=Takishima/cmake-pre-commit-hooks\&utm_campaign=Badge_Grade)
 
+This is a [pre-commit](https://pre-commit.com) hooks repo that integrates C/C++ linters/formatters to work with
+CMake-based projects.
 
-This is a [pre-commit](https://pre-commit.com) hooks repo that integrates C/C++ linters/formatters to work with CMake-based projects.
 > [clang-format](https://clang.llvm.org/docs/ClangFormatStyleOptions.html),
-[clang-tidy](https://clang.llvm.org/extra/clang-tidy/),
-[cppcheck](http://cppcheck.sourceforge.net/),
-[cpplint](https://github.com/cpplint/cpplint),
-[lizard](http://www.lizard.ws) and
-[iwyu](https://include-what-you-use.org/)
+> [clang-tidy](https://clang.llvm.org/extra/clang-tidy/),
+> [cppcheck](http://cppcheck.sourceforge.net/),
+> [cpplint](https://github.com/cpplint/cpplint),
+> [lizard](http://www.lizard.ws) and
+> [iwyu](https://include-what-you-use.org/)
 
 It is largely based on the work found [here](https://github.com/pocc/pre-commit-hooks). The main difference with POCC's
 pre-commit hooks is that the ones from this repository will do a CMake configuration step prior to running any
 pre-commit hooks. This is done in order to have CMake generate the compilation database file that can then be used by
 the various hooks (using the `-DCMAKE_EXPORT_COMPILE_COMMANDS=ON` CMake option).
 
 This repository is only has Python-based pre-commit hooks.
 
 ## Current known issues
 
-Currently, the hooks that depend on having a compilation database generated by CMake (e.g. `clang-tidy`, `cppcheck`) are
-not working on Windows if you are not using the `Ninja` or `Makefile` generators.
+1.  Currently, the hooks that depend on having a compilation database generated by CMake (e.g. `clang-tidy`, `cppcheck`)
+    are not working on Windows if you are not using the `Ninja` or `Makefile` generators.
 
+2.  Currently, arguments set in a TOML configuration file (`pyproject.toml`, `cmake_pc_hooks.toml` or else) are applied
+    to all hooks. Future improvements may allow to customize arguments on a per-hook basis.
 
 ## Example usage
 
 Assuming that you have the following directory structure for your projects
 
-    root
-    ├── .pre-commit-config.yaml
-    ├── CMakeLists.txt
-    └── src
-        └── err.cpp
+```text
+root
+├── .pre-commit-config.yaml
+├── CMakeLists.txt
+└── src
+    └── err.cpp
+```
 
 with the following file contents:
 
-__.pre-commit-config.yaml__
-
-    repos:
-      - repo: https://github.com/Takishima/cmake-pre-commit-hooks
-        rev: v1.8.0
-        hooks:
-          - id: clang-format
-          - id: clang-tidy
-            args: [--checks=readability-magic-numbers,--warnings-as-errors=*]
-          - id: cppcheck
-          - id: include-what-you-use
+**.pre-commit-config.yaml**
 
+```yaml
+repos:
+  - repo: https://github.com/Takishima/cmake-pre-commit-hooks
+    rev: v1.8.0
+    hooks:
+      - id: clang-format
+      - id: clang-tidy
+        args: [--checks=readability-magic-numbers,--warnings-as-errors=*]
+      - id: cppcheck
+      - id: include-what-you-use
+```
 
-__CMakeLists.txt__
+**CMakeLists.txt**
 
-    cmake_minimum_required(VERSION 3.15)
-    project(LANGUAGE CXX)
-    add_library(mylib STATIC src/err.cpp)
+```cmake
+cmake_minimum_required(VERSION 3.15)
+project(LANGUAGE CXX)
+add_library(mylib STATIC src/err.cpp)
+```
 
-__src/err.cpp__
+**src/err.cpp**
 
-    #include <string>
-    int main() { int i; return 10; }
+```cpp
+#include <string>
+int main() { int i; return 10; }
+```
 
 Running pre-commit on the above project will lead to an output similar to this one:
 
-    $ pre-commit run --all-files
-    clang-format.............................................................Failed
-    - hook id: clang-format
-    - exit code: 1
-
-    src/err.cpp
-    ====================
-    <  int main() { int i; return 10; }
-    ---
-    >  int main() {
-    >    int i;
-    >    return 10;
-    >  }
-
-    clang-tidy...............................................................Failed
-    - hook id: clang-tidy
-    - exit code: 1
-
-    /tmp/temp/src/err.cpp:2:28: error: 10 is a magic number; consider replacing it with a named constant [readability-magic-numbers,-warnings-as-errors]
-    int main() { int i; return 10; }
-                               ^
-
-    cppcheck.................................................................Failed
-    - hook id: cppcheck
-    - exit code: 1
-
-    /tmp/temp/src/err.cpp:2:18: style: Unused variable: i [unusedVariable]
-    int main() { int i; return 10; }
-                     ^
-    include-what-you-use.....................................................Failed
-    - hook id: include-what-you-use
-    - exit code: 1
-
-    Problem with /usr/local/bin/iwyu_tool.py: Include-What-You-Use violations found
-
-    /tmp/temp/src/err.cpp should add these lines:
-    /tmp/temp/src/err.cpp should remove these lines:
-    - #include <string>  // lines 1-1
-    The full include-list for /tmp/temp/src/err.cpp:
-    ---
+```text
+$ pre-commit run --all-files
+clang-format.............................................................Failed
+- hook id: clang-format
+- exit code: 1
+
+src/err.cpp
+====================
+<  int main() { int i; return 10; }
+---
+>  int main() {
+>    int i;
+>    return 10;
+>  }
+
+clang-tidy...............................................................Failed
+- hook id: clang-tidy
+- exit code: 1
+
+/tmp/temp/src/err.cpp:2:28: error: 10 is a magic number; consider replacing it with a named constant [readability-magic-numbers,-warnings-as-errors]
+int main() { int i; return 10; }
+                           ^
+
+cppcheck.................................................................Failed
+- hook id: cppcheck
+- exit code: 1
+
+/tmp/temp/src/err.cpp:2:18: style: Unused variable: i [unusedVariable]
+int main() { int i; return 10; }
+                 ^
+include-what-you-use.....................................................Failed
+- hook id: include-what-you-use
+- exit code: 1
+
+Problem with /usr/local/bin/iwyu_tool.py: Include-What-You-Use violations found
+
+/tmp/temp/src/err.cpp should add these lines:
+/tmp/temp/src/err.cpp should remove these lines:
+- #include <string>  // lines 1-1
+The full include-list for /tmp/temp/src/err.cpp:
+---
+```
 
 Note that your mileage may vary depending on the version of the tools. The example above was generated using
 `clang-format` 12.0.0, `clang-tidy` 12.0.0, `cppcheck` 2.4.1 and `include-what-you-use` 0.16.
 
 ## Using the Hooks
 
-Python 3.6+ is required to use these hooks as all 3 invoking scripts are written in it. As this is also the minimum
+Python 3.8+ is required to use these hooks as all 3 invoking scripts are written in it. As this is also the minimum
 version of pre-commit, this should not be an issue.
 
 Running multiple hooks in parallel is currently supported by using the `fastener` Python package. If the hooks are run
 in parallel, only one of the hooks will run the CMake configure step while the others will simply wait until the call to
 CMake ends to continue. In the case where the hooks are run serially, all the hooks will be running the CMake configure
 step. However, if nothing changed in your CMake configuration, this should not cost too much time.
 
-
 ### Installation
 
 For installing the various utilities, refer to your package manager documentation. Some guidance can also be found
 [here](https://github.com/pocc/pre-commit-hooks#installation).
 
-
 ### Hook Info
 
-| Hook Info                                                                | Type                     | Languages        |
-|--------------------------------------------------------------------------|--------------------------|------------------|
-| [clang-format](https://clang.llvm.org/docs/ClangFormatStyleOptions.html) | Formatter                | C, C++, ObjC     |
-| [clang-tidy](https://clang.llvm.org/extra/clang-tidy/)                   | Static code analyzer     | C, C++, ObjC     |
-| [cppcheck](http://cppcheck.sourceforge.net/)                             | Static code analyzer     | C, C++           |
-| [cpplint](https://github.com/cpplint/cpplint)                            | Static code analyzer     | C, C++           |
-| [include-what-you-use](https://include-what-you-use.org/)                | Static code analyzer     | C, C++           |
-| [lizard](http://www.lizard.ws)                                           | code complexity analyzer | C/C++, ObjC, ... |
+| Hook Info                | Type                     | Languages        |
+|--------------------------|--------------------------|------------------|
+| [clang-format][]         | Formatter                | C, C++, ObjC     |
+| [clang-tidy][]           | Static code analyzer     | C, C++, ObjC     |
+| [cppcheck][]             | Static code analyzer     | C, C++           |
+| [cpplint][]              | Static code analyzer     | C, C++           |
+| [include-what-you-use][] | Static code analyzer     | C, C++           |
+| [lizard][]               | Code complexity analyzer | C/C++, ObjC, ... |
+
+[clang-format]: https://clang.llvm.org/docs/ClangFormatStyleOptions.html
+
+[clang-tidy]: https://clang.llvm.org/extra/clang-tidy/
+
+[cppcheck]: http://cppcheck.sourceforge.net/
+
+[cpplint]: https://github.com/cpplint/cpplint
+
+[include-what-you-use]: https://include-what-you-use.org/
+
+[lizard]: http://www.lizard.ws
 
 ### Hook options
 
 Since v1.1.0 all hooks that depend on a compilation database (e.g. `clang-tidy`, `cppcheck`, `include-what-you-use`)
 will attempt to generate a CMake build directory before running the actual command.
 
 These hooks accept all the most common CMake options:
@@ -181,35 +182,38 @@
 argument (`-B`) multiple times. The hooks will then simply cycle through all of the values provided and choose the first
 directory that contains a configured CMake project (by looking at the presence of the `CMakeCache.txt` file). This may
 be useful if you already have a build directory available somewhere that you would like to re-use. In the case where
 none of the provided options is viable, the first one will automatically be selected as the build directory.
 
 In addition to the above CMake options, the hooks also accept the following:
 
-| Other hook options           | Description                                      | Note         |
-|------------------------------|--------------------------------------------------|--------------|
-| `--all-at-once`              | Pass all filenames to the command at once        | Since v1.4.0 |
-| `--read-json-db`             | Append file list from compile database           | Since v1.7.0 |
-| `--cmake`                    | Specify path to CMake executable                 | Since v1.4.0 |
-| `--linux`                    | Linux-only CMake options                         | Since v1.3.0 |
-| `--mac`                      | MacOS-only CMake options                         | Since v1.3.0 |
-| `--win`                      | Windows-only CMake options                       | Since v1.3.0 |
+| Other hook options           | Description                                            | Note         |
+|------------------------------|--------------------------------------------------------|--------------|
+| `--all-at-once`              | Pass all filenames to the command at once              | Since v1.4.0 |
+| `--clean`                    | Perform a clean CMake build                            | Since v1.4.0 |
+| `--cmake`                    | Specify path to CMake executable                       | Since v1.4.0 |
+| `--detect-configured-files`  | Enable cmake tracing and detection of configured files | Since v1.9.0 |
+| `--dump-toml`                | Dump the current configuration as TOML on stdout       | Since v1.9.0 |
+| `--no-automatic-discovery`   | Disable automatic build directory discovery            | Since v1.9.0 |
+| `--read-json-db`             | Append file list from compile database                 | Since v1.7.0 |
+| `--linux`                    | Linux-only CMake options                               | Since v1.3.0 |
+| `--mac`                      | MacOS-only CMake options                               | Since v1.3.0 |
+| `--win`                      | Windows-only CMake options                             | Since v1.3.0 |
 
 NB: by specifying `--all-at-once` the linter/formatter command will only be called once for all the files instead of
 calling the command once per file.
 
 NB: Since v1.6.0, the `--debug` command line argument has been removed. Use the `LOGLEVEL` environment variable instead
 to control the level of verbosity of each of the commands. To show all debug messages, set `LOGLEVEL=DEBUG` in your
 environment variables when running the hooks.
 
 NB: by specifying `--read-json-db` the hook will read the list of files from the `compile_commands.json` generated by
 CMake and will append those files to the list of files to process regardless of the list of files otherwise passed on
 the command line.
 
-
 Usage example:
 
 ```yaml
 repos:
 - repo: https://github.com/Takishima/cmake-pre-commit-hooks
   rev: v1.8.0
   hooks:
@@ -228,32 +232,74 @@
 that contains some CMake cache files), then it will be used. If none qualify, the hooks will default to using
 `path/to/build_dir` as a build directory, creating it as necessary.
 
 Also, builds on Linux and MacOS will set the C++ compiler to `g++-10`, while builds on Windows will be using
 `cl.exe`. This is done by looking at the value returned by
 [`platform.system()`](https://docs.python.org/3/library/platform.html#platform.system).
 
+### TOML support
+
+Since v1.9.0, the hooks support loading the CLI arguments from TOML files. This can be used to configure all the hooks
+for a particular repository using either of:
+
+1.  `pyproject.toml`
+2.  `cmake_pc_hooks.toml`
+3.  TOML file specified using `--config=/path/to/file.toml`
+4.  Command line arguments
+
+Note that each step in the above list is overridden by the steps that happen **after** it. For example, CLI arguments
+will always override any arguments read from any TOML file.
+
+A good place to start if you plan on creating a TOML configuration file is to use the hooks using the CLI arguments as
+you would normally and then run the hook manually and with the addition of `--dump-toml`. This will output a
+TOML-formatted configuration on the standard output for all the parameters that *diverge* from their default values.
+
+For example, running the following command (assuming that no valid TOML configuration exists):
+
+```bash
+cmake-pc-clang-format-hook tests/cmake_bad/bad.cpp  --dump-toml -B /tmp/build -S source -Wdev --no-automatic-discovery
+```
+
+will result in the following output:
+
+```toml
+automatic_discovery = false
+source_dir = "source"
+build_dir = [ "/tmp/build",]
+dev_warnings = true
+```
+
+### CMake configured file detection
+
+Since v1.9.0, the hooks support the use of CMake with trace mode enabled in order to keep track of files that are
+generated using calls to the `configure_file(...)` CMake function. If `--detect-configured-files` is specified on the
+command line (or in some TOML configuration file), the hooks will attempt to locate those generated files and
+automatically add them to the list of processed files for any hook invocation.
+
 ### Hook Option Comparison
 
-| Hook Options                                                             | Fix In Place       | Enable all Checks                       | Set key/value |
-|--------------------------------------------------------------------------|--------------------|-----------------------------------------|---------------|
-| [clang-format](https://clang.llvm.org/docs/ClangFormatStyleOptions.html) | `-i`               |                                         |               |
-| [clang-tidy](https://clang.llvm.org/extra/clang-tidy/)                   | `--fix-errors` [1] | `-checks=*` `-warnings-as-errors=*` [2] |               |
-| [cppcheck](http://cppcheck.sourceforge.net/)                             |                    | `-enable=all`                           |               |
-| [include-what-you-use](https://include-what-you-use.org/)                |                    |                                         |               |
+| Hook Options             | Fix In Place        | Enable all Checks                        | Set key/value |
+|--------------------------|---------------------|------------------------------------------|---------------|
+| [clang-format][]         | `-i`                |                                          |               |
+| [clang-tidy][]           | `--fix-errors` [^1] | `-checks=*` `-warnings-as-errors=*` [^2] |               |
+| [cppcheck][]             |                     | `-enable=all`                            |               |
+| [include-what-you-use][] |                     |                                          |               |
 
-[1]: `-fix` will fail if there are compiler errors. `-fix-errors` will `-fix` and fix compiler errors if it can, like missing semicolons.
+[^1]: `-fix` will fail if there are compiler errors. `-fix-errors` will `-fix` and fix compiler errors if it can, like missing semicolons.
 
-[2]: Be careful with `-checks=*`.  can have self-contradictory rules in newer versions of llvm (9+): modernize wants to use [trailing return type](https://clang.llvm.org/extra/clang-tidy/checks/modernize-use-trailing-return-type.html) but Fuchsia [disallows it](https://clang.llvm.org/extra/clang-tidy/checks/fuchsia-trailing-return.html).
+[^2]: Be careful with `-checks=*`; some checks can have self-contradictory rules in newer versions of LLVM (9+). For
+    example, modernize wants to use [trailing return type][] but Fuchsia [disallows it][].
 
+[trailing return type]: https://clang.llvm.org/extra/clang-tidy/checks/modernize-use-trailing-return-type.html
+
+[disallows it]: https://clang.llvm.org/extra/clang-tidy/checks/fuchsia-trailing-return.html
 
 ### The '--' doubledash option
 
 Options after `--` like `-std=c++11` will be interpreted correctly for `clang-tidy`. Make sure they sequentially follow
 the `--` argument in the hook's args list.
 
-
 ### Standalone Hooks
 
 If you want to have predictable return codes for your C linters outside of pre-commit, these hooks are available via
 [PyPI](https://pypi.org/project/cmake-pre-commit-hooks/).  Install it with `pip install cmake-pre-commit-hooks`.  They
 are named as `cmake-pc-$cmd-hook`, so `clang-format` becomes `cmake-pc-clang-format-hook`.
```

### Comparing `cmake_pre_commit_hooks-1.8.1/README.md` & `cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,142 +1,186 @@
+Metadata-Version: 2.1
+Name: cmake-pre-commit-hooks
+Version: 1.9.0
+Summary: pre-commit hooks for CMake based projects
+Home-page: https://github.com/Takishima/cmake-pre-commit-hooks
+Author: Damien Nguyen
+Author-email: ngn.damien@gmail.com
+License: Apache2
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: clang-format
+Provides-Extra: lizard
+Provides-Extra: test
+License-File: LICENSE
+
 # pre-commit hooks
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cmake-pre-commit-hooks?label=Python) [![PyPI version](https://badge.fury.io/py/cmake-pre-commit-hooks.svg)](https://badge.fury.io/py/cmake-pre-commit-hooks) [![CI Build](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml) [![CodeQL](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Takishima/cmake-pre-commit-hooks/main.svg)](https://results.pre-commit.ci/latest/github/Takishima/cmake-pre-commit-hooks/main) [![CodeFactor](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks/badge)](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Takishima_cmake-pre-commit-hooks&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Takishima_cmake-pre-commit-hooks)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cmake-pre-commit-hooks?label=Python) [![PyPI version](https://badge.fury.io/py/cmake-pre-commit-hooks.svg)](https://badge.fury.io/py/cmake-pre-commit-hooks) [![CI Build](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml) [![CodeQL](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Takishima/cmake-pre-commit-hooks/main.svg)](https://results.pre-commit.ci/latest/github/Takishima/cmake-pre-commit-hooks/main) [![CodeFactor](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks/badge)](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Takishima_cmake-pre-commit-hooks\&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Takishima_cmake-pre-commit-hooks)[![Codacy Badge](https://api.codacy.com/project/badge/Grade/a3a1139e4bed4d4694bb12991b7df775)](https://app.codacy.com/gh/Takishima/cmake-pre-commit-hooks?utm_source=github.com\&utm_medium=referral\&utm_content=Takishima/cmake-pre-commit-hooks\&utm_campaign=Badge_Grade)
 
+This is a [pre-commit](https://pre-commit.com) hooks repo that integrates C/C++ linters/formatters to work with
+CMake-based projects.
 
-This is a [pre-commit](https://pre-commit.com) hooks repo that integrates C/C++ linters/formatters to work with CMake-based projects.
 > [clang-format](https://clang.llvm.org/docs/ClangFormatStyleOptions.html),
-[clang-tidy](https://clang.llvm.org/extra/clang-tidy/),
-[cppcheck](http://cppcheck.sourceforge.net/),
-[cpplint](https://github.com/cpplint/cpplint),
-[lizard](http://www.lizard.ws) and
-[iwyu](https://include-what-you-use.org/)
+> [clang-tidy](https://clang.llvm.org/extra/clang-tidy/),
+> [cppcheck](http://cppcheck.sourceforge.net/),
+> [cpplint](https://github.com/cpplint/cpplint),
+> [lizard](http://www.lizard.ws) and
+> [iwyu](https://include-what-you-use.org/)
 
 It is largely based on the work found [here](https://github.com/pocc/pre-commit-hooks). The main difference with POCC's
 pre-commit hooks is that the ones from this repository will do a CMake configuration step prior to running any
 pre-commit hooks. This is done in order to have CMake generate the compilation database file that can then be used by
 the various hooks (using the `-DCMAKE_EXPORT_COMPILE_COMMANDS=ON` CMake option).
 
 This repository is only has Python-based pre-commit hooks.
 
 ## Current known issues
 
-Currently, the hooks that depend on having a compilation database generated by CMake (e.g. `clang-tidy`, `cppcheck`) are
-not working on Windows if you are not using the `Ninja` or `Makefile` generators.
+1.  Currently, the hooks that depend on having a compilation database generated by CMake (e.g. `clang-tidy`, `cppcheck`)
+    are not working on Windows if you are not using the `Ninja` or `Makefile` generators.
 
+2.  Currently, arguments set in a TOML configuration file (`pyproject.toml`, `cmake_pc_hooks.toml` or else) are applied
+    to all hooks. Future improvements may allow to customize arguments on a per-hook basis.
 
 ## Example usage
 
 Assuming that you have the following directory structure for your projects
 
-    root
-    ├── .pre-commit-config.yaml
-    ├── CMakeLists.txt
-    └── src
-        └── err.cpp
+```text
+root
+├── .pre-commit-config.yaml
+├── CMakeLists.txt
+└── src
+    └── err.cpp
+```
 
 with the following file contents:
 
-__.pre-commit-config.yaml__
-
-    repos:
-      - repo: https://github.com/Takishima/cmake-pre-commit-hooks
-        rev: v1.8.0
-        hooks:
-          - id: clang-format
-          - id: clang-tidy
-            args: [--checks=readability-magic-numbers,--warnings-as-errors=*]
-          - id: cppcheck
-          - id: include-what-you-use
+**.pre-commit-config.yaml**
 
+```yaml
+repos:
+  - repo: https://github.com/Takishima/cmake-pre-commit-hooks
+    rev: v1.8.0
+    hooks:
+      - id: clang-format
+      - id: clang-tidy
+        args: [--checks=readability-magic-numbers,--warnings-as-errors=*]
+      - id: cppcheck
+      - id: include-what-you-use
+```
 
-__CMakeLists.txt__
+**CMakeLists.txt**
 
-    cmake_minimum_required(VERSION 3.15)
-    project(LANGUAGE CXX)
-    add_library(mylib STATIC src/err.cpp)
+```cmake
+cmake_minimum_required(VERSION 3.15)
+project(LANGUAGE CXX)
+add_library(mylib STATIC src/err.cpp)
+```
 
-__src/err.cpp__
+**src/err.cpp**
 
-    #include <string>
-    int main() { int i; return 10; }
+```cpp
+#include <string>
+int main() { int i; return 10; }
+```
 
 Running pre-commit on the above project will lead to an output similar to this one:
 
-    $ pre-commit run --all-files
-    clang-format.............................................................Failed
-    - hook id: clang-format
-    - exit code: 1
-
-    src/err.cpp
-    ====================
-    <  int main() { int i; return 10; }
-    ---
-    >  int main() {
-    >    int i;
-    >    return 10;
-    >  }
-
-    clang-tidy...............................................................Failed
-    - hook id: clang-tidy
-    - exit code: 1
-
-    /tmp/temp/src/err.cpp:2:28: error: 10 is a magic number; consider replacing it with a named constant [readability-magic-numbers,-warnings-as-errors]
-    int main() { int i; return 10; }
-                               ^
-
-    cppcheck.................................................................Failed
-    - hook id: cppcheck
-    - exit code: 1
-
-    /tmp/temp/src/err.cpp:2:18: style: Unused variable: i [unusedVariable]
-    int main() { int i; return 10; }
-                     ^
-    include-what-you-use.....................................................Failed
-    - hook id: include-what-you-use
-    - exit code: 1
-
-    Problem with /usr/local/bin/iwyu_tool.py: Include-What-You-Use violations found
-
-    /tmp/temp/src/err.cpp should add these lines:
-    /tmp/temp/src/err.cpp should remove these lines:
-    - #include <string>  // lines 1-1
-    The full include-list for /tmp/temp/src/err.cpp:
-    ---
+```text
+$ pre-commit run --all-files
+clang-format.............................................................Failed
+- hook id: clang-format
+- exit code: 1
+
+src/err.cpp
+====================
+<  int main() { int i; return 10; }
+---
+>  int main() {
+>    int i;
+>    return 10;
+>  }
+
+clang-tidy...............................................................Failed
+- hook id: clang-tidy
+- exit code: 1
+
+/tmp/temp/src/err.cpp:2:28: error: 10 is a magic number; consider replacing it with a named constant [readability-magic-numbers,-warnings-as-errors]
+int main() { int i; return 10; }
+                           ^
+
+cppcheck.................................................................Failed
+- hook id: cppcheck
+- exit code: 1
+
+/tmp/temp/src/err.cpp:2:18: style: Unused variable: i [unusedVariable]
+int main() { int i; return 10; }
+                 ^
+include-what-you-use.....................................................Failed
+- hook id: include-what-you-use
+- exit code: 1
+
+Problem with /usr/local/bin/iwyu_tool.py: Include-What-You-Use violations found
+
+/tmp/temp/src/err.cpp should add these lines:
+/tmp/temp/src/err.cpp should remove these lines:
+- #include <string>  // lines 1-1
+The full include-list for /tmp/temp/src/err.cpp:
+---
+```
 
 Note that your mileage may vary depending on the version of the tools. The example above was generated using
 `clang-format` 12.0.0, `clang-tidy` 12.0.0, `cppcheck` 2.4.1 and `include-what-you-use` 0.16.
 
 ## Using the Hooks
 
-Python 3.6+ is required to use these hooks as all 3 invoking scripts are written in it. As this is also the minimum
+Python 3.8+ is required to use these hooks as all 3 invoking scripts are written in it. As this is also the minimum
 version of pre-commit, this should not be an issue.
 
 Running multiple hooks in parallel is currently supported by using the `fastener` Python package. If the hooks are run
 in parallel, only one of the hooks will run the CMake configure step while the others will simply wait until the call to
 CMake ends to continue. In the case where the hooks are run serially, all the hooks will be running the CMake configure
 step. However, if nothing changed in your CMake configuration, this should not cost too much time.
 
-
 ### Installation
 
 For installing the various utilities, refer to your package manager documentation. Some guidance can also be found
 [here](https://github.com/pocc/pre-commit-hooks#installation).
 
-
 ### Hook Info
 
-| Hook Info                                                                | Type                     | Languages        |
-|--------------------------------------------------------------------------|--------------------------|------------------|
-| [clang-format](https://clang.llvm.org/docs/ClangFormatStyleOptions.html) | Formatter                | C, C++, ObjC     |
-| [clang-tidy](https://clang.llvm.org/extra/clang-tidy/)                   | Static code analyzer     | C, C++, ObjC     |
-| [cppcheck](http://cppcheck.sourceforge.net/)                             | Static code analyzer     | C, C++           |
-| [cpplint](https://github.com/cpplint/cpplint)                            | Static code analyzer     | C, C++           |
-| [include-what-you-use](https://include-what-you-use.org/)                | Static code analyzer     | C, C++           |
-| [lizard](http://www.lizard.ws)                                           | code complexity analyzer | C/C++, ObjC, ... |
+| Hook Info                | Type                     | Languages        |
+|--------------------------|--------------------------|------------------|
+| [clang-format][]         | Formatter                | C, C++, ObjC     |
+| [clang-tidy][]           | Static code analyzer     | C, C++, ObjC     |
+| [cppcheck][]             | Static code analyzer     | C, C++           |
+| [cpplint][]              | Static code analyzer     | C, C++           |
+| [include-what-you-use][] | Static code analyzer     | C, C++           |
+| [lizard][]               | Code complexity analyzer | C/C++, ObjC, ... |
+
+[clang-format]: https://clang.llvm.org/docs/ClangFormatStyleOptions.html
+
+[clang-tidy]: https://clang.llvm.org/extra/clang-tidy/
+
+[cppcheck]: http://cppcheck.sourceforge.net/
+
+[cpplint]: https://github.com/cpplint/cpplint
+
+[include-what-you-use]: https://include-what-you-use.org/
+
+[lizard]: http://www.lizard.ws
 
 ### Hook options
 
 Since v1.1.0 all hooks that depend on a compilation database (e.g. `clang-tidy`, `cppcheck`, `include-what-you-use`)
 will attempt to generate a CMake build directory before running the actual command.
 
 These hooks accept all the most common CMake options:
@@ -160,35 +204,38 @@
 argument (`-B`) multiple times. The hooks will then simply cycle through all of the values provided and choose the first
 directory that contains a configured CMake project (by looking at the presence of the `CMakeCache.txt` file). This may
 be useful if you already have a build directory available somewhere that you would like to re-use. In the case where
 none of the provided options is viable, the first one will automatically be selected as the build directory.
 
 In addition to the above CMake options, the hooks also accept the following:
 
-| Other hook options           | Description                                      | Note         |
-|------------------------------|--------------------------------------------------|--------------|
-| `--all-at-once`              | Pass all filenames to the command at once        | Since v1.4.0 |
-| `--read-json-db`             | Append file list from compile database           | Since v1.7.0 |
-| `--cmake`                    | Specify path to CMake executable                 | Since v1.4.0 |
-| `--linux`                    | Linux-only CMake options                         | Since v1.3.0 |
-| `--mac`                      | MacOS-only CMake options                         | Since v1.3.0 |
-| `--win`                      | Windows-only CMake options                       | Since v1.3.0 |
+| Other hook options           | Description                                            | Note         |
+|------------------------------|--------------------------------------------------------|--------------|
+| `--all-at-once`              | Pass all filenames to the command at once              | Since v1.4.0 |
+| `--clean`                    | Perform a clean CMake build                            | Since v1.4.0 |
+| `--cmake`                    | Specify path to CMake executable                       | Since v1.4.0 |
+| `--detect-configured-files`  | Enable cmake tracing and detection of configured files | Since v1.9.0 |
+| `--dump-toml`                | Dump the current configuration as TOML on stdout       | Since v1.9.0 |
+| `--no-automatic-discovery`   | Disable automatic build directory discovery            | Since v1.9.0 |
+| `--read-json-db`             | Append file list from compile database                 | Since v1.7.0 |
+| `--linux`                    | Linux-only CMake options                               | Since v1.3.0 |
+| `--mac`                      | MacOS-only CMake options                               | Since v1.3.0 |
+| `--win`                      | Windows-only CMake options                             | Since v1.3.0 |
 
 NB: by specifying `--all-at-once` the linter/formatter command will only be called once for all the files instead of
 calling the command once per file.
 
 NB: Since v1.6.0, the `--debug` command line argument has been removed. Use the `LOGLEVEL` environment variable instead
 to control the level of verbosity of each of the commands. To show all debug messages, set `LOGLEVEL=DEBUG` in your
 environment variables when running the hooks.
 
 NB: by specifying `--read-json-db` the hook will read the list of files from the `compile_commands.json` generated by
 CMake and will append those files to the list of files to process regardless of the list of files otherwise passed on
 the command line.
 
-
 Usage example:
 
 ```yaml
 repos:
 - repo: https://github.com/Takishima/cmake-pre-commit-hooks
   rev: v1.8.0
   hooks:
@@ -207,32 +254,74 @@
 that contains some CMake cache files), then it will be used. If none qualify, the hooks will default to using
 `path/to/build_dir` as a build directory, creating it as necessary.
 
 Also, builds on Linux and MacOS will set the C++ compiler to `g++-10`, while builds on Windows will be using
 `cl.exe`. This is done by looking at the value returned by
 [`platform.system()`](https://docs.python.org/3/library/platform.html#platform.system).
 
+### TOML support
+
+Since v1.9.0, the hooks support loading the CLI arguments from TOML files. This can be used to configure all the hooks
+for a particular repository using either of:
+
+1.  `pyproject.toml`
+2.  `cmake_pc_hooks.toml`
+3.  TOML file specified using `--config=/path/to/file.toml`
+4.  Command line arguments
+
+Note that each step in the above list is overridden by the steps that happen **after** it. For example, CLI arguments
+will always override any arguments read from any TOML file.
+
+A good place to start if you plan on creating a TOML configuration file is to use the hooks using the CLI arguments as
+you would normally and then run the hook manually and with the addition of `--dump-toml`. This will output a
+TOML-formatted configuration on the standard output for all the parameters that *diverge* from their default values.
+
+For example, running the following command (assuming that no valid TOML configuration exists):
+
+```bash
+cmake-pc-clang-format-hook tests/cmake_bad/bad.cpp  --dump-toml -B /tmp/build -S source -Wdev --no-automatic-discovery
+```
+
+will result in the following output:
+
+```toml
+automatic_discovery = false
+source_dir = "source"
+build_dir = [ "/tmp/build",]
+dev_warnings = true
+```
+
+### CMake configured file detection
+
+Since v1.9.0, the hooks support the use of CMake with trace mode enabled in order to keep track of files that are
+generated using calls to the `configure_file(...)` CMake function. If `--detect-configured-files` is specified on the
+command line (or in some TOML configuration file), the hooks will attempt to locate those generated files and
+automatically add them to the list of processed files for any hook invocation.
+
 ### Hook Option Comparison
 
-| Hook Options                                                             | Fix In Place       | Enable all Checks                       | Set key/value |
-|--------------------------------------------------------------------------|--------------------|-----------------------------------------|---------------|
-| [clang-format](https://clang.llvm.org/docs/ClangFormatStyleOptions.html) | `-i`               |                                         |               |
-| [clang-tidy](https://clang.llvm.org/extra/clang-tidy/)                   | `--fix-errors` [1] | `-checks=*` `-warnings-as-errors=*` [2] |               |
-| [cppcheck](http://cppcheck.sourceforge.net/)                             |                    | `-enable=all`                           |               |
-| [include-what-you-use](https://include-what-you-use.org/)                |                    |                                         |               |
+| Hook Options             | Fix In Place        | Enable all Checks                        | Set key/value |
+|--------------------------|---------------------|------------------------------------------|---------------|
+| [clang-format][]         | `-i`                |                                          |               |
+| [clang-tidy][]           | `--fix-errors` [^1] | `-checks=*` `-warnings-as-errors=*` [^2] |               |
+| [cppcheck][]             |                     | `-enable=all`                            |               |
+| [include-what-you-use][] |                     |                                          |               |
 
-[1]: `-fix` will fail if there are compiler errors. `-fix-errors` will `-fix` and fix compiler errors if it can, like missing semicolons.
+[^1]: `-fix` will fail if there are compiler errors. `-fix-errors` will `-fix` and fix compiler errors if it can, like missing semicolons.
 
-[2]: Be careful with `-checks=*`.  can have self-contradictory rules in newer versions of llvm (9+): modernize wants to use [trailing return type](https://clang.llvm.org/extra/clang-tidy/checks/modernize-use-trailing-return-type.html) but Fuchsia [disallows it](https://clang.llvm.org/extra/clang-tidy/checks/fuchsia-trailing-return.html).
+[^2]: Be careful with `-checks=*`; some checks can have self-contradictory rules in newer versions of LLVM (9+). For
+    example, modernize wants to use [trailing return type][] but Fuchsia [disallows it][].
 
+[trailing return type]: https://clang.llvm.org/extra/clang-tidy/checks/modernize-use-trailing-return-type.html
+
+[disallows it]: https://clang.llvm.org/extra/clang-tidy/checks/fuchsia-trailing-return.html
 
 ### The '--' doubledash option
 
 Options after `--` like `-std=c++11` will be interpreted correctly for `clang-tidy`. Make sure they sequentially follow
 the `--` argument in the hook's args list.
 
-
 ### Standalone Hooks
 
 If you want to have predictable return codes for your C linters outside of pre-commit, these hooks are available via
 [PyPI](https://pypi.org/project/cmake-pre-commit-hooks/).  Install it with `pip install cmake-pre-commit-hooks`.  They
 are named as `cmake-pc-$cmd-hook`, so `clang-format` becomes `cmake-pc-clang-format-hook`.
```

### Comparing `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/__init__.py` & `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,7 +7,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+"""Main module for cmake-pre-commit-hooks."""
```

### Comparing `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/clang_format.py` & `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/clang_format.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 
 from ._utils import FormatterCmd
 
 
 class ClangFormatCmd(FormatterCmd):
     """Class for the ClangFormat command."""
 
-    command = "clang-format"
-    lookbehind = "clang-format version "
+    command = 'clang-format'
+    lookbehind = 'clang-format version '
 
     def __init__(self, args):
         """Initialize a ClangFormatCmd object."""
         super().__init__(self.command, self.lookbehind, args)
         self.check_installed()
         self.parse_args(args)
         self.set_diff_flag()
-        self.edit_in_place = "-i" in self.args
+        self.edit_in_place = '-i' in self.args
 
     def run(self):
         """Run clang-format. Error if diff is incorrect."""
         for filename in self.files:
             self.compare_to_formatted(filename)
         if self.returncode != 0:
             sys.stdout.buffer.write(self.stderr)
@@ -51,9 +51,9 @@
     """
     if argv is None:
         argv = sys.argv
     cmd = ClangFormatCmd(argv)
     cmd.run()
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':  # pragma: nocover
     main()
```

### Comparing `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/clang_tidy.py` & `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/clang_tidy.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 
 from ._utils import ClangAnalyzerCmd
 
 
 class ClangTidyCmd(ClangAnalyzerCmd):
     """Class for the clang-tidy command."""
 
-    command = "clang-tidy"
-    lookbehind = "LLVM version "
+    command = 'clang-tidy'
+    lookbehind = 'LLVM version '
 
     def __init__(self, args):
         """Initialize a ClangTidyCmd object."""
         super().__init__(self.command, self.lookbehind, args)
         self.parse_args(args)
-        self.edit_in_place = "-fix" in self.args or "--fix-errors" in self.args
+        self.edit_in_place = '-fix' in self.args or '--fix-errors' in self.args
         self.handle_ddash_args()
 
         # Force location of compile database
-        self.add_if_missing([f'-p={Path(self.build_dir, "compile_commands.json")}'])
+        self.add_if_missing([f'-p={Path(self.cmake.build_dir, "compile_commands.json")}'])
 
     def _parse_output(self, result):
         """
         Parse output and check whether some errors occurred.
 
         Args:
             result (namedtuple): Result from calling a command
@@ -73,9 +73,9 @@
     """
     if argv is None:
         argv = sys.argv
     cmd = ClangTidyCmd(argv)
     cmd.run()
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':  # pragma: nocover
     main()
```

### Comparing `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/cppcheck.py` & `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/cppcheck.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,51 +14,60 @@
 
 """Wrapper script for cppcheck."""
 
 import logging
 import sys
 from pathlib import Path
 
+from . import _call_process
 from ._utils import Command
 
 
 class CppcheckCmd(Command):
     """Class for the cppcheck command."""
 
-    command = "cppcheck"
-    lookbehind = "Cppcheck "
+    command = 'cppcheck'
+    lookbehind = 'Cppcheck '
 
     def __init__(self, args):
         """Initialize a CppcheckCmd object."""
         super().__init__(self.command, self.lookbehind, args)
         self.parse_args(args)
         # quiet for stdout purposes
-        self.add_if_missing(["-q"])
+        self.add_if_missing(['-q'])
         # make cppcheck behave as expected for pre-commit
-        self.add_if_missing(["--error-exitcode=1"])
+        self.add_if_missing(['--error-exitcode=1'])
         # Enable all of the checks
-        self.add_if_missing(["--enable=all"])
+        self.add_if_missing(['--enable=all'])
         # Force location of compile database
-        self.add_if_missing([f'--project={Path(self.build_dir, "compile_commands.json")}'])
+        self.add_if_missing([f'--project={Path(self.cmake.build_dir, "compile_commands.json")}'])
+
+    def run_command(self, filenames):
+        """Run the command and check for errors."""
+        filter_args = [f'--file-filter=*{Path(filename).parent.name}/{Path(filename).name}' for filename in filenames]
+        self.history.append(_call_process.call_process([self.command, *filter_args, *self.args, *self.ddash_args]))
+        self._clinters_compat()
 
     def _parse_output(self, result):
         """
         Parse output and check whether some errors occurred.
 
         Args:
             result (namedtuple): Result from calling a command
 
         Returns:
             False if no errors were detected, True in all other cases.
         """
         # Useless error see https://stackoverflow.com/questions/6986033
         logging.debug('parsing output from %s', result.stderr)
-        useless_error_part = "Cppcheck cannot find all the include files"
-        result.stderr = [line for line in result.stderr.splitlines(keepends=True) if useless_error_part not in line]
-
+        useless_error_part = 'Cppcheck cannot find all the include files'
+        result.stderr = ''.join(
+            [line for line in result.stderr.splitlines(keepends=True) if useless_error_part not in line]
+        )
+        self._clinters_compat()
         return result.returncode != 0
 
 
 def main(argv=None):
     """
     Run command.
 
@@ -67,9 +76,9 @@
     """
     if argv is None:
         argv = sys.argv
     cmd = CppcheckCmd(argv)
     cmd.run()
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':  # pragma: nocover
     main()
```

### Comparing `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/cpplint.py` & `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/cpplint.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Wrapper script for cpplint."""
 
 from hooks.cpplint import main
 
-if __name__ == '__main__':
+if __name__ == '__main__':  # pragma: nocover
     main()
```

### Comparing `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/include_what_you_use.py` & `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/include_what_you_use.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Wrapper script for cppcheck."""
 
 import logging
-import re
 import shutil
 import sys
 from pathlib import Path
 
 from ._utils import ClangAnalyzerCmd
 
 
@@ -64,55 +63,35 @@
     # Nothing worked -> give up!
     return None
 
 
 class IWYUToolCmd(ClangAnalyzerCmd):
     """Class for the iwyu_tool.py command."""
 
-    command = get_iwyu_tool_command()
-    command_for_version = get_iwyu_command()
-    lookbehind = "include-what-you-use "
+    command = None
+    command_for_version = None
+    lookbehind = 'include-what-you-use '
 
     def __init__(self, args):
         """Initialize an IWYUToolCmd object."""
-        if self.command is None:
-            raise RuntimeError('Unable to locate path to iwyu-tool')
-        if self.command_for_version is None:
-            raise RuntimeError('Unable to locate path to include-what-you-use executable!')
+        IWYUToolCmd.command = get_iwyu_tool_command()
+        IWYUToolCmd.command_for_version = get_iwyu_command()
+
+        if IWYUToolCmd.command is None:
+            raise FileNotFoundError('Unable to locate path to iwyu-tool')
+        if IWYUToolCmd.command_for_version is None:
+            raise FileNotFoundError('Unable to locate path to include-what-you-use executable!')
 
         super().__init__(self.command, self.lookbehind, args)
-        self.file_regex = ""
         self.check_installed()
         self.parse_args(args)
         self.handle_ddash_args()
 
         # Force location of compile database
-        self.add_if_missing([f'-p={Path(self.build_dir, "compile_commands.json")}'])
-
-    def get_version_str(self):
-        """Get the version string like 8.0.0 for a given command."""
-        result = self._call_process([self.command_for_version, '--version'])
-        logging.debug('string for version: %s', result)
-        version_str = result.stdout
-
-        # After version like `8.0.0` is expected to be '\n' or ' '
-        if not re.search(self.look_behind, version_str):
-            self.raise_error(
-                'getting version',
-                'The version format for this command has changed. Create an issue at '
-                'github.com/Takishima/cmake-pre-commit-hooks.',
-            )
-        regex = self.look_behind + r'((?:\d+\.)+[\d+_\+\-a-z]+)'
-        version = re.search(regex, version_str).group(1)
-        logging.debug('extracted version: %s', version)
-        return version
-
-    def set_file_regex(self):
-        """Get the file regex for a command's target files from the .pre-commit-hooks.yaml."""
-        self.file_regex = r".*\.(?:c|cc|cxx|cpp|cu|h|hpp|hxx)$"
+        self.add_if_missing([f'-p={Path(self.cmake.build_dir, "compile_commands.json")}'])
 
     def _parse_output(self, result):
         """
         Parse output and check whether some errors occurred.
 
         Args:
             result (namedtuple): Result from calling a command
@@ -120,17 +99,17 @@
         Returns:
             False if no errors were detected, True in all other cases.
 
         Notes:
             Include-What-You-Use return code is never 0
         """
         logging.debug('parsing output from %s', result.stdout)
-        is_correct = "has correct #includes/fwd-decls" in result.stdout
+        is_correct = 'has correct #includes/fwd-decls' in result.stdout
 
-        return result.stdout and not is_correct
+        return bool(result.stdout) and not is_correct
 
 
 def main(argv=None):
     """
     Run command.
 
     Args:
@@ -138,9 +117,9 @@
     """
     if argv is None:
         argv = sys.argv
     cmd = IWYUToolCmd(argv)
     cmd.run()
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':  # pragma: nocover
     main()
```

### Comparing `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/lizard.py` & `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/lizard.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,40 +19,35 @@
 
 from ._utils import StaticAnalyzerCmd, _read_compile_commands_json
 
 
 class LizardCmd(StaticAnalyzerCmd):
     """Class for the lizard command."""
 
-    command = "lizard"
-    lookbehind = ""
+    command = 'lizard'
+    lookbehind = ''
 
     def __init__(self, args):
         """Initialize a LizardCmd object."""
         super().__init__(self.command, self.lookbehind, args)
-        self.file_regex = ""
         self.parse_args(args)
 
-    def set_file_regex(self):
-        """Get the file regex for a command's target files from the .pre-commit-hooks.yaml."""
-        self.file_regex = r".*\.(?:c|cc|cxx|cpp|cu|h|hpp|hxx|py)$"
-
     def run(self):
         """Run lizard."""
         if self.read_json_db:
-            self.run_cmake_configure()
-            self.files.extend(set(self.files).symmetric_difference(set(_read_compile_commands_json(self.build_dir))))
+            self.cmake.configure(self.command)
+            self.files.extend(set(_read_compile_commands_json(self.cmake.build_dir)) - set(self.files))
 
         if self.all_at_once:
             self.run_command(self.files)
             self.exit_on_error()
         else:
             for filename in self.files:
                 self.run_command([filename])
-                self.exit_on_error()
+            self.exit_on_error()
 
 
 def main(argv=None):
     """
     Run command.
 
     Args:
@@ -60,9 +55,9 @@
     """
     if argv is None:
         argv = sys.argv
     cmd = LizardCmd(argv)
     cmd.run()
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':  # pragma: nocover
     main()
```

### Comparing `cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/PKG-INFO` & `cmake_pre_commit_hooks-1.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cmake-pre-commit-hooks
-Version: 1.8.1
+Name: cmake_pre_commit_hooks
+Version: 1.9.0
 Summary: pre-commit hooks for CMake based projects
 Home-page: https://github.com/Takishima/cmake-pre-commit-hooks
 Author: Damien Nguyen
 Author-email: ngn.damien@gmail.com
 License: Apache2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -13,151 +13,174 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: clang-format
 Provides-Extra: lizard
+Provides-Extra: test
 License-File: LICENSE
 
 # pre-commit hooks
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cmake-pre-commit-hooks?label=Python) [![PyPI version](https://badge.fury.io/py/cmake-pre-commit-hooks.svg)](https://badge.fury.io/py/cmake-pre-commit-hooks) [![CI Build](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml) [![CodeQL](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Takishima/cmake-pre-commit-hooks/main.svg)](https://results.pre-commit.ci/latest/github/Takishima/cmake-pre-commit-hooks/main) [![CodeFactor](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks/badge)](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Takishima_cmake-pre-commit-hooks&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Takishima_cmake-pre-commit-hooks)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cmake-pre-commit-hooks?label=Python) [![PyPI version](https://badge.fury.io/py/cmake-pre-commit-hooks.svg)](https://badge.fury.io/py/cmake-pre-commit-hooks) [![CI Build](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/ci.yml) [![CodeQL](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Takishima/cmake-pre-commit-hooks/actions/workflows/codeql-analysis.yml) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Takishima/cmake-pre-commit-hooks/main.svg)](https://results.pre-commit.ci/latest/github/Takishima/cmake-pre-commit-hooks/main) [![CodeFactor](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks/badge)](https://www.codefactor.io/repository/github/takishima/cmake-pre-commit-hooks) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Takishima_cmake-pre-commit-hooks\&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Takishima_cmake-pre-commit-hooks)[![Codacy Badge](https://api.codacy.com/project/badge/Grade/a3a1139e4bed4d4694bb12991b7df775)](https://app.codacy.com/gh/Takishima/cmake-pre-commit-hooks?utm_source=github.com\&utm_medium=referral\&utm_content=Takishima/cmake-pre-commit-hooks\&utm_campaign=Badge_Grade)
 
+This is a [pre-commit](https://pre-commit.com) hooks repo that integrates C/C++ linters/formatters to work with
+CMake-based projects.
 
-This is a [pre-commit](https://pre-commit.com) hooks repo that integrates C/C++ linters/formatters to work with CMake-based projects.
 > [clang-format](https://clang.llvm.org/docs/ClangFormatStyleOptions.html),
-[clang-tidy](https://clang.llvm.org/extra/clang-tidy/),
-[cppcheck](http://cppcheck.sourceforge.net/),
-[cpplint](https://github.com/cpplint/cpplint),
-[lizard](http://www.lizard.ws) and
-[iwyu](https://include-what-you-use.org/)
+> [clang-tidy](https://clang.llvm.org/extra/clang-tidy/),
+> [cppcheck](http://cppcheck.sourceforge.net/),
+> [cpplint](https://github.com/cpplint/cpplint),
+> [lizard](http://www.lizard.ws) and
+> [iwyu](https://include-what-you-use.org/)
 
 It is largely based on the work found [here](https://github.com/pocc/pre-commit-hooks). The main difference with POCC's
 pre-commit hooks is that the ones from this repository will do a CMake configuration step prior to running any
 pre-commit hooks. This is done in order to have CMake generate the compilation database file that can then be used by
 the various hooks (using the `-DCMAKE_EXPORT_COMPILE_COMMANDS=ON` CMake option).
 
 This repository is only has Python-based pre-commit hooks.
 
 ## Current known issues
 
-Currently, the hooks that depend on having a compilation database generated by CMake (e.g. `clang-tidy`, `cppcheck`) are
-not working on Windows if you are not using the `Ninja` or `Makefile` generators.
+1.  Currently, the hooks that depend on having a compilation database generated by CMake (e.g. `clang-tidy`, `cppcheck`)
+    are not working on Windows if you are not using the `Ninja` or `Makefile` generators.
 
+2.  Currently, arguments set in a TOML configuration file (`pyproject.toml`, `cmake_pc_hooks.toml` or else) are applied
+    to all hooks. Future improvements may allow to customize arguments on a per-hook basis.
 
 ## Example usage
 
 Assuming that you have the following directory structure for your projects
 
-    root
-    ├── .pre-commit-config.yaml
-    ├── CMakeLists.txt
-    └── src
-        └── err.cpp
+```text
+root
+├── .pre-commit-config.yaml
+├── CMakeLists.txt
+└── src
+    └── err.cpp
+```
 
 with the following file contents:
 
-__.pre-commit-config.yaml__
-
-    repos:
-      - repo: https://github.com/Takishima/cmake-pre-commit-hooks
-        rev: v1.8.0
-        hooks:
-          - id: clang-format
-          - id: clang-tidy
-            args: [--checks=readability-magic-numbers,--warnings-as-errors=*]
-          - id: cppcheck
-          - id: include-what-you-use
+**.pre-commit-config.yaml**
 
+```yaml
+repos:
+  - repo: https://github.com/Takishima/cmake-pre-commit-hooks
+    rev: v1.8.0
+    hooks:
+      - id: clang-format
+      - id: clang-tidy
+        args: [--checks=readability-magic-numbers,--warnings-as-errors=*]
+      - id: cppcheck
+      - id: include-what-you-use
+```
 
-__CMakeLists.txt__
+**CMakeLists.txt**
 
-    cmake_minimum_required(VERSION 3.15)
-    project(LANGUAGE CXX)
-    add_library(mylib STATIC src/err.cpp)
+```cmake
+cmake_minimum_required(VERSION 3.15)
+project(LANGUAGE CXX)
+add_library(mylib STATIC src/err.cpp)
+```
 
-__src/err.cpp__
+**src/err.cpp**
 
-    #include <string>
-    int main() { int i; return 10; }
+```cpp
+#include <string>
+int main() { int i; return 10; }
+```
 
 Running pre-commit on the above project will lead to an output similar to this one:
 
-    $ pre-commit run --all-files
-    clang-format.............................................................Failed
-    - hook id: clang-format
-    - exit code: 1
-
-    src/err.cpp
-    ====================
-    <  int main() { int i; return 10; }
-    ---
-    >  int main() {
-    >    int i;
-    >    return 10;
-    >  }
-
-    clang-tidy...............................................................Failed
-    - hook id: clang-tidy
-    - exit code: 1
-
-    /tmp/temp/src/err.cpp:2:28: error: 10 is a magic number; consider replacing it with a named constant [readability-magic-numbers,-warnings-as-errors]
-    int main() { int i; return 10; }
-                               ^
-
-    cppcheck.................................................................Failed
-    - hook id: cppcheck
-    - exit code: 1
-
-    /tmp/temp/src/err.cpp:2:18: style: Unused variable: i [unusedVariable]
-    int main() { int i; return 10; }
-                     ^
-    include-what-you-use.....................................................Failed
-    - hook id: include-what-you-use
-    - exit code: 1
-
-    Problem with /usr/local/bin/iwyu_tool.py: Include-What-You-Use violations found
-
-    /tmp/temp/src/err.cpp should add these lines:
-    /tmp/temp/src/err.cpp should remove these lines:
-    - #include <string>  // lines 1-1
-    The full include-list for /tmp/temp/src/err.cpp:
-    ---
+```text
+$ pre-commit run --all-files
+clang-format.............................................................Failed
+- hook id: clang-format
+- exit code: 1
+
+src/err.cpp
+====================
+<  int main() { int i; return 10; }
+---
+>  int main() {
+>    int i;
+>    return 10;
+>  }
+
+clang-tidy...............................................................Failed
+- hook id: clang-tidy
+- exit code: 1
+
+/tmp/temp/src/err.cpp:2:28: error: 10 is a magic number; consider replacing it with a named constant [readability-magic-numbers,-warnings-as-errors]
+int main() { int i; return 10; }
+                           ^
+
+cppcheck.................................................................Failed
+- hook id: cppcheck
+- exit code: 1
+
+/tmp/temp/src/err.cpp:2:18: style: Unused variable: i [unusedVariable]
+int main() { int i; return 10; }
+                 ^
+include-what-you-use.....................................................Failed
+- hook id: include-what-you-use
+- exit code: 1
+
+Problem with /usr/local/bin/iwyu_tool.py: Include-What-You-Use violations found
+
+/tmp/temp/src/err.cpp should add these lines:
+/tmp/temp/src/err.cpp should remove these lines:
+- #include <string>  // lines 1-1
+The full include-list for /tmp/temp/src/err.cpp:
+---
+```
 
 Note that your mileage may vary depending on the version of the tools. The example above was generated using
 `clang-format` 12.0.0, `clang-tidy` 12.0.0, `cppcheck` 2.4.1 and `include-what-you-use` 0.16.
 
 ## Using the Hooks
 
-Python 3.6+ is required to use these hooks as all 3 invoking scripts are written in it. As this is also the minimum
+Python 3.8+ is required to use these hooks as all 3 invoking scripts are written in it. As this is also the minimum
 version of pre-commit, this should not be an issue.
 
 Running multiple hooks in parallel is currently supported by using the `fastener` Python package. If the hooks are run
 in parallel, only one of the hooks will run the CMake configure step while the others will simply wait until the call to
 CMake ends to continue. In the case where the hooks are run serially, all the hooks will be running the CMake configure
 step. However, if nothing changed in your CMake configuration, this should not cost too much time.
 
-
 ### Installation
 
 For installing the various utilities, refer to your package manager documentation. Some guidance can also be found
 [here](https://github.com/pocc/pre-commit-hooks#installation).
 
-
 ### Hook Info
 
-| Hook Info                                                                | Type                     | Languages        |
-|--------------------------------------------------------------------------|--------------------------|------------------|
-| [clang-format](https://clang.llvm.org/docs/ClangFormatStyleOptions.html) | Formatter                | C, C++, ObjC     |
-| [clang-tidy](https://clang.llvm.org/extra/clang-tidy/)                   | Static code analyzer     | C, C++, ObjC     |
-| [cppcheck](http://cppcheck.sourceforge.net/)                             | Static code analyzer     | C, C++           |
-| [cpplint](https://github.com/cpplint/cpplint)                            | Static code analyzer     | C, C++           |
-| [include-what-you-use](https://include-what-you-use.org/)                | Static code analyzer     | C, C++           |
-| [lizard](http://www.lizard.ws)                                           | code complexity analyzer | C/C++, ObjC, ... |
+| Hook Info                | Type                     | Languages        |
+|--------------------------|--------------------------|------------------|
+| [clang-format][]         | Formatter                | C, C++, ObjC     |
+| [clang-tidy][]           | Static code analyzer     | C, C++, ObjC     |
+| [cppcheck][]             | Static code analyzer     | C, C++           |
+| [cpplint][]              | Static code analyzer     | C, C++           |
+| [include-what-you-use][] | Static code analyzer     | C, C++           |
+| [lizard][]               | Code complexity analyzer | C/C++, ObjC, ... |
+
+[clang-format]: https://clang.llvm.org/docs/ClangFormatStyleOptions.html
+
+[clang-tidy]: https://clang.llvm.org/extra/clang-tidy/
+
+[cppcheck]: http://cppcheck.sourceforge.net/
+
+[cpplint]: https://github.com/cpplint/cpplint
+
+[include-what-you-use]: https://include-what-you-use.org/
+
+[lizard]: http://www.lizard.ws
 
 ### Hook options
 
 Since v1.1.0 all hooks that depend on a compilation database (e.g. `clang-tidy`, `cppcheck`, `include-what-you-use`)
 will attempt to generate a CMake build directory before running the actual command.
 
 These hooks accept all the most common CMake options:
@@ -181,35 +204,38 @@
 argument (`-B`) multiple times. The hooks will then simply cycle through all of the values provided and choose the first
 directory that contains a configured CMake project (by looking at the presence of the `CMakeCache.txt` file). This may
 be useful if you already have a build directory available somewhere that you would like to re-use. In the case where
 none of the provided options is viable, the first one will automatically be selected as the build directory.
 
 In addition to the above CMake options, the hooks also accept the following:
 
-| Other hook options           | Description                                      | Note         |
-|------------------------------|--------------------------------------------------|--------------|
-| `--all-at-once`              | Pass all filenames to the command at once        | Since v1.4.0 |
-| `--read-json-db`             | Append file list from compile database           | Since v1.7.0 |
-| `--cmake`                    | Specify path to CMake executable                 | Since v1.4.0 |
-| `--linux`                    | Linux-only CMake options                         | Since v1.3.0 |
-| `--mac`                      | MacOS-only CMake options                         | Since v1.3.0 |
-| `--win`                      | Windows-only CMake options                       | Since v1.3.0 |
+| Other hook options           | Description                                            | Note         |
+|------------------------------|--------------------------------------------------------|--------------|
+| `--all-at-once`              | Pass all filenames to the command at once              | Since v1.4.0 |
+| `--clean`                    | Perform a clean CMake build                            | Since v1.4.0 |
+| `--cmake`                    | Specify path to CMake executable                       | Since v1.4.0 |
+| `--detect-configured-files`  | Enable cmake tracing and detection of configured files | Since v1.9.0 |
+| `--dump-toml`                | Dump the current configuration as TOML on stdout       | Since v1.9.0 |
+| `--no-automatic-discovery`   | Disable automatic build directory discovery            | Since v1.9.0 |
+| `--read-json-db`             | Append file list from compile database                 | Since v1.7.0 |
+| `--linux`                    | Linux-only CMake options                               | Since v1.3.0 |
+| `--mac`                      | MacOS-only CMake options                               | Since v1.3.0 |
+| `--win`                      | Windows-only CMake options                             | Since v1.3.0 |
 
 NB: by specifying `--all-at-once` the linter/formatter command will only be called once for all the files instead of
 calling the command once per file.
 
 NB: Since v1.6.0, the `--debug` command line argument has been removed. Use the `LOGLEVEL` environment variable instead
 to control the level of verbosity of each of the commands. To show all debug messages, set `LOGLEVEL=DEBUG` in your
 environment variables when running the hooks.
 
 NB: by specifying `--read-json-db` the hook will read the list of files from the `compile_commands.json` generated by
 CMake and will append those files to the list of files to process regardless of the list of files otherwise passed on
 the command line.
 
-
 Usage example:
 
 ```yaml
 repos:
 - repo: https://github.com/Takishima/cmake-pre-commit-hooks
   rev: v1.8.0
   hooks:
@@ -228,32 +254,74 @@
 that contains some CMake cache files), then it will be used. If none qualify, the hooks will default to using
 `path/to/build_dir` as a build directory, creating it as necessary.
 
 Also, builds on Linux and MacOS will set the C++ compiler to `g++-10`, while builds on Windows will be using
 `cl.exe`. This is done by looking at the value returned by
 [`platform.system()`](https://docs.python.org/3/library/platform.html#platform.system).
 
+### TOML support
+
+Since v1.9.0, the hooks support loading the CLI arguments from TOML files. This can be used to configure all the hooks
+for a particular repository using either of:
+
+1.  `pyproject.toml`
+2.  `cmake_pc_hooks.toml`
+3.  TOML file specified using `--config=/path/to/file.toml`
+4.  Command line arguments
+
+Note that each step in the above list is overridden by the steps that happen **after** it. For example, CLI arguments
+will always override any arguments read from any TOML file.
+
+A good place to start if you plan on creating a TOML configuration file is to use the hooks using the CLI arguments as
+you would normally and then run the hook manually and with the addition of `--dump-toml`. This will output a
+TOML-formatted configuration on the standard output for all the parameters that *diverge* from their default values.
+
+For example, running the following command (assuming that no valid TOML configuration exists):
+
+```bash
+cmake-pc-clang-format-hook tests/cmake_bad/bad.cpp  --dump-toml -B /tmp/build -S source -Wdev --no-automatic-discovery
+```
+
+will result in the following output:
+
+```toml
+automatic_discovery = false
+source_dir = "source"
+build_dir = [ "/tmp/build",]
+dev_warnings = true
+```
+
+### CMake configured file detection
+
+Since v1.9.0, the hooks support the use of CMake with trace mode enabled in order to keep track of files that are
+generated using calls to the `configure_file(...)` CMake function. If `--detect-configured-files` is specified on the
+command line (or in some TOML configuration file), the hooks will attempt to locate those generated files and
+automatically add them to the list of processed files for any hook invocation.
+
 ### Hook Option Comparison
 
-| Hook Options                                                             | Fix In Place       | Enable all Checks                       | Set key/value |
-|--------------------------------------------------------------------------|--------------------|-----------------------------------------|---------------|
-| [clang-format](https://clang.llvm.org/docs/ClangFormatStyleOptions.html) | `-i`               |                                         |               |
-| [clang-tidy](https://clang.llvm.org/extra/clang-tidy/)                   | `--fix-errors` [1] | `-checks=*` `-warnings-as-errors=*` [2] |               |
-| [cppcheck](http://cppcheck.sourceforge.net/)                             |                    | `-enable=all`                           |               |
-| [include-what-you-use](https://include-what-you-use.org/)                |                    |                                         |               |
+| Hook Options             | Fix In Place        | Enable all Checks                        | Set key/value |
+|--------------------------|---------------------|------------------------------------------|---------------|
+| [clang-format][]         | `-i`                |                                          |               |
+| [clang-tidy][]           | `--fix-errors` [^1] | `-checks=*` `-warnings-as-errors=*` [^2] |               |
+| [cppcheck][]             |                     | `-enable=all`                            |               |
+| [include-what-you-use][] |                     |                                          |               |
 
-[1]: `-fix` will fail if there are compiler errors. `-fix-errors` will `-fix` and fix compiler errors if it can, like missing semicolons.
+[^1]: `-fix` will fail if there are compiler errors. `-fix-errors` will `-fix` and fix compiler errors if it can, like missing semicolons.
 
-[2]: Be careful with `-checks=*`.  can have self-contradictory rules in newer versions of llvm (9+): modernize wants to use [trailing return type](https://clang.llvm.org/extra/clang-tidy/checks/modernize-use-trailing-return-type.html) but Fuchsia [disallows it](https://clang.llvm.org/extra/clang-tidy/checks/fuchsia-trailing-return.html).
+[^2]: Be careful with `-checks=*`; some checks can have self-contradictory rules in newer versions of LLVM (9+). For
+    example, modernize wants to use [trailing return type][] but Fuchsia [disallows it][].
 
+[trailing return type]: https://clang.llvm.org/extra/clang-tidy/checks/modernize-use-trailing-return-type.html
+
+[disallows it]: https://clang.llvm.org/extra/clang-tidy/checks/fuchsia-trailing-return.html
 
 ### The '--' doubledash option
 
 Options after `--` like `-std=c++11` will be interpreted correctly for `clang-tidy`. Make sure they sequentially follow
 the `--` argument in the hook's args list.
 
-
 ### Standalone Hooks
 
 If you want to have predictable return codes for your C linters outside of pre-commit, these hooks are available via
 [PyPI](https://pypi.org/project/cmake-pre-commit-hooks/).  Install it with `pip install cmake-pre-commit-hooks`.  They
 are named as `cmake-pc-$cmd-hook`, so `clang-format` becomes `cmake-pc-clang-format-hook`.
```

### Comparing `cmake_pre_commit_hooks-1.8.1/misc/license_header.txt` & `cmake_pre_commit_hooks-1.9.0/misc/license_header.txt`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.1/setup.cfg` & `cmake_pre_commit_hooks-1.9.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
+	toml
 	CLinters >= 1.3.0
 	fasteners
 	filelock
 
 [options.entry_points]
 console_scripts = 
 	cmake-pc-clang-format-hook = cmake_pc_hooks.clang_format:main
@@ -35,14 +36,19 @@
 	cmake-pc-lizard-hook = cmake_pc_hooks.lizard:main
 
 [options.extras_require]
 clang-format = 
 	clang-format
 lizard = 
 	lizard
+test = 
+	pytest
+	pytest-cov
+	pytest-mock
+	mock
 
 [bdist_wheel]
 universal = True
 
 [flake8]
 max-line-length = 120
 exclude =
```

### Comparing `cmake_pre_commit_hooks-1.8.1/setup.py` & `cmake_pre_commit_hooks-1.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,52 +15,54 @@
 """Dummy setup script."""
 
 import logging
 import os
 import shutil
 import subprocess
 import sys
+from pathlib import Path
 
 from setuptools import setup
 from setuptools.command.egg_info import egg_info
 
 
 def get_executable(exec_name):
     """Try to locate an executable in a Python virtual environment."""
-    # pylint: disable=no-member
+    python_executable = Path(sys.executable)
     try:
-        root_path = os.environ['VIRTUAL_ENV']
-        python = os.path.basename(sys.executable)
+        root_path = Path(os.environ['VIRTUAL_ENV'])
+        python = python_executable.name
     except KeyError:
-        root_path, python = os.path.split(sys.executable)
+        root_path = python_executable.parent
+        python = python_executable.name
 
-    exec_name = os.path.basename(exec_name)
+    exec_name = Path(exec_name).name
 
     logging.info('trying to locate %s in %s', exec_name, root_path)
 
-    search_paths = [root_path, os.path.join(root_path, 'bin'), os.path.join(root_path, 'Scripts')]
+    search_paths = [root_path, root_path / 'bin', root_path / 'Scripts']
 
     # First try executing the program directly
     for base_path in search_paths:
         try:
-            cmd = os.path.join(base_path, exec_name)
-            with open(os.devnull, 'w', encoding='utf-8') as devnull:
+            cmd = base_path / exec_name
+            with Path(os.devnull).open(mode='w', encoding='utf-8') as devnull:
                 subprocess.check_call([cmd, '--version'], stdout=devnull, stderr=devnull)
         except (OSError, subprocess.CalledProcessError):
             logging.info('  failed in %s', base_path)
         else:
             logging.info('  command found: %s', cmd)
             return cmd
 
     # That did not work: try calling it through Python
     for base_path in search_paths:
         try:
-            cmd = [python, os.path.join(base_path, exec_name)]
-            with open(os.devnull, 'w', encoding='utf-8') as devnull:
-                subprocess.check_call(cmd + ['--version'], stdout=devnull, stderr=devnull)
+            cmd = [python, base_path / exec_name]
+            with Path(os.devnull).open(mode='w', encoding='utf-8') as devnull:
+                subprocess.check_call([*cmd, '--version'], stdout=devnull, stderr=devnull)
         except (OSError, subprocess.CalledProcessError):
             logging.info('  failed in %s', base_path)
         else:
             logging.info('  command found: %s', cmd)
             return cmd
 
     logging.info('  command *not* found in virtualenv!')
```

### Comparing `cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.1/tests/cmake_good/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.9.0/tests/cmake_good/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.1/tests/run_tests.ps1` & `cmake_pre_commit_hooks-1.9.0/tests/run_tests.ps1`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.1/tests/run_tests.sh` & `cmake_pre_commit_hooks-1.9.0/tests/run_tests.sh`

 * *Files identical despite different names*

