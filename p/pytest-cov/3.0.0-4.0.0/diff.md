# Comparing `tmp/pytest-cov-3.0.0.tar.gz` & `tmp/pytest-cov-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-cov-3.0.0.tar", last modified: Mon Oct  4 01:48:46 2021, max compression
+gzip compressed data, was "pytest-cov-4.0.0.tar", last modified: Wed Sep 28 18:39:17 2022, max compression
```

## Comparing `pytest-cov-3.0.0.tar` & `pytest-cov-4.0.0.tar`

### file list

```diff
@@ -1,93 +1,91 @@
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.416629 pytest-cov-3.0.0/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2383 2021-08-26 14:33:24.000000 pytest-cov-3.0.0/.appveyor.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      634 2021-10-04 01:48:36.000000 pytest-cov-3.0.0/.bumpversion.cfg
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1825 2021-01-11 12:03:54.000000 pytest-cov-3.0.0/.cookiecutterrc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2021-01-11 12:03:54.000000 pytest-cov-3.0.0/.editorconfig
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.409629 pytest-cov-3.0.0/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.412629 pytest-cov-3.0.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      647 2020-08-14 15:43:50.000000 pytest-cov-3.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      419 2020-01-12 19:40:03.000000 pytest-cov-3.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      938 2020-01-12 19:40:03.000000 pytest-cov-3.0.0/.github/ISSUE_TEMPLATE/support_request.md
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.412629 pytest-cov-3.0.0/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1280 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/.github/workflows/examples.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      876 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/.github/workflows/lint.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2793 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/.github/workflows/test.yml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      666 2021-01-11 12:03:54.000000 pytest-cov-3.0.0/.gitignore
--rw-r--r--   0 ionel     (1000) ionel     (1000)      640 2021-08-26 14:33:24.000000 pytest-cov-3.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      244 2021-01-10 20:53:35.000000 pytest-cov-3.0.0/.readthedocs.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2314 2021-10-04 00:04:15.000000 pytest-cov-3.0.0/AUTHORS.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)    17167 2021-10-04 00:07:31.000000 pytest-cov-3.0.0/CHANGELOG.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2687 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1071 2021-01-10 20:53:35.000000 pytest-cov-3.0.0/LICENSE
--rw-r--r--   0 ionel     (1000) ionel     (1000)      578 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/MANIFEST.in
--rw-r--r--   0 ionel     (1000) ionel     (1000)    27977 2021-10-04 01:48:46.416629 pytest-cov-3.0.0/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)     5541 2021-10-04 01:48:36.000000 pytest-cov-3.0.0/README.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.412629 pytest-cov-3.0.0/ci/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      763 2021-01-10 20:52:27.000000 pytest-cov-3.0.0/ci/appveyor-with-compiler.cmd
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2850 2021-08-26 14:33:24.000000 pytest-cov-3.0.0/ci/bootstrap.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       62 2021-01-10 20:52:27.000000 pytest-cov-3.0.0/ci/requirements.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.412629 pytest-cov-3.0.0/ci/templates/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1931 2021-07-28 17:10:11.000000 pytest-cov-3.0.0/ci/templates/.appveyor.yml
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.414629 pytest-cov-3.0.0/docs/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2021-01-10 20:52:27.000000 pytest-cov-3.0.0/docs/authors.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2021-01-10 20:52:27.000000 pytest-cov-3.0.0/docs/changelog.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1301 2021-10-04 01:48:36.000000 pytest-cov-3.0.0/docs/conf.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3384 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/docs/config.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1163 2021-08-26 13:21:22.000000 pytest-cov-3.0.0/docs/contexts.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2021-01-10 20:52:27.000000 pytest-cov-3.0.0/docs/contributing.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      768 2019-01-06 18:11:51.000000 pytest-cov-3.0.0/docs/debuggers.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      407 2021-01-10 20:53:35.000000 pytest-cov-3.0.0/docs/index.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      804 2019-01-06 18:23:09.000000 pytest-cov-3.0.0/docs/markers-fixtures.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      996 2020-01-12 19:20:51.000000 pytest-cov-3.0.0/docs/plugins.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2021-01-10 20:52:27.000000 pytest-cov-3.0.0/docs/readme.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1395 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/docs/releasing.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2920 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/docs/reporting.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       70 2021-01-10 20:54:22.000000 pytest-cov-3.0.0/docs/requirements.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2021-01-10 20:52:27.000000 pytest-cov-3.0.0/docs/spelling_wordlist.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     5501 2020-01-12 19:40:03.000000 pytest-cov-3.0.0/docs/subprocess-support.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1728 2019-03-25 13:17:13.000000 pytest-cov-3.0.0/docs/tox.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2841 2019-09-04 15:33:31.000000 pytest-cov-3.0.0/docs/xdist.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.414629 pytest-cov-3.0.0/examples/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      540 2019-03-25 13:17:13.000000 pytest-cov-3.0.0/examples/README.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.414629 pytest-cov-3.0.0/examples/adhoc-layout/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      168 2019-03-25 13:17:13.000000 pytest-cov-3.0.0/examples/adhoc-layout/.coveragerc
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.414629 pytest-cov-3.0.0/examples/adhoc-layout/example/
--rw-r--r--   0 ionel     (1000) ionel     (1000)      215 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/examples/adhoc-layout/example/__init__.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      144 2020-08-14 15:43:50.000000 pytest-cov-3.0.0/examples/adhoc-layout/setup.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.414629 pytest-cov-3.0.0/examples/adhoc-layout/tests/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      105 2019-03-25 13:17:13.000000 pytest-cov-3.0.0/examples/adhoc-layout/tests/test_example.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      743 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/examples/adhoc-layout/tox.ini
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.414629 pytest-cov-3.0.0/examples/src-layout/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      155 2020-05-10 18:21:51.000000 pytest-cov-3.0.0/examples/src-layout/.coveragerc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      160 2020-08-14 15:43:50.000000 pytest-cov-3.0.0/examples/src-layout/setup.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.410629 pytest-cov-3.0.0/examples/src-layout/src/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.415629 pytest-cov-3.0.0/examples/src-layout/src/example/
--rw-r--r--   0 ionel     (1000) ionel     (1000)      215 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/examples/src-layout/src/example/__init__.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.415629 pytest-cov-3.0.0/examples/src-layout/tests/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      105 2019-03-25 13:17:13.000000 pytest-cov-3.0.0/examples/src-layout/tests/test_example.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      606 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/examples/src-layout/tox.ini
--rw-r--r--   0 ionel     (1000) ionel     (1000)      405 2021-10-04 01:48:46.417629 pytest-cov-3.0.0/setup.cfg
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     4664 2021-10-04 01:48:36.000000 pytest-cov-3.0.0/setup.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.415629 pytest-cov-3.0.0/src/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      425 2019-02-25 13:30:52.000000 pytest-cov-3.0.0/src/pytest-cov.embed
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      376 2020-07-24 13:11:44.000000 pytest-cov-3.0.0/src/pytest-cov.pth
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.415629 pytest-cov-3.0.0/src/pytest_cov/
--rw-r--r--   0 ionel     (1000) ionel     (1000)       93 2021-10-04 01:48:36.000000 pytest-cov-3.0.0/src/pytest_cov/__init__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      708 2021-08-26 14:33:24.000000 pytest-cov-3.0.0/src/pytest_cov/compat.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     3983 2021-01-10 21:22:38.000000 pytest-cov-3.0.0/src/pytest_cov/embed.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    14761 2021-08-26 14:33:24.000000 pytest-cov-3.0.0/src/pytest_cov/engine.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    14791 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/src/pytest_cov/plugin.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.416629 pytest-cov-3.0.0/src/pytest_cov.egg-info/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)    27977 2021-10-04 01:48:46.000000 pytest-cov-3.0.0/src/pytest_cov.egg-info/PKG-INFO
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1741 2021-10-04 01:48:46.000000 pytest-cov-3.0.0/src/pytest_cov.egg-info/SOURCES.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)        1 2021-10-04 01:48:46.000000 pytest-cov-3.0.0/src/pytest_cov.egg-info/dependency_links.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       43 2021-10-04 01:48:46.000000 pytest-cov-3.0.0/src/pytest_cov.egg-info/entry_points.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)        1 2019-01-06 18:31:54.000000 pytest-cov-3.0.0/src/pytest_cov.egg-info/not-zip-safe
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      101 2021-10-04 01:48:46.000000 pytest-cov-3.0.0/src/pytest_cov.egg-info/requires.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       11 2021-10-04 01:48:46.000000 pytest-cov-3.0.0/src/pytest_cov.egg-info/top_level.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2021-10-04 01:48:46.416629 pytest-cov-3.0.0/tests/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       73 2019-01-06 18:11:51.000000 pytest-cov-3.0.0/tests/conftest.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2425 2020-01-12 18:10:07.000000 pytest-cov-3.0.0/tests/contextful.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       39 2019-01-06 18:11:51.000000 pytest-cov-3.0.0/tests/helper.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    66636 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/tests/test_pytest_cov.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2666 2021-10-03 22:03:28.000000 pytest-cov-3.0.0/tox.ini
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.180606 pytest-cov-4.0.0/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      634 2022-09-28 15:20:20.000000 pytest-cov-4.0.0/.bumpversion.cfg
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1801 2022-07-22 09:48:47.000000 pytest-cov-4.0.0/.cookiecutterrc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2022-02-02 17:42:23.000000 pytest-cov-4.0.0/.editorconfig
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.174606 pytest-cov-4.0.0/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.176606 pytest-cov-4.0.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      647 2020-08-14 15:43:50.000000 pytest-cov-4.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      419 2020-01-12 19:40:03.000000 pytest-cov-4.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      938 2020-01-12 19:40:03.000000 pytest-cov-4.0.0/.github/ISSUE_TEMPLATE/support_request.md
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.176606 pytest-cov-4.0.0/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     7719 2022-09-28 09:32:18.000000 pytest-cov-4.0.0/.github/workflows/test.yml
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      666 2022-02-02 17:42:23.000000 pytest-cov-4.0.0/.gitignore
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      641 2022-07-22 09:48:47.000000 pytest-cov-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      244 2022-02-02 17:44:23.000000 pytest-cov-4.0.0/.readthedocs.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2646 2022-09-28 15:18:55.000000 pytest-cov-4.0.0/AUTHORS.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    18361 2022-09-28 15:17:58.000000 pytest-cov-4.0.0/CHANGELOG.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2687 2022-02-02 17:44:23.000000 pytest-cov-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1071 2022-02-02 17:44:23.000000 pytest-cov-4.0.0/LICENSE
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      557 2022-07-22 09:48:47.000000 pytest-cov-4.0.0/MANIFEST.in
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    25461 2022-09-28 18:39:17.180606 pytest-cov-4.0.0/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     5540 2022-09-28 15:20:20.000000 pytest-cov-4.0.0/README.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.177606 pytest-cov-4.0.0/ci/
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2877 2022-07-22 09:48:47.000000 pytest-cov-4.0.0/ci/bootstrap.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       66 2022-07-22 09:48:47.000000 pytest-cov-4.0.0/ci/requirements.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.174606 pytest-cov-4.0.0/ci/templates/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.174606 pytest-cov-4.0.0/ci/templates/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.177606 pytest-cov-4.0.0/ci/templates/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3640 2022-09-28 09:32:18.000000 pytest-cov-4.0.0/ci/templates/.github/workflows/test.yml
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.178606 pytest-cov-4.0.0/docs/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2022-02-02 17:42:24.000000 pytest-cov-4.0.0/docs/authors.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2022-02-02 17:42:24.000000 pytest-cov-4.0.0/docs/changelog.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1301 2022-09-28 15:20:20.000000 pytest-cov-4.0.0/docs/conf.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3380 2022-09-28 15:03:24.000000 pytest-cov-4.0.0/docs/config.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1163 2021-08-26 13:21:22.000000 pytest-cov-4.0.0/docs/contexts.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2022-02-02 17:42:24.000000 pytest-cov-4.0.0/docs/contributing.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      965 2022-07-22 09:48:47.000000 pytest-cov-4.0.0/docs/debuggers.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      407 2022-02-02 17:44:23.000000 pytest-cov-4.0.0/docs/index.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      804 2019-01-06 18:23:09.000000 pytest-cov-4.0.0/docs/markers-fixtures.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      996 2020-01-12 19:20:51.000000 pytest-cov-4.0.0/docs/plugins.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2022-02-02 17:42:24.000000 pytest-cov-4.0.0/docs/readme.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1395 2021-10-03 22:03:28.000000 pytest-cov-4.0.0/docs/releasing.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3003 2022-09-28 15:03:24.000000 pytest-cov-4.0.0/docs/reporting.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       81 2022-07-22 09:48:47.000000 pytest-cov-4.0.0/docs/requirements.txt
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2022-02-02 17:42:24.000000 pytest-cov-4.0.0/docs/spelling_wordlist.txt
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)     5501 2020-01-12 19:40:03.000000 pytest-cov-4.0.0/docs/subprocess-support.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)     1728 2019-03-25 13:17:13.000000 pytest-cov-4.0.0/docs/tox.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)     2841 2019-09-04 15:33:31.000000 pytest-cov-4.0.0/docs/xdist.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.178606 pytest-cov-4.0.0/examples/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      540 2019-03-25 13:17:13.000000 pytest-cov-4.0.0/examples/README.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.178606 pytest-cov-4.0.0/examples/adhoc-layout/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      168 2019-03-25 13:17:13.000000 pytest-cov-4.0.0/examples/adhoc-layout/.coveragerc
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.178606 pytest-cov-4.0.0/examples/adhoc-layout/example/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      215 2021-10-03 22:03:28.000000 pytest-cov-4.0.0/examples/adhoc-layout/example/__init__.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      144 2020-08-14 15:43:50.000000 pytest-cov-4.0.0/examples/adhoc-layout/setup.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.178606 pytest-cov-4.0.0/examples/adhoc-layout/tests/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      105 2019-03-25 13:17:13.000000 pytest-cov-4.0.0/examples/adhoc-layout/tests/test_example.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      743 2021-10-03 22:03:28.000000 pytest-cov-4.0.0/examples/adhoc-layout/tox.ini
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.179606 pytest-cov-4.0.0/examples/src-layout/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      155 2020-05-10 18:21:51.000000 pytest-cov-4.0.0/examples/src-layout/.coveragerc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      160 2020-08-14 15:43:50.000000 pytest-cov-4.0.0/examples/src-layout/setup.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.175606 pytest-cov-4.0.0/examples/src-layout/src/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.179606 pytest-cov-4.0.0/examples/src-layout/src/example/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      215 2021-10-03 22:03:28.000000 pytest-cov-4.0.0/examples/src-layout/src/example/__init__.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.179606 pytest-cov-4.0.0/examples/src-layout/tests/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      105 2019-03-25 13:17:13.000000 pytest-cov-4.0.0/examples/src-layout/tests/test_example.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      606 2021-10-03 22:03:28.000000 pytest-cov-4.0.0/examples/src-layout/tox.ini
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      405 2022-09-28 18:39:17.181606 pytest-cov-4.0.0/setup.cfg
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     5027 2022-09-28 15:20:20.000000 pytest-cov-4.0.0/setup.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.179606 pytest-cov-4.0.0/src/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      425 2019-02-25 13:30:52.000000 pytest-cov-4.0.0/src/pytest-cov.embed
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      377 2022-07-22 09:48:47.000000 pytest-cov-4.0.0/src/pytest-cov.pth
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.179606 pytest-cov-4.0.0/src/pytest_cov/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       93 2022-09-28 15:20:20.000000 pytest-cov-4.0.0/src/pytest_cov/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      560 2022-09-28 09:32:18.000000 pytest-cov-4.0.0/src/pytest_cov/compat.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3556 2022-07-22 09:48:47.000000 pytest-cov-4.0.0/src/pytest_cov/embed.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    15387 2022-09-28 15:03:24.000000 pytest-cov-4.0.0/src/pytest_cov/engine.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    15171 2022-09-28 15:03:24.000000 pytest-cov-4.0.0/src/pytest_cov/plugin.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.180606 pytest-cov-4.0.0/src/pytest_cov.egg-info/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    25461 2022-09-28 18:39:17.000000 pytest-cov-4.0.0/src/pytest_cov.egg-info/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1652 2022-09-28 18:39:17.000000 pytest-cov-4.0.0/src/pytest_cov.egg-info/SOURCES.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2022-09-28 18:39:17.000000 pytest-cov-4.0.0/src/pytest_cov.egg-info/dependency_links.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       43 2022-09-28 18:39:17.000000 pytest-cov-4.0.0/src/pytest_cov.egg-info/entry_points.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2022-09-28 18:39:16.000000 pytest-cov-4.0.0/src/pytest_cov.egg-info/not-zip-safe
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      101 2022-09-28 18:39:17.000000 pytest-cov-4.0.0/src/pytest_cov.egg-info/requires.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       11 2022-09-28 18:39:17.000000 pytest-cov-4.0.0/src/pytest_cov.egg-info/top_level.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-09-28 18:39:17.180606 pytest-cov-4.0.0/tests/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       73 2019-01-06 18:11:51.000000 pytest-cov-4.0.0/tests/conftest.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)     2425 2020-01-12 18:10:07.000000 pytest-cov-4.0.0/tests/contextful.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       39 2019-01-06 18:11:51.000000 pytest-cov-4.0.0/tests/helper.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    62190 2022-09-28 15:03:24.000000 pytest-cov-4.0.0/tests/test_pytest_cov.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2954 2022-09-28 14:52:50.000000 pytest-cov-4.0.0/tox.ini
```

### Comparing `pytest-cov-3.0.0/.bumpversion.cfg` & `pytest-cov-4.0.0/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.0.0
+current_version = 4.0.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `pytest-cov-3.0.0/.cookiecutterrc` & `pytest-cov-4.0.0/.cookiecutterrc`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 # Generated by cookiepatcher, a small shim around cookiecutter (pip install cookiepatcher)
 
 default_context:
     allow_tests_inside_package: no
-    appveyor: yes
+    appveyor: no
     c_extension_function: '-'
     c_extension_module: '-'
     c_extension_optional: no
     c_extension_support: no
     c_extension_test_pypi: no
     c_extension_test_pypi_username: '-'
     codacy: no
     codacy_projectid: '[Get ID from https://app.codacy.com/app/ionelmc/pytest-cov/settings]'
     codeclimate: no
     codecov: no
     command_line_interface: no
     command_line_interface_bin_name: '-'
     coveralls: no
-    coveralls_token: '[Required for Appveyor, take it from https://coveralls.io/github/ionelmc/pytest-cov]'
     distribution_name: pytest-cov
     email: contact@ionelmc.ro
     full_name: Ionel Cristian Mărieș
+    github_actions: yes
     legacy_python: yes
     license: MIT license
     linter: flake8
     package_name: pytest_cov
     pre_commit: yes
     project_name: pytest-cov
     project_short_description: This plugin produces coverage reports. It supports centralised testing and distributed testing in both load and each modes. It also supports coverage of subprocesses.
     pypi_badge: yes
     pypi_disable_upload: no
-    release_date: '2020-06-12'
+    release_date: '2021-10-04'
     repo_hosting: github.com
     repo_hosting_domain: github.com
+    repo_main_branch: master
     repo_name: pytest-cov
     repo_username: pytest-dev
     requiresio: yes
     scrutinizer: no
     setup_py_uses_setuptools_scm: no
     setup_py_uses_test_runner: no
     sphinx_docs: yes
     sphinx_docs_hosting: https://pytest-cov.readthedocs.io/
     sphinx_doctest: no
     sphinx_theme: sphinx-py3doc-enhanced-theme
     test_matrix_configurator: no
     test_matrix_separate_coverage: no
     test_runner: pytest
-    travis: yes
+    travis: no
     travis_osx: no
-    version: 2.10.1
+    version: 3.0.0
+    version_manager: bump2version
     website: http://blog.ionelmc.ro
     year_from: '2010'
-    year_to: '2020'
+    year_to: '2022'
```

### Comparing `pytest-cov-3.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `pytest-cov-4.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/.github/ISSUE_TEMPLATE/support_request.md` & `pytest-cov-4.0.0/.github/ISSUE_TEMPLATE/support_request.md`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/.gitignore` & `pytest-cov-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/.pre-commit-config.yaml` & `pytest-cov-4.0.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # To install the git pre-commit hook run:
 #   pre-commit install
 # To update the pre-commit hooks run:
 #   pre-commit install-hooks
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.1
+    rev: v4.2.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
         exclude: '.*\.pth$'
       - id: debug-statements
   - repo: https://github.com/PyCQA/isort
-    rev: 5.9.3
+    rev: 5.10.1
     hooks:
       - id: isort
   - repo: https://github.com/PyCQA/flake8
-    rev: 3.9.2
+    rev: 4.0.1
     hooks:
       - id: flake8
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.23.3
+    rev: v2.32.1
     hooks:
       - id: pyupgrade
         args: [--py36-plus]
```

### Comparing `pytest-cov-3.0.0/AUTHORS.rst` & `pytest-cov-4.0.0/AUTHORS.rst`

 * *Files 7% similar despite different names*

```diff
@@ -46,7 +46,14 @@
 * Pamela McA'Nulty - https://github.com/PamelaM
 * Christian Riedel - https://github.com/Cielquan
 * Chris Sreesangkom - https://github.com/csreesan
 * Sorin Sbarnea - https://github.com/ssbarnea
 * Brian Rutledge - https://github.com/bhrutledge
 * Danilo Šegan - https://github.com/dsegan
 * Michał Bielawski - https://github.com/D3X
+* Zac Hatfield-Dodds - https://github.com/Zac-HD
+* Ben Greiner - https://github.com/bnavigator
+* Delgan - https://github.com/Delgan
+* Andre Brisco - https://github.com/abrisco
+* Colin O'Dell - https://github.com/colinodell
+* Ronny Pfannschmidt - https://github.com/RonnyPfannschmidt
+* Christian Fetzer - https://github.com/fetzerch
```

### Comparing `pytest-cov-3.0.0/CHANGELOG.rst` & `pytest-cov-4.0.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,43 @@
 Changelog
 =========
 
 
+4.0.0 (2022-09-28)
+------------------
+
+**Note that this release drops support for multiprocessing.**
+
+
+* `--cov-fail-under` no longer causes `pytest --collect-only` to fail
+  Contributed by Zac Hatfield-Dodds in `#511 <https://github.com/pytest-dev/pytest-cov/pull/511>`_.
+* Dropped support for multiprocessing (mostly because `issue 82408 <https://github.com/python/cpython/issues/82408>`_). This feature was
+  mostly working but very broken in certain scenarios and made the test suite very flaky and slow.
+
+  There is builtin multiprocessing support in coverage and you can migrate to that. All you need is this in your
+  ``.coveragerc``::
+
+    [run]
+    concurrency = multiprocessing
+    parallel = true
+    sigterm = true
+* Fixed deprecation in ``setup.py`` by trying to import setuptools before distutils.
+  Contributed by Ben Greiner in `#545 <https://github.com/pytest-dev/pytest-cov/pull/545>`_.
+* Removed undesirable new lines that were displayed while reporting was disabled.
+  Contributed by Delgan in `#540 <https://github.com/pytest-dev/pytest-cov/pull/540>`_.
+* Documentation fixes.
+  Contributed by Andre Brisco in `#543 <https://github.com/pytest-dev/pytest-cov/pull/543>`_
+  and Colin O'Dell in `#525 <https://github.com/pytest-dev/pytest-cov/pull/525>`_.
+* Added support for LCOV output format via `--cov-report=lcov`. Only works with coverage 6.3+.
+  Contributed by Christian Fetzer in `#536 <https://github.com/pytest-dev/pytest-cov/issues/536>`_.
+* Modernized pytest hook implementation.
+  Contributed by Bruno Oliveira in `#549 <https://github.com/pytest-dev/pytest-cov/pull/549>`_
+  and Ronny Pfannschmidt in `#550 <https://github.com/pytest-dev/pytest-cov/pull/550>`_.
+
+
 3.0.0 (2021-10-04)
 -------------------
 
 **Note that this release drops support for Python 2.7 and Python 3.5.**
 
 * Added support for Python 3.10 and updated various test dependencies.
   Contributed by Hugo van Kemenade in
@@ -20,25 +52,17 @@
   Contributed by ... Ronny Pfannschmidt's desire for skark in
   `#480 <https://github.com/pytest-dev/pytest-cov/pull/480>`_.
 * Dropped Python 2.7 support.
   Contributed by Thomas Grainger in
   `#488 <https://github.com/pytest-dev/pytest-cov/pull/488>`_.
 * Updated trove classifiers. Contributed by Michał Bielawski in
   `#481 <https://github.com/pytest-dev/pytest-cov/pull/481>`_.
-
-
-2.13.0 (2021-06-01)
--------------------
-
-* Changed the `toml` requirement to be always be directly required (instead of being required through a coverage extra).
-  This fixes issues with pip-compile (`pip-tools#1300 <https://github.com/jazzband/pip-tools/issues/1300>`_).
-  Contributed by Sorin Sbarnea in `#472 <https://github.com/pytest-dev/pytest-cov/pull/472>`_.
-* Documented ``show_contexts``.
-  Contributed by Brian Rutledge in `#473 <https://github.com/pytest-dev/pytest-cov/pull/473>`_.
-
+* Reverted change for `toml` requirement.
+  Contributed by Thomas Grainger in
+  `#477 <https://github.com/pytest-dev/pytest-cov/pull/477>`_.
 
 2.12.1 (2021-06-01)
 -------------------
 
 * Changed the `toml` requirement to be always be directly required (instead of being required through a coverage extra).
   This fixes issues with pip-compile (`pip-tools#1300 <https://github.com/jazzband/pip-tools/issues/1300>`_).
   Contributed by Sorin Sbarnea in `#472 <https://github.com/pytest-dev/pytest-cov/pull/472>`_.
@@ -181,16 +205,14 @@
   Contributed by Alexander Shadchin in `#263 <https://github.com/pytest-dev/pytest-cov/pull/263>`_.
 * Various testing and CI improvements. Contributed by Daniel Hahler in
   `#255 <https://github.com/pytest-dev/pytest-cov/pull/255>`_,
   `#266 <https://github.com/pytest-dev/pytest-cov/pull/266>`_,
   `#272 <https://github.com/pytest-dev/pytest-cov/pull/272>`_,
   `#271 <https://github.com/pytest-dev/pytest-cov/pull/271>`_ and
   `#269 <https://github.com/pytest-dev/pytest-cov/pull/269>`_.
-* Improved documentation regarding subprocess and multiprocessing.
-  Contributed in `#265 <https://github.com/pytest-dev/pytest-cov/pull/265>`_.
 * Improved ``pytest_cov.embed.cleanup_on_sigterm`` to be reentrant (signal deliveries while signal handling is
   running won't break stuff).
 * Added ``pytest_cov.embed.cleanup_on_signal`` for customized cleanup.
 * Improved cleanup code and fixed various issues with leftover data files. All contributed in
   `#265 <https://github.com/pytest-dev/pytest-cov/pull/265>`_ or
   `#262 <https://github.com/pytest-dev/pytest-cov/pull/262>`_.
 * Improved examples. Now there are two examples for the common project layouts, complete with working coverage
```

### Comparing `pytest-cov-3.0.0/CONTRIBUTING.rst` & `pytest-cov-4.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/LICENSE` & `pytest-cov-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/MANIFEST.in` & `pytest-cov-4.0.0/MANIFEST.in`

 * *Files 18% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 
 graft .github/workflows
 graft src
 graft ci
 graft tests
 
 include .bumpversion.cfg
-include .coveragerc
 include .cookiecutterrc
+include .coveragerc
 include .editorconfig
-
+include tox.ini
+include .readthedocs.yml
+include .pre-commit-config.yaml
 include AUTHORS.rst
 include CHANGELOG.rst
 include CONTRIBUTING.rst
 include LICENSE
 include README.rst
 
-include tox.ini .appveyor.yml .readthedocs.yml .pre-commit-config.yaml
 
-global-exclude *.py[cod] __pycache__/* *.so *.dylib .coverage .coverage.*
+global-exclude *.py[cod] __pycache__/* *.so *.dylib
```

### Comparing `pytest-cov-3.0.0/PKG-INFO` & `pytest-cov-4.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,512 +1,18 @@
 Metadata-Version: 2.1
 Name: pytest-cov
-Version: 3.0.0
+Version: 4.0.0
 Summary: Pytest plugin for measuring coverage.
 Home-page: https://github.com/pytest-dev/pytest-cov
 Author: Marc Schlaich
 Author-email: marc.schlaich@gmail.com
 License: MIT
-Description: ========
-        Overview
-        ========
-        
-        .. start-badges
-        
-        .. list-table::
-            :stub-columns: 1
-        
-            * - docs
-              - |docs|
-            * - tests
-              - | |github-actions| |appveyor| |requires|
-            * - package
-              - | |version| |conda-forge| |wheel| |supported-versions| |supported-implementations|
-                | |commits-since|
-        
-        .. |docs| image:: https://readthedocs.org/projects/pytest-cov/badge/?style=flat
-            :target: https://readthedocs.org/projects/pytest-cov
-            :alt: Documentation Status
-        
-        .. |github-actions| image:: https://github.com/pytest-dev/pytest-cov/actions/workflows/test.yml/badge.svg
-            :alt: GitHub Actions Status
-            :target: https://github.com/pytest-dev/pytest-cov/actions
-        
-        .. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/pytest-dev/pytest-cov?branch=master&svg=true
-            :alt: AppVeyor Build Status
-            :target: https://ci.appveyor.com/project/pytestbot/pytest-cov
-        
-        .. |requires| image:: https://requires.io/github/pytest-dev/pytest-cov/requirements.svg?branch=master
-            :alt: Requirements Status
-            :target: https://requires.io/github/pytest-dev/pytest-cov/requirements/?branch=master
-        
-        .. |version| image:: https://img.shields.io/pypi/v/pytest-cov.svg
-            :alt: PyPI Package latest release
-            :target: https://pypi.org/project/pytest-cov
-        
-        .. |conda-forge| image:: https://img.shields.io/conda/vn/conda-forge/pytest-cov.svg
-            :target: https://anaconda.org/conda-forge/pytest-cov
-        
-        .. |commits-since| image:: https://img.shields.io/github/commits-since/pytest-dev/pytest-cov/v3.0.0.svg
-            :alt: Commits since latest release
-            :target: https://github.com/pytest-dev/pytest-cov/compare/v3.0.0...master
-        
-        .. |wheel| image:: https://img.shields.io/pypi/wheel/pytest-cov.svg
-            :alt: PyPI Wheel
-            :target: https://pypi.org/project/pytest-cov
-        
-        .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pytest-cov.svg
-            :alt: Supported versions
-            :target: https://pypi.org/project/pytest-cov
-        
-        .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pytest-cov.svg
-            :alt: Supported implementations
-            :target: https://pypi.org/project/pytest-cov
-        
-        .. end-badges
-        
-        This plugin produces coverage reports. Compared to just using ``coverage run`` this plugin does some extras:
-        
-        * Subprocess support: you can fork or run stuff in a subprocess and will get covered without any fuss.
-        * Xdist support: you can use all of pytest-xdist's features and still get coverage.
-        * Consistent pytest behavior. If you run ``coverage run -m pytest`` you will have slightly different ``sys.path`` (CWD will be
-          in it, unlike when running ``pytest``).
-        
-        All features offered by the coverage package should work, either through pytest-cov's command line options or
-        through coverage's config file.
-        
-        * Free software: MIT license
-        
-        Installation
-        ============
-        
-        Install with pip::
-        
-            pip install pytest-cov
-        
-        For distributed testing support install pytest-xdist::
-        
-            pip install pytest-xdist
-        
-        Upgrading from ancient pytest-cov
-        ---------------------------------
-        
-        `pytest-cov 2.0` is using a new ``.pth`` file (``pytest-cov.pth``). You may want to manually remove the older
-        ``init_cov_core.pth`` from site-packages as it's not automatically removed.
-        
-        Uninstalling
-        ------------
-        
-        Uninstall with pip::
-        
-            pip uninstall pytest-cov
-        
-        Under certain scenarios a stray ``.pth`` file may be left around in site-packages.
-        
-        * `pytest-cov 2.0` may leave a ``pytest-cov.pth`` if you installed without wheels
-          (``easy_install``, ``setup.py install`` etc).
-        * `pytest-cov 1.8 or older` will leave a ``init_cov_core.pth``.
-        
-        Usage
-        =====
-        
-        ::
-        
-            pytest --cov=myproj tests/
-        
-        Would produce a report like::
-        
-            -------------------- coverage: ... ---------------------
-            Name                 Stmts   Miss  Cover
-            ----------------------------------------
-            myproj/__init__          2      0   100%
-            myproj/myproj          257     13    94%
-            myproj/feature4286      94      7    92%
-            ----------------------------------------
-            TOTAL                  353     20    94%
-        
-        Documentation
-        =============
-        
-            http://pytest-cov.rtfd.org/
-        
-        
-        
-        
-        
-        
-        Coverage Data File
-        ==================
-        
-        The data file is erased at the beginning of testing to ensure clean data for each test run. If you
-        need to combine the coverage of several test runs you can use the ``--cov-append`` option to append
-        this coverage data to coverage data from previous test runs.
-        
-        The data file is left at the end of testing so that it is possible to use normal coverage tools to
-        examine it.
-        
-        Limitations
-        ===========
-        
-        For distributed testing the workers must have the pytest-cov package installed.  This is needed since
-        the plugin must be registered through setuptools for pytest to start the plugin on the
-        worker.
-        
-        For subprocess measurement environment variables must make it from the main process to the
-        subprocess.  The python used by the subprocess must have pytest-cov installed.  The subprocess must
-        do normal site initialisation so that the environment variables can be detected and coverage
-        started.
-        
-        
-        Acknowledgements
-        ================
-        
-        Whilst this plugin has been built fresh from the ground up it has been influenced by the work done
-        on pytest-coverage (Ross Lawley, James Mills, Holger Krekel) and nose-cover (Jason Pellerin) which are
-        other coverage plugins.
-        
-        Ned Batchelder for coverage and its ability to combine the coverage results of parallel runs.
-        
-        Holger Krekel for pytest with its distributed testing support.
-        
-        Jason Pellerin for nose.
-        
-        Michael Foord for unittest2.
-        
-        No doubt others have contributed to these tools as well.
-        
-        Changelog
-        =========
-        
-        
-        3.0.0 (2021-10-04)
-        -------------------
-        
-        **Note that this release drops support for Python 2.7 and Python 3.5.**
-        
-        * Added support for Python 3.10 and updated various test dependencies.
-          Contributed by Hugo van Kemenade in
-          `#500 <https://github.com/pytest-dev/pytest-cov/pull/500>`_.
-        * Switched from Travis CI to GitHub Actions. Contributed by Hugo van Kemenade in
-          `#494 <https://github.com/pytest-dev/pytest-cov/pull/494>`_ and
-          `#495 <https://github.com/pytest-dev/pytest-cov/pull/495>`_.
-        * Add a ``--cov-reset`` CLI option.
-          Contributed by Danilo Šegan in
-          `#459 <https://github.com/pytest-dev/pytest-cov/pull/459>`_.
-        * Improved validation of ``--cov-fail-under`` CLI option.
-          Contributed by ... Ronny Pfannschmidt's desire for skark in
-          `#480 <https://github.com/pytest-dev/pytest-cov/pull/480>`_.
-        * Dropped Python 2.7 support.
-          Contributed by Thomas Grainger in
-          `#488 <https://github.com/pytest-dev/pytest-cov/pull/488>`_.
-        * Updated trove classifiers. Contributed by Michał Bielawski in
-          `#481 <https://github.com/pytest-dev/pytest-cov/pull/481>`_.
-        
-        
-        2.13.0 (2021-06-01)
-        -------------------
-        
-        * Changed the `toml` requirement to be always be directly required (instead of being required through a coverage extra).
-          This fixes issues with pip-compile (`pip-tools#1300 <https://github.com/jazzband/pip-tools/issues/1300>`_).
-          Contributed by Sorin Sbarnea in `#472 <https://github.com/pytest-dev/pytest-cov/pull/472>`_.
-        * Documented ``show_contexts``.
-          Contributed by Brian Rutledge in `#473 <https://github.com/pytest-dev/pytest-cov/pull/473>`_.
-        
-        
-        2.12.1 (2021-06-01)
-        -------------------
-        
-        * Changed the `toml` requirement to be always be directly required (instead of being required through a coverage extra).
-          This fixes issues with pip-compile (`pip-tools#1300 <https://github.com/jazzband/pip-tools/issues/1300>`_).
-          Contributed by Sorin Sbarnea in `#472 <https://github.com/pytest-dev/pytest-cov/pull/472>`_.
-        * Documented ``show_contexts``.
-          Contributed by Brian Rutledge in `#473 <https://github.com/pytest-dev/pytest-cov/pull/473>`_.
-        
-        2.12.0 (2021-05-14)
-        -------------------
-        
-        * Added coverage's `toml` extra to install requirements in setup.py.
-          Contributed by Christian Riedel in `#410 <https://github.com/pytest-dev/pytest-cov/pull/410>`_.
-        * Fixed ``pytest_cov.__version__`` to have the right value (string with version instead of a string
-          including ``__version__ =``).
-        * Fixed license classifier in ``setup.py``.
-          Contributed by Chris Sreesangkom in `#467 <https://github.com/pytest-dev/pytest-cov/pull/467>`_.
-        * Fixed *commits since* badge.
-          Contributed by Terence Honles in `#470 <https://github.com/pytest-dev/pytest-cov/pull/470>`_.
-        
-        2.11.1 (2021-01-20)
-        -------------------
-        
-        * Fixed support for newer setuptools (v42+).
-          Contributed by Michał Górny in `#451 <https://github.com/pytest-dev/pytest-cov/pull/451>`_.
-        
-        2.11.0 (2021-01-18)
-        -------------------
-        
-        * Bumped minimum coverage requirement to 5.2.1. This prevents reporting issues.
-          Contributed by Mateus Berardo de Souza Terra in `#433 <https://github.com/pytest-dev/pytest-cov/pull/433>`_.
-        * Improved sample projects (from the `examples <https://github.com/pytest-dev/pytest-cov/tree/master/examples>`_
-          directory) to support running `tox -e pyXY`. Now the example configures a suffixed coverage data file,
-          and that makes the cleanup environment unnecessary.
-          Contributed by Ganden Schaffner in `#435 <https://github.com/pytest-dev/pytest-cov/pull/435>`_.
-        * Removed the empty `console_scripts` entrypoint that confused some Gentoo build script.
-          I didn't ask why it was so broken cause I didn't want to ruin my day.
-          Contributed by Michał Górny in `#434 <https://github.com/pytest-dev/pytest-cov/pull/434>`_.
-        * Fixed the missing `coverage context <https://coverage.readthedocs.io/en/stable/contexts.html>`_
-          when using subprocesses.
-          Contributed by Bernát Gábor in `#443 <https://github.com/pytest-dev/pytest-cov/pull/443>`_.
-        * Updated the config section in the docs.
-          Contributed by Pamela McA'Nulty in `#429 <https://github.com/pytest-dev/pytest-cov/pull/429>`_.
-        * Migrated CI to travis-ci.com (from .org).
-        
-        2.10.1 (2020-08-14)
-        -------------------
-        
-        * Support for ``pytest-xdist`` 2.0, which breaks compatibility with ``pytest-xdist`` before 1.22.3 (from 2017).
-          Contributed by Zac Hatfield-Dodds in `#412 <https://github.com/pytest-dev/pytest-cov/pull/412>`_.
-        * Fixed the ``LocalPath has no attribute startswith`` failure that occurred when using the ``pytester`` plugin
-          in inline mode.
-        
-        2.10.0 (2020-06-12)
-        -------------------
-        
-        * Improved the ``--no-cov`` warning. Now it's only shown if ``--no-cov`` is present before ``--cov``.
-        * Removed legacy pytest support. Changed ``setup.py`` so that ``pytest>=4.6`` is required.
-        
-        2.9.0 (2020-05-22)
-        ------------------
-        
-        * Fixed ``RemovedInPytest4Warning`` when using Pytest 3.10.
-          Contributed by Michael Manganiello in `#354 <https://github.com/pytest-dev/pytest-cov/pull/354>`_.
-        * Made pytest startup faster when plugin not active by lazy-importing.
-          Contributed by Anders Hovmöller in `#339 <https://github.com/pytest-dev/pytest-cov/pull/339>`_.
-        * Various CI improvements.
-          Contributed by Daniel Hahler in `#363 <https://github.com/pytest-dev/pytest-cov/pull/>`_ and
-          `#364 <https://github.com/pytest-dev/pytest-cov/pull/364>`_.
-        * Various Python support updates (drop EOL 3.4, test against 3.8 final).
-          Contributed by Hugo van Kemenade in
-          `#336 <https://github.com/pytest-dev/pytest-cov/pull/336>`_ and
-          `#367 <https://github.com/pytest-dev/pytest-cov/pull/367>`_.
-        * Changed ``--cov-append`` to always enable ``data_suffix`` (a coverage setting).
-          Contributed by Harm Geerts in
-          `#387 <https://github.com/pytest-dev/pytest-cov/pull/387>`_.
-        * Changed ``--cov-append`` to handle loading previous data better
-          (fixes various path aliasing issues).
-        * Various other testing improvements, github issue templates, example updates.
-        * Fixed internal failures that are caused by tests that change the current working directory by
-          ensuring a consistent working directory when coverage is called.
-          See `#306 <https://github.com/pytest-dev/pytest-cov/issues/306>`_ and
-          `coveragepy#881 <https://github.com/nedbat/coveragepy/issues/881>`_
-        
-        2.8.1 (2019-10-05)
-        ------------------
-        
-        * Fixed `#348 <https://github.com/pytest-dev/pytest-cov/issues/348>`_ -
-          regression when only certain reports (html or xml) are used then ``--cov-fail-under`` always fails.
-        
-        2.8.0 (2019-10-04)
-        ------------------
-        
-        * Fixed ``RecursionError`` that can occur when using
-          `cleanup_on_signal <https://pytest-cov.readthedocs.io/en/latest/subprocess-support.html#if-you-got-custom-signal-handling>`__ or
-          `cleanup_on_sigterm <https://pytest-cov.readthedocs.io/en/latest/subprocess-support.html#if-you-got-custom-signal-handling>`__.
-          See: `#294 <https://github.com/pytest-dev/pytest-cov/issues/294>`_.
-          The 2.7.x releases of pytest-cov should be considered broken regarding aforementioned cleanup API.
-        * Added compatibility with future xdist release that deprecates some internals
-          (match pytest-xdist master/worker terminology).
-          Contributed by Thomas Grainger in `#321 <https://github.com/pytest-dev/pytest-cov/pull/321>`_
-        * Fixed breakage that occurs when multiple reporting options are used.
-          Contributed by Thomas Grainger in `#338 <https://github.com/pytest-dev/pytest-cov/pull/338>`_.
-        * Changed internals to use a stub instead of ``os.devnull``.
-          Contributed by Thomas Grainger in `#332 <https://github.com/pytest-dev/pytest-cov/pull/332>`_.
-        * Added support for Coverage 5.0.
-          Contributed by Ned Batchelder in `#319 <https://github.com/pytest-dev/pytest-cov/pull/319>`_.
-        * Added support for float values in ``--cov-fail-under``.
-          Contributed by Martín Gaitán in `#311 <https://github.com/pytest-dev/pytest-cov/pull/311>`_.
-        * Various documentation fixes. Contributed by
-          Juanjo Bazán,
-          Andrew Murray and
-          Albert Tugushev in
-          `#298 <https://github.com/pytest-dev/pytest-cov/pull/298>`_,
-          `#299 <https://github.com/pytest-dev/pytest-cov/pull/299>`_ and
-          `#307 <https://github.com/pytest-dev/pytest-cov/pull/307>`_.
-        * Various testing improvements. Contributed by
-          Ned Batchelder,
-          Daniel Hahler,
-          Ionel Cristian Mărieș and
-          Hugo van Kemenade in
-          `#313 <https://github.com/pytest-dev/pytest-cov/pull/313>`_,
-          `#314 <https://github.com/pytest-dev/pytest-cov/pull/314>`_,
-          `#315 <https://github.com/pytest-dev/pytest-cov/pull/315>`_,
-          `#316 <https://github.com/pytest-dev/pytest-cov/pull/316>`_,
-          `#325 <https://github.com/pytest-dev/pytest-cov/pull/325>`_,
-          `#326 <https://github.com/pytest-dev/pytest-cov/pull/326>`_,
-          `#334 <https://github.com/pytest-dev/pytest-cov/pull/334>`_ and
-          `#335 <https://github.com/pytest-dev/pytest-cov/pull/335>`_.
-        * Added the ``--cov-context`` CLI options that enables coverage contexts. Only works with coverage 5.0+.
-          Contributed by Ned Batchelder in `#345 <https://github.com/pytest-dev/pytest-cov/pull/345>`_.
-        
-        2.7.1 (2019-05-03)
-        ------------------
-        
-        * Fixed source distribution manifest so that garbage ain't included in the tarball.
-        
-        2.7.0 (2019-05-03)
-        ------------------
-        
-        * Fixed ``AttributeError: 'NoneType' object has no attribute 'configure_node'`` error when ``--no-cov`` is used.
-          Contributed by Alexander Shadchin in `#263 <https://github.com/pytest-dev/pytest-cov/pull/263>`_.
-        * Various testing and CI improvements. Contributed by Daniel Hahler in
-          `#255 <https://github.com/pytest-dev/pytest-cov/pull/255>`_,
-          `#266 <https://github.com/pytest-dev/pytest-cov/pull/266>`_,
-          `#272 <https://github.com/pytest-dev/pytest-cov/pull/272>`_,
-          `#271 <https://github.com/pytest-dev/pytest-cov/pull/271>`_ and
-          `#269 <https://github.com/pytest-dev/pytest-cov/pull/269>`_.
-        * Improved documentation regarding subprocess and multiprocessing.
-          Contributed in `#265 <https://github.com/pytest-dev/pytest-cov/pull/265>`_.
-        * Improved ``pytest_cov.embed.cleanup_on_sigterm`` to be reentrant (signal deliveries while signal handling is
-          running won't break stuff).
-        * Added ``pytest_cov.embed.cleanup_on_signal`` for customized cleanup.
-        * Improved cleanup code and fixed various issues with leftover data files. All contributed in
-          `#265 <https://github.com/pytest-dev/pytest-cov/pull/265>`_ or
-          `#262 <https://github.com/pytest-dev/pytest-cov/pull/262>`_.
-        * Improved examples. Now there are two examples for the common project layouts, complete with working coverage
-          configuration. The examples have CI testing. Contributed in
-          `#267 <https://github.com/pytest-dev/pytest-cov/pull/267>`_.
-        * Improved help text for CLI options.
-        
-        2.6.1 (2019-01-07)
-        ------------------
-        
-        * Added support for Pytest 4.1. Contributed by Daniel Hahler and Семён Марьясин in
-          `#253 <https://github.com/pytest-dev/pytest-cov/pull/253>`_ and
-          `#230 <https://github.com/pytest-dev/pytest-cov/pull/230>`_.
-        * Various test and docs fixes. Contributed by Daniel Hahler in
-          `#224 <https://github.com/pytest-dev/pytest-cov/pull/224>`_ and
-          `#223 <https://github.com/pytest-dev/pytest-cov/pull/223>`_.
-        * Fixed the "Module already imported" issue (`#211 <https://github.com/pytest-dev/pytest-cov/issues/211>`_).
-          Contributed by Daniel Hahler in `#228 <https://github.com/pytest-dev/pytest-cov/pull/228>`_.
-        
-        2.6.0 (2018-09-03)
-        ------------------
-        
-        * Dropped support for Python 3 < 3.4, Pytest < 3.5 and Coverage < 4.4.
-        * Fixed some documentation formatting. Contributed by Jean Jordaan and Julian.
-        * Added an example with ``addopts`` in documentation. Contributed by Samuel Giffard in
-          `#195 <https://github.com/pytest-dev/pytest-cov/pull/195>`_.
-        * Fixed ``TypeError: 'NoneType' object is not iterable`` in certain xdist configurations. Contributed by Jeremy Bowman in
-          `#213 <https://github.com/pytest-dev/pytest-cov/pull/213>`_.
-        * Added a ``no_cover`` marker and fixture. Fixes
-          `#78 <https://github.com/pytest-dev/pytest-cov/issues/78>`_.
-        * Fixed broken ``no_cover`` check when running doctests. Contributed by Terence Honles in
-          `#200 <https://github.com/pytest-dev/pytest-cov/pull/200>`_.
-        * Fixed various issues with path normalization in reports (when combining coverage data from parallel mode). Fixes
-          `#130 <https://github.com/pytest-dev/pytest-cov/issues/161>`_.
-          Contributed by Ryan Hiebert & Ionel Cristian Mărieș in
-          `#178 <https://github.com/pytest-dev/pytest-cov/pull/178>`_.
-        * Report generation failures don't raise exceptions anymore. A warning will be logged instead. Fixes
-          `#161 <https://github.com/pytest-dev/pytest-cov/issues/161>`_.
-        * Fixed multiprocessing issue on Windows (empty env vars are not passed). Fixes
-          `#165 <https://github.com/pytest-dev/pytest-cov/issues/165>`_.
-        
-        2.5.1 (2017-05-11)
-        ------------------
-        
-        * Fixed xdist breakage (regression in ``2.5.0``).
-          Fixes `#157 <https://github.com/pytest-dev/pytest-cov/issues/157>`_.
-        * Allow setting custom ``data_file`` name in ``.coveragerc``.
-          Fixes `#145 <https://github.com/pytest-dev/pytest-cov/issues/145>`_.
-          Contributed by Jannis Leidel & Ionel Cristian Mărieș in
-          `#156 <https://github.com/pytest-dev/pytest-cov/pull/156>`_.
-        
-        2.5.0 (2017-05-09)
-        ------------------
-        
-        * Always show a summary when ``--cov-fail-under`` is used. Contributed by Francis Niu in `PR#141
-          <https://github.com/pytest-dev/pytest-cov/pull/141>`_.
-        * Added ``--cov-branch`` option. Fixes `#85 <https://github.com/pytest-dev/pytest-cov/issues/85>`_.
-        * Improve exception handling in subprocess setup. Fixes `#144 <https://github.com/pytest-dev/pytest-cov/issues/144>`_.
-        * Fixed handling when ``--cov`` is used multiple times. Fixes `#151 <https://github.com/pytest-dev/pytest-cov/issues/151>`_.
-        
-        2.4.0 (2016-10-10)
-        ------------------
-        
-        * Added a "disarm" option: ``--no-cov``. It will disable coverage measurements. Contributed by Zoltan Kozma in
-          `PR#135 <https://github.com/pytest-dev/pytest-cov/pull/135>`_.
-        
-          **WARNING: Do not put this in your configuration files, it's meant to be an one-off for situations where you want to
-          disable coverage from command line.**
-        * Fixed broken exception handling on ``.pth`` file. See `#136 <https://github.com/pytest-dev/pytest-cov/issues/136>`_.
-        
-        2.3.1 (2016-08-07)
-        ------------------
-        
-        * Fixed regression causing spurious errors when xdist was used. See `#124
-          <https://github.com/pytest-dev/pytest-cov/issues/124>`_.
-        * Fixed DeprecationWarning about incorrect `addoption` use. Contributed by Florian Bruhin in `PR#127
-          <https://github.com/pytest-dev/pytest-cov/pull/127>`_.
-        * Fixed deprecated use of funcarg fixture API. Contributed by Daniel Hahler in `PR#125
-          <https://github.com/pytest-dev/pytest-cov/pull/125>`_.
-        
-        2.3.0 (2016-07-05)
-        ------------------
-        
-        * Add support for specifying output location for html, xml, and annotate report.
-          Contributed by Patrick Lannigan in `PR#113 <https://github.com/pytest-dev/pytest-cov/pull/113>`_.
-        * Fix bug hiding test failure when cov-fail-under failed.
-        * For coverage >= 4.0, match the default behaviour of `coverage report` and
-          error if coverage fails to find the source instead of just printing a warning.
-          Contributed by David Szotten in `PR#116 <https://github.com/pytest-dev/pytest-cov/pull/116>`_.
-        * Fixed bug occurred when bare ``--cov`` parameter was used with xdist.
-          Contributed by Michael Elovskikh in `PR#120 <https://github.com/pytest-dev/pytest-cov/pull/120>`_.
-        * Add support for ``skip_covered`` and added ``--cov-report=term-skip-covered`` command
-          line options. Contributed by Saurabh Kumar in `PR#115 <https://github.com/pytest-dev/pytest-cov/pull/115>`_.
-        
-        2.2.1 (2016-01-30)
-        ------------------
-        
-        * Fixed incorrect merging of coverage data when xdist was used and coverage was ``>= 4.0``.
-        
-        2.2.0 (2015-10-04)
-        ------------------
-        
-        * Added support for changing working directory in tests. Previously changing working
-          directory would disable coverage measurements in suprocesses.
-        * Fixed broken handling for ``--cov-report=annotate``.
-        
-        2.1.0 (2015-08-23)
-        ------------------
-        
-        * Added support for `coverage 4.0b2`.
-        * Added the ``--cov-append`` command line options. Contributed by Christian Ledermann
-          in `PR#80 <https://github.com/pytest-dev/pytest-cov/pull/80>`_.
-        
-        2.0.0 (2015-07-28)
-        ------------------
-        
-        * Added ``--cov-fail-under``, akin to the new ``fail_under`` option in `coverage-4.0`
-          (automatically activated if there's a ``[report] fail_under = ...`` in ``.coveragerc``).
-        * Changed ``--cov-report=term`` to automatically upgrade to ``--cov-report=term-missing``
-          if there's ``[run] show_missing = True`` in ``.coveragerc``.
-        * Changed ``--cov`` so it can be used with no path argument (in which case the source
-          settings from ``.coveragerc`` will be used instead).
-        * Fixed `.pth` installation to work in all cases (install, easy_install, wheels, develop etc).
-        * Fixed `.pth` uninstallation to work for wheel installs.
-        * Support for coverage 4.0.
-        * Data file suffixing changed to use coverage's ``data_suffix=True`` option (instead of the
-          custom suffixing).
-        * Avoid warning about missing coverage data (just like ``coverage.control.process_startup``).
-        * Fixed a race condition when running with xdist (all the workers tried to combine the files).
-          It's possible that this issue is not present in `pytest-cov 1.8.X`.
-        
-        1.8.2 (2014-11-06)
-        ------------------
-        
-        * N/A
-        
+Project-URL: Documentation, https://pytest-cov.readthedocs.io/
+Project-URL: Changelog, https://pytest-cov.readthedocs.io/en/latest/changelog.html
+Project-URL: Issue Tracker, https://github.com/pytest-dev/pytest-cov/issues
 Keywords: cover,coverage,pytest,py.test,distributed,parallel
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -522,7 +28,531 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Provides-Extra: testing
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+========
+Overview
+========
+
+.. start-badges
+
+.. list-table::
+    :stub-columns: 1
+
+    * - docs
+      - |docs|
+    * - tests
+      - | |github-actions| |requires|
+        |
+    * - package
+      - | |version| |conda-forge| |wheel| |supported-versions| |supported-implementations|
+        | |commits-since|
+
+.. |docs| image:: https://readthedocs.org/projects/pytest-cov/badge/?style=flat
+    :target: https://readthedocs.org/projects/pytest-cov
+    :alt: Documentation Status
+
+.. |github-actions| image:: https://github.com/pytest-dev/pytest-cov/actions/workflows/test.yml/badge.svg
+    :alt: GitHub Actions Status
+    :target: https://github.com/pytest-dev/pytest-cov/actions
+
+.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/pytest-dev/pytest-cov?branch=master&svg=true
+    :alt: AppVeyor Build Status
+    :target: https://ci.appveyor.com/project/pytestbot/pytest-cov
+
+.. |requires| image:: https://requires.io/github/pytest-dev/pytest-cov/requirements.svg?branch=master
+    :alt: Requirements Status
+    :target: https://requires.io/github/pytest-dev/pytest-cov/requirements/?branch=master
+
+.. |version| image:: https://img.shields.io/pypi/v/pytest-cov.svg
+    :alt: PyPI Package latest release
+    :target: https://pypi.org/project/pytest-cov
+
+.. |conda-forge| image:: https://img.shields.io/conda/vn/conda-forge/pytest-cov.svg
+    :target: https://anaconda.org/conda-forge/pytest-cov
+
+.. |commits-since| image:: https://img.shields.io/github/commits-since/pytest-dev/pytest-cov/v4.0.0.svg
+    :alt: Commits since latest release
+    :target: https://github.com/pytest-dev/pytest-cov/compare/v4.0.0...master
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/pytest-cov.svg
+    :alt: PyPI Wheel
+    :target: https://pypi.org/project/pytest-cov
+
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pytest-cov.svg
+    :alt: Supported versions
+    :target: https://pypi.org/project/pytest-cov
+
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pytest-cov.svg
+    :alt: Supported implementations
+    :target: https://pypi.org/project/pytest-cov
+
+.. end-badges
+
+This plugin produces coverage reports. Compared to just using ``coverage run`` this plugin does some extras:
+
+* Subprocess support: you can fork or run stuff in a subprocess and will get covered without any fuss.
+* Xdist support: you can use all of pytest-xdist's features and still get coverage.
+* Consistent pytest behavior. If you run ``coverage run -m pytest`` you will have slightly different ``sys.path`` (CWD will be
+  in it, unlike when running ``pytest``).
+
+All features offered by the coverage package should work, either through pytest-cov's command line options or
+through coverage's config file.
+
+* Free software: MIT license
+
+Installation
+============
+
+Install with pip::
+
+    pip install pytest-cov
+
+For distributed testing support install pytest-xdist::
+
+    pip install pytest-xdist
+
+Upgrading from ancient pytest-cov
+---------------------------------
+
+`pytest-cov 2.0` is using a new ``.pth`` file (``pytest-cov.pth``). You may want to manually remove the older
+``init_cov_core.pth`` from site-packages as it's not automatically removed.
+
+Uninstalling
+------------
+
+Uninstall with pip::
+
+    pip uninstall pytest-cov
+
+Under certain scenarios a stray ``.pth`` file may be left around in site-packages.
+
+* `pytest-cov 2.0` may leave a ``pytest-cov.pth`` if you installed without wheels
+  (``easy_install``, ``setup.py install`` etc).
+* `pytest-cov 1.8 or older` will leave a ``init_cov_core.pth``.
+
+Usage
+=====
+
+::
+
+    pytest --cov=myproj tests/
+
+Would produce a report like::
+
+    -------------------- coverage: ... ---------------------
+    Name                 Stmts   Miss  Cover
+    ----------------------------------------
+    myproj/__init__          2      0   100%
+    myproj/myproj          257     13    94%
+    myproj/feature4286      94      7    92%
+    ----------------------------------------
+    TOTAL                  353     20    94%
+
+Documentation
+=============
+
+    http://pytest-cov.rtfd.org/
+
+
+
+
+
+
+Coverage Data File
+==================
+
+The data file is erased at the beginning of testing to ensure clean data for each test run. If you
+need to combine the coverage of several test runs you can use the ``--cov-append`` option to append
+this coverage data to coverage data from previous test runs.
+
+The data file is left at the end of testing so that it is possible to use normal coverage tools to
+examine it.
+
+Limitations
+===========
+
+For distributed testing the workers must have the pytest-cov package installed.  This is needed since
+the plugin must be registered through setuptools for pytest to start the plugin on the
+worker.
+
+For subprocess measurement environment variables must make it from the main process to the
+subprocess.  The python used by the subprocess must have pytest-cov installed.  The subprocess must
+do normal site initialisation so that the environment variables can be detected and coverage
+started.
+
+
+Acknowledgements
+================
+
+Whilst this plugin has been built fresh from the ground up it has been influenced by the work done
+on pytest-coverage (Ross Lawley, James Mills, Holger Krekel) and nose-cover (Jason Pellerin) which are
+other coverage plugins.
+
+Ned Batchelder for coverage and its ability to combine the coverage results of parallel runs.
+
+Holger Krekel for pytest with its distributed testing support.
+
+Jason Pellerin for nose.
+
+Michael Foord for unittest2.
+
+No doubt others have contributed to these tools as well.
+
+Changelog
+=========
+
+
+4.0.0 (2022-09-28)
+------------------
+
+**Note that this release drops support for multiprocessing.**
+
+
+* `--cov-fail-under` no longer causes `pytest --collect-only` to fail
+  Contributed by Zac Hatfield-Dodds in `#511 <https://github.com/pytest-dev/pytest-cov/pull/511>`_.
+* Dropped support for multiprocessing (mostly because `issue 82408 <https://github.com/python/cpython/issues/82408>`_). This feature was
+  mostly working but very broken in certain scenarios and made the test suite very flaky and slow.
+
+  There is builtin multiprocessing support in coverage and you can migrate to that. All you need is this in your
+  ``.coveragerc``::
+
+    [run]
+    concurrency = multiprocessing
+    parallel = true
+    sigterm = true
+* Fixed deprecation in ``setup.py`` by trying to import setuptools before distutils.
+  Contributed by Ben Greiner in `#545 <https://github.com/pytest-dev/pytest-cov/pull/545>`_.
+* Removed undesirable new lines that were displayed while reporting was disabled.
+  Contributed by Delgan in `#540 <https://github.com/pytest-dev/pytest-cov/pull/540>`_.
+* Documentation fixes.
+  Contributed by Andre Brisco in `#543 <https://github.com/pytest-dev/pytest-cov/pull/543>`_
+  and Colin O'Dell in `#525 <https://github.com/pytest-dev/pytest-cov/pull/525>`_.
+* Added support for LCOV output format via `--cov-report=lcov`. Only works with coverage 6.3+.
+  Contributed by Christian Fetzer in `#536 <https://github.com/pytest-dev/pytest-cov/issues/536>`_.
+* Modernized pytest hook implementation.
+  Contributed by Bruno Oliveira in `#549 <https://github.com/pytest-dev/pytest-cov/pull/549>`_
+  and Ronny Pfannschmidt in `#550 <https://github.com/pytest-dev/pytest-cov/pull/550>`_.
+
+
+3.0.0 (2021-10-04)
+-------------------
+
+**Note that this release drops support for Python 2.7 and Python 3.5.**
+
+* Added support for Python 3.10 and updated various test dependencies.
+  Contributed by Hugo van Kemenade in
+  `#500 <https://github.com/pytest-dev/pytest-cov/pull/500>`_.
+* Switched from Travis CI to GitHub Actions. Contributed by Hugo van Kemenade in
+  `#494 <https://github.com/pytest-dev/pytest-cov/pull/494>`_ and
+  `#495 <https://github.com/pytest-dev/pytest-cov/pull/495>`_.
+* Add a ``--cov-reset`` CLI option.
+  Contributed by Danilo Šegan in
+  `#459 <https://github.com/pytest-dev/pytest-cov/pull/459>`_.
+* Improved validation of ``--cov-fail-under`` CLI option.
+  Contributed by ... Ronny Pfannschmidt's desire for skark in
+  `#480 <https://github.com/pytest-dev/pytest-cov/pull/480>`_.
+* Dropped Python 2.7 support.
+  Contributed by Thomas Grainger in
+  `#488 <https://github.com/pytest-dev/pytest-cov/pull/488>`_.
+* Updated trove classifiers. Contributed by Michał Bielawski in
+  `#481 <https://github.com/pytest-dev/pytest-cov/pull/481>`_.
+* Reverted change for `toml` requirement.
+  Contributed by Thomas Grainger in
+  `#477 <https://github.com/pytest-dev/pytest-cov/pull/477>`_.
+
+2.12.1 (2021-06-01)
+-------------------
+
+* Changed the `toml` requirement to be always be directly required (instead of being required through a coverage extra).
+  This fixes issues with pip-compile (`pip-tools#1300 <https://github.com/jazzband/pip-tools/issues/1300>`_).
+  Contributed by Sorin Sbarnea in `#472 <https://github.com/pytest-dev/pytest-cov/pull/472>`_.
+* Documented ``show_contexts``.
+  Contributed by Brian Rutledge in `#473 <https://github.com/pytest-dev/pytest-cov/pull/473>`_.
+
+2.12.0 (2021-05-14)
+-------------------
+
+* Added coverage's `toml` extra to install requirements in setup.py.
+  Contributed by Christian Riedel in `#410 <https://github.com/pytest-dev/pytest-cov/pull/410>`_.
+* Fixed ``pytest_cov.__version__`` to have the right value (string with version instead of a string
+  including ``__version__ =``).
+* Fixed license classifier in ``setup.py``.
+  Contributed by Chris Sreesangkom in `#467 <https://github.com/pytest-dev/pytest-cov/pull/467>`_.
+* Fixed *commits since* badge.
+  Contributed by Terence Honles in `#470 <https://github.com/pytest-dev/pytest-cov/pull/470>`_.
+
+2.11.1 (2021-01-20)
+-------------------
+
+* Fixed support for newer setuptools (v42+).
+  Contributed by Michał Górny in `#451 <https://github.com/pytest-dev/pytest-cov/pull/451>`_.
+
+2.11.0 (2021-01-18)
+-------------------
+
+* Bumped minimum coverage requirement to 5.2.1. This prevents reporting issues.
+  Contributed by Mateus Berardo de Souza Terra in `#433 <https://github.com/pytest-dev/pytest-cov/pull/433>`_.
+* Improved sample projects (from the `examples <https://github.com/pytest-dev/pytest-cov/tree/master/examples>`_
+  directory) to support running `tox -e pyXY`. Now the example configures a suffixed coverage data file,
+  and that makes the cleanup environment unnecessary.
+  Contributed by Ganden Schaffner in `#435 <https://github.com/pytest-dev/pytest-cov/pull/435>`_.
+* Removed the empty `console_scripts` entrypoint that confused some Gentoo build script.
+  I didn't ask why it was so broken cause I didn't want to ruin my day.
+  Contributed by Michał Górny in `#434 <https://github.com/pytest-dev/pytest-cov/pull/434>`_.
+* Fixed the missing `coverage context <https://coverage.readthedocs.io/en/stable/contexts.html>`_
+  when using subprocesses.
+  Contributed by Bernát Gábor in `#443 <https://github.com/pytest-dev/pytest-cov/pull/443>`_.
+* Updated the config section in the docs.
+  Contributed by Pamela McA'Nulty in `#429 <https://github.com/pytest-dev/pytest-cov/pull/429>`_.
+* Migrated CI to travis-ci.com (from .org).
+
+2.10.1 (2020-08-14)
+-------------------
+
+* Support for ``pytest-xdist`` 2.0, which breaks compatibility with ``pytest-xdist`` before 1.22.3 (from 2017).
+  Contributed by Zac Hatfield-Dodds in `#412 <https://github.com/pytest-dev/pytest-cov/pull/412>`_.
+* Fixed the ``LocalPath has no attribute startswith`` failure that occurred when using the ``pytester`` plugin
+  in inline mode.
+
+2.10.0 (2020-06-12)
+-------------------
+
+* Improved the ``--no-cov`` warning. Now it's only shown if ``--no-cov`` is present before ``--cov``.
+* Removed legacy pytest support. Changed ``setup.py`` so that ``pytest>=4.6`` is required.
+
+2.9.0 (2020-05-22)
+------------------
+
+* Fixed ``RemovedInPytest4Warning`` when using Pytest 3.10.
+  Contributed by Michael Manganiello in `#354 <https://github.com/pytest-dev/pytest-cov/pull/354>`_.
+* Made pytest startup faster when plugin not active by lazy-importing.
+  Contributed by Anders Hovmöller in `#339 <https://github.com/pytest-dev/pytest-cov/pull/339>`_.
+* Various CI improvements.
+  Contributed by Daniel Hahler in `#363 <https://github.com/pytest-dev/pytest-cov/pull/>`_ and
+  `#364 <https://github.com/pytest-dev/pytest-cov/pull/364>`_.
+* Various Python support updates (drop EOL 3.4, test against 3.8 final).
+  Contributed by Hugo van Kemenade in
+  `#336 <https://github.com/pytest-dev/pytest-cov/pull/336>`_ and
+  `#367 <https://github.com/pytest-dev/pytest-cov/pull/367>`_.
+* Changed ``--cov-append`` to always enable ``data_suffix`` (a coverage setting).
+  Contributed by Harm Geerts in
+  `#387 <https://github.com/pytest-dev/pytest-cov/pull/387>`_.
+* Changed ``--cov-append`` to handle loading previous data better
+  (fixes various path aliasing issues).
+* Various other testing improvements, github issue templates, example updates.
+* Fixed internal failures that are caused by tests that change the current working directory by
+  ensuring a consistent working directory when coverage is called.
+  See `#306 <https://github.com/pytest-dev/pytest-cov/issues/306>`_ and
+  `coveragepy#881 <https://github.com/nedbat/coveragepy/issues/881>`_
+
+2.8.1 (2019-10-05)
+------------------
+
+* Fixed `#348 <https://github.com/pytest-dev/pytest-cov/issues/348>`_ -
+  regression when only certain reports (html or xml) are used then ``--cov-fail-under`` always fails.
+
+2.8.0 (2019-10-04)
+------------------
+
+* Fixed ``RecursionError`` that can occur when using
+  `cleanup_on_signal <https://pytest-cov.readthedocs.io/en/latest/subprocess-support.html#if-you-got-custom-signal-handling>`__ or
+  `cleanup_on_sigterm <https://pytest-cov.readthedocs.io/en/latest/subprocess-support.html#if-you-got-custom-signal-handling>`__.
+  See: `#294 <https://github.com/pytest-dev/pytest-cov/issues/294>`_.
+  The 2.7.x releases of pytest-cov should be considered broken regarding aforementioned cleanup API.
+* Added compatibility with future xdist release that deprecates some internals
+  (match pytest-xdist master/worker terminology).
+  Contributed by Thomas Grainger in `#321 <https://github.com/pytest-dev/pytest-cov/pull/321>`_
+* Fixed breakage that occurs when multiple reporting options are used.
+  Contributed by Thomas Grainger in `#338 <https://github.com/pytest-dev/pytest-cov/pull/338>`_.
+* Changed internals to use a stub instead of ``os.devnull``.
+  Contributed by Thomas Grainger in `#332 <https://github.com/pytest-dev/pytest-cov/pull/332>`_.
+* Added support for Coverage 5.0.
+  Contributed by Ned Batchelder in `#319 <https://github.com/pytest-dev/pytest-cov/pull/319>`_.
+* Added support for float values in ``--cov-fail-under``.
+  Contributed by Martín Gaitán in `#311 <https://github.com/pytest-dev/pytest-cov/pull/311>`_.
+* Various documentation fixes. Contributed by
+  Juanjo Bazán,
+  Andrew Murray and
+  Albert Tugushev in
+  `#298 <https://github.com/pytest-dev/pytest-cov/pull/298>`_,
+  `#299 <https://github.com/pytest-dev/pytest-cov/pull/299>`_ and
+  `#307 <https://github.com/pytest-dev/pytest-cov/pull/307>`_.
+* Various testing improvements. Contributed by
+  Ned Batchelder,
+  Daniel Hahler,
+  Ionel Cristian Mărieș and
+  Hugo van Kemenade in
+  `#313 <https://github.com/pytest-dev/pytest-cov/pull/313>`_,
+  `#314 <https://github.com/pytest-dev/pytest-cov/pull/314>`_,
+  `#315 <https://github.com/pytest-dev/pytest-cov/pull/315>`_,
+  `#316 <https://github.com/pytest-dev/pytest-cov/pull/316>`_,
+  `#325 <https://github.com/pytest-dev/pytest-cov/pull/325>`_,
+  `#326 <https://github.com/pytest-dev/pytest-cov/pull/326>`_,
+  `#334 <https://github.com/pytest-dev/pytest-cov/pull/334>`_ and
+  `#335 <https://github.com/pytest-dev/pytest-cov/pull/335>`_.
+* Added the ``--cov-context`` CLI options that enables coverage contexts. Only works with coverage 5.0+.
+  Contributed by Ned Batchelder in `#345 <https://github.com/pytest-dev/pytest-cov/pull/345>`_.
+
+2.7.1 (2019-05-03)
+------------------
+
+* Fixed source distribution manifest so that garbage ain't included in the tarball.
+
+2.7.0 (2019-05-03)
+------------------
+
+* Fixed ``AttributeError: 'NoneType' object has no attribute 'configure_node'`` error when ``--no-cov`` is used.
+  Contributed by Alexander Shadchin in `#263 <https://github.com/pytest-dev/pytest-cov/pull/263>`_.
+* Various testing and CI improvements. Contributed by Daniel Hahler in
+  `#255 <https://github.com/pytest-dev/pytest-cov/pull/255>`_,
+  `#266 <https://github.com/pytest-dev/pytest-cov/pull/266>`_,
+  `#272 <https://github.com/pytest-dev/pytest-cov/pull/272>`_,
+  `#271 <https://github.com/pytest-dev/pytest-cov/pull/271>`_ and
+  `#269 <https://github.com/pytest-dev/pytest-cov/pull/269>`_.
+* Improved ``pytest_cov.embed.cleanup_on_sigterm`` to be reentrant (signal deliveries while signal handling is
+  running won't break stuff).
+* Added ``pytest_cov.embed.cleanup_on_signal`` for customized cleanup.
+* Improved cleanup code and fixed various issues with leftover data files. All contributed in
+  `#265 <https://github.com/pytest-dev/pytest-cov/pull/265>`_ or
+  `#262 <https://github.com/pytest-dev/pytest-cov/pull/262>`_.
+* Improved examples. Now there are two examples for the common project layouts, complete with working coverage
+  configuration. The examples have CI testing. Contributed in
+  `#267 <https://github.com/pytest-dev/pytest-cov/pull/267>`_.
+* Improved help text for CLI options.
+
+2.6.1 (2019-01-07)
+------------------
+
+* Added support for Pytest 4.1. Contributed by Daniel Hahler and Семён Марьясин in
+  `#253 <https://github.com/pytest-dev/pytest-cov/pull/253>`_ and
+  `#230 <https://github.com/pytest-dev/pytest-cov/pull/230>`_.
+* Various test and docs fixes. Contributed by Daniel Hahler in
+  `#224 <https://github.com/pytest-dev/pytest-cov/pull/224>`_ and
+  `#223 <https://github.com/pytest-dev/pytest-cov/pull/223>`_.
+* Fixed the "Module already imported" issue (`#211 <https://github.com/pytest-dev/pytest-cov/issues/211>`_).
+  Contributed by Daniel Hahler in `#228 <https://github.com/pytest-dev/pytest-cov/pull/228>`_.
+
+2.6.0 (2018-09-03)
+------------------
+
+* Dropped support for Python 3 < 3.4, Pytest < 3.5 and Coverage < 4.4.
+* Fixed some documentation formatting. Contributed by Jean Jordaan and Julian.
+* Added an example with ``addopts`` in documentation. Contributed by Samuel Giffard in
+  `#195 <https://github.com/pytest-dev/pytest-cov/pull/195>`_.
+* Fixed ``TypeError: 'NoneType' object is not iterable`` in certain xdist configurations. Contributed by Jeremy Bowman in
+  `#213 <https://github.com/pytest-dev/pytest-cov/pull/213>`_.
+* Added a ``no_cover`` marker and fixture. Fixes
+  `#78 <https://github.com/pytest-dev/pytest-cov/issues/78>`_.
+* Fixed broken ``no_cover`` check when running doctests. Contributed by Terence Honles in
+  `#200 <https://github.com/pytest-dev/pytest-cov/pull/200>`_.
+* Fixed various issues with path normalization in reports (when combining coverage data from parallel mode). Fixes
+  `#130 <https://github.com/pytest-dev/pytest-cov/issues/161>`_.
+  Contributed by Ryan Hiebert & Ionel Cristian Mărieș in
+  `#178 <https://github.com/pytest-dev/pytest-cov/pull/178>`_.
+* Report generation failures don't raise exceptions anymore. A warning will be logged instead. Fixes
+  `#161 <https://github.com/pytest-dev/pytest-cov/issues/161>`_.
+* Fixed multiprocessing issue on Windows (empty env vars are not passed). Fixes
+  `#165 <https://github.com/pytest-dev/pytest-cov/issues/165>`_.
+
+2.5.1 (2017-05-11)
+------------------
+
+* Fixed xdist breakage (regression in ``2.5.0``).
+  Fixes `#157 <https://github.com/pytest-dev/pytest-cov/issues/157>`_.
+* Allow setting custom ``data_file`` name in ``.coveragerc``.
+  Fixes `#145 <https://github.com/pytest-dev/pytest-cov/issues/145>`_.
+  Contributed by Jannis Leidel & Ionel Cristian Mărieș in
+  `#156 <https://github.com/pytest-dev/pytest-cov/pull/156>`_.
+
+2.5.0 (2017-05-09)
+------------------
+
+* Always show a summary when ``--cov-fail-under`` is used. Contributed by Francis Niu in `PR#141
+  <https://github.com/pytest-dev/pytest-cov/pull/141>`_.
+* Added ``--cov-branch`` option. Fixes `#85 <https://github.com/pytest-dev/pytest-cov/issues/85>`_.
+* Improve exception handling in subprocess setup. Fixes `#144 <https://github.com/pytest-dev/pytest-cov/issues/144>`_.
+* Fixed handling when ``--cov`` is used multiple times. Fixes `#151 <https://github.com/pytest-dev/pytest-cov/issues/151>`_.
+
+2.4.0 (2016-10-10)
+------------------
+
+* Added a "disarm" option: ``--no-cov``. It will disable coverage measurements. Contributed by Zoltan Kozma in
+  `PR#135 <https://github.com/pytest-dev/pytest-cov/pull/135>`_.
+
+  **WARNING: Do not put this in your configuration files, it's meant to be an one-off for situations where you want to
+  disable coverage from command line.**
+* Fixed broken exception handling on ``.pth`` file. See `#136 <https://github.com/pytest-dev/pytest-cov/issues/136>`_.
+
+2.3.1 (2016-08-07)
+------------------
+
+* Fixed regression causing spurious errors when xdist was used. See `#124
+  <https://github.com/pytest-dev/pytest-cov/issues/124>`_.
+* Fixed DeprecationWarning about incorrect `addoption` use. Contributed by Florian Bruhin in `PR#127
+  <https://github.com/pytest-dev/pytest-cov/pull/127>`_.
+* Fixed deprecated use of funcarg fixture API. Contributed by Daniel Hahler in `PR#125
+  <https://github.com/pytest-dev/pytest-cov/pull/125>`_.
+
+2.3.0 (2016-07-05)
+------------------
+
+* Add support for specifying output location for html, xml, and annotate report.
+  Contributed by Patrick Lannigan in `PR#113 <https://github.com/pytest-dev/pytest-cov/pull/113>`_.
+* Fix bug hiding test failure when cov-fail-under failed.
+* For coverage >= 4.0, match the default behaviour of `coverage report` and
+  error if coverage fails to find the source instead of just printing a warning.
+  Contributed by David Szotten in `PR#116 <https://github.com/pytest-dev/pytest-cov/pull/116>`_.
+* Fixed bug occurred when bare ``--cov`` parameter was used with xdist.
+  Contributed by Michael Elovskikh in `PR#120 <https://github.com/pytest-dev/pytest-cov/pull/120>`_.
+* Add support for ``skip_covered`` and added ``--cov-report=term-skip-covered`` command
+  line options. Contributed by Saurabh Kumar in `PR#115 <https://github.com/pytest-dev/pytest-cov/pull/115>`_.
+
+2.2.1 (2016-01-30)
+------------------
+
+* Fixed incorrect merging of coverage data when xdist was used and coverage was ``>= 4.0``.
+
+2.2.0 (2015-10-04)
+------------------
+
+* Added support for changing working directory in tests. Previously changing working
+  directory would disable coverage measurements in suprocesses.
+* Fixed broken handling for ``--cov-report=annotate``.
+
+2.1.0 (2015-08-23)
+------------------
+
+* Added support for `coverage 4.0b2`.
+* Added the ``--cov-append`` command line options. Contributed by Christian Ledermann
+  in `PR#80 <https://github.com/pytest-dev/pytest-cov/pull/80>`_.
+
+2.0.0 (2015-07-28)
+------------------
+
+* Added ``--cov-fail-under``, akin to the new ``fail_under`` option in `coverage-4.0`
+  (automatically activated if there's a ``[report] fail_under = ...`` in ``.coveragerc``).
+* Changed ``--cov-report=term`` to automatically upgrade to ``--cov-report=term-missing``
+  if there's ``[run] show_missing = True`` in ``.coveragerc``.
+* Changed ``--cov`` so it can be used with no path argument (in which case the source
+  settings from ``.coveragerc`` will be used instead).
+* Fixed `.pth` installation to work in all cases (install, easy_install, wheels, develop etc).
+* Fixed `.pth` uninstallation to work for wheel installs.
+* Support for coverage 4.0.
+* Data file suffixing changed to use coverage's ``data_suffix=True`` option (instead of the
+  custom suffixing).
+* Avoid warning about missing coverage data (just like ``coverage.control.process_startup``).
+* Fixed a race condition when running with xdist (all the workers tried to combine the files).
+  It's possible that this issue is not present in `pytest-cov 1.8.X`.
+
+1.8.2 (2014-11-06)
+------------------
+
+* N/A
+
+
```

### Comparing `pytest-cov-3.0.0/README.rst` & `pytest-cov-4.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 .. list-table::
     :stub-columns: 1
 
     * - docs
       - |docs|
     * - tests
-      - | |github-actions| |appveyor| |requires|
+      - | |github-actions| |requires|
+        |
     * - package
       - | |version| |conda-forge| |wheel| |supported-versions| |supported-implementations|
         | |commits-since|
 
 .. |docs| image:: https://readthedocs.org/projects/pytest-cov/badge/?style=flat
     :target: https://readthedocs.org/projects/pytest-cov
     :alt: Documentation Status
@@ -34,17 +35,17 @@
 .. |version| image:: https://img.shields.io/pypi/v/pytest-cov.svg
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/pytest-cov
 
 .. |conda-forge| image:: https://img.shields.io/conda/vn/conda-forge/pytest-cov.svg
     :target: https://anaconda.org/conda-forge/pytest-cov
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/pytest-dev/pytest-cov/v3.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/pytest-dev/pytest-cov/v4.0.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/pytest-dev/pytest-cov/compare/v3.0.0...master
+    :target: https://github.com/pytest-dev/pytest-cov/compare/v4.0.0...master
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/pytest-cov.svg
     :alt: PyPI Wheel
     :target: https://pypi.org/project/pytest-cov
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pytest-cov.svg
     :alt: Supported versions
```

### Comparing `pytest-cov-3.0.0/ci/bootstrap.py` & `pytest-cov-4.0.0/ci/bootstrap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 
 import os
 import subprocess
 import sys
-from collections import defaultdict
 from os.path import abspath
 from os.path import dirname
 from os.path import exists
 from os.path import join
+from os.path import relpath
 
 base_path = dirname(dirname(abspath(__file__)))
+templates_path = join(base_path, "ci", "templates")
 
 
 def check_call(args):
     print("+", *args)
     subprocess.check_call(args)
 
 
@@ -47,38 +48,37 @@
 
 def main():
     import jinja2
 
     print(f"Project path: {base_path}")
 
     jinja = jinja2.Environment(
-        loader=jinja2.FileSystemLoader(join(base_path, "ci", "templates")),
+        loader=jinja2.FileSystemLoader(templates_path),
         trim_blocks=True,
         lstrip_blocks=True,
         keep_trailing_newline=True
     )
 
     tox_environments = [
         line.strip()
-        # WARNING: 'tox' must be installed globally or in the project's virtualenv
-        for line in subprocess.check_output(['tox', '--listenvs'], universal_newlines=True).splitlines()
+        # 'tox' need not be installed globally, but must be importable
+        # by the Python that is running this script.
+        # This uses sys.executable the same way that the call in
+        # cookiecutter-pylibrary/hooks/post_gen_project.py
+        # invokes this bootstrap.py itself.
+        for line in subprocess.check_output([sys.executable, '-m', 'tox', '--listenvs'], universal_newlines=True).splitlines()
     ]
-    tox_environments = [line for line in tox_environments if line not in ['clean', 'report', 'docs', 'check']]
+    tox_environments = [line for line in tox_environments if line.startswith('py')]
 
-    template_vars = defaultdict(list)
-    template_vars['tox_environments'] = tox_environments
-    for env in tox_environments:
-        first, _ = env.split('-', 1)
-        template_vars['%s_environments' % first].append(env)
-
-    for name in os.listdir(join("ci", "templates")):
-        with open(join(base_path, name), "w") as fh:
-            fh.write('# NOTE: this file is auto-generated via ci/bootstrap.py (ci/templates/%s).\n' % name)
-            fh.write(jinja.get_template(name).render(**template_vars))
-        print(f"Wrote {name}")
+    for root, _, files in os.walk(templates_path):
+        for name in files:
+            relative = relpath(root, templates_path)
+            with open(join(base_path, relative, name), "w") as fh:
+                fh.write(jinja.get_template(join(relative, name)).render(tox_environments=tox_environments))
+            print(f"Wrote {name}")
     print("DONE.")
 
 
 if __name__ == "__main__":
     args = sys.argv[1:]
     if args == ["--no-env"]:
         main()
```

### Comparing `pytest-cov-3.0.0/docs/conf.py` & `pytest-cov-4.0.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'pytest-cov'
 year = '2016'
 author = 'pytest-cov contributors'
 copyright = f'{year}, {author}'
-version = release = '3.0.0'
+version = release = '4.0.0'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/pytest-dev/pytest-cov/issues/%s', '#'),
     'pr': ('https://github.com/pytest-dev/pytest-cov/pull/%s', 'PR #'),
 }
```

### Comparing `pytest-cov-3.0.0/docs/config.rst` & `pytest-cov-4.0.0/docs/config.rst`

 * *Files 9% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 
 For full details refer to the `coverage config file`_ documentation.
 
 .. _`coverage config file`: https://coverage.readthedocs.io/en/latest/config.html
 
 .. note:: Important Note
 
-    This plugin overrides the ``data_file`` and ``parallel`` options of coverage. Unless you also run coverage without
-    pytest-cov it's pointless to set those options in your ``.coveragerc``.
+    This plugin overrides the ``parallel`` option of coverage. Unless you also run coverage without pytest-cov it's
+    pointless to set those options in your ``.coveragerc``.
 
-    If you use the ``--cov=something`` option (with a value) then coverage's ``source`` option will also get overriden.
-    If you have multiple sources it might be easier to set those in ``.coveragerc`` and always use ``--cov`` (wihout a value)
+    If you use the ``--cov=something`` option (with a value) then coverage's ``source`` option will also get overridden.
+    If you have multiple sources it might be easier to set those in ``.coveragerc`` and always use ``--cov`` (without a value)
     instead of having a long command line with ``--cov=pkg1 --cov=pkg2 --cov=pkg3 ...``.
 
-    If you use the ``--cov-branch`` option then coverage's ``branch`` option will also get overriden.
+    If you use the ``--cov-branch`` option then coverage's ``branch`` option will also get overridden.
 
 If you wish to always add pytest-cov with pytest, you can use ``addopts`` under ``pytest`` or ``tool:pytest`` section.
 For example: ::
 
     [tool:pytest]
     addopts = --cov=<project-name> --cov-report html
 
@@ -52,17 +52,17 @@
 Reference
 =========
 
 The complete list of command line options is:
 
   --cov=PATH            Measure coverage for filesystem path. (multi-allowed)
   --cov-report=type     Type of report to generate: term, term-missing,
-                        annotate, html, xml (multi-allowed). term, term-
+                        annotate, html, xml, lcov (multi-allowed). term, term-
                         missing may be followed by ":skip-covered". annotate,
-                        html and xml may be followed by ":DEST" where DEST
+                        html, xml and lcov may be followed by ":DEST" where DEST
                         specifies the output location. Use --cov-report= to
                         not generate any output.
   --cov-config=path     Config file for coverage. Default: .coveragerc
   --no-cov-on-fail      Do not report coverage if test run fails. Default:
                         False
   --no-cov              Disable coverage report completely (useful for
                         debuggers). Default: False
```

### Comparing `pytest-cov-3.0.0/docs/contexts.rst` & `pytest-cov-4.0.0/docs/contexts.rst`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/docs/debuggers.rst` & `pytest-cov-4.0.0/docs/debuggers.rst`

 * *Files 19% similar despite different names*

```diff
@@ -3,13 +3,19 @@
 =====================
 
 (or other IDEs)
 
 When it comes to TDD one obviously would like to debug tests. Debuggers in Python use mostly the sys.settrace function
 to gain access to context. Coverage uses the same technique to get access to the lines executed. Coverage does not play
 well with other tracers simultaneously running. This manifests itself in behaviour that PyCharm might not hit a
-breakpoint no matter what the user does. Since it is common practice to have coverage configuration in the pytest.ini
+breakpoint no matter what the user does, or encountering an error like this::
+
+    PYDEV DEBUGGER WARNING:
+    sys.settrace() should not be used when the debugger is being used.
+    This may cause the debugger to stop working correctly.
+
+Since it is common practice to have coverage configuration in the pytest.ini
 file and pytest does not support removeopts or similar the `--no-cov` flag can disable coverage completely.
 
 At the reporting part a warning message will show on screen::
 
     Coverage disabled via --no-cov switch!
```

### Comparing `pytest-cov-3.0.0/docs/markers-fixtures.rst` & `pytest-cov-4.0.0/docs/markers-fixtures.rst`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/docs/plugins.rst` & `pytest-cov-4.0.0/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/docs/releasing.rst` & `pytest-cov-4.0.0/docs/releasing.rst`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/docs/reporting.rst` & `pytest-cov-4.0.0/docs/reporting.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Reporting
 =========
 
 It is possible to generate any combination of the reports for a single test run.
 
-The available reports are terminal (with or without missing line numbers shown), HTML, XML and
+The available reports are terminal (with or without missing line numbers shown), HTML, XML, LCOV and
 annotated source code.
 
 The terminal report without line numbers (default)::
 
     pytest --cov-report term --cov=myproj tests/
 
     -------------------- coverage: platform linux2, python 2.6.4-final-0 ---------------------
@@ -45,27 +45,29 @@
     ----------------------------------------
     TOTAL                  353     20    94%
 
     1 files skipped due to complete coverage.
 
 You can use ``skip-covered`` with ``term-missing`` as well. e.g. ``--cov-report term-missing:skip-covered``
 
-These three report options output to files without showing anything on the terminal::
+These four report options output to files without showing anything on the terminal::
 
     pytest --cov-report html
             --cov-report xml
+            --cov-report lcov
             --cov-report annotate
             --cov=myproj tests/
 
-The output location for each of these reports can be specified. The output location for the XML
+The output location for each of these reports can be specified. The output location for the XML and LCOV
 report is a file. Where as the output location for the HTML and annotated source code reports are
 directories::
 
     pytest --cov-report html:cov_html
             --cov-report xml:cov.xml
+            --cov-report lcov:cov.info
             --cov-report annotate:cov_annotate
             --cov=myproj tests/
 
 The final report option can also suppress printing to the terminal::
 
     pytest --cov-report= --cov=myproj tests/
```

### Comparing `pytest-cov-3.0.0/docs/subprocess-support.rst` & `pytest-cov-4.0.0/docs/subprocess-support.rst`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/docs/tox.rst` & `pytest-cov-4.0.0/docs/tox.rst`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/docs/xdist.rst` & `pytest-cov-4.0.0/docs/xdist.rst`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/examples/README.rst` & `pytest-cov-4.0.0/examples/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/examples/adhoc-layout/tox.ini` & `pytest-cov-4.0.0/examples/adhoc-layout/tox.ini`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/examples/src-layout/tox.ini` & `pytest-cov-4.0.0/examples/src-layout/tox.ini`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/setup.py` & `pytest-cov-4.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 #!/usr/bin/env python
 
 import re
-from distutils.command.build import build
 from glob import glob
 from itertools import chain
 from os.path import basename
 from os.path import dirname
 from os.path import join
 from os.path import splitext
 
 from setuptools import Command
 from setuptools import find_packages
 from setuptools import setup
+
+try:
+    # https://setuptools.pypa.io/en/latest/deprecated/distutils-legacy.html
+    from setuptools.command.build import build
+except ImportError:
+    from distutils.command.build import build
+
 from setuptools.command.develop import develop
 from setuptools.command.easy_install import easy_install
 from setuptools.command.install_lib import install_lib
 
 
 def read(*names, **kwargs):
     with open(
@@ -23,43 +29,43 @@
         encoding=kwargs.get('encoding', 'utf8')
     ) as fh:
         return fh.read()
 
 
 class BuildWithPTH(build):
     def run(self, *args, **kwargs):
-        build.run(self, *args, **kwargs)
+        super().run(*args, **kwargs)
         path = join(dirname(__file__), 'src', 'pytest-cov.pth')
         dest = join(self.build_lib, basename(path))
         self.copy_file(path, dest)
 
 
 class EasyInstallWithPTH(easy_install):
     def run(self, *args, **kwargs):
-        easy_install.run(self, *args, **kwargs)
+        super().run(*args, **kwargs)
         path = join(dirname(__file__), 'src', 'pytest-cov.pth')
         dest = join(self.install_dir, basename(path))
         self.copy_file(path, dest)
 
 
 class InstallLibWithPTH(install_lib):
     def run(self, *args, **kwargs):
-        install_lib.run(self, *args, **kwargs)
+        super().run(*args, **kwargs)
         path = join(dirname(__file__), 'src', 'pytest-cov.pth')
         dest = join(self.install_dir, basename(path))
         self.copy_file(path, dest)
         self.outputs = [dest]
 
     def get_outputs(self):
-        return chain(install_lib.get_outputs(self), self.outputs)
+        return chain(super().get_outputs(), self.outputs)
 
 
 class DevelopWithPTH(develop):
     def run(self, *args, **kwargs):
-        develop.run(self, *args, **kwargs)
+        super().run(*args, **kwargs)
         path = join(dirname(__file__), 'src', 'pytest-cov.pth')
         dest = join(self.install_dir, basename(path))
         self.copy_file(path, dest)
 
 
 class GeneratePTH(Command):
     user_options = []
@@ -77,15 +83,15 @@
                     'import os, sys;'
                     'exec(%r)' % sh.read().replace('    ', ' ')
                 )
 
 
 setup(
     name='pytest-cov',
-    version='3.0.0',
+    version='4.0.0',
     license='MIT',
     description='Pytest plugin for measuring coverage.',
     long_description='{}\n{}'.format(read('README.rst'), re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))),
     author='Marc Schlaich',
     author_email='marc.schlaich@gmail.com',
     url='https://github.com/pytest-dev/pytest-cov',
     packages=find_packages('src'),
@@ -111,14 +117,19 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Software Development :: Testing',
         'Topic :: Utilities',
     ],
+    project_urls={
+        'Documentation': 'https://pytest-cov.readthedocs.io/',
+        'Changelog': 'https://pytest-cov.readthedocs.io/en/latest/changelog.html',
+        'Issue Tracker': 'https://github.com/pytest-dev/pytest-cov/issues',
+    },
     keywords=[
         'cover', 'coverage', 'pytest', 'py.test', 'distributed', 'parallel',
     ],
     install_requires=[
         'pytest>=4.6',
         'coverage[toml]>=5.2.1'
     ],
```

### Comparing `pytest-cov-3.0.0/src/pytest_cov/embed.py` & `pytest-cov-4.0.0/src/pytest_cov/embed.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,30 +16,14 @@
 import atexit
 import os
 import signal
 
 _active_cov = None
 
 
-def multiprocessing_start(_):
-    global _active_cov
-    cov = init()
-    if cov:
-        _active_cov = cov
-        multiprocessing.util.Finalize(None, cleanup, exitpriority=1000)
-
-
-try:
-    import multiprocessing.util
-except ImportError:
-    pass
-else:
-    multiprocessing.util.register_after_fork(multiprocessing_start, multiprocessing_start)
-
-
 def init():
     # Only continue if ancestor process has set everything needed in
     # the env.
     global _active_cov
 
     cov_source = os.environ.get('COV_CORE_SOURCE')
     cov_config = os.environ.get('COV_CORE_CONFIG')
@@ -96,20 +80,18 @@
     global _pending_signal
 
     _cleanup_in_progress = True
     _cleanup(_active_cov)
     _active_cov = None
     _cleanup_in_progress = False
     if _pending_signal:
-        pending_singal = _pending_signal
+        pending_signal = _pending_signal
         _pending_signal = None
-        _signal_cleanup_handler(*pending_singal)
-
+        _signal_cleanup_handler(*pending_signal)
 
-multiprocessing_finish = cleanup  # in case someone dared to use this internal
 
 _previous_handlers = {}
 _pending_signal = None
 _cleanup_in_progress = False
 
 
 def _signal_cleanup_handler(signum, frame):
```

### Comparing `pytest-cov-3.0.0/src/pytest_cov/engine.py` & `pytest-cov-4.0.0/src/pytest_cov/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,26 @@
         # Produce xml report if wanted.
         if 'xml' in self.cov_report:
             output = self.cov_report['xml']
             with _backup(self.cov, "config"):
                 total = self.cov.xml_report(ignore_errors=True, outfile=output)
             stream.write('Coverage XML written to file %s\n' % (self.cov.config.xml_output if output is None else output))
 
+        # Produce lcov report if wanted.
+        if 'lcov' in self.cov_report:
+            output = self.cov_report['lcov']
+            with _backup(self.cov, "config"):
+                self.cov.lcov_report(ignore_errors=True, outfile=output)
+
+                # We need to call Coverage.report here, just to get the total
+                # Coverage.lcov_report doesn't return any total and we need it for --cov-fail-under.
+                total = self.cov.report(ignore_errors=True, file=_NullFile)
+
+            stream.write('Coverage LCOV written to file %s\n' % (self.cov.config.lcov_output if output is None else output))
+
         return total
 
 
 class Central(CovController):
     """Implementation for centralised operation."""
 
     @_ensure_topdir
```

### Comparing `pytest-cov-3.0.0/src/pytest_cov/plugin.py` & `pytest-cov-4.0.0/src/pytest_cov/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,24 +25,27 @@
 
 
 class CovReportWarning(PytestCovWarning):
     """Indicates that we failed to generate a report"""
 
 
 def validate_report(arg):
-    file_choices = ['annotate', 'html', 'xml']
+    file_choices = ['annotate', 'html', 'xml', 'lcov']
     term_choices = ['term', 'term-missing']
     term_modifier_choices = ['skip-covered']
     all_choices = term_choices + file_choices
     values = arg.split(":", 1)
     report_type = values[0]
     if report_type not in all_choices + ['']:
         msg = f'invalid choice: "{arg}" (choose from "{all_choices}")'
         raise argparse.ArgumentTypeError(msg)
 
+    if report_type == 'lcov' and coverage.version_info <= (6, 3):
+        raise argparse.ArgumentTypeError('LCOV output is only supported with coverage.py >= 6.3')
+
     if len(values) == 1:
         return report_type, None
 
     report_modifier = values[1]
     if report_type in term_choices and report_modifier in term_modifier_choices:
         return report_type, report_modifier
 
@@ -92,17 +95,17 @@
                     help='Path or package name to measure during execution (multi-allowed). '
                          'Use --cov= to not do any source filtering and record everything.')
     group.addoption('--cov-reset', action='store_const', const=[], dest='cov_source',
                     help='Reset cov sources accumulated in options so far. ')
     group.addoption('--cov-report', action=StoreReport, default={},
                     metavar='TYPE', type=validate_report,
                     help='Type of report to generate: term, term-missing, '
-                         'annotate, html, xml (multi-allowed). '
+                         'annotate, html, xml, lcov (multi-allowed). '
                          'term, term-missing may be followed by ":skip-covered". '
-                         'annotate, html and xml may be followed by ":DEST" '
+                         'annotate, html, xml and lcov may be followed by ":DEST" '
                          'where DEST specifies the output location. '
                          'Use --cov-report= to not generate any output.')
     group.addoption('--cov-config', action='store', default='.coveragerc',
                     metavar='PATH',
                     help='Config file for coverage. Default: .coveragerc')
     group.addoption('--no-cov-on-fail', action='store_true', default=False,
                     help='Do not report coverage if test run fails. '
@@ -129,15 +132,15 @@
 
      --cov --cov=foobar is equivalent to --cov (cov_source=None)
      --cov=foo --cov=bar is equivalent to cov_source=['foo', 'bar']
     """
     return None if True in cov_source else [path for path in cov_source if path is not True]
 
 
-@pytest.mark.tryfirst
+@pytest.hookimpl(tryfirst=True)
 def pytest_load_initial_conftests(early_config, parser, args):
     options = early_config.known_args_namespace
     no_cov = options.no_cov_should_warn = False
     for arg in args:
         arg = str(arg)
         if arg == '--no-cov':
             no_cov = True
@@ -249,42 +252,42 @@
             self.start(engine.DistWorker, session.config, nodeid)
         elif not self._started:
             self.start(engine.Central)
 
         if self.options.cov_context == 'test':
             session.config.pluginmanager.register(TestContextPlugin(self.cov_controller.cov), '_cov_contexts')
 
+    @pytest.hookimpl(optionalhook=True)
     def pytest_configure_node(self, node):
         """Delegate to our implementation.
 
         Mark this hook as optional in case xdist is not installed.
         """
         if not self._disabled:
             self.cov_controller.configure_node(node)
-    pytest_configure_node.optionalhook = True
 
+    @pytest.hookimpl(optionalhook=True)
     def pytest_testnodedown(self, node, error):
         """Delegate to our implementation.
 
         Mark this hook as optional in case xdist is not installed.
         """
         if not self._disabled:
             self.cov_controller.testnodedown(node, error)
-    pytest_testnodedown.optionalhook = True
 
     def _should_report(self):
         return not (self.failed and self.options.no_cov_on_fail)
 
     def _failed_cov_total(self):
         cov_fail_under = self.options.cov_fail_under
         return cov_fail_under is not None and self.cov_total < cov_fail_under
 
     # we need to wrap pytest_runtestloop. by the time pytest_sessionfinish
     # runs, it's too late to set testsfailed
-    @compat.hookwrapper
+    @pytest.hookimpl(hookwrapper=True)
     def pytest_runtestloop(self, session):
         yield
 
         if self._disabled:
             return
 
         compat_session = compat.SessionWrapper(session)
@@ -304,15 +307,15 @@
             except CoverageException as exc:
                 message = 'Failed to generate report: %s\n' % exc
                 session.config.pluginmanager.getplugin("terminalreporter").write(
                     'WARNING: %s\n' % message, red=True, bold=True)
                 warnings.warn(CovReportWarning(message))
                 self.cov_total = 0
             assert self.cov_total is not None, 'Test coverage should never be `None`'
-            if self._failed_cov_total():
+            if self._failed_cov_total() and not self.options.collectonly:
                 # make sure we get the EXIT_TESTSFAILED exit code
                 compat_session.testsfailed += 1
 
     def pytest_terminal_summary(self, terminalreporter):
         if self._disabled:
             if self.options.no_cov_should_warn:
                 message = 'Coverage disabled via --no-cov switch!'
@@ -322,15 +325,19 @@
         if self.cov_controller is None:
             return
 
         if self.cov_total is None:
             # we shouldn't report, or report generation failed (error raised above)
             return
 
-        terminalreporter.write('\n' + self.cov_report.getvalue() + '\n')
+        report = self.cov_report.getvalue()
+
+        # Avoid undesirable new lines when output is disabled with "--cov-report=".
+        if report:
+            terminalreporter.write('\n' + report + '\n')
 
         if self.options.cov_fail_under is not None and self.options.cov_fail_under > 0:
             failed = self.cov_total < self.options.cov_fail_under
             markup = {'red': True, 'bold': True} if failed else {'green': True}
             message = (
                 '{fail}Required test coverage of {required}% {reached}. '
                 'Total coverage: {actual:.2f}%\n'
@@ -348,15 +355,15 @@
             # test is run in another process than session, run
             # coverage manually
             embed.init()
 
     def pytest_runtest_teardown(self, item):
         embed.cleanup()
 
-    @compat.hookwrapper
+    @pytest.hookimpl(hookwrapper=True)
     def pytest_runtest_call(self, item):
         if (item.get_closest_marker('no_cover')
                 or 'no_cover' in getattr(item, 'fixturenames', ())):
             self.cov_controller.pause()
             yield
             self.cov_controller.resume()
         else:
```

### Comparing `pytest-cov-3.0.0/src/pytest_cov.egg-info/PKG-INFO` & `pytest-cov-4.0.0/src/pytest_cov.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,512 +1,18 @@
 Metadata-Version: 2.1
 Name: pytest-cov
-Version: 3.0.0
+Version: 4.0.0
 Summary: Pytest plugin for measuring coverage.
 Home-page: https://github.com/pytest-dev/pytest-cov
 Author: Marc Schlaich
 Author-email: marc.schlaich@gmail.com
 License: MIT
-Description: ========
-        Overview
-        ========
-        
-        .. start-badges
-        
-        .. list-table::
-            :stub-columns: 1
-        
-            * - docs
-              - |docs|
-            * - tests
-              - | |github-actions| |appveyor| |requires|
-            * - package
-              - | |version| |conda-forge| |wheel| |supported-versions| |supported-implementations|
-                | |commits-since|
-        
-        .. |docs| image:: https://readthedocs.org/projects/pytest-cov/badge/?style=flat
-            :target: https://readthedocs.org/projects/pytest-cov
-            :alt: Documentation Status
-        
-        .. |github-actions| image:: https://github.com/pytest-dev/pytest-cov/actions/workflows/test.yml/badge.svg
-            :alt: GitHub Actions Status
-            :target: https://github.com/pytest-dev/pytest-cov/actions
-        
-        .. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/pytest-dev/pytest-cov?branch=master&svg=true
-            :alt: AppVeyor Build Status
-            :target: https://ci.appveyor.com/project/pytestbot/pytest-cov
-        
-        .. |requires| image:: https://requires.io/github/pytest-dev/pytest-cov/requirements.svg?branch=master
-            :alt: Requirements Status
-            :target: https://requires.io/github/pytest-dev/pytest-cov/requirements/?branch=master
-        
-        .. |version| image:: https://img.shields.io/pypi/v/pytest-cov.svg
-            :alt: PyPI Package latest release
-            :target: https://pypi.org/project/pytest-cov
-        
-        .. |conda-forge| image:: https://img.shields.io/conda/vn/conda-forge/pytest-cov.svg
-            :target: https://anaconda.org/conda-forge/pytest-cov
-        
-        .. |commits-since| image:: https://img.shields.io/github/commits-since/pytest-dev/pytest-cov/v3.0.0.svg
-            :alt: Commits since latest release
-            :target: https://github.com/pytest-dev/pytest-cov/compare/v3.0.0...master
-        
-        .. |wheel| image:: https://img.shields.io/pypi/wheel/pytest-cov.svg
-            :alt: PyPI Wheel
-            :target: https://pypi.org/project/pytest-cov
-        
-        .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pytest-cov.svg
-            :alt: Supported versions
-            :target: https://pypi.org/project/pytest-cov
-        
-        .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pytest-cov.svg
-            :alt: Supported implementations
-            :target: https://pypi.org/project/pytest-cov
-        
-        .. end-badges
-        
-        This plugin produces coverage reports. Compared to just using ``coverage run`` this plugin does some extras:
-        
-        * Subprocess support: you can fork or run stuff in a subprocess and will get covered without any fuss.
-        * Xdist support: you can use all of pytest-xdist's features and still get coverage.
-        * Consistent pytest behavior. If you run ``coverage run -m pytest`` you will have slightly different ``sys.path`` (CWD will be
-          in it, unlike when running ``pytest``).
-        
-        All features offered by the coverage package should work, either through pytest-cov's command line options or
-        through coverage's config file.
-        
-        * Free software: MIT license
-        
-        Installation
-        ============
-        
-        Install with pip::
-        
-            pip install pytest-cov
-        
-        For distributed testing support install pytest-xdist::
-        
-            pip install pytest-xdist
-        
-        Upgrading from ancient pytest-cov
-        ---------------------------------
-        
-        `pytest-cov 2.0` is using a new ``.pth`` file (``pytest-cov.pth``). You may want to manually remove the older
-        ``init_cov_core.pth`` from site-packages as it's not automatically removed.
-        
-        Uninstalling
-        ------------
-        
-        Uninstall with pip::
-        
-            pip uninstall pytest-cov
-        
-        Under certain scenarios a stray ``.pth`` file may be left around in site-packages.
-        
-        * `pytest-cov 2.0` may leave a ``pytest-cov.pth`` if you installed without wheels
-          (``easy_install``, ``setup.py install`` etc).
-        * `pytest-cov 1.8 or older` will leave a ``init_cov_core.pth``.
-        
-        Usage
-        =====
-        
-        ::
-        
-            pytest --cov=myproj tests/
-        
-        Would produce a report like::
-        
-            -------------------- coverage: ... ---------------------
-            Name                 Stmts   Miss  Cover
-            ----------------------------------------
-            myproj/__init__          2      0   100%
-            myproj/myproj          257     13    94%
-            myproj/feature4286      94      7    92%
-            ----------------------------------------
-            TOTAL                  353     20    94%
-        
-        Documentation
-        =============
-        
-            http://pytest-cov.rtfd.org/
-        
-        
-        
-        
-        
-        
-        Coverage Data File
-        ==================
-        
-        The data file is erased at the beginning of testing to ensure clean data for each test run. If you
-        need to combine the coverage of several test runs you can use the ``--cov-append`` option to append
-        this coverage data to coverage data from previous test runs.
-        
-        The data file is left at the end of testing so that it is possible to use normal coverage tools to
-        examine it.
-        
-        Limitations
-        ===========
-        
-        For distributed testing the workers must have the pytest-cov package installed.  This is needed since
-        the plugin must be registered through setuptools for pytest to start the plugin on the
-        worker.
-        
-        For subprocess measurement environment variables must make it from the main process to the
-        subprocess.  The python used by the subprocess must have pytest-cov installed.  The subprocess must
-        do normal site initialisation so that the environment variables can be detected and coverage
-        started.
-        
-        
-        Acknowledgements
-        ================
-        
-        Whilst this plugin has been built fresh from the ground up it has been influenced by the work done
-        on pytest-coverage (Ross Lawley, James Mills, Holger Krekel) and nose-cover (Jason Pellerin) which are
-        other coverage plugins.
-        
-        Ned Batchelder for coverage and its ability to combine the coverage results of parallel runs.
-        
-        Holger Krekel for pytest with its distributed testing support.
-        
-        Jason Pellerin for nose.
-        
-        Michael Foord for unittest2.
-        
-        No doubt others have contributed to these tools as well.
-        
-        Changelog
-        =========
-        
-        
-        3.0.0 (2021-10-04)
-        -------------------
-        
-        **Note that this release drops support for Python 2.7 and Python 3.5.**
-        
-        * Added support for Python 3.10 and updated various test dependencies.
-          Contributed by Hugo van Kemenade in
-          `#500 <https://github.com/pytest-dev/pytest-cov/pull/500>`_.
-        * Switched from Travis CI to GitHub Actions. Contributed by Hugo van Kemenade in
-          `#494 <https://github.com/pytest-dev/pytest-cov/pull/494>`_ and
-          `#495 <https://github.com/pytest-dev/pytest-cov/pull/495>`_.
-        * Add a ``--cov-reset`` CLI option.
-          Contributed by Danilo Šegan in
-          `#459 <https://github.com/pytest-dev/pytest-cov/pull/459>`_.
-        * Improved validation of ``--cov-fail-under`` CLI option.
-          Contributed by ... Ronny Pfannschmidt's desire for skark in
-          `#480 <https://github.com/pytest-dev/pytest-cov/pull/480>`_.
-        * Dropped Python 2.7 support.
-          Contributed by Thomas Grainger in
-          `#488 <https://github.com/pytest-dev/pytest-cov/pull/488>`_.
-        * Updated trove classifiers. Contributed by Michał Bielawski in
-          `#481 <https://github.com/pytest-dev/pytest-cov/pull/481>`_.
-        
-        
-        2.13.0 (2021-06-01)
-        -------------------
-        
-        * Changed the `toml` requirement to be always be directly required (instead of being required through a coverage extra).
-          This fixes issues with pip-compile (`pip-tools#1300 <https://github.com/jazzband/pip-tools/issues/1300>`_).
-          Contributed by Sorin Sbarnea in `#472 <https://github.com/pytest-dev/pytest-cov/pull/472>`_.
-        * Documented ``show_contexts``.
-          Contributed by Brian Rutledge in `#473 <https://github.com/pytest-dev/pytest-cov/pull/473>`_.
-        
-        
-        2.12.1 (2021-06-01)
-        -------------------
-        
-        * Changed the `toml` requirement to be always be directly required (instead of being required through a coverage extra).
-          This fixes issues with pip-compile (`pip-tools#1300 <https://github.com/jazzband/pip-tools/issues/1300>`_).
-          Contributed by Sorin Sbarnea in `#472 <https://github.com/pytest-dev/pytest-cov/pull/472>`_.
-        * Documented ``show_contexts``.
-          Contributed by Brian Rutledge in `#473 <https://github.com/pytest-dev/pytest-cov/pull/473>`_.
-        
-        2.12.0 (2021-05-14)
-        -------------------
-        
-        * Added coverage's `toml` extra to install requirements in setup.py.
-          Contributed by Christian Riedel in `#410 <https://github.com/pytest-dev/pytest-cov/pull/410>`_.
-        * Fixed ``pytest_cov.__version__`` to have the right value (string with version instead of a string
-          including ``__version__ =``).
-        * Fixed license classifier in ``setup.py``.
-          Contributed by Chris Sreesangkom in `#467 <https://github.com/pytest-dev/pytest-cov/pull/467>`_.
-        * Fixed *commits since* badge.
-          Contributed by Terence Honles in `#470 <https://github.com/pytest-dev/pytest-cov/pull/470>`_.
-        
-        2.11.1 (2021-01-20)
-        -------------------
-        
-        * Fixed support for newer setuptools (v42+).
-          Contributed by Michał Górny in `#451 <https://github.com/pytest-dev/pytest-cov/pull/451>`_.
-        
-        2.11.0 (2021-01-18)
-        -------------------
-        
-        * Bumped minimum coverage requirement to 5.2.1. This prevents reporting issues.
-          Contributed by Mateus Berardo de Souza Terra in `#433 <https://github.com/pytest-dev/pytest-cov/pull/433>`_.
-        * Improved sample projects (from the `examples <https://github.com/pytest-dev/pytest-cov/tree/master/examples>`_
-          directory) to support running `tox -e pyXY`. Now the example configures a suffixed coverage data file,
-          and that makes the cleanup environment unnecessary.
-          Contributed by Ganden Schaffner in `#435 <https://github.com/pytest-dev/pytest-cov/pull/435>`_.
-        * Removed the empty `console_scripts` entrypoint that confused some Gentoo build script.
-          I didn't ask why it was so broken cause I didn't want to ruin my day.
-          Contributed by Michał Górny in `#434 <https://github.com/pytest-dev/pytest-cov/pull/434>`_.
-        * Fixed the missing `coverage context <https://coverage.readthedocs.io/en/stable/contexts.html>`_
-          when using subprocesses.
-          Contributed by Bernát Gábor in `#443 <https://github.com/pytest-dev/pytest-cov/pull/443>`_.
-        * Updated the config section in the docs.
-          Contributed by Pamela McA'Nulty in `#429 <https://github.com/pytest-dev/pytest-cov/pull/429>`_.
-        * Migrated CI to travis-ci.com (from .org).
-        
-        2.10.1 (2020-08-14)
-        -------------------
-        
-        * Support for ``pytest-xdist`` 2.0, which breaks compatibility with ``pytest-xdist`` before 1.22.3 (from 2017).
-          Contributed by Zac Hatfield-Dodds in `#412 <https://github.com/pytest-dev/pytest-cov/pull/412>`_.
-        * Fixed the ``LocalPath has no attribute startswith`` failure that occurred when using the ``pytester`` plugin
-          in inline mode.
-        
-        2.10.0 (2020-06-12)
-        -------------------
-        
-        * Improved the ``--no-cov`` warning. Now it's only shown if ``--no-cov`` is present before ``--cov``.
-        * Removed legacy pytest support. Changed ``setup.py`` so that ``pytest>=4.6`` is required.
-        
-        2.9.0 (2020-05-22)
-        ------------------
-        
-        * Fixed ``RemovedInPytest4Warning`` when using Pytest 3.10.
-          Contributed by Michael Manganiello in `#354 <https://github.com/pytest-dev/pytest-cov/pull/354>`_.
-        * Made pytest startup faster when plugin not active by lazy-importing.
-          Contributed by Anders Hovmöller in `#339 <https://github.com/pytest-dev/pytest-cov/pull/339>`_.
-        * Various CI improvements.
-          Contributed by Daniel Hahler in `#363 <https://github.com/pytest-dev/pytest-cov/pull/>`_ and
-          `#364 <https://github.com/pytest-dev/pytest-cov/pull/364>`_.
-        * Various Python support updates (drop EOL 3.4, test against 3.8 final).
-          Contributed by Hugo van Kemenade in
-          `#336 <https://github.com/pytest-dev/pytest-cov/pull/336>`_ and
-          `#367 <https://github.com/pytest-dev/pytest-cov/pull/367>`_.
-        * Changed ``--cov-append`` to always enable ``data_suffix`` (a coverage setting).
-          Contributed by Harm Geerts in
-          `#387 <https://github.com/pytest-dev/pytest-cov/pull/387>`_.
-        * Changed ``--cov-append`` to handle loading previous data better
-          (fixes various path aliasing issues).
-        * Various other testing improvements, github issue templates, example updates.
-        * Fixed internal failures that are caused by tests that change the current working directory by
-          ensuring a consistent working directory when coverage is called.
-          See `#306 <https://github.com/pytest-dev/pytest-cov/issues/306>`_ and
-          `coveragepy#881 <https://github.com/nedbat/coveragepy/issues/881>`_
-        
-        2.8.1 (2019-10-05)
-        ------------------
-        
-        * Fixed `#348 <https://github.com/pytest-dev/pytest-cov/issues/348>`_ -
-          regression when only certain reports (html or xml) are used then ``--cov-fail-under`` always fails.
-        
-        2.8.0 (2019-10-04)
-        ------------------
-        
-        * Fixed ``RecursionError`` that can occur when using
-          `cleanup_on_signal <https://pytest-cov.readthedocs.io/en/latest/subprocess-support.html#if-you-got-custom-signal-handling>`__ or
-          `cleanup_on_sigterm <https://pytest-cov.readthedocs.io/en/latest/subprocess-support.html#if-you-got-custom-signal-handling>`__.
-          See: `#294 <https://github.com/pytest-dev/pytest-cov/issues/294>`_.
-          The 2.7.x releases of pytest-cov should be considered broken regarding aforementioned cleanup API.
-        * Added compatibility with future xdist release that deprecates some internals
-          (match pytest-xdist master/worker terminology).
-          Contributed by Thomas Grainger in `#321 <https://github.com/pytest-dev/pytest-cov/pull/321>`_
-        * Fixed breakage that occurs when multiple reporting options are used.
-          Contributed by Thomas Grainger in `#338 <https://github.com/pytest-dev/pytest-cov/pull/338>`_.
-        * Changed internals to use a stub instead of ``os.devnull``.
-          Contributed by Thomas Grainger in `#332 <https://github.com/pytest-dev/pytest-cov/pull/332>`_.
-        * Added support for Coverage 5.0.
-          Contributed by Ned Batchelder in `#319 <https://github.com/pytest-dev/pytest-cov/pull/319>`_.
-        * Added support for float values in ``--cov-fail-under``.
-          Contributed by Martín Gaitán in `#311 <https://github.com/pytest-dev/pytest-cov/pull/311>`_.
-        * Various documentation fixes. Contributed by
-          Juanjo Bazán,
-          Andrew Murray and
-          Albert Tugushev in
-          `#298 <https://github.com/pytest-dev/pytest-cov/pull/298>`_,
-          `#299 <https://github.com/pytest-dev/pytest-cov/pull/299>`_ and
-          `#307 <https://github.com/pytest-dev/pytest-cov/pull/307>`_.
-        * Various testing improvements. Contributed by
-          Ned Batchelder,
-          Daniel Hahler,
-          Ionel Cristian Mărieș and
-          Hugo van Kemenade in
-          `#313 <https://github.com/pytest-dev/pytest-cov/pull/313>`_,
-          `#314 <https://github.com/pytest-dev/pytest-cov/pull/314>`_,
-          `#315 <https://github.com/pytest-dev/pytest-cov/pull/315>`_,
-          `#316 <https://github.com/pytest-dev/pytest-cov/pull/316>`_,
-          `#325 <https://github.com/pytest-dev/pytest-cov/pull/325>`_,
-          `#326 <https://github.com/pytest-dev/pytest-cov/pull/326>`_,
-          `#334 <https://github.com/pytest-dev/pytest-cov/pull/334>`_ and
-          `#335 <https://github.com/pytest-dev/pytest-cov/pull/335>`_.
-        * Added the ``--cov-context`` CLI options that enables coverage contexts. Only works with coverage 5.0+.
-          Contributed by Ned Batchelder in `#345 <https://github.com/pytest-dev/pytest-cov/pull/345>`_.
-        
-        2.7.1 (2019-05-03)
-        ------------------
-        
-        * Fixed source distribution manifest so that garbage ain't included in the tarball.
-        
-        2.7.0 (2019-05-03)
-        ------------------
-        
-        * Fixed ``AttributeError: 'NoneType' object has no attribute 'configure_node'`` error when ``--no-cov`` is used.
-          Contributed by Alexander Shadchin in `#263 <https://github.com/pytest-dev/pytest-cov/pull/263>`_.
-        * Various testing and CI improvements. Contributed by Daniel Hahler in
-          `#255 <https://github.com/pytest-dev/pytest-cov/pull/255>`_,
-          `#266 <https://github.com/pytest-dev/pytest-cov/pull/266>`_,
-          `#272 <https://github.com/pytest-dev/pytest-cov/pull/272>`_,
-          `#271 <https://github.com/pytest-dev/pytest-cov/pull/271>`_ and
-          `#269 <https://github.com/pytest-dev/pytest-cov/pull/269>`_.
-        * Improved documentation regarding subprocess and multiprocessing.
-          Contributed in `#265 <https://github.com/pytest-dev/pytest-cov/pull/265>`_.
-        * Improved ``pytest_cov.embed.cleanup_on_sigterm`` to be reentrant (signal deliveries while signal handling is
-          running won't break stuff).
-        * Added ``pytest_cov.embed.cleanup_on_signal`` for customized cleanup.
-        * Improved cleanup code and fixed various issues with leftover data files. All contributed in
-          `#265 <https://github.com/pytest-dev/pytest-cov/pull/265>`_ or
-          `#262 <https://github.com/pytest-dev/pytest-cov/pull/262>`_.
-        * Improved examples. Now there are two examples for the common project layouts, complete with working coverage
-          configuration. The examples have CI testing. Contributed in
-          `#267 <https://github.com/pytest-dev/pytest-cov/pull/267>`_.
-        * Improved help text for CLI options.
-        
-        2.6.1 (2019-01-07)
-        ------------------
-        
-        * Added support for Pytest 4.1. Contributed by Daniel Hahler and Семён Марьясин in
-          `#253 <https://github.com/pytest-dev/pytest-cov/pull/253>`_ and
-          `#230 <https://github.com/pytest-dev/pytest-cov/pull/230>`_.
-        * Various test and docs fixes. Contributed by Daniel Hahler in
-          `#224 <https://github.com/pytest-dev/pytest-cov/pull/224>`_ and
-          `#223 <https://github.com/pytest-dev/pytest-cov/pull/223>`_.
-        * Fixed the "Module already imported" issue (`#211 <https://github.com/pytest-dev/pytest-cov/issues/211>`_).
-          Contributed by Daniel Hahler in `#228 <https://github.com/pytest-dev/pytest-cov/pull/228>`_.
-        
-        2.6.0 (2018-09-03)
-        ------------------
-        
-        * Dropped support for Python 3 < 3.4, Pytest < 3.5 and Coverage < 4.4.
-        * Fixed some documentation formatting. Contributed by Jean Jordaan and Julian.
-        * Added an example with ``addopts`` in documentation. Contributed by Samuel Giffard in
-          `#195 <https://github.com/pytest-dev/pytest-cov/pull/195>`_.
-        * Fixed ``TypeError: 'NoneType' object is not iterable`` in certain xdist configurations. Contributed by Jeremy Bowman in
-          `#213 <https://github.com/pytest-dev/pytest-cov/pull/213>`_.
-        * Added a ``no_cover`` marker and fixture. Fixes
-          `#78 <https://github.com/pytest-dev/pytest-cov/issues/78>`_.
-        * Fixed broken ``no_cover`` check when running doctests. Contributed by Terence Honles in
-          `#200 <https://github.com/pytest-dev/pytest-cov/pull/200>`_.
-        * Fixed various issues with path normalization in reports (when combining coverage data from parallel mode). Fixes
-          `#130 <https://github.com/pytest-dev/pytest-cov/issues/161>`_.
-          Contributed by Ryan Hiebert & Ionel Cristian Mărieș in
-          `#178 <https://github.com/pytest-dev/pytest-cov/pull/178>`_.
-        * Report generation failures don't raise exceptions anymore. A warning will be logged instead. Fixes
-          `#161 <https://github.com/pytest-dev/pytest-cov/issues/161>`_.
-        * Fixed multiprocessing issue on Windows (empty env vars are not passed). Fixes
-          `#165 <https://github.com/pytest-dev/pytest-cov/issues/165>`_.
-        
-        2.5.1 (2017-05-11)
-        ------------------
-        
-        * Fixed xdist breakage (regression in ``2.5.0``).
-          Fixes `#157 <https://github.com/pytest-dev/pytest-cov/issues/157>`_.
-        * Allow setting custom ``data_file`` name in ``.coveragerc``.
-          Fixes `#145 <https://github.com/pytest-dev/pytest-cov/issues/145>`_.
-          Contributed by Jannis Leidel & Ionel Cristian Mărieș in
-          `#156 <https://github.com/pytest-dev/pytest-cov/pull/156>`_.
-        
-        2.5.0 (2017-05-09)
-        ------------------
-        
-        * Always show a summary when ``--cov-fail-under`` is used. Contributed by Francis Niu in `PR#141
-          <https://github.com/pytest-dev/pytest-cov/pull/141>`_.
-        * Added ``--cov-branch`` option. Fixes `#85 <https://github.com/pytest-dev/pytest-cov/issues/85>`_.
-        * Improve exception handling in subprocess setup. Fixes `#144 <https://github.com/pytest-dev/pytest-cov/issues/144>`_.
-        * Fixed handling when ``--cov`` is used multiple times. Fixes `#151 <https://github.com/pytest-dev/pytest-cov/issues/151>`_.
-        
-        2.4.0 (2016-10-10)
-        ------------------
-        
-        * Added a "disarm" option: ``--no-cov``. It will disable coverage measurements. Contributed by Zoltan Kozma in
-          `PR#135 <https://github.com/pytest-dev/pytest-cov/pull/135>`_.
-        
-          **WARNING: Do not put this in your configuration files, it's meant to be an one-off for situations where you want to
-          disable coverage from command line.**
-        * Fixed broken exception handling on ``.pth`` file. See `#136 <https://github.com/pytest-dev/pytest-cov/issues/136>`_.
-        
-        2.3.1 (2016-08-07)
-        ------------------
-        
-        * Fixed regression causing spurious errors when xdist was used. See `#124
-          <https://github.com/pytest-dev/pytest-cov/issues/124>`_.
-        * Fixed DeprecationWarning about incorrect `addoption` use. Contributed by Florian Bruhin in `PR#127
-          <https://github.com/pytest-dev/pytest-cov/pull/127>`_.
-        * Fixed deprecated use of funcarg fixture API. Contributed by Daniel Hahler in `PR#125
-          <https://github.com/pytest-dev/pytest-cov/pull/125>`_.
-        
-        2.3.0 (2016-07-05)
-        ------------------
-        
-        * Add support for specifying output location for html, xml, and annotate report.
-          Contributed by Patrick Lannigan in `PR#113 <https://github.com/pytest-dev/pytest-cov/pull/113>`_.
-        * Fix bug hiding test failure when cov-fail-under failed.
-        * For coverage >= 4.0, match the default behaviour of `coverage report` and
-          error if coverage fails to find the source instead of just printing a warning.
-          Contributed by David Szotten in `PR#116 <https://github.com/pytest-dev/pytest-cov/pull/116>`_.
-        * Fixed bug occurred when bare ``--cov`` parameter was used with xdist.
-          Contributed by Michael Elovskikh in `PR#120 <https://github.com/pytest-dev/pytest-cov/pull/120>`_.
-        * Add support for ``skip_covered`` and added ``--cov-report=term-skip-covered`` command
-          line options. Contributed by Saurabh Kumar in `PR#115 <https://github.com/pytest-dev/pytest-cov/pull/115>`_.
-        
-        2.2.1 (2016-01-30)
-        ------------------
-        
-        * Fixed incorrect merging of coverage data when xdist was used and coverage was ``>= 4.0``.
-        
-        2.2.0 (2015-10-04)
-        ------------------
-        
-        * Added support for changing working directory in tests. Previously changing working
-          directory would disable coverage measurements in suprocesses.
-        * Fixed broken handling for ``--cov-report=annotate``.
-        
-        2.1.0 (2015-08-23)
-        ------------------
-        
-        * Added support for `coverage 4.0b2`.
-        * Added the ``--cov-append`` command line options. Contributed by Christian Ledermann
-          in `PR#80 <https://github.com/pytest-dev/pytest-cov/pull/80>`_.
-        
-        2.0.0 (2015-07-28)
-        ------------------
-        
-        * Added ``--cov-fail-under``, akin to the new ``fail_under`` option in `coverage-4.0`
-          (automatically activated if there's a ``[report] fail_under = ...`` in ``.coveragerc``).
-        * Changed ``--cov-report=term`` to automatically upgrade to ``--cov-report=term-missing``
-          if there's ``[run] show_missing = True`` in ``.coveragerc``.
-        * Changed ``--cov`` so it can be used with no path argument (in which case the source
-          settings from ``.coveragerc`` will be used instead).
-        * Fixed `.pth` installation to work in all cases (install, easy_install, wheels, develop etc).
-        * Fixed `.pth` uninstallation to work for wheel installs.
-        * Support for coverage 4.0.
-        * Data file suffixing changed to use coverage's ``data_suffix=True`` option (instead of the
-          custom suffixing).
-        * Avoid warning about missing coverage data (just like ``coverage.control.process_startup``).
-        * Fixed a race condition when running with xdist (all the workers tried to combine the files).
-          It's possible that this issue is not present in `pytest-cov 1.8.X`.
-        
-        1.8.2 (2014-11-06)
-        ------------------
-        
-        * N/A
-        
+Project-URL: Documentation, https://pytest-cov.readthedocs.io/
+Project-URL: Changelog, https://pytest-cov.readthedocs.io/en/latest/changelog.html
+Project-URL: Issue Tracker, https://github.com/pytest-dev/pytest-cov/issues
 Keywords: cover,coverage,pytest,py.test,distributed,parallel
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -522,7 +28,531 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Provides-Extra: testing
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+========
+Overview
+========
+
+.. start-badges
+
+.. list-table::
+    :stub-columns: 1
+
+    * - docs
+      - |docs|
+    * - tests
+      - | |github-actions| |requires|
+        |
+    * - package
+      - | |version| |conda-forge| |wheel| |supported-versions| |supported-implementations|
+        | |commits-since|
+
+.. |docs| image:: https://readthedocs.org/projects/pytest-cov/badge/?style=flat
+    :target: https://readthedocs.org/projects/pytest-cov
+    :alt: Documentation Status
+
+.. |github-actions| image:: https://github.com/pytest-dev/pytest-cov/actions/workflows/test.yml/badge.svg
+    :alt: GitHub Actions Status
+    :target: https://github.com/pytest-dev/pytest-cov/actions
+
+.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/pytest-dev/pytest-cov?branch=master&svg=true
+    :alt: AppVeyor Build Status
+    :target: https://ci.appveyor.com/project/pytestbot/pytest-cov
+
+.. |requires| image:: https://requires.io/github/pytest-dev/pytest-cov/requirements.svg?branch=master
+    :alt: Requirements Status
+    :target: https://requires.io/github/pytest-dev/pytest-cov/requirements/?branch=master
+
+.. |version| image:: https://img.shields.io/pypi/v/pytest-cov.svg
+    :alt: PyPI Package latest release
+    :target: https://pypi.org/project/pytest-cov
+
+.. |conda-forge| image:: https://img.shields.io/conda/vn/conda-forge/pytest-cov.svg
+    :target: https://anaconda.org/conda-forge/pytest-cov
+
+.. |commits-since| image:: https://img.shields.io/github/commits-since/pytest-dev/pytest-cov/v4.0.0.svg
+    :alt: Commits since latest release
+    :target: https://github.com/pytest-dev/pytest-cov/compare/v4.0.0...master
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/pytest-cov.svg
+    :alt: PyPI Wheel
+    :target: https://pypi.org/project/pytest-cov
+
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pytest-cov.svg
+    :alt: Supported versions
+    :target: https://pypi.org/project/pytest-cov
+
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pytest-cov.svg
+    :alt: Supported implementations
+    :target: https://pypi.org/project/pytest-cov
+
+.. end-badges
+
+This plugin produces coverage reports. Compared to just using ``coverage run`` this plugin does some extras:
+
+* Subprocess support: you can fork or run stuff in a subprocess and will get covered without any fuss.
+* Xdist support: you can use all of pytest-xdist's features and still get coverage.
+* Consistent pytest behavior. If you run ``coverage run -m pytest`` you will have slightly different ``sys.path`` (CWD will be
+  in it, unlike when running ``pytest``).
+
+All features offered by the coverage package should work, either through pytest-cov's command line options or
+through coverage's config file.
+
+* Free software: MIT license
+
+Installation
+============
+
+Install with pip::
+
+    pip install pytest-cov
+
+For distributed testing support install pytest-xdist::
+
+    pip install pytest-xdist
+
+Upgrading from ancient pytest-cov
+---------------------------------
+
+`pytest-cov 2.0` is using a new ``.pth`` file (``pytest-cov.pth``). You may want to manually remove the older
+``init_cov_core.pth`` from site-packages as it's not automatically removed.
+
+Uninstalling
+------------
+
+Uninstall with pip::
+
+    pip uninstall pytest-cov
+
+Under certain scenarios a stray ``.pth`` file may be left around in site-packages.
+
+* `pytest-cov 2.0` may leave a ``pytest-cov.pth`` if you installed without wheels
+  (``easy_install``, ``setup.py install`` etc).
+* `pytest-cov 1.8 or older` will leave a ``init_cov_core.pth``.
+
+Usage
+=====
+
+::
+
+    pytest --cov=myproj tests/
+
+Would produce a report like::
+
+    -------------------- coverage: ... ---------------------
+    Name                 Stmts   Miss  Cover
+    ----------------------------------------
+    myproj/__init__          2      0   100%
+    myproj/myproj          257     13    94%
+    myproj/feature4286      94      7    92%
+    ----------------------------------------
+    TOTAL                  353     20    94%
+
+Documentation
+=============
+
+    http://pytest-cov.rtfd.org/
+
+
+
+
+
+
+Coverage Data File
+==================
+
+The data file is erased at the beginning of testing to ensure clean data for each test run. If you
+need to combine the coverage of several test runs you can use the ``--cov-append`` option to append
+this coverage data to coverage data from previous test runs.
+
+The data file is left at the end of testing so that it is possible to use normal coverage tools to
+examine it.
+
+Limitations
+===========
+
+For distributed testing the workers must have the pytest-cov package installed.  This is needed since
+the plugin must be registered through setuptools for pytest to start the plugin on the
+worker.
+
+For subprocess measurement environment variables must make it from the main process to the
+subprocess.  The python used by the subprocess must have pytest-cov installed.  The subprocess must
+do normal site initialisation so that the environment variables can be detected and coverage
+started.
+
+
+Acknowledgements
+================
+
+Whilst this plugin has been built fresh from the ground up it has been influenced by the work done
+on pytest-coverage (Ross Lawley, James Mills, Holger Krekel) and nose-cover (Jason Pellerin) which are
+other coverage plugins.
+
+Ned Batchelder for coverage and its ability to combine the coverage results of parallel runs.
+
+Holger Krekel for pytest with its distributed testing support.
+
+Jason Pellerin for nose.
+
+Michael Foord for unittest2.
+
+No doubt others have contributed to these tools as well.
+
+Changelog
+=========
+
+
+4.0.0 (2022-09-28)
+------------------
+
+**Note that this release drops support for multiprocessing.**
+
+
+* `--cov-fail-under` no longer causes `pytest --collect-only` to fail
+  Contributed by Zac Hatfield-Dodds in `#511 <https://github.com/pytest-dev/pytest-cov/pull/511>`_.
+* Dropped support for multiprocessing (mostly because `issue 82408 <https://github.com/python/cpython/issues/82408>`_). This feature was
+  mostly working but very broken in certain scenarios and made the test suite very flaky and slow.
+
+  There is builtin multiprocessing support in coverage and you can migrate to that. All you need is this in your
+  ``.coveragerc``::
+
+    [run]
+    concurrency = multiprocessing
+    parallel = true
+    sigterm = true
+* Fixed deprecation in ``setup.py`` by trying to import setuptools before distutils.
+  Contributed by Ben Greiner in `#545 <https://github.com/pytest-dev/pytest-cov/pull/545>`_.
+* Removed undesirable new lines that were displayed while reporting was disabled.
+  Contributed by Delgan in `#540 <https://github.com/pytest-dev/pytest-cov/pull/540>`_.
+* Documentation fixes.
+  Contributed by Andre Brisco in `#543 <https://github.com/pytest-dev/pytest-cov/pull/543>`_
+  and Colin O'Dell in `#525 <https://github.com/pytest-dev/pytest-cov/pull/525>`_.
+* Added support for LCOV output format via `--cov-report=lcov`. Only works with coverage 6.3+.
+  Contributed by Christian Fetzer in `#536 <https://github.com/pytest-dev/pytest-cov/issues/536>`_.
+* Modernized pytest hook implementation.
+  Contributed by Bruno Oliveira in `#549 <https://github.com/pytest-dev/pytest-cov/pull/549>`_
+  and Ronny Pfannschmidt in `#550 <https://github.com/pytest-dev/pytest-cov/pull/550>`_.
+
+
+3.0.0 (2021-10-04)
+-------------------
+
+**Note that this release drops support for Python 2.7 and Python 3.5.**
+
+* Added support for Python 3.10 and updated various test dependencies.
+  Contributed by Hugo van Kemenade in
+  `#500 <https://github.com/pytest-dev/pytest-cov/pull/500>`_.
+* Switched from Travis CI to GitHub Actions. Contributed by Hugo van Kemenade in
+  `#494 <https://github.com/pytest-dev/pytest-cov/pull/494>`_ and
+  `#495 <https://github.com/pytest-dev/pytest-cov/pull/495>`_.
+* Add a ``--cov-reset`` CLI option.
+  Contributed by Danilo Šegan in
+  `#459 <https://github.com/pytest-dev/pytest-cov/pull/459>`_.
+* Improved validation of ``--cov-fail-under`` CLI option.
+  Contributed by ... Ronny Pfannschmidt's desire for skark in
+  `#480 <https://github.com/pytest-dev/pytest-cov/pull/480>`_.
+* Dropped Python 2.7 support.
+  Contributed by Thomas Grainger in
+  `#488 <https://github.com/pytest-dev/pytest-cov/pull/488>`_.
+* Updated trove classifiers. Contributed by Michał Bielawski in
+  `#481 <https://github.com/pytest-dev/pytest-cov/pull/481>`_.
+* Reverted change for `toml` requirement.
+  Contributed by Thomas Grainger in
+  `#477 <https://github.com/pytest-dev/pytest-cov/pull/477>`_.
+
+2.12.1 (2021-06-01)
+-------------------
+
+* Changed the `toml` requirement to be always be directly required (instead of being required through a coverage extra).
+  This fixes issues with pip-compile (`pip-tools#1300 <https://github.com/jazzband/pip-tools/issues/1300>`_).
+  Contributed by Sorin Sbarnea in `#472 <https://github.com/pytest-dev/pytest-cov/pull/472>`_.
+* Documented ``show_contexts``.
+  Contributed by Brian Rutledge in `#473 <https://github.com/pytest-dev/pytest-cov/pull/473>`_.
+
+2.12.0 (2021-05-14)
+-------------------
+
+* Added coverage's `toml` extra to install requirements in setup.py.
+  Contributed by Christian Riedel in `#410 <https://github.com/pytest-dev/pytest-cov/pull/410>`_.
+* Fixed ``pytest_cov.__version__`` to have the right value (string with version instead of a string
+  including ``__version__ =``).
+* Fixed license classifier in ``setup.py``.
+  Contributed by Chris Sreesangkom in `#467 <https://github.com/pytest-dev/pytest-cov/pull/467>`_.
+* Fixed *commits since* badge.
+  Contributed by Terence Honles in `#470 <https://github.com/pytest-dev/pytest-cov/pull/470>`_.
+
+2.11.1 (2021-01-20)
+-------------------
+
+* Fixed support for newer setuptools (v42+).
+  Contributed by Michał Górny in `#451 <https://github.com/pytest-dev/pytest-cov/pull/451>`_.
+
+2.11.0 (2021-01-18)
+-------------------
+
+* Bumped minimum coverage requirement to 5.2.1. This prevents reporting issues.
+  Contributed by Mateus Berardo de Souza Terra in `#433 <https://github.com/pytest-dev/pytest-cov/pull/433>`_.
+* Improved sample projects (from the `examples <https://github.com/pytest-dev/pytest-cov/tree/master/examples>`_
+  directory) to support running `tox -e pyXY`. Now the example configures a suffixed coverage data file,
+  and that makes the cleanup environment unnecessary.
+  Contributed by Ganden Schaffner in `#435 <https://github.com/pytest-dev/pytest-cov/pull/435>`_.
+* Removed the empty `console_scripts` entrypoint that confused some Gentoo build script.
+  I didn't ask why it was so broken cause I didn't want to ruin my day.
+  Contributed by Michał Górny in `#434 <https://github.com/pytest-dev/pytest-cov/pull/434>`_.
+* Fixed the missing `coverage context <https://coverage.readthedocs.io/en/stable/contexts.html>`_
+  when using subprocesses.
+  Contributed by Bernát Gábor in `#443 <https://github.com/pytest-dev/pytest-cov/pull/443>`_.
+* Updated the config section in the docs.
+  Contributed by Pamela McA'Nulty in `#429 <https://github.com/pytest-dev/pytest-cov/pull/429>`_.
+* Migrated CI to travis-ci.com (from .org).
+
+2.10.1 (2020-08-14)
+-------------------
+
+* Support for ``pytest-xdist`` 2.0, which breaks compatibility with ``pytest-xdist`` before 1.22.3 (from 2017).
+  Contributed by Zac Hatfield-Dodds in `#412 <https://github.com/pytest-dev/pytest-cov/pull/412>`_.
+* Fixed the ``LocalPath has no attribute startswith`` failure that occurred when using the ``pytester`` plugin
+  in inline mode.
+
+2.10.0 (2020-06-12)
+-------------------
+
+* Improved the ``--no-cov`` warning. Now it's only shown if ``--no-cov`` is present before ``--cov``.
+* Removed legacy pytest support. Changed ``setup.py`` so that ``pytest>=4.6`` is required.
+
+2.9.0 (2020-05-22)
+------------------
+
+* Fixed ``RemovedInPytest4Warning`` when using Pytest 3.10.
+  Contributed by Michael Manganiello in `#354 <https://github.com/pytest-dev/pytest-cov/pull/354>`_.
+* Made pytest startup faster when plugin not active by lazy-importing.
+  Contributed by Anders Hovmöller in `#339 <https://github.com/pytest-dev/pytest-cov/pull/339>`_.
+* Various CI improvements.
+  Contributed by Daniel Hahler in `#363 <https://github.com/pytest-dev/pytest-cov/pull/>`_ and
+  `#364 <https://github.com/pytest-dev/pytest-cov/pull/364>`_.
+* Various Python support updates (drop EOL 3.4, test against 3.8 final).
+  Contributed by Hugo van Kemenade in
+  `#336 <https://github.com/pytest-dev/pytest-cov/pull/336>`_ and
+  `#367 <https://github.com/pytest-dev/pytest-cov/pull/367>`_.
+* Changed ``--cov-append`` to always enable ``data_suffix`` (a coverage setting).
+  Contributed by Harm Geerts in
+  `#387 <https://github.com/pytest-dev/pytest-cov/pull/387>`_.
+* Changed ``--cov-append`` to handle loading previous data better
+  (fixes various path aliasing issues).
+* Various other testing improvements, github issue templates, example updates.
+* Fixed internal failures that are caused by tests that change the current working directory by
+  ensuring a consistent working directory when coverage is called.
+  See `#306 <https://github.com/pytest-dev/pytest-cov/issues/306>`_ and
+  `coveragepy#881 <https://github.com/nedbat/coveragepy/issues/881>`_
+
+2.8.1 (2019-10-05)
+------------------
+
+* Fixed `#348 <https://github.com/pytest-dev/pytest-cov/issues/348>`_ -
+  regression when only certain reports (html or xml) are used then ``--cov-fail-under`` always fails.
+
+2.8.0 (2019-10-04)
+------------------
+
+* Fixed ``RecursionError`` that can occur when using
+  `cleanup_on_signal <https://pytest-cov.readthedocs.io/en/latest/subprocess-support.html#if-you-got-custom-signal-handling>`__ or
+  `cleanup_on_sigterm <https://pytest-cov.readthedocs.io/en/latest/subprocess-support.html#if-you-got-custom-signal-handling>`__.
+  See: `#294 <https://github.com/pytest-dev/pytest-cov/issues/294>`_.
+  The 2.7.x releases of pytest-cov should be considered broken regarding aforementioned cleanup API.
+* Added compatibility with future xdist release that deprecates some internals
+  (match pytest-xdist master/worker terminology).
+  Contributed by Thomas Grainger in `#321 <https://github.com/pytest-dev/pytest-cov/pull/321>`_
+* Fixed breakage that occurs when multiple reporting options are used.
+  Contributed by Thomas Grainger in `#338 <https://github.com/pytest-dev/pytest-cov/pull/338>`_.
+* Changed internals to use a stub instead of ``os.devnull``.
+  Contributed by Thomas Grainger in `#332 <https://github.com/pytest-dev/pytest-cov/pull/332>`_.
+* Added support for Coverage 5.0.
+  Contributed by Ned Batchelder in `#319 <https://github.com/pytest-dev/pytest-cov/pull/319>`_.
+* Added support for float values in ``--cov-fail-under``.
+  Contributed by Martín Gaitán in `#311 <https://github.com/pytest-dev/pytest-cov/pull/311>`_.
+* Various documentation fixes. Contributed by
+  Juanjo Bazán,
+  Andrew Murray and
+  Albert Tugushev in
+  `#298 <https://github.com/pytest-dev/pytest-cov/pull/298>`_,
+  `#299 <https://github.com/pytest-dev/pytest-cov/pull/299>`_ and
+  `#307 <https://github.com/pytest-dev/pytest-cov/pull/307>`_.
+* Various testing improvements. Contributed by
+  Ned Batchelder,
+  Daniel Hahler,
+  Ionel Cristian Mărieș and
+  Hugo van Kemenade in
+  `#313 <https://github.com/pytest-dev/pytest-cov/pull/313>`_,
+  `#314 <https://github.com/pytest-dev/pytest-cov/pull/314>`_,
+  `#315 <https://github.com/pytest-dev/pytest-cov/pull/315>`_,
+  `#316 <https://github.com/pytest-dev/pytest-cov/pull/316>`_,
+  `#325 <https://github.com/pytest-dev/pytest-cov/pull/325>`_,
+  `#326 <https://github.com/pytest-dev/pytest-cov/pull/326>`_,
+  `#334 <https://github.com/pytest-dev/pytest-cov/pull/334>`_ and
+  `#335 <https://github.com/pytest-dev/pytest-cov/pull/335>`_.
+* Added the ``--cov-context`` CLI options that enables coverage contexts. Only works with coverage 5.0+.
+  Contributed by Ned Batchelder in `#345 <https://github.com/pytest-dev/pytest-cov/pull/345>`_.
+
+2.7.1 (2019-05-03)
+------------------
+
+* Fixed source distribution manifest so that garbage ain't included in the tarball.
+
+2.7.0 (2019-05-03)
+------------------
+
+* Fixed ``AttributeError: 'NoneType' object has no attribute 'configure_node'`` error when ``--no-cov`` is used.
+  Contributed by Alexander Shadchin in `#263 <https://github.com/pytest-dev/pytest-cov/pull/263>`_.
+* Various testing and CI improvements. Contributed by Daniel Hahler in
+  `#255 <https://github.com/pytest-dev/pytest-cov/pull/255>`_,
+  `#266 <https://github.com/pytest-dev/pytest-cov/pull/266>`_,
+  `#272 <https://github.com/pytest-dev/pytest-cov/pull/272>`_,
+  `#271 <https://github.com/pytest-dev/pytest-cov/pull/271>`_ and
+  `#269 <https://github.com/pytest-dev/pytest-cov/pull/269>`_.
+* Improved ``pytest_cov.embed.cleanup_on_sigterm`` to be reentrant (signal deliveries while signal handling is
+  running won't break stuff).
+* Added ``pytest_cov.embed.cleanup_on_signal`` for customized cleanup.
+* Improved cleanup code and fixed various issues with leftover data files. All contributed in
+  `#265 <https://github.com/pytest-dev/pytest-cov/pull/265>`_ or
+  `#262 <https://github.com/pytest-dev/pytest-cov/pull/262>`_.
+* Improved examples. Now there are two examples for the common project layouts, complete with working coverage
+  configuration. The examples have CI testing. Contributed in
+  `#267 <https://github.com/pytest-dev/pytest-cov/pull/267>`_.
+* Improved help text for CLI options.
+
+2.6.1 (2019-01-07)
+------------------
+
+* Added support for Pytest 4.1. Contributed by Daniel Hahler and Семён Марьясин in
+  `#253 <https://github.com/pytest-dev/pytest-cov/pull/253>`_ and
+  `#230 <https://github.com/pytest-dev/pytest-cov/pull/230>`_.
+* Various test and docs fixes. Contributed by Daniel Hahler in
+  `#224 <https://github.com/pytest-dev/pytest-cov/pull/224>`_ and
+  `#223 <https://github.com/pytest-dev/pytest-cov/pull/223>`_.
+* Fixed the "Module already imported" issue (`#211 <https://github.com/pytest-dev/pytest-cov/issues/211>`_).
+  Contributed by Daniel Hahler in `#228 <https://github.com/pytest-dev/pytest-cov/pull/228>`_.
+
+2.6.0 (2018-09-03)
+------------------
+
+* Dropped support for Python 3 < 3.4, Pytest < 3.5 and Coverage < 4.4.
+* Fixed some documentation formatting. Contributed by Jean Jordaan and Julian.
+* Added an example with ``addopts`` in documentation. Contributed by Samuel Giffard in
+  `#195 <https://github.com/pytest-dev/pytest-cov/pull/195>`_.
+* Fixed ``TypeError: 'NoneType' object is not iterable`` in certain xdist configurations. Contributed by Jeremy Bowman in
+  `#213 <https://github.com/pytest-dev/pytest-cov/pull/213>`_.
+* Added a ``no_cover`` marker and fixture. Fixes
+  `#78 <https://github.com/pytest-dev/pytest-cov/issues/78>`_.
+* Fixed broken ``no_cover`` check when running doctests. Contributed by Terence Honles in
+  `#200 <https://github.com/pytest-dev/pytest-cov/pull/200>`_.
+* Fixed various issues with path normalization in reports (when combining coverage data from parallel mode). Fixes
+  `#130 <https://github.com/pytest-dev/pytest-cov/issues/161>`_.
+  Contributed by Ryan Hiebert & Ionel Cristian Mărieș in
+  `#178 <https://github.com/pytest-dev/pytest-cov/pull/178>`_.
+* Report generation failures don't raise exceptions anymore. A warning will be logged instead. Fixes
+  `#161 <https://github.com/pytest-dev/pytest-cov/issues/161>`_.
+* Fixed multiprocessing issue on Windows (empty env vars are not passed). Fixes
+  `#165 <https://github.com/pytest-dev/pytest-cov/issues/165>`_.
+
+2.5.1 (2017-05-11)
+------------------
+
+* Fixed xdist breakage (regression in ``2.5.0``).
+  Fixes `#157 <https://github.com/pytest-dev/pytest-cov/issues/157>`_.
+* Allow setting custom ``data_file`` name in ``.coveragerc``.
+  Fixes `#145 <https://github.com/pytest-dev/pytest-cov/issues/145>`_.
+  Contributed by Jannis Leidel & Ionel Cristian Mărieș in
+  `#156 <https://github.com/pytest-dev/pytest-cov/pull/156>`_.
+
+2.5.0 (2017-05-09)
+------------------
+
+* Always show a summary when ``--cov-fail-under`` is used. Contributed by Francis Niu in `PR#141
+  <https://github.com/pytest-dev/pytest-cov/pull/141>`_.
+* Added ``--cov-branch`` option. Fixes `#85 <https://github.com/pytest-dev/pytest-cov/issues/85>`_.
+* Improve exception handling in subprocess setup. Fixes `#144 <https://github.com/pytest-dev/pytest-cov/issues/144>`_.
+* Fixed handling when ``--cov`` is used multiple times. Fixes `#151 <https://github.com/pytest-dev/pytest-cov/issues/151>`_.
+
+2.4.0 (2016-10-10)
+------------------
+
+* Added a "disarm" option: ``--no-cov``. It will disable coverage measurements. Contributed by Zoltan Kozma in
+  `PR#135 <https://github.com/pytest-dev/pytest-cov/pull/135>`_.
+
+  **WARNING: Do not put this in your configuration files, it's meant to be an one-off for situations where you want to
+  disable coverage from command line.**
+* Fixed broken exception handling on ``.pth`` file. See `#136 <https://github.com/pytest-dev/pytest-cov/issues/136>`_.
+
+2.3.1 (2016-08-07)
+------------------
+
+* Fixed regression causing spurious errors when xdist was used. See `#124
+  <https://github.com/pytest-dev/pytest-cov/issues/124>`_.
+* Fixed DeprecationWarning about incorrect `addoption` use. Contributed by Florian Bruhin in `PR#127
+  <https://github.com/pytest-dev/pytest-cov/pull/127>`_.
+* Fixed deprecated use of funcarg fixture API. Contributed by Daniel Hahler in `PR#125
+  <https://github.com/pytest-dev/pytest-cov/pull/125>`_.
+
+2.3.0 (2016-07-05)
+------------------
+
+* Add support for specifying output location for html, xml, and annotate report.
+  Contributed by Patrick Lannigan in `PR#113 <https://github.com/pytest-dev/pytest-cov/pull/113>`_.
+* Fix bug hiding test failure when cov-fail-under failed.
+* For coverage >= 4.0, match the default behaviour of `coverage report` and
+  error if coverage fails to find the source instead of just printing a warning.
+  Contributed by David Szotten in `PR#116 <https://github.com/pytest-dev/pytest-cov/pull/116>`_.
+* Fixed bug occurred when bare ``--cov`` parameter was used with xdist.
+  Contributed by Michael Elovskikh in `PR#120 <https://github.com/pytest-dev/pytest-cov/pull/120>`_.
+* Add support for ``skip_covered`` and added ``--cov-report=term-skip-covered`` command
+  line options. Contributed by Saurabh Kumar in `PR#115 <https://github.com/pytest-dev/pytest-cov/pull/115>`_.
+
+2.2.1 (2016-01-30)
+------------------
+
+* Fixed incorrect merging of coverage data when xdist was used and coverage was ``>= 4.0``.
+
+2.2.0 (2015-10-04)
+------------------
+
+* Added support for changing working directory in tests. Previously changing working
+  directory would disable coverage measurements in suprocesses.
+* Fixed broken handling for ``--cov-report=annotate``.
+
+2.1.0 (2015-08-23)
+------------------
+
+* Added support for `coverage 4.0b2`.
+* Added the ``--cov-append`` command line options. Contributed by Christian Ledermann
+  in `PR#80 <https://github.com/pytest-dev/pytest-cov/pull/80>`_.
+
+2.0.0 (2015-07-28)
+------------------
+
+* Added ``--cov-fail-under``, akin to the new ``fail_under`` option in `coverage-4.0`
+  (automatically activated if there's a ``[report] fail_under = ...`` in ``.coveragerc``).
+* Changed ``--cov-report=term`` to automatically upgrade to ``--cov-report=term-missing``
+  if there's ``[run] show_missing = True`` in ``.coveragerc``.
+* Changed ``--cov`` so it can be used with no path argument (in which case the source
+  settings from ``.coveragerc`` will be used instead).
+* Fixed `.pth` installation to work in all cases (install, easy_install, wheels, develop etc).
+* Fixed `.pth` uninstallation to work for wheel installs.
+* Support for coverage 4.0.
+* Data file suffixing changed to use coverage's ``data_suffix=True`` option (instead of the
+  custom suffixing).
+* Avoid warning about missing coverage data (just like ``coverage.control.process_startup``).
+* Fixed a race condition when running with xdist (all the workers tried to combine the files).
+  It's possible that this issue is not present in `pytest-cov 1.8.X`.
+
+1.8.2 (2014-11-06)
+------------------
+
+* N/A
+
+
```

### Comparing `pytest-cov-3.0.0/src/pytest_cov.egg-info/SOURCES.txt` & `pytest-cov-4.0.0/src/pytest_cov.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.appveyor.yml
 .bumpversion.cfg
 .cookiecutterrc
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.rst
@@ -13,21 +12,18 @@
 README.rst
 setup.cfg
 setup.py
 tox.ini
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/support_request.md
-.github/workflows/examples.yml
-.github/workflows/lint.yml
 .github/workflows/test.yml
-ci/appveyor-with-compiler.cmd
 ci/bootstrap.py
 ci/requirements.txt
-ci/templates/.appveyor.yml
+ci/templates/.github/workflows/test.yml
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/config.rst
 docs/contexts.rst
 docs/contributing.rst
 docs/debuggers.rst
```

### Comparing `pytest-cov-3.0.0/tests/contextful.py` & `pytest-cov-4.0.0/tests/contextful.py`

 * *Files identical despite different names*

### Comparing `pytest-cov-3.0.0/tests/test_pytest_cov.py` & `pytest-cov-4.0.0/tests/test_pytest_cov.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,15 +146,16 @@
 def test_foo(cov):
     assert cov is None
 '''
 
 CHILD_SCRIPT_RESULT = '[56] * 100%'
 PARENT_SCRIPT_RESULT = '9 * 100%'
 DEST_DIR = 'cov_dest'
-REPORT_NAME = 'cov.xml'
+XML_REPORT_NAME = 'cov.xml'
+LCOV_REPORT_NAME = 'cov.info'
 
 xdist_params = pytest.mark.parametrize('opts', [
     '',
     pytest.param('-n 1', marks=pytest.mark.skipif('sys.platform == "win32" and platform.python_implementation() == "PyPy"'))
 ], ids=['nodist', 'xdist'])
 
 
@@ -190,15 +191,15 @@
         prefixedfullconf='[coverage:run]\n%s\n' % request.param[0],
         args=request.param[1].split(),
         result=request.param[2],
         result2=request.param[3],
     )
 
 
-def test_central(testdir, prop):
+def test_central(pytester, testdir, prop):
     script = testdir.makepyfile(prop.code)
     testdir.tmpdir.join('.coveragerc').write(prop.fullconf)
 
     result = testdir.runpytest('-v',
                                '--cov=%s' % script.dirpath(),
                                '--cov-report=term-missing',
                                script,
@@ -329,26 +330,58 @@
 
 
 def test_xml_output_dir(testdir):
     script = testdir.makepyfile(SCRIPT)
 
     result = testdir.runpytest('-v',
                                '--cov=%s' % script.dirpath(),
-                               '--cov-report=xml:' + REPORT_NAME,
+                               '--cov-report=xml:' + XML_REPORT_NAME,
                                script)
 
     result.stdout.fnmatch_lines([
         '*- coverage: platform *, python * -*',
-        'Coverage XML written to file ' + REPORT_NAME,
+        'Coverage XML written to file ' + XML_REPORT_NAME,
         '*10 passed*',
     ])
-    assert testdir.tmpdir.join(REPORT_NAME).check()
+    assert testdir.tmpdir.join(XML_REPORT_NAME).check()
     assert result.ret == 0
 
 
+@pytest.mark.skipif("coverage.version_info < (6, 3)")
+def test_lcov_output_dir(testdir):
+    script = testdir.makepyfile(SCRIPT)
+
+    result = testdir.runpytest('-v',
+                               '--cov=%s' % script.dirpath(),
+                               '--cov-report=lcov:' + LCOV_REPORT_NAME,
+                               script)
+
+    result.stdout.fnmatch_lines([
+        '*- coverage: platform *, python * -*',
+        'Coverage LCOV written to file ' + LCOV_REPORT_NAME,
+        '*10 passed*',
+    ])
+    assert testdir.tmpdir.join(LCOV_REPORT_NAME).check()
+    assert result.ret == 0
+
+
+@pytest.mark.skipif("coverage.version_info >= (6, 3)")
+def test_lcov_not_supported(testdir):
+    script = testdir.makepyfile("a = 1")
+    result = testdir.runpytest('-v',
+                               '--cov=%s' % script.dirpath(),
+                               '--cov-report=lcov',
+                               script,
+                               )
+    result.stderr.fnmatch_lines([
+        '*argument --cov-report: LCOV output is only supported with coverage.py >= 6.3',
+    ])
+    assert result.ret != 0
+
+
 def test_term_output_dir(testdir):
     script = testdir.makepyfile(SCRIPT)
 
     result = testdir.runpytest('-v',
                                '--cov=%s' % script.dirpath(),
                                '--cov-report=term:' + DEST_DIR,
                                script)
@@ -385,14 +418,27 @@
 
     assert result.ret != 0
     result.stdout.fnmatch_lines([
         'FAIL Required test coverage of 100% not reached. Total coverage: *%'
     ])
 
 
+def test_cov_min_100_passes_if_collectonly(testdir):
+    script = testdir.makepyfile(SCRIPT)
+
+    result = testdir.runpytest('-v',
+                               '--cov=%s' % script.dirpath(),
+                               '--cov-report=term-missing',
+                               '--cov-fail-under=100',
+                               '--collect-only',
+                               script)
+
+    assert result.ret == 0
+
+
 def test_cov_min_50(testdir):
     script = testdir.makepyfile(SCRIPT)
 
     result = testdir.runpytest('-v',
                                '--cov=%s' % script.dirpath(),
                                '--cov-report=html',
                                '--cov-report=xml',
@@ -444,15 +490,15 @@
 
     assert result.ret == 0
     result.stdout.fnmatch_lines([
         'Required test coverage of 50% reached. Total coverage: *%'
     ])
 
 
-def test_central_nonspecific(testdir, prop):
+def test_central_nonspecific(pytester, testdir, prop):
     script = testdir.makepyfile(prop.code)
     testdir.tmpdir.join('.coveragerc').write(prop.fullconf)
     result = testdir.runpytest('-v',
                                '--cov',
                                '--cov-report=term-missing',
                                script, *prop.args)
 
@@ -479,15 +525,15 @@
                                '--cov=%s' % script.dirpath(),
                                '--cov-report=term-missing',
                                script)
 
     assert result.ret != 0
 
 
-def test_central_coveragerc(testdir, prop):
+def test_central_coveragerc(pytester, testdir, prop):
     script = testdir.makepyfile(prop.code)
     testdir.tmpdir.join('.coveragerc').write(COVERAGERC_SOURCE + prop.conf)
 
     result = testdir.runpytest('-v',
                                '--cov',
                                '--cov-report=term-missing',
                                script, *prop.args)
@@ -497,15 +543,15 @@
         'test_central_coveragerc* %s *' % prop.result,
         '*10 passed*',
     ])
     assert result.ret == 0
 
 
 @xdist_params
-def test_central_with_path_aliasing(testdir, monkeypatch, opts, prop):
+def test_central_with_path_aliasing(pytester, testdir, monkeypatch, opts, prop):
     mod1 = testdir.mkdir('src').join('mod.py')
     mod1.write(SCRIPT)
     mod2 = testdir.mkdir('aliased').join('mod.py')
     mod2.write(SCRIPT)
     script = testdir.makepyfile('''
 from mod import *
 ''')
@@ -531,15 +577,15 @@
         'src[\\/]mod* %s *' % prop.result,
         '*10 passed*',
     ])
     assert result.ret == 0
 
 
 @xdist_params
-def test_borken_cwd(testdir, monkeypatch, opts):
+def test_borken_cwd(pytester, testdir, monkeypatch, opts):
     testdir.makepyfile(mod='''
 def foobar(a, b):
     return a + b
 ''')
 
     script = testdir.makepyfile('''
 import os
@@ -570,15 +616,15 @@
         '*mod* 100%',
         '*1 passed*',
     ])
 
     assert result.ret == 0
 
 
-def test_subprocess_with_path_aliasing(testdir, monkeypatch):
+def test_subprocess_with_path_aliasing(pytester, testdir, monkeypatch):
     src = testdir.mkdir('src')
     src.join('parent_script.py').write(SCRIPT_PARENT)
     src.join('child_script.py').write(SCRIPT_CHILD)
     aliased = testdir.mkdir('aliased')
     parent_script = aliased.join('parent_script.py')
     parent_script.write(SCRIPT_PARENT)
     aliased.join('child_script.py').write(SCRIPT_CHILD)
@@ -606,15 +652,15 @@
         '*- coverage: platform *, python * -*',
         'src[\\/]child_script* %s*' % CHILD_SCRIPT_RESULT,
         'src[\\/]parent_script* %s*' % PARENT_SCRIPT_RESULT,
     ])
     assert result.ret == 0
 
 
-def test_show_missing_coveragerc(testdir, prop):
+def test_show_missing_coveragerc(pytester, testdir, prop):
     script = testdir.makepyfile(prop.code)
     testdir.tmpdir.join('.coveragerc').write("""
 [run]
 source = .
 %s
 
 [report]
@@ -649,15 +695,15 @@
                                '--no-cov-on-fail',
                                script)
 
     assert 'coverage: platform' not in result.stdout.str()
     result.stdout.fnmatch_lines(['*1 failed*'])
 
 
-def test_no_cov(testdir, monkeypatch):
+def test_no_cov(pytester, testdir, monkeypatch):
     script = testdir.makepyfile(SCRIPT)
     testdir.makeini("""
         [pytest]
         addopts=--no-cov
     """)
     result = testdir.runpytest('-vvv',
                                '--cov=%s' % script.dirpath(),
@@ -716,15 +762,15 @@
     for line in chain(result.stdout.lines, result.stderr.lines):
         assert 'The following workers failed to return coverage data' not in line
         assert 'INTERNALERROR' not in line
     assert result.ret == 0
 
 
 @pytest.mark.skipif('sys.platform == "win32" and platform.python_implementation() == "PyPy"')
-def test_dist_collocated(testdir, prop):
+def test_dist_collocated(pytester, testdir, prop):
     script = testdir.makepyfile(prop.code)
     testdir.tmpdir.join('.coveragerc').write(prop.fullconf)
     result = testdir.runpytest('-v',
                                '--cov=%s' % script.dirpath(),
                                '--cov-report=term-missing',
                                '--dist=load',
                                '--tx=2*popen',
@@ -736,15 +782,15 @@
         'test_dist_collocated* %s *' % prop.result,
         '*10 passed*'
     ])
     assert result.ret == 0
 
 
 @pytest.mark.skipif('sys.platform == "win32" and platform.python_implementation() == "PyPy"')
-def test_dist_not_collocated(testdir, prop):
+def test_dist_not_collocated(pytester, testdir, prop):
     script = testdir.makepyfile(prop.code)
     dir1 = testdir.mkdir('dir1')
     dir2 = testdir.mkdir('dir2')
     testdir.tmpdir.join('.coveragerc').write('''
 [run]
 %s
 [paths]
@@ -769,15 +815,15 @@
         'test_dist_not_collocated* %s *' % prop.result,
         '*10 passed*'
     ])
     assert result.ret == 0
 
 
 @pytest.mark.skipif('sys.platform == "win32" and platform.python_implementation() == "PyPy"')
-def test_dist_not_collocated_coveragerc_source(testdir, prop):
+def test_dist_not_collocated_coveragerc_source(pytester, testdir, prop):
     script = testdir.makepyfile(prop.code)
     dir1 = testdir.mkdir('dir1')
     dir2 = testdir.mkdir('dir2')
     testdir.tmpdir.join('.coveragerc').write('''
 [run]
 {}
 source = {}
@@ -844,15 +890,15 @@
         '*- coverage: platform *, python * -*',
         '*child_script* %s*' % CHILD_SCRIPT_RESULT,
         '*parent_script* 100%*',
     ])
     assert result.ret == 0
 
 
-def test_central_subprocess_change_cwd_with_pythonpath(testdir, monkeypatch):
+def test_central_subprocess_change_cwd_with_pythonpath(pytester, testdir, monkeypatch):
     stuff = testdir.mkdir('stuff')
     parent_script = stuff.join('parent_script.py')
     parent_script.write(SCRIPT_PARENT_CHANGE_CWD_IMPORT_CHILD)
     stuff.join('child_script.py').write(SCRIPT_CHILD)
     testdir.makefile('', coveragerc="""
 [run]
 parallel = true
@@ -915,15 +961,15 @@
         'child_script* %s*' % CHILD_SCRIPT_RESULT,
         'parent_script* %s*' % PARENT_SCRIPT_RESULT,
     ])
     assert result.ret == 0
 
 
 @pytest.mark.skipif('sys.platform == "win32" and platform.python_implementation() == "PyPy"')
-def test_dist_subprocess_not_collocated(testdir, tmpdir):
+def test_dist_subprocess_not_collocated(pytester, testdir, tmpdir):
     scripts = testdir.makepyfile(parent_script=SCRIPT_PARENT,
                                  child_script=SCRIPT_CHILD)
     parent_script = scripts.dirpath().join('parent_script.py')
     child_script = scripts.dirpath().join('child_script.py')
 
     dir1 = tmpdir.mkdir('dir1')
     dir2 = tmpdir.mkdir('dir2')
@@ -964,27 +1010,29 @@
                                '--cov-report=term-missing',
                                script)
 
     result.stdout.fnmatch_lines([
         '*10 passed*'
     ])
     result.stderr.fnmatch_lines([
-        'Coverage.py warning: No data was collected.*'
+        '*No data was collected.*'
     ])
     result.stdout.fnmatch_lines([
         '*Failed to generate report: No data to report.',
     ])
     assert result.ret == 0
 
     matching_lines = [line for line in result.outlines if '%' in line]
     assert not matching_lines
 
 
 @pytest.mark.skipif("'dev' in pytest.__version__")
 @pytest.mark.skipif('sys.platform == "win32" and platform.python_implementation() == "PyPy"')
+@pytest.mark.skipif('tuple(map(int, xdist.__version__.split("."))) >= (2, 3, 0)',
+                    reason="Since pytest-xdist 2.3.0 the parent sys.path is copied in the child process")
 def test_dist_missing_data(testdir):
     """Test failure when using a worker without pytest-cov installed."""
     venv_path = os.path.join(str(testdir.tmpdir), 'venv')
     virtualenv.cli_run([venv_path])
     if sys.platform == 'win32':
         if platform.python_implementation() == "PyPy":
             exe = os.path.join(venv_path, 'bin', 'python.exe')
@@ -1006,15 +1054,15 @@
     result = testdir.runpytest('-v',
                                '--assert=plain',
                                '--cov=%s' % script.dirpath(),
                                '--cov-report=term-missing',
                                '--dist=load',
                                '--tx=popen//python=%s' % exe,
                                max_worker_restart_0,
-                               script)
+                               str(script))
     result.stdout.fnmatch_lines([
         'The following workers failed to return coverage data, ensure that pytest-cov is installed on these workers.'
     ])
 
 
 def test_funcarg(testdir):
     script = testdir.makepyfile(SCRIPT_FUNCARG)
@@ -1040,239 +1088,16 @@
 
     result.stdout.fnmatch_lines([
         '*1 passed*'
     ])
     assert result.ret == 0
 
 
-@pytest.mark.skipif("sys.version_info[0] < 3", reason="no context manager api on Python 2")
-@pytest.mark.skipif('sys.platform == "win32"', reason="multiprocessing support is broken on Windows")
-@pytest.mark.skipif('platform.python_implementation() == "PyPy"', reason="often deadlocks on PyPy")
-@pytest.mark.skipif('sys.version_info[:2] >= (3, 8)', reason="deadlocks on Python 3.8+, see: https://bugs.python.org/issue38227")
-def test_multiprocessing_pool(testdir):
-    pytest.importorskip('multiprocessing.util')
-
-    script = testdir.makepyfile('''
-import multiprocessing
-
-def target_fn(a):
-    %sse:  # pragma: nocover
-        return None
-
-def test_run_target():
-    from pytest_cov.embed import cleanup_on_sigterm
-    cleanup_on_sigterm()
-
-    for i in range(33):
-        with multiprocessing.Pool(3) as p:
-            p.map(target_fn, [i * 3 + j for j in range(3)])
-        p.join()
-''' % ''.join('''if a == %r:
-        return a
-    el''' % i for i in range(99)))
-
-    result = testdir.runpytest('-v',
-                               '--cov=%s' % script.dirpath(),
-                               '--cov-report=term-missing',
-                               script)
-
-    assert "Doesn't seem to be a coverage.py data file" not in result.stdout.str()
-    assert "Doesn't seem to be a coverage.py data file" not in result.stderr.str()
-    assert not testdir.tmpdir.listdir(".coverage.*")
-    result.stdout.fnmatch_lines([
-        '*- coverage: platform *, python * -*',
-        'test_multiprocessing_pool* 100%*',
-        '*1 passed*'
-    ])
-    assert result.ret == 0
-
-
-@pytest.mark.skipif('sys.platform == "win32"', reason="multiprocessing support is broken on Windows")
-@pytest.mark.skipif('platform.python_implementation() == "PyPy"', reason="often deadlocks on PyPy")
-@pytest.mark.skipif('sys.version_info[:2] >= (3, 8)', reason="deadlocks on Python 3.8, see: https://bugs.python.org/issue38227")
-def test_multiprocessing_pool_terminate(testdir):
-    pytest.importorskip('multiprocessing.util')
-
-    script = testdir.makepyfile('''
-import multiprocessing
-
-def target_fn(a):
-    %sse:  # pragma: nocover
-        return None
-
-def test_run_target():
-    from pytest_cov.embed import cleanup_on_sigterm
-    cleanup_on_sigterm()
-
-    for i in range(33):
-        p = multiprocessing.Pool(3)
-        try:
-            p.map(target_fn, [i * 3 + j for j in range(3)])
-        finally:
-            p.terminate()
-            p.join()
-''' % ''.join('''if a == %r:
-        return a
-    el''' % i for i in range(99)))
-
-    result = testdir.runpytest('-v',
-                               '--cov=%s' % script.dirpath(),
-                               '--cov-report=term-missing',
-                               script)
-
-    assert "Doesn't seem to be a coverage.py data file" not in result.stdout.str()
-    assert "Doesn't seem to be a coverage.py data file" not in result.stderr.str()
-    assert not testdir.tmpdir.listdir(".coverage.*")
-    result.stdout.fnmatch_lines([
-        '*- coverage: platform *, python * -*',
-        'test_multiprocessing_pool* 100%*',
-        '*1 passed*'
-    ])
-    assert result.ret == 0
-
-
-@pytest.mark.skipif('sys.platform == "win32"', reason="multiprocessing support is broken on Windows")
-@pytest.mark.skipif('sys.version_info[0] > 2 and platform.python_implementation() == "PyPy"', reason="broken on PyPy3")
-def test_multiprocessing_pool_close(testdir):
-    pytest.importorskip('multiprocessing.util')
-
-    script = testdir.makepyfile('''
-import multiprocessing
-
-def target_fn(a):
-    %sse:  # pragma: nocover
-        return None
-
-def test_run_target():
-    for i in range(33):
-        p = multiprocessing.Pool(3)
-        try:
-            p.map(target_fn, [i * 3 + j for j in range(3)])
-        finally:
-            p.close()
-            p.join()
-''' % ''.join('''if a == %r:
-        return a
-    el''' % i for i in range(99)))
-
-    result = testdir.runpytest('-v',
-                               '--cov=%s' % script.dirpath(),
-                               '--cov-report=term-missing',
-                               script)
-    assert "Doesn't seem to be a coverage.py data file" not in result.stdout.str()
-    assert "Doesn't seem to be a coverage.py data file" not in result.stderr.str()
-    assert not testdir.tmpdir.listdir(".coverage.*")
-    result.stdout.fnmatch_lines([
-        '*- coverage: platform *, python * -*',
-        'test_multiprocessing_pool* 100%*',
-        '*1 passed*'
-    ])
-    assert result.ret == 0
-
-
-@pytest.mark.skipif('sys.platform == "win32"', reason="multiprocessing support is broken on Windows")
-def test_multiprocessing_process(testdir):
-    pytest.importorskip('multiprocessing.util')
-
-    script = testdir.makepyfile('''
-import multiprocessing
-
-def target_fn():
-    a = True
-    return a
-
-def test_run_target():
-    p = multiprocessing.Process(target=target_fn)
-    p.start()
-    p.join()
-''')
-
-    result = testdir.runpytest('-v',
-                               '--cov=%s' % script.dirpath(),
-                               '--cov-report=term-missing',
-                               script)
-
-    result.stdout.fnmatch_lines([
-        '*- coverage: platform *, python * -*',
-        'test_multiprocessing_process* 8 * 100%*',
-        '*1 passed*'
-    ])
-    assert result.ret == 0
-
-
-@pytest.mark.skipif('sys.platform == "win32"', reason="multiprocessing support is broken on Windows")
-def test_multiprocessing_process_no_source(testdir):
-    pytest.importorskip('multiprocessing.util')
-
-    script = testdir.makepyfile('''
-import multiprocessing
-
-def target_fn():
-    a = True
-    return a
-
-def test_run_target():
-    p = multiprocessing.Process(target=target_fn)
-    p.start()
-    p.join()
-''')
-
-    result = testdir.runpytest('-v',
-                               '--cov',
-                               '--cov-report=term-missing',
-                               script)
-
-    result.stdout.fnmatch_lines([
-        '*- coverage: platform *, python * -*',
-        'test_multiprocessing_process* 8 * 100%*',
-        '*1 passed*'
-    ])
-    assert result.ret == 0
-
-
-@pytest.mark.skipif('sys.platform == "win32"', reason="multiprocessing support is broken on Windows")
-def test_multiprocessing_process_with_terminate(testdir):
-    pytest.importorskip('multiprocessing.util')
-
-    script = testdir.makepyfile('''
-import multiprocessing
-import time
-from pytest_cov.embed import cleanup_on_sigterm
-cleanup_on_sigterm()
-
-event = multiprocessing.Event()
-
-def target_fn():
-    a = True
-    event.set()
-    time.sleep(5)
-
-def test_run_target():
-    p = multiprocessing.Process(target=target_fn)
-    p.start()
-    time.sleep(0.5)
-    event.wait(1)
-    p.terminate()
-    p.join()
-''')
-
-    result = testdir.runpytest('-v',
-                               '--cov=%s' % script.dirpath(),
-                               '--cov-report=term-missing',
-                               script)
-
-    result.stdout.fnmatch_lines([
-        '*- coverage: platform *, python * -*',
-        'test_multiprocessing_process* 16 * 100%*',
-        '*1 passed*'
-    ])
-    assert result.ret == 0
-
-
 @pytest.mark.skipif('sys.platform == "win32"', reason="SIGTERM isn't really supported on Windows")
+@pytest.mark.xfail('platform.python_implementation() == "PyPy"', reason="Interpreter seems buggy")
 def test_cleanup_on_sigterm(testdir):
     script = testdir.makepyfile('''
 import os, signal, subprocess, sys, time
 
 def cleanup(num, frame):
     print("num == signal.SIGTERM => %s" % (num == signal.SIGTERM))
     raise Exception()
@@ -1315,15 +1140,15 @@
 
 @pytest.mark.skipif('sys.platform != "win32"')
 @pytest.mark.parametrize('setup', [
     ('signal.signal(signal.SIGBREAK, signal.SIG_DFL); cleanup_on_signal(signal.SIGBREAK)', '87%   21-22'),
     ('cleanup_on_signal(signal.SIGBREAK)', '87%   21-22'),
     ('cleanup()', '73%   19-22'),
 ])
-def test_cleanup_on_sigterm_sig_break(testdir, setup):
+def test_cleanup_on_sigterm_sig_break(pytester, testdir, setup):
     # worth a read: https://stefan.sofa-rockers.org/2013/08/15/handling-sub-process-hierarchies-python-linux-os-x/
     script = testdir.makepyfile('''
 import os, signal, subprocess, sys, time
 
 def test_run():
     proc = subprocess.Popen(
         [sys.executable, __file__],
@@ -1356,20 +1181,22 @@
         'test_cleanup_on_sigterm* %s' % setup[1],
         '*1 passed*'
     ])
     assert result.ret == 0
 
 
 @pytest.mark.skipif('sys.platform == "win32"', reason="SIGTERM isn't really supported on Windows")
+@pytest.mark.xfail('sys.platform == "darwin"', reason="Something weird going on Macs...")
+@pytest.mark.xfail('platform.python_implementation() == "PyPy"', reason="Interpreter seems buggy")
 @pytest.mark.parametrize('setup', [
     ('signal.signal(signal.SIGTERM, signal.SIG_DFL); cleanup_on_sigterm()', '88%   18-19'),
     ('cleanup_on_sigterm()', '88%   18-19'),
     ('cleanup()', '75%   16-19'),
 ])
-def test_cleanup_on_sigterm_sig_dfl(testdir, setup):
+def test_cleanup_on_sigterm_sig_dfl(pytester, testdir, setup):
     script = testdir.makepyfile('''
 import os, signal, subprocess, sys, time
 
 def test_run():
     proc = subprocess.Popen([sys.executable, __file__], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     time.sleep(1)
     proc.terminate()
@@ -1399,14 +1226,16 @@
         'test_cleanup_on_sigterm* %s' % setup[1],
         '*1 passed*'
     ])
     assert result.ret == 0
 
 
 @pytest.mark.skipif('sys.platform == "win32"', reason="SIGINT is subtly broken on Windows")
+@pytest.mark.xfail('sys.platform == "darwin"', reason="Something weird going on Macs...")
+@pytest.mark.xfail('platform.python_implementation() == "PyPy"', reason="Interpreter seems buggy")
 def test_cleanup_on_sigterm_sig_dfl_sigint(testdir):
     script = testdir.makepyfile('''
 import os, signal, subprocess, sys, time
 
 def test_run():
     proc = subprocess.Popen([sys.executable, __file__], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     time.sleep(1)
@@ -1438,14 +1267,15 @@
         'test_cleanup_on_sigterm* 88%   19-20',
         '*1 passed*'
     ])
     assert result.ret == 0
 
 
 @pytest.mark.skipif('sys.platform == "win32"', reason="fork not available on Windows")
+@pytest.mark.xfail('platform.python_implementation() == "PyPy"', reason="Interpreter seems buggy")
 def test_cleanup_on_sigterm_sig_ign(testdir):
     script = testdir.makepyfile('''
 import os, signal, subprocess, sys, time
 
 def test_run():
     proc = subprocess.Popen([sys.executable, __file__], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     time.sleep(1)
@@ -1603,15 +1433,14 @@
 
 
 COVERAGERC = '''
 [report]
 # Regexes for lines to exclude from consideration
 exclude_lines =
     raise NotImplementedError
-
 '''
 
 EXCLUDED_TEST = '''
 
 def func():
     raise NotImplementedError
 
@@ -1670,15 +1499,15 @@
 
 SKIP_COVERED_RESULT = '1 file skipped due to complete coverage.'
 
 
 @pytest.mark.parametrize('report_option', [
     'term-missing:skip-covered',
     'term:skip-covered'])
-def test_skip_covered_cli(testdir, report_option):
+def test_skip_covered_cli(pytester, testdir, report_option):
     testdir.makefile('', coveragerc=SKIP_COVERED_COVERAGERC)
     script = testdir.makepyfile(SKIP_COVERED_TEST)
     result = testdir.runpytest('-v',
                                '--cov=%s' % script.dirpath(),
                                '--cov-report=%s' % report_option,
                                script)
     assert result.ret == 0
@@ -1764,14 +1593,15 @@
     assert result.ret == 0
 
 
 def test_not_started_plugin_does_not_fail(testdir):
     class ns:
         cov_source = [True]
         cov_report = ''
+
     plugin = pytest_cov.plugin.CovPlugin(ns, None, start=False)
     plugin.pytest_runtestloop(None)
     plugin.pytest_terminal_summary(None)
 
 
 def test_default_output_setting(testdir):
     script = testdir.makepyfile(SCRIPT)
@@ -1875,38 +1705,38 @@
                                '--cov=%s' % script.dirpath(),
                                script)
     assert result.ret == 0
     assert glob.glob(str(testdir.tmpdir.join('.coverage*')))
 
 
 @xdist_params
-def test_append_coverage(testdir, opts, prop):
+def test_append_coverage(pytester, testdir, opts, prop):
     script = testdir.makepyfile(test_1=prop.code)
     testdir.tmpdir.join('.coveragerc').write(prop.fullconf)
     result = testdir.runpytest('-v',
                                '--cov=%s' % script.dirpath(),
                                script,
-                               *opts.split()+prop.args)
+                               *opts.split() + prop.args)
     result.stdout.fnmatch_lines([
         'test_1* %s*' % prop.result,
     ])
     script2 = testdir.makepyfile(test_2=prop.code2)
     result = testdir.runpytest('-v',
                                '--cov-append',
                                '--cov=%s' % script2.dirpath(),
                                script2,
-                               *opts.split()+prop.args)
+                               *opts.split() + prop.args)
     result.stdout.fnmatch_lines([
         'test_1* %s*' % prop.result,
         'test_2* %s*' % prop.result2,
     ])
 
 
 @xdist_params
-def test_do_not_append_coverage(testdir, opts, prop):
+def test_do_not_append_coverage(pytester, testdir, opts, prop):
     script = testdir.makepyfile(test_1=prop.code)
     testdir.tmpdir.join('.coveragerc').write(prop.fullconf)
     result = testdir.runpytest('-v',
                                '--cov=%s' % script.dirpath(),
                                script,
                                *opts.split()+prop.args)
     result.stdout.fnmatch_lines([
@@ -1960,16 +1790,19 @@
 
     from pytest_cov import embed
 
     monkeypatch.setattr(embed, 'init', bad_init)
     monkeypatch.setattr(sys, 'stderr', buff)
     monkeypatch.setitem(os.environ, 'COV_CORE_SOURCE', 'foobar')
     exec(payload)
-    assert buff.getvalue() == '''pytest-cov: Failed to setup subprocess coverage. Environ: {'COV_CORE_SOURCE': 'foobar'} Exception: SpecificError()
-'''
+    expected = (
+        "pytest-cov: Failed to setup subprocess coverage. "
+        "Environ: {'COV_CORE_SOURCE': 'foobar'} Exception: SpecificError()\n"
+    )
+    assert buff.getvalue() == expected
 
 
 def test_double_cov(testdir):
     script = testdir.makepyfile(SCRIPT_SIMPLE)
     result = testdir.runpytest('-v',
                                '--assert=plain',
                                '--cov', '--cov=%s' % script.dirpath(),
@@ -2080,15 +1913,15 @@
     'test_contexts.py::test_13[4-1]|run': 'r13-3',
     'test_contexts.py::test_13[4-2]|run': 'r13-4',
 }
 
 
 @pytest.mark.skipif("coverage.version_info < (5, 0)")
 @xdist_params
-def test_contexts(testdir, opts):
+def test_contexts(pytester, testdir, opts):
     with open(os.path.join(os.path.dirname(__file__), "contextful.py")) as f:
         contextful_tests = f.read()
     script = testdir.makepyfile(contextful_tests)
     result = testdir.runpytest('-v',
                                '--cov=%s' % script.dirpath(),
                                '--cov-context=test',
                                script,
```

### Comparing `pytest-cov-3.0.0/tox.ini` & `pytest-cov-4.0.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,75 @@
 [testenv:bootstrap]
 deps =
     jinja2
-    matrix
     tox
 skip_install = true
 commands =
     python ci/bootstrap.py --no-env
 passenv =
     *
 ; a generative tox configuration, see: https://tox.readthedocs.io/en/latest/config.html#generative-envlist
 
 [tox]
 envlist =
     check
-    py{36,37,py,py3}-pytest46-xdist127-coverage{55}
-    py{36,37,38,py3}-pytest{46,54}-xdist133-coverage{55}
-    py{36,37,38,39,310,py3}-pytest{62}-xdist202-coverage{55}
+    py{36}-pytest{70}-xdist250-coverage{62}
+    py{37,38,39,310,py37,py38}-pytest{71}-xdist250-coverage{64}
     docs
 
 [testenv]
 extras = testing
 setenv =
     PYTHONUNBUFFERED=yes
 
     # Use env vars for (optional) pinning of deps.
     pytest46:  _DEP_PYTEST=pytest==4.6.10
     pytest53:  _DEP_PYTEST=pytest==5.3.2
     pytest54:  _DEP_PYTEST=pytest==5.4.3
     pytest60:  _DEP_PYTEST=pytest==6.0.2
     pytest61:  _DEP_PYTEST=pytest==6.1.2
     pytest62:  _DEP_PYTEST=pytest==6.2.5
+    pytest70:  _DEP_PYTEST=pytest==7.0.1
+    pytest71:  _DEP_PYTEST=pytest==7.1.2
 
     xdist127: _DEP_PYTESTXDIST=pytest-xdist==1.27.0
     xdist129: _DEP_PYTESTXDIST=pytest-xdist==1.29.0
     xdist131: _DEP_PYTESTXDIST=pytest-xdist==1.31.0
     xdist132: _DEP_PYTESTXDIST=pytest-xdist==1.32.0
     xdist133: _DEP_PYTESTXDIST=pytest-xdist==1.33.0
     xdist134: _DEP_PYTESTXDIST=pytest-xdist==1.34.0
     xdist200: _DEP_PYTESTXDIST=pytest-xdist==2.0.0
     xdist201: _DEP_PYTESTXDIST=pytest-xdist==2.1.0
     xdist202: _DEP_PYTESTXDIST=pytest-xdist==2.2.0
+    xdist250: _DEP_PYTESTXDIST=pytest-xdist==2.5.0
     xdistdev: _DEP_PYTESTXDIST=git+https://github.com/pytest-dev/pytest-xdist.git#egg=pytest-xdist
 
     coverage45: _DEP_COVERAGE=coverage==4.5.4
     coverage50: _DEP_COVERAGE=coverage==5.0.4
     coverage51: _DEP_COVERAGE=coverage==5.1
     coverage52: _DEP_COVERAGE=coverage==5.2.1
     coverage53: _DEP_COVERAGE=coverage==5.3.1
     coverage54: _DEP_COVERAGE=coverage==5.4
     coverage55: _DEP_COVERAGE=coverage==5.5
+    coverage60: _DEP_COVERAGE=coverage==6.0.2
+    coverage61: _DEP_COVERAGE=coverage==6.1.2
+    coverage62: _DEP_COVERAGE=coverage==6.2
+    coverage63: _DEP_COVERAGE=coverage==6.3.3
+    coverage64: _DEP_COVERAGE=coverage==6.4.2
     # For testing against a coverage.py working tree.
     coveragedev: _DEP_COVERAGE=-e{env:COVERAGE_HOME}
 passenv =
     *
 deps =
     {env:_DEP_PYTEST:pytest}
     {env:_DEP_PYTESTXDIST:pytest-xdist}
     {env:_DEP_COVERAGE:coverage}
 pip_pre = true
 commands =
-    pytest {posargs:-vv}
+    {posargs:pytest -vv}
 
 [testenv:spell]
 setenv =
     SPELLCHECK=1
 commands =
     sphinx-build -b spelling docs dist/docs
 skip_install = true
```

