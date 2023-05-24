# Comparing `tmp/abqpy-2023.5.1.tar.gz` & `tmp/abqpy-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abqpy-2023.5.1.tar", last modified: Sat May 13 13:06:48 2023, max compression
+gzip compressed data, was "abqpy-2023.5.2.tar", last modified: Wed May 24 15:24:23 2023, max compression
```

## Comparing `abqpy-2023.5.1.tar` & `abqpy-2023.5.2.tar`

### file list

```diff
@@ -1,1651 +1,1645 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.527859 abqpy-2023.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.279837 abqpy-2023.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.279837 abqpy-2023.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/keylabeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/release-drafter-2016.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/release-drafter-2017.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/release-drafter-2018.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/release-drafter-2019.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/release-drafter-2020.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/release-drafter-2021.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/release-drafter-2022.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/release-drafter-2023.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.279837 abqpy-2023.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/workflows/changes.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/workflows/conflicts.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/workflows/rtd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.github/workflows/translations.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-13 13:06:35.000000 abqpy-2023.5.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-13 13:06:35.000000 abqpy-2023.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-13 13:06:48.527859 abqpy-2023.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-13 13:06:35.000000 abqpy-2023.5.1/README-zh-cn.md
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-13 13:06:35.000000 abqpy-2023.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.279837 abqpy-2023.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.283838 abqpy-2023.5.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)    60200 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/CHANGES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.283838 abqpy-2023.5.1/docs/source/_autoapi_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/_autoapi_templates/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.283838 abqpy-2023.5.1/docs/source/_autoapi_templates/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/_autoapi_templates/python/class.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.283838 abqpy-2023.5.1/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/_ext/automembers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/_ext/changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/_ext/classdocumenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/_ext/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.283838 abqpy-2023.5.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/_static/3ds-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/_static/PyPI_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/_static/rtd-logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/_static/rtd-logo-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/envvars.md
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/getting_started.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.295839 abqpy-2023.5.1/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/acl-all-schematic-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/afxI_commandLine.png
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/afxI_messageArea.png
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-abstract-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-aexample-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-cae.png
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-exception-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-model-assembly-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-model-model-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-model-odb-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-model-overview-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-model-part-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-model-session-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)    10845 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-model-viewport-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-table-editor-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-int-unix-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-odb-api-acousticviz.png
--rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-pde-debugger-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-pde-filemenu-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-pde-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-pde-settingsmenu-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-righttoleft-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-skew-dim.png
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/cmd-super.png
--rw-r--r--   0 runner    (1001) docker     (123)   144708 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/compression.png
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/exxskew-quadmesh-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/gst-beam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/ico_guiCli.png
--rw-r--r--   0 runner    (1001) docker     (123)    33118 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/job_monitor.png
--rw-r--r--   0 runner    (1001) docker     (123)  2734175 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/model-code.gif
--rw-r--r--   0 runner    (1001) docker     (123)    63477 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/model-code.png
--rw-r--r--   0 runner    (1001) docker     (123)    61111 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/model.png
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/odb-field-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/odb-history-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/odb-model-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/odb-overview-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)  2534245 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/output-code.gif
--rw-r--r--   0 runner    (1001) docker     (123)    53417 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/output-code.png
--rw-r--r--   0 runner    (1001) docker     (123)    32580 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/output.png
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/utl-getinput-default-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/utl-getinput-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/utl-getinputs-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/images/utl-getwarningreply-nls.png
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/localization.md
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/policy.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.295839 abqpy-2023.5.1/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.295839 abqpy-2023.5.1/docs/source/reference/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/kernel/cae_display_preferences.md
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/kernel/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/kernel/input.md
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/kernel/kernel.md
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/kernel/messaging.md
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/kernel/table_collection.md
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/kernel/text_representation.md
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/kernel/utility.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.295839 abqpy-2023.5.1/docs/source/reference/mdb/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/annotation.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/edit_mesh.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/job.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.299839 abqpy-2023.5.1/docs/source/reference/mdb/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/adaptivity.md
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/amplitude.md
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/bc.md
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/calibration.md
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/constraint.md
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/field.md
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/filter.md
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/interaction.md
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/load.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/material.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/mesh.md
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/optimization.md
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/output.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.299839 abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/assembly.md
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/datum.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/engineering.md
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/geometry.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/part.md
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/region.md
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/predefined.md
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/profile.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/property.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.299839 abqpy-2023.5.1/docs/source/reference/mdb/model/section/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/section/connector.md
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/section/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/sketcher.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.299839 abqpy-2023.5.1/docs/source/reference/mdb/model/step/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/step/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/mdb/model/step/step_miscellaneous.md
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/odb.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.303840 abqpy-2023.5.1/docs/source/reference/session/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/session/animation.md
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/session/canvas.md
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/session/display.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/session/display_options.md
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/session/field_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/session/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/session/odb_display.md
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/session/path.md
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/session/plot_options.md
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/session/print.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/reference/session/xy.md
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/tutorials.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.303840 abqpy-2023.5.1/docs/source/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.303840 abqpy-2023.5.1/docs/source/user/about/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.303840 abqpy-2023.5.1/docs/source/user/about/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/about/examples/create-part.md
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/about/examples/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/about/examples/read-output.md
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/about/examples/summary.md
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/about/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/about/interact.md
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/about/interface.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.307840 abqpy-2023.5.1/docs/source/user/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/environment/about.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/environment/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/environment/pde-basics.md
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/environment/use-pde.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.307840 abqpy-2023.5.1/docs/source/user/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/examples/cantilever.md
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/examples/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/examples/plot.md
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/examples/sensitivity.md
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/examples/settings.md
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.311840 abqpy-2023.5.1/docs/source/user/output/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.311840 abqpy-2023.5.1/docs/source/user/output/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/about.md
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/access.md
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/compile-link.md
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/computations.md
--rw-r--r--   0 runner    (1001) docker     (123)    32551 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/improve-efficiency.md
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/need-what-access.md
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/object-model.md
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/output-object-model.md
--rw-r--r--   0 runner    (1001) docker     (123)    35243 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/read.md
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/style.md
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/utility.md
--rw-r--r--   0 runner    (1001) docker     (123)    20430 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/cpp/write.md
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.315841 abqpy-2023.5.1/docs/source/user/output/python/
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/python/computations.md
--rw-r--r--   0 runner    (1001) docker     (123)    43196 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/python/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/python/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/python/execute-script.md
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/python/improve-efficiency.md
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/python/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/python/need-what-to-understand.md
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/python/object-model.md
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/python/output-object-model.md
--rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/python/read.md
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/output/python/write.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.315841 abqpy-2023.5.1/docs/source/user/python/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.315841 abqpy-2023.5.1/docs/source/user/python/introduction/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/introduction/further-reading.md
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/introduction/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/introduction/oop-basics.md
--rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/introduction/programming.md
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/introduction/python-abaqus.md
--rw-r--r--   0 runner    (1001) docker     (123)    18341 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/introduction/python-basics.md
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/introduction/python-interpreter.md
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/introduction/python-resources.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.319841 abqpy-2023.5.1/docs/source/user/python/python-abaqus/
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/python-abaqus/errors.md
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/python-abaqus/executing.md
--rw-r--r--   0 runner    (1001) docker     (123)    19635 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/python-abaqus/extending.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/python-abaqus/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/python-abaqus/oop.md
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/python-abaqus/style.md
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/python-abaqus/types.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.319841 abqpy-2023.5.1/docs/source/user/python/use-scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/use-scripts/environment-file.md
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/use-scripts/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/use-scripts/interact.md
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/use-scripts/modify-objects.md
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/use-scripts/namespace.md
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/use-scripts/object-model.md
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/use-scripts/sequences.md
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/use-scripts/specify-region.md
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/use-scripts/specify-viewport.md
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/source/user/python/use-scripts/user-input.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-13 13:06:35.000000 abqpy-2023.5.1/docs/update-locale.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.319841 abqpy-2023.5.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.319841 abqpy-2023.5.1/examples/Abaqus/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/Abaqus/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/Abaqus/cantilever.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/Abaqus/skewExample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/Abaqus/viewerOpenOdbAndContour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/Abaqus/viewerPrintContours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.319841 abqpy-2023.5.1/examples/Compression/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/Compression/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/Compression/compression-output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/Compression/compression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.319841 abqpy-2023.5.1/examples/Parameter-Identification/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/Parameter-Identification/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/Parameter-Identification/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/Parameter-Identification/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-13 13:06:35.000000 abqpy-2023.5.1/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-13 13:06:35.000000 abqpy-2023.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.323841 abqpy-2023.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-13 13:06:35.000000 abqpy-2023.5.1/requirements/deps.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-13 13:06:35.000000 abqpy-2023.5.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-13 13:06:35.000000 abqpy-2023.5.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-13 13:06:35.000000 abqpy-2023.5.1/requirements/jupyter.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.323841 abqpy-2023.5.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-13 13:06:35.000000 abqpy-2023.5.1/scripts/conflicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-13 13:06:35.000000 abqpy-2023.5.1/scripts/rtd.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-13 13:06:35.000000 abqpy-2023.5.1/scripts/rtd.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 13:06:48.527859 abqpy-2023.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.327842 abqpy-2023.5.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/ababltin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.327842 abqpy-2023.5.1/src/abaqus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.327842 abqpy-2023.5.1/src/abaqus/AbaqusCAEDisplayPreferences/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/AbaqusCAEDisplayPreferences/CaeGuiPrefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/AbaqusCAEDisplayPreferences/CaeKerPrefs.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/AbaqusCAEDisplayPreferences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/AbaqusCAEDisplayPreferences/caePrefsAccess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.331842 abqpy-2023.5.1/src/abaqus/Adaptivity/
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptiveMeshConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptiveMeshConstraintState.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptiveMeshControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptiveMeshDomain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptivityIteration.py
--rw-r--r--   0 runner    (1001) docker     (123)    22664 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptivityModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptivityProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptivityStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/DisplacementAdaptiveMeshConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/DisplacementAdaptiveMeshConstraintState.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/ErrorIndicatorResult.py
--rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/RemeshingRule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/RuleResult.py
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/VelocityAdaptiveMeshConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/VelocityAdaptiveMeshConstraintState.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Adaptivity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.335842 abqpy-2023.5.1/src/abaqus/Amplitude/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/ActuatorAmplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/Amplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    19516 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/AmplitudeModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19562 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/AmplitudeOdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/BaselineCorrection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/Correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/DecayAmplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/EquallySpacedAmplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/ModulatedAmplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/PeriodicAmplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/PsdDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/SmoothStepAmplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/SolutionDependentAmplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/SpectrumAmplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/TabularAmplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Amplitude/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.335842 abqpy-2023.5.1/src/abaqus/Animation/
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Animation/AVIOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Animation/AnimationController.py
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Animation/AnimationOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Animation/AnimationSession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Animation/ImageAnimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Animation/ImageAnimationOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Animation/Movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Animation/QuickTimeOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Animation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.335842 abqpy-2023.5.1/src/abaqus/Annotation/
--rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Annotation/AnimationUserData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Annotation/Annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Annotation/AnnotationViewport.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Annotation/AnnotationsToPlotArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    17272 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Annotation/Arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Annotation/Text.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Annotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.339842 abqpy-2023.5.1/src/abaqus/Assembly/
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Assembly/Assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    41256 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Assembly/AssemblyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Assembly/AssemblyFeature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Assembly/AssemblyModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Assembly/ConnectorOrientation.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Assembly/ConnectorOrientationArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Assembly/ModelInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)    21362 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Assembly/PartInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Assembly/PartInstanceArray.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Assembly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.343843 abqpy-2023.5.1/src/abaqus/BasicGeometry/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/BasicGeometryPart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/Cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/CellArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/Edge.py
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/EdgeArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/Face.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/FaceArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/IgnoredEdge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/IgnoredEdgeArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/IgnoredVertex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/IgnoredVertexArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/InterestingPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/ModelDot.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/ModelDotArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/ReferencePoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/ReferencePointArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/ReferencePoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/Transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/Vertex.py
--rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/VertexArray.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BasicGeometry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.343843 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/ArbitraryProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/BeamSectionProfileModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15359 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/BeamSectionProfileOdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/BoxProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/CircularProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/GeneralizedProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/HexagonalProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/IProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/LProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/PipeProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/RectangularProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/TProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/TrapezoidalProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BeamSectionProfile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.351843 abqpy-2023.5.1/src/abaqus/BoundaryCondition/
--rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/AccelerationBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/AccelerationBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/AccelerationBaseMotionBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/AccelerationBaseMotionBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/AcousticPressureBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/AcousticPressureBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/BoundaryCondition.py
--rw-r--r--   0 runner    (1001) docker     (123)    93767 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/BoundaryConditionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/BoundaryConditionState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConcentrationBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConcentrationBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnAccelerationBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnAccelerationBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnDisplacementBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnDisplacementBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnVelocityBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnVelocityBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/DisplacementBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/DisplacementBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/DisplacementBaseMotionBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/DisplacementBaseMotionBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/ElectricPotentialBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/ElectricPotentialBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/EulerianBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/EulerianBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)    24508 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/EulerianMotionBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/EulerianMotionBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/FluidCavityPressureBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/FluidCavityPressureBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/MagneticVectorPotentialBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/MaterialFlowBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/MaterialFlowBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/PorePressureBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/PorePressureBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/RetainedNodalDofsBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/SecondaryBaseBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/SecondaryBaseBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/SubmodelBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/SubmodelBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/TemperatureBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/TemperatureBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/TypeBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/TypeBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/VelocityBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/VelocityBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/VelocityBaseMotionBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/VelocityBaseMotionBCState.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/BoundaryCondition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.355844 abqpy-2023.5.1/src/abaqus/Calibration/
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Calibration/Behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Calibration/Calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Calibration/CalibrationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Calibration/DataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Calibration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.355844 abqpy-2023.5.1/src/abaqus/Canvas/
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/AttributeColorMap.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/Canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/CanvasSession.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/Displayable.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/DrawingArea.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/Highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/ImageOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/Layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/MovieOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/Viewport.py
--rw-r--r--   0 runner    (1001) docker     (123)    30234 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/ViewportBase.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Canvas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.359844 abqpy-2023.5.1/src/abaqus/Connector/
--rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/CDCTerm.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/CDCTermArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorBehaviorOption.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorBehaviorOptionArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    20054 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorDamage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorDamping.py
--rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorElasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorFailure.py
--rw-r--r--   0 runner    (1001) docker     (123)    17056 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorFriction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorLock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorPlasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorPotential.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorPotentialArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    39337 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/ConnectorStop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/DerivedComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/TangentialBehavior.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.359844 abqpy-2023.5.1/src/abaqus/Constraint/
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/AdjustPoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/ConstraintModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/Coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/DisplayBody.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/EmbeddedRegion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/Equation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/MultipointConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/RigidBody.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/ShellSolidCoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/Tie.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Constraint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.363844 abqpy-2023.5.1/src/abaqus/CustomKernel/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/CustomKernel/CommandRegister.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/CustomKernel/RegisteredDictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/CustomKernel/RegisteredList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/CustomKernel/RegisteredTuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/CustomKernel/RepositorySupport.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/CustomKernel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.363844 abqpy-2023.5.1/src/abaqus/Datum/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Datum/Datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Datum/DatumAxis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Datum/DatumCsys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Datum/DatumPlane.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Datum/DatumPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Datum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.367845 abqpy-2023.5.1/src/abaqus/DisplayGroup/
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/DisplayGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/DisplayGroupArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/DisplayGroupInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/DisplayGroupInstanceRepository.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/DisplayGroupSession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/Leaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromConstraintNames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromDatums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromDisplayGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromElementLabels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromElementSets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromElementVarRange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromGeometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromInstanceElementLabels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromInstanceNodeLabels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromMeshElementLabels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromMeshNodeLabels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromMeshSurfaceSets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromModelElemLabels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromModelNodeLabels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromNodeLabels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromNodeSets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromNodeVarRange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbEdgePick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementLayups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementMaterials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementPick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementPlies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementSections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbNodePick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromPartElementLabels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromPartInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromPartNodeLabels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromReferencePoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromSets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromSurfaceSets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromSurfaceVarRange.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayGroup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.371845 abqpy-2023.5.1/src/abaqus/DisplayOptions/
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/AssemblyDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/BCDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/ConstraintDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/EngineeringFeatureDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/GeometricRestrictionDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/GeometryDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/GraphicsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    35297 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/GraphicsOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/InteractionDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/Light.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/LightArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/LightOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/LoadDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/MeshDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/OptimizationTaskDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/PartDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/PredefinedFieldDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/StopConditionDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/SymbolDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/ViewportAnnotationOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/DisplayOptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.371845 abqpy-2023.5.1/src/abaqus/EditMesh/
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EditMesh/MeshEditAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EditMesh/MeshEditOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25450 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EditMesh/MeshEditPart.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EditMesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.375846 abqpy-2023.5.1/src/abaqus/EngineeringFeature/
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/AssembledFastener.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/ContourIntegral.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/Crack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/DataImperfection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/DebondVCCT.py
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/DiscreteFastener.py
--rw-r--r--   0 runner    (1001) docker     (123)    44363 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/EngineeringFeature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/EngineeringFeatureBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/Fastener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/FileImperfection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/HeatCapacitance.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/Imperfection.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/Inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/InputImperfection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/NonstructuralMass.py
--rw-r--r--   0 runner    (1001) docker     (123)    23813 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/PointFastener.py
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/PointMassInertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/SpringDashpot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/SpringDashpotToGround.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/TwoPointSpringDashpot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/XFEMCrack.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/EngineeringFeature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.375846 abqpy-2023.5.1/src/abaqus/Feature/
--rw-r--r--   0 runner    (1001) docker     (123)    80578 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Feature/Feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Feature/FeatureOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Feature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.375846 abqpy-2023.5.1/src/abaqus/Field/
--rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Field/AnalyticalField.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Field/DataTable.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Field/DataTableArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Field/DiscreteField.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Field/ExpressionField.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Field/Field.py
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Field/FieldModel.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Field/FieldOdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Field/MappedField.py
--rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Field/OdbMeshRegionData.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Field/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.379846 abqpy-2023.5.1/src/abaqus/FieldReport/
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/FieldReport/FieldReportOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/FieldReport/FieldReportSession.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/FieldReport/FreeBodyReportOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/FieldReport/OdbFieldVarList.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/FieldReport/OdbModelFieldVarList.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/FieldReport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/FieldReport/writeFieldReport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/FieldReport/writeFreeBodyReport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.379846 abqpy-2023.5.1/src/abaqus/Filter/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Filter/ButterworthFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Filter/Chebyshev1Filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Filter/Chebyshev2Filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Filter/Filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Filter/FilterModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Filter/FilterOdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Filter/OperatorFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.379846 abqpy-2023.5.1/src/abaqus/InputFileParser/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/InputFileParser/AbaqusNDarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/InputFileParser/InputFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/InputFileParser/Keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/InputFileParser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.395847 abqpy-2023.5.1/src/abaqus/Interaction/
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/AcousticImpedance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/AcousticImpedanceProp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/AcousticImpedanceState.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ActuatorSensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ActuatorSensorProp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ActuatorSensorState.py
--rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/CavityRadiation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/CavityRadiationProp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/CavityRadiationState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/CohesiveBehavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ConcentratedFilmCondition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ConcentratedFilmConditionState.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ConcentratedRadiationToAmbient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ConcentratedRadiationToAmbientState.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ContactControl.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ContactDamage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ContactDamping.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ContactExp.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ContactInitialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    35831 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ContactProperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ContactPropertyAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ContactStabilization.py
--rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ContactStd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ContactTangentialBehavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/CyclicSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/CyclicSymmetryState.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ElasticFoundation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ElasticFoundationState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ExpContactControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ExpInitialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FilmCondition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FilmConditionProp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FilmConditionState.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FluidCavity.py
--rw-r--r--   0 runner    (1001) docker     (123)    21420 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FluidCavityProperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FluidCavityState.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FluidExchange.py
--rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FluidExchangeProperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FluidExchangeState.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FluidInflator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FluidInflatorProperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FluidInflatorState.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/FractureCriterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/GapElectricalConductance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/GapHeatGeneration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/GeometricProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/IncidentWave.py
--rw-r--r--   0 runner    (1001) docker     (123)    27503 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/IncidentWaveProperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/IncidentWaveState.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/InitializationAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/Interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/InteractionContactControlModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/InteractionContactInitializationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/InteractionContactStabilizationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)   101262 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/InteractionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/InteractionProperty.py
--rw-r--r--   0 runner    (1001) docker     (123)    33997 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/InteractionPropertyModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/InteractionState.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/MainSecondaryAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ModelChange.py
--rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/NormalBehavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/PolarityAssignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/PressurePenetration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/PressurePenetrationState.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/Radiation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/RadiationToAmbient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/RadiationToAmbientState.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/RegionPairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SelfContactExp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SelfContactExpState.py
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SelfContactStd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SelfContactStdState.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SlidingFormulationAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SlidingTransitionAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SmoothingAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/StabilizationAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    20726 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/StdContactControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/StdInitialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/StdStabilization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/StdXplCosimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/StdXplCosimulationState.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SurfaceBeamSmoothingAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SurfaceCrushTriggerAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SurfaceFeatureAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SurfaceFrictionAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SurfaceOffsetAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SurfaceThicknessAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SurfaceToSurfaceContactExp.py
--rw-r--r--   0 runner    (1001) docker     (123)    27980 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SurfaceToSurfaceContactStd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SurfaceToSurfaceExpState.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SurfaceToSurfaceStdState.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/SurfaceVertexCriteriaAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/ThermalConductance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/XFEMCrackGrowth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/XFEMCrackGrowthState.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Interaction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.395847 abqpy-2023.5.1/src/abaqus/Job/
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Job/Coexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Job/Job.py
--rw-r--r--   0 runner    (1001) docker     (123)    19885 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Job/JobFromInputFile.py
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Job/JobMdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Job/JobSession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Job/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Job/MessageArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Job/ModelJob.py
--rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Job/OptimizationProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Job/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.411849 abqpy-2023.5.1/src/abaqus/Load/
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BodyCharge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BodyChargeState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BodyConcentrationFlux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BodyConcentrationFluxState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BodyCurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BodyCurrentDensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BodyCurrentState.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BodyForce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BodyForceState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BodyHeatFlux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BodyHeatFluxState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BoltLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/BoltLoadState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcCharge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcConcFlux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcCurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcCurrentState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcPoreFluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcentratedChargeState.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcentratedConcentrationFluxState.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcentratedForce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcentratedForceState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcentratedHeatFlux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcentratedHeatFluxState.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConcentratedPoreFluidState.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConnectorForce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConnectorForceState.py
--rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConnectorMoment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ConnectorMomentState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/CoriolisForce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/CoriolisForceState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/Gravity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/GravityState.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/HydrostaticFluidFlowState.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/InertiaRelief.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/InertiaReliefState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/InwardVolAccel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/InwardVolAccelState.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/LineLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/LineLoadState.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/Load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/LoadCase.py
--rw-r--r--   0 runner    (1001) docker     (123)    88930 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/LoadModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/LoadState.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/LoadStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/Moment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/MomentState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/PEGLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/PEGLoadState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/PipePressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/PipePressureState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/Pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/PressureState.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/RotationalBodyForce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/RotationalBodyForceState.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ShellEdgeLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/ShellEdgeLoadState.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SubmodelSB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SubmodelSBState.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SubstructureLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SubstructureLoadState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfaceCharge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfaceChargeState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfaceConcentrationFlux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfaceConcentrationFluxState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfaceCurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfaceCurrentDensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfaceCurrentState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfaceHeatFlux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfaceHeatFluxState.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfacePoreFluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfacePoreFluidState.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfaceTraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/SurfaceTractionState.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Load/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.411849 abqpy-2023.5.1/src/abaqus/Material/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.411849 abqpy-2023.5.1/src/abaqus/Material/Acoustic/
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Acoustic/AcousticMedium.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Acoustic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.411849 abqpy-2023.5.1/src/abaqus/Material/Density/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Density/Density.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Density/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.411849 abqpy-2023.5.1/src/abaqus/Material/Elastic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.411849 abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.411849 abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/HyperFoam/
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/HyperFoam/Hyperfoam.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/HyperFoam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/Hyperelastic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.411849 abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/CombinedTestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/Hysteresis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/Viscoelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.411849 abqpy-2023.5.1/src/abaqus/Material/Elastic/HypoElastic/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/HypoElastic/Hypoelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/HypoElastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.415849 abqpy-2023.5.1/src/abaqus/Material/Elastic/Linear/
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/Linear/Elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/Linear/FailStrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/Linear/FailStress.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/Linear/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.415849 abqpy-2023.5.1/src/abaqus/Material/Elastic/LowDensityFoam/
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/LowDensityFoam/LowDensityFoam.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/LowDensityFoam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.415849 abqpy-2023.5.1/src/abaqus/Material/Elastic/Porous/
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/Porous/PorousElastic.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/Porous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.415849 abqpy-2023.5.1/src/abaqus/Material/Elastic/SuperElastic/
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/SuperElastic/SuperElasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/SuperElastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Elastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.415849 abqpy-2023.5.1/src/abaqus/Material/Electromagnetic/
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Electromagnetic/Dielectric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Electromagnetic/ElectricalConductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Electromagnetic/MagneticPermeability.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Electromagnetic/Piezoelectric.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Electromagnetic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.415849 abqpy-2023.5.1/src/abaqus/Material/Eos/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Eos/DetonationPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Eos/Eos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Eos/EosCompaction.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.415849 abqpy-2023.5.1/src/abaqus/Material/Gap/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Gap/GapConductance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Gap/GapConvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Gap/GapFlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Gap/GapRadiation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Gap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.419849 abqpy-2023.5.1/src/abaqus/Material/Gasket/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Gasket/ContactArea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Gasket/GasketMembraneElastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Gasket/GasketThicknessBehavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Gasket/GasketTransverseShearElastic.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Gasket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.419849 abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/Conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/HeatGeneration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/InelasticHeatFraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/JouleHeatFraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/LatentHeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/SpecificHeat.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.419849 abqpy-2023.5.1/src/abaqus/Material/MassDiffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/MassDiffusion/Diffusivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/MassDiffusion/PressureEffect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/MassDiffusion/Solubility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/MassDiffusion/SoretEffect.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/MassDiffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   154625 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Material.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/MaterialBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/MaterialModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/MaterialOdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.419849 abqpy-2023.5.1/src/abaqus/Material/Mechanical/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Mechanical/Damping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Mechanical/Expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Mechanical/PoreFluidExpansion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.419849 abqpy-2023.5.1/src/abaqus/Material/Mechanical/Viscosity/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Mechanical/Viscosity/Trs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Mechanical/Viscosity/Viscosity.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Mechanical/Viscosity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Mechanical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.423850 abqpy-2023.5.1/src/abaqus/Material/Multiscale/
--rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Multiscale/MeanFieldHomogenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Multiscale/MeanFieldInclusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Multiscale/MeanFieldMatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Multiscale/MeanFieldVoid.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Multiscale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.423850 abqpy-2023.5.1/src/abaqus/Material/Plastic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.423850 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/BrittleCracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/BrittleFailure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/BrittleShear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/Concrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ConcreteCompressionDamage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ConcreteCompressionHardening.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ConcreteDamagedPlasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ConcreteTensionDamage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ConcreteTensionStiffening.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/FailureRatios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ShearRetention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/TensionStiffening.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.423850 abqpy-2023.5.1/src/abaqus/Material/Plastic/Creep/
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Creep/Creep.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Creep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.423850 abqpy-2023.5.1/src/abaqus/Material/Plastic/CriticalStateClay/
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/CriticalStateClay/ClayHardening.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/CriticalStateClay/ClayPlasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/CriticalStateClay/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.427850 abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushStress/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushStress/CrushStress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushStress/CrushStressVelocityFactor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushStress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.427850 abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushableFoam/
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushableFoam/CrushableFoam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushableFoam/CrushableFoamHardening.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushableFoam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.427850 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.427850 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/Extended/
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPrager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPragerCreep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPragerHardening.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/Extended/TriaxialTestData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/Extended/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.427850 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapCreepCohesion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapCreepConsolidation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapHardening.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapPlasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.427850 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.427850 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Annealing/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Annealing/AnnealTemperature.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Annealing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.431850 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/CastIron/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/CastIron/CastIronCompressionHardening.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/CastIron/CastIronPlasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/CastIron/CastIronTensionHardening.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/CastIron/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.431850 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Cyclic/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Cyclic/CycledPlastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Cyclic/CyclicHardening.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Cyclic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.431850 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Deformation/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Deformation/DeformationPlasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Deformation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.431850 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/ORNL/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/ORNL/Ornl.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/ORNL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.431850 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Porous/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Porous/PorousFailureCriteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Porous/PorousMetalPlasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Porous/VoidNucleation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Porous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.431850 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/RateDependent/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/RateDependent/RateDependent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/RateDependent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.431850 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/TwoLayerViscoPlasticity/
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/TwoLayerViscoPlasticity/Viscous.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/TwoLayerViscoPlasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.431850 abqpy-2023.5.1/src/abaqus/Material/Plastic/MohrCoulomb/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/MohrCoulomb/MohrCoulombHardening.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/MohrCoulomb/MohrCoulombPlasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/MohrCoulomb/TensionCutOff.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/MohrCoulomb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Plastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/PlasticityCorrection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Potential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.435851 abqpy-2023.5.1/src/abaqus/Material/Plastic/SuperElastic/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/SuperElastic/SuperElasticHardening.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/SuperElastic/SuperElasticHardeningModifications.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/SuperElastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.435851 abqpy-2023.5.1/src/abaqus/Material/Plastic/Swelling/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Swelling/Swelling.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/Swelling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/TensileFailure.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Plastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.435851 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/FluidLeakoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Gel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.435851 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/MoistureSwelling/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/MoistureSwelling/MoistureSwelling.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/MoistureSwelling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.435851 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Permeability/
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Permeability/Permeability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Permeability/SaturationDependence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Permeability/VelocityDependence.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Permeability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/PorousBulkModuli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Sorption.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.435851 abqpy-2023.5.1/src/abaqus/Material/ProgressiveDamageFailure/
--rw-r--r--   0 runner    (1001) docker     (123)    14495 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/ProgressiveDamageFailure/DamageEvolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    76301 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/ProgressiveDamageFailure/DamageInitiation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/ProgressiveDamageFailure/DamageStabilization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/ProgressiveDamageFailure/DamageStabilizationCohesive.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/ProgressiveDamageFailure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Ratios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/Regularization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.439851 abqpy-2023.5.1/src/abaqus/Material/TestData/
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/TestData/BiaxialTestData.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/TestData/BiaxialTestDataArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/TestData/MullinsEffect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/TestData/PlanarTestData.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/TestData/PlanarTestDataArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/TestData/ShearTestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/TestData/SimpleShearTestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/TestData/UniaxialTestData.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/TestData/UniaxialTestDataArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/TestData/VolumetricTestData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/TestData/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.439851 abqpy-2023.5.1/src/abaqus/Material/User/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/User/Depvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/User/UserDefinedField.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/User/UserMaterial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/User/UserOutputVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/User/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Material/evaluateMaterial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.439851 abqpy-2023.5.1/src/abaqus/Mdb/
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mdb/Mdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mdb/MdbBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mdb/MdbCommands.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.443851 abqpy-2023.5.1/src/abaqus/Mesh/
--rw-r--r--   0 runner    (1001) docker     (123)    18075 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/ElemType.py
--rw-r--r--   0 runner    (1001) docker     (123)    54470 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MeshAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MeshEdge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MeshEdgeArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MeshElement.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MeshElementArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MeshFace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MeshFaceArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MeshNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MeshNodeArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    55851 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MeshPart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MeshStats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/MesherOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.443851 abqpy-2023.5.1/src/abaqus/Messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Messaging/DataObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Messaging/MonitorMgr.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.443851 abqpy-2023.5.1/src/abaqus/Model/
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Model/KeywordBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Model/Model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20842 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Model/ModelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.451852 abqpy-2023.5.1/src/abaqus/Odb/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/AnalyticSurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/AnalyticSurfaceSegment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/BeamOrientation.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/BeamOrientationArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/FieldBulkData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/FieldLocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/FieldLocationArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    31720 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/FieldOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/FieldValue.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/FieldValueArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/HistoryOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/HistoryPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/HistoryRegion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/JobData.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/Odb.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbAssemblyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbCommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbDatumCsys.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbFrameArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbInstanceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbLoadCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbMeshElement.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbMeshElementArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbMeshNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbMeshNodeArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbPart.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbPartBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbPretensionSection.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbPretensionSectionArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbRigidBody.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbRigidBodyArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbSequenceAnalyticSurfaceSegment.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbSession.py
--rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/OdbStepBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/RebarOrientation.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/RebarOrientationArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/ScratchOdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/SectionCategory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/SectionPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/SectionPointArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/SectorDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/UserData.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/UserDataBase.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Odb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.455852 abqpy-2023.5.1/src/abaqus/OdbDisplay/
--rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/OdbDisplay/CommonOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21285 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/OdbDisplay/ContourOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/OdbDisplay/DefaultOdbDisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/OdbDisplay/DisplayBodyOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29603 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/OdbDisplay/OdbDisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/OdbDisplay/OrientationOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/OdbDisplay/SuperimposeOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16333 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/OdbDisplay/SymbolOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/OdbDisplay/ViewCut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/OdbDisplay/ViewerOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/OdbDisplay/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.463853 abqpy-2023.5.1/src/abaqus/Optimization/
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/BeadFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/BeadFixedRegion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/BeadGrowth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/BeadPenetrationCheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/BeadPlanarSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/BeadPointSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/BeadRotationalSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/BeadTask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/CombinedTermDesignResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/DesignDirection.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/DesignResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/DrillControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/FixedRegion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/FrozenArea.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/GeometricRestriction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/Growth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/LocalStopCondition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/ObjectiveFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/OptimizationConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/OptimizationObjective.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/OptimizationObjectiveArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    85890 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/OptimizationTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/OptimizationTaskBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    36241 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/OptimizationTaskModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/PenetrationCheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/ShapeDemoldControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/ShapeMemberSize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/ShapePlanarSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/ShapePointSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/ShapeRotationalSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    36078 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/ShapeTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/SingleTermDesignResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/SizingClusterAreas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/SizingCyclicSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/SizingFrozenArea.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/SizingMemberSize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/SizingPlanarSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/SizingPointSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/SizingRotationalSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/SizingTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/SlideRegionControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/StampControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/StepOption.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/StepOptionArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/StopCondition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/TopologyCyclicSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/TopologyDemoldControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/TopologyMemberSize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/TopologyMillingControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/TopologyOverhangControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/TopologyPlanarSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/TopologyPointSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/TopologyRibDesign.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/TopologyRotationalSymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/TopologyTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/TurnControl.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.467853 abqpy-2023.5.1/src/abaqus/Part/
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Part/AcisFile.py
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Part/AcisMdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Part/Part.py
--rw-r--r--   0 runner    (1001) docker     (123)    75046 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Part/PartBase.py
--rw-r--r--   0 runner    (1001) docker     (123)   105971 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Part/PartFeature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Part/PartModel.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Part/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.467853 abqpy-2023.5.1/src/abaqus/Partition/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Partition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.467853 abqpy-2023.5.1/src/abaqus/PathAndProbe/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PathAndProbe/CurrentProbeValues.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PathAndProbe/FreeBody.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PathAndProbe/NodeQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PathAndProbe/Path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PathAndProbe/PathSession.py
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PathAndProbe/ProbeOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PathAndProbe/ProbeReport.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PathAndProbe/SelectedProbeValues.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PathAndProbe/Spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PathAndProbe/Stream.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PathAndProbe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.475854 abqpy-2023.5.1/src/abaqus/PlotOptions/
--rw-r--r--   0 runner    (1001) docker     (123)    45429 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/BasicOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/CouplingConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/DGCommonOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/DGContourOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/DGDisplayBodyOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/DGOrientationOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/DGSuperimposeOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/DGSymbolOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/DetailPlotOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/DisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/FreeBodyOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/HistoryVariable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/MdbData.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/MdbDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/MdbDataFrameArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/MdbDataInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/MdbDataStep.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/MpcConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbAnalysisError.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbAnalysisWarning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbAuxiliaryData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbContactDiagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataDatumCsys.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataElementSet.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataFrameArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataMaterial.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataNodeSet.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataSection.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataStep.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataSurfaceSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDiagnosticAttempt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDiagnosticData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDiagnosticIncrement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDiagnosticStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDisplayOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbJobTime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OdbNumericalProblemSummary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/OptionArg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/PlyStackPlotOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/RigidBodyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/StreamOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/TieConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/ViewCutOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlotOptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.475854 abqpy-2023.5.1/src/abaqus/PlugInRegistration/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PlugInRegistration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.479854 abqpy-2023.5.1/src/abaqus/PredefinedField/
--rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/Field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/FieldState.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/FluidCavityPressure.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/IMAField.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/IMARegion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/InitialState.py
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/KinematicHardening.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/MaterialAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/PorePressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/PredefinedField.py
--rw-r--r--   0 runner    (1001) docker     (123)    36889 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/PredefinedFieldModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/PredefinedFieldState.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/Saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/Stress.py
--rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/Temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/TemperatureState.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/TiffOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/Velocity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/VoidsRatio.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/PredefinedField/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.479854 abqpy-2023.5.1/src/abaqus/Print/
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Print/EpsOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Print/PageSetupOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Print/PngOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Print/PrintOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Print/PsOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Print/SvgOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Print/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.483855 abqpy-2023.5.1/src/abaqus/Property/
--rw-r--r--   0 runner    (1001) docker     (123)    29078 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/CompositeLayup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/CompositePly.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/CompositePlyArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/MaterialOrientation.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/MaterialOrientationArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/PlyStackPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/Property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/PropertyAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/PropertyPart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/SectionAssignment.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/SectionAssignmentArray.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Property/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.483855 abqpy-2023.5.1/src/abaqus/Region/
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Region/Region.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Region/RegionArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Region/RegionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Region/RegionAssemblyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Region/RegionPart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Region/RegionPartBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Region/Set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Region/Skin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Region/Stringer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Region/Surface.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Region/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.491855 abqpy-2023.5.1/src/abaqus/Section/
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/AcousticInfiniteSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/AcousticInterfaceSection.py
--rw-r--r--   0 runner    (1001) docker     (123)    20316 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/BeamSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/CohesiveSection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/CompositeShellSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/CompositeSolidSection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22390 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/ConnectorSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/EulerianSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/GasketSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/GeneralStiffnessSection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/GeometryShellSection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/HomogeneousShellSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/HomogeneousSolidSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/LayerProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/LayerPropertiesArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/MPCSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/MembraneSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/PEGSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/RebarLayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/Section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/SectionBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/SectionLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/SectionLayerArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    51672 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/SectionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    50473 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/SectionOdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/ShellSection.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/SolidSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/SurfaceSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/TransverseShearBeam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/TransverseShearShell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/TrussSection.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Section/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.491855 abqpy-2023.5.1/src/abaqus/Session/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Session/AutoColors.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Session/Color.py
--rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Session/Drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Session/Image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Session/JournalOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Session/MemoryReductionOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Session/NetworkDatabaseConnector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Session/NumberFormat.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Session/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)    25463 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Session/SessionBase.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Session/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.495856 abqpy-2023.5.1/src/abaqus/Sketcher/
--rw-r--r--   0 runner    (1001) docker     (123)    27746 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.495856 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/CoincidentConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/ConcentricConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/ConstrainedSketchConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/ConstrainedSketchConstraintModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualDistanceConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualLengthConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualRadiusConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/FixedConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/HorizontalConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/ParallelConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/PerpendicularConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/TangentConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/VerticalConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.495856 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/AngularDimension.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/ConstrainedSketchDimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/ConstrainedSketchDimensionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/DistanceDimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/HorizontalDimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/ObliqueDimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/RadialDimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/VerticalDimension.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.499856 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/Arc3Points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ArcByCenterEnds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ArcByStartEndTangent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/CircleByCenterPerimeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometryArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    12880 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometryModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstructionCircleByCenterPerimeter.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstructionLine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/EllipseByCenterPerimeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/FilletByRadius.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/Line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/Spline.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/Spot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/getPointAtDistance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.499856 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchOptions/
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketchImageOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketchOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketcherOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchOptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.499856 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchParameter/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchParameter/ConstrainedSketchParameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchParameter/ConstrainedSketchParameterModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchParameter/Parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchParameter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.499856 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchVertex/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertexArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertexModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchVertex/Spot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchVertex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/SketchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Sketcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.507857 abqpy-2023.5.1/src/abaqus/Step/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/AnalysisStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/AnnealStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/BuckleStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/ComplexFrequencyStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/CoupledTempDisplacementStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    16566 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/CoupledThermalElectricStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/CoupledThermalElectricalStructuralStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/DirectCyclicStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/EmagTimeHarmonicStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    14926 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/ExplicitDynamicsStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/FrequencyStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/GeostaticStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/HeatTransferStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/ImplicitDynamicsStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/InitialStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/MassDiffusionStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/ModalDynamicsStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/RandomResponseStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/ResponseSpectrumStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    22799 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/SoilsStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/StaticLinearPerturbationStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/StaticRiksStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    22372 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/StaticStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/SteadyStateDirectStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/SteadyStateModalStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/SteadyStateSubspaceStep.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/Step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/StepBase.py
--rw-r--r--   0 runner    (1001) docker     (123)   138090 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/StepModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/SubspaceDynamicsStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    16766 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/SubstructureGenerateStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/TempDisplacementDynamicsStep.py
--rw-r--r--   0 runner    (1001) docker     (123)    20885 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/ViscoStep.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/Step/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.511857 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/CompositeDamping.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/CompositeDampingComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/CompositeDampingComponentArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/Control.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/DirectDamping.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/DirectDampingByFrequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/DirectDampingByFrequencyComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/DirectDampingByFrequencyComponentArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/DirectDampingComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/DirectDampingComponentArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/EmagTimeHarmonicFrequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/EmagTimeHarmonicFrequencyArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/MassScaling.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/MassScalingArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RandomResponseFrequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RandomResponseFrequencyArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RayleighDamping.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RayleighDampingByFrequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RayleighDampingByFrequencyComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RayleighDampingByFrequencyComponentArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RayleighDampingComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RayleighDampingComponentArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/ResponseSpectrumComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/ResponseSpectrumComponentArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SolverControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SteadyStateDirectFrequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SteadyStateDirectFrequencyArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SteadyStateModalFrequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SteadyStateModalFrequencyArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SteadyStateSubspaceFrequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SteadyStateSubspaceFrequencyArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/StructuralDamping.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/StructuralDampingByFrequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/StructuralDampingByFrequencyComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/StructuralDampingByFrequencyComponentArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/StructuralDampingComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/StructuralDampingComponentArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SubstructureGenerateFrequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SubstructureGenerateFrequencyArray.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SubstructureGenerateModes.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SubstructureGenerateModesArray.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepMiscellaneous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.515858 abqpy-2023.5.1/src/abaqus/StepOutput/
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/DiagnosticPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/FieldOutputRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/FieldOutputRequestState.py
--rw-r--r--   0 runner    (1001) docker     (123)    17487 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/HistoryOutputRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/HistoryOutputRequestState.py
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/IntegratedOutputSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/Monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/OutputModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/OutputStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/Restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/TimePoint.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/StepOutput/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.519858 abqpy-2023.5.1/src/abaqus/TableCollection/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/ActivateElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/DataTable.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/DataTableArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/ElementProgressiveActivation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/EventSeries.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/EventSeriesData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/EventSeriesType.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/ParameterColumn.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/ParameterColumnArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/ParameterTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/PropertyTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/PropertyTableData.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/TableCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/TableCollectionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/TableCollectionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/TableCollectionStep.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TableCollection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.519858 abqpy-2023.5.1/src/abaqus/TextRepresentation/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TextRepresentation/TextReprOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TextRepresentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TextRepresentation/redentABQ.py
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/TextRepresentation/textRepr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.519858 abqpy-2023.5.1/src/abaqus/UtilityAndView/
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/AbaqusBoolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/BackwardCompatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/Callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/Customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/Delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/Method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/Repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/Status.py
--rw-r--r--   0 runner    (1001) docker     (123)    84660 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/SymbolicConstant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/Upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/User.py
--rw-r--r--   0 runner    (1001) docker     (123)    21795 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/View.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   123933 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/UtilityAndView/abaqusConstants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.523858 abqpy-2023.5.1/src/abaqus/XY/
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/Area.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/AreaStyle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/Axis.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/AxisArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/AxisData.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/Chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/DefaultChartOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/DefaultPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/Legend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/LineStyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/QuantityType.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/SymbolStyle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/TextStyle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/Title.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/XYCurve.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/XYCurveArray.py
--rw-r--r--   0 runner    (1001) docker     (123)    40433 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/XYData.py
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/XYPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/XYPlotBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/XYReportOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    46541 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/XYSession.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/XYSessionBase.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/XY/writeXYReport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/_OptionsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqus/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abaqusConstants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.527859 abqpy-2023.5.1/src/abqpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abqpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abqpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-13 13:06:47.000000 abqpy-2023.5.1/src/abqpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abqpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abqpy/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/abqpy/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.527859 abqpy-2023.5.1/src/abqpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-13 13:06:47.000000 abqpy-2023.5.1/src/abqpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    63906 2023-05-13 13:06:48.000000 abqpy-2023.5.1/src/abqpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:06:47.000000 abqpy-2023.5.1/src/abqpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-13 13:06:47.000000 abqpy-2023.5.1/src/abqpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-13 13:06:47.000000 abqpy-2023.5.1/src/abqpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-13 13:06:47.000000 abqpy-2023.5.1/src/abqpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/annotationToolset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/caeModules.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/caePrefsAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/connectorBehavior.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/customKernel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/deleteObjectCallback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/displayGroupMdbToolset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/displayGroupOdbToolset.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/driverUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/field.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/inpParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/material.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/meshEdit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/methodCallback.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/monitorManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/odbAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/odbConnectorBehavior.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/odbMaterial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/odbSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/part.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/redentABQ.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/regionToolset.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/section.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/sketch.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/symbolicConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/textRepr.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/upgradeScript.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    28760 2023-05-13 13:06:35.000000 abqpy-2023.5.1/src/xyPlot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:06:48.527859 abqpy-2023.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-13 13:06:35.000000 abqpy-2023.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-13 13:06:35.000000 abqpy-2023.5.1/tests/test_mdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-13 13:06:35.000000 abqpy-2023.5.1/tests/test_odb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.530050 abqpy-2023.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.154047 abqpy-2023.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.154047 abqpy-2023.5.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/keylabeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/release-drafter-2016.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/release-drafter-2017.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/release-drafter-2018.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/release-drafter-2019.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/release-drafter-2020.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/release-drafter-2021.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/release-drafter-2022.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/release-drafter-2023.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.158047 abqpy-2023.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/workflows/changes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/workflows/conflicts.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/workflows/rtd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.github/workflows/translations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-24 15:24:03.000000 abqpy-2023.5.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 15:24:03.000000 abqpy-2023.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-24 15:24:23.530050 abqpy-2023.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-24 15:24:03.000000 abqpy-2023.5.2/README-zh-cn.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-24 15:24:03.000000 abqpy-2023.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.158047 abqpy-2023.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.158047 abqpy-2023.5.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    60200 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/CHANGES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.158047 abqpy-2023.5.2/docs/source/_autoapi_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/_autoapi_templates/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.158047 abqpy-2023.5.2/docs/source/_autoapi_templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/_autoapi_templates/python/class.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.162047 abqpy-2023.5.2/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/_ext/automembers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/_ext/changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/_ext/classdocumenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/_ext/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.162047 abqpy-2023.5.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/_static/3ds-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/_static/PyPI_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/_static/rtd-logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/_static/rtd-logo-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/envvars.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.178048 abqpy-2023.5.2/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/acl-all-schematic-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/afxI_commandLine.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/afxI_messageArea.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-abstract-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-aexample-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-cae.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-exception-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-model-assembly-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-model-model-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-model-odb-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-model-overview-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-model-part-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-model-session-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10845 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-model-viewport-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-table-editor-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-int-unix-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-odb-api-acousticviz.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-pde-debugger-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-pde-filemenu-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-pde-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-pde-settingsmenu-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-righttoleft-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-skew-dim.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/cmd-super.png
+-rw-r--r--   0 runner    (1001) docker     (123)   144708 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/compression.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/exxskew-quadmesh-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/gst-beam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/ico_guiCli.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33118 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/job_monitor.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2734175 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/model-code.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    63477 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/model-code.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61111 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/model.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/odb-field-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/odb-history-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/odb-model-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/odb-overview-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2534245 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/output-code.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    53417 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/output-code.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32580 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/output.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/utl-getinput-default-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/utl-getinput-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/utl-getinputs-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/images/utl-getwarningreply-nls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/localization.md
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/policy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.178048 abqpy-2023.5.2/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.182047 abqpy-2023.5.2/docs/source/reference/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/kernel/cae_display_preferences.md
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/kernel/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/kernel/input.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/kernel/kernel.md
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/kernel/messaging.md
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/kernel/table_collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/kernel/text_representation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/kernel/utility.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.182047 abqpy-2023.5.2/docs/source/reference/mdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/annotation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/edit_mesh.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/job.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.186047 abqpy-2023.5.2/docs/source/reference/mdb/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/adaptivity.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/amplitude.md
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/bc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/calibration.md
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/constraint.md
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/field.md
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/filter.md
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/interaction.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/load.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/material.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/mesh.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/optimization.md
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/output.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.186047 abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/assembly.md
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/datum.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/engineering.md
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/geometry.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/part.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/region.md
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/predefined.md
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/profile.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/property.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.190048 abqpy-2023.5.2/docs/source/reference/mdb/model/section/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/section/connector.md
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/section/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/sketcher.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.190048 abqpy-2023.5.2/docs/source/reference/mdb/model/step/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/step/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/mdb/model/step/step_miscellaneous.md
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/odb.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.190048 abqpy-2023.5.2/docs/source/reference/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/session/animation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/session/canvas.md
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/session/display.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/session/display_options.md
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/session/field_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/session/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/session/odb_display.md
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/session/path.md
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/session/plot_options.md
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/session/print.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/reference/session/xy.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/tutorials.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.190048 abqpy-2023.5.2/docs/source/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.190048 abqpy-2023.5.2/docs/source/user/about/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.194048 abqpy-2023.5.2/docs/source/user/about/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/about/examples/create-part.md
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/about/examples/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/about/examples/read-output.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/about/examples/summary.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/about/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/about/interact.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/about/interface.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.194048 abqpy-2023.5.2/docs/source/user/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/environment/about.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/environment/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/environment/pde-basics.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/environment/use-pde.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.194048 abqpy-2023.5.2/docs/source/user/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/examples/cantilever.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/examples/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/examples/plot.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/examples/sensitivity.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/examples/settings.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.194048 abqpy-2023.5.2/docs/source/user/output/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.198048 abqpy-2023.5.2/docs/source/user/output/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/about.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/access.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/compile-link.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/computations.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32551 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/improve-efficiency.md
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/need-what-access.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/object-model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/output-object-model.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35243 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/read.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/style.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/utility.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20430 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/cpp/write.md
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.202048 abqpy-2023.5.2/docs/source/user/output/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/python/computations.md
+-rw-r--r--   0 runner    (1001) docker     (123)    43196 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/python/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/python/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/python/execute-script.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/python/improve-efficiency.md
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/python/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/python/need-what-to-understand.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/python/object-model.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/python/output-object-model.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/python/read.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/output/python/write.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.202048 abqpy-2023.5.2/docs/source/user/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.202048 abqpy-2023.5.2/docs/source/user/python/introduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/introduction/further-reading.md
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/introduction/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/introduction/oop-basics.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/introduction/programming.md
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/introduction/python-abaqus.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18341 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/introduction/python-basics.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/introduction/python-interpreter.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/introduction/python-resources.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.206048 abqpy-2023.5.2/docs/source/user/python/python-abaqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/python-abaqus/errors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/python-abaqus/executing.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19635 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/python-abaqus/extending.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/python-abaqus/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/python-abaqus/oop.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/python-abaqus/style.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/python-abaqus/types.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.206048 abqpy-2023.5.2/docs/source/user/python/use-scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/use-scripts/environment-file.md
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/use-scripts/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/use-scripts/interact.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/use-scripts/modify-objects.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/use-scripts/namespace.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/use-scripts/object-model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/use-scripts/sequences.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/use-scripts/specify-region.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/use-scripts/specify-viewport.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/source/user/python/use-scripts/user-input.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-24 15:24:03.000000 abqpy-2023.5.2/docs/update-locale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.206048 abqpy-2023.5.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.210048 abqpy-2023.5.2/examples/Abaqus/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/Abaqus/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/Abaqus/cantilever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/Abaqus/skewExample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/Abaqus/viewerOpenOdbAndContour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/Abaqus/viewerPrintContours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.210048 abqpy-2023.5.2/examples/Compression/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/Compression/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/Compression/compression-output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/Compression/compression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.210048 abqpy-2023.5.2/examples/Parameter-Identification/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/Parameter-Identification/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/Parameter-Identification/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/Parameter-Identification/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-24 15:24:03.000000 abqpy-2023.5.2/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-24 15:24:03.000000 abqpy-2023.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.210048 abqpy-2023.5.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-24 15:24:03.000000 abqpy-2023.5.2/scripts/conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-24 15:24:03.000000 abqpy-2023.5.2/scripts/rtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-24 15:24:03.000000 abqpy-2023.5.2/scripts/rtd.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:24:23.530050 abqpy-2023.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.222048 abqpy-2023.5.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/ababltin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.222048 abqpy-2023.5.2/src/abaqus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.222048 abqpy-2023.5.2/src/abaqus/AbaqusCAEDisplayPreferences/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/AbaqusCAEDisplayPreferences/CaeGuiPrefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/AbaqusCAEDisplayPreferences/CaeKerPrefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/AbaqusCAEDisplayPreferences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/AbaqusCAEDisplayPreferences/caePrefsAccess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.226048 abqpy-2023.5.2/src/abaqus/Adaptivity/
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptiveMeshConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptiveMeshConstraintState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptiveMeshControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptiveMeshDomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptivityIteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22664 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptivityModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptivityProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptivityStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/DisplacementAdaptiveMeshConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/DisplacementAdaptiveMeshConstraintState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/ErrorIndicatorResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/RemeshingRule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/RuleResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/VelocityAdaptiveMeshConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/VelocityAdaptiveMeshConstraintState.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Adaptivity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.230048 abqpy-2023.5.2/src/abaqus/Amplitude/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/ActuatorAmplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/Amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19516 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/AmplitudeModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19562 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/AmplitudeOdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/BaselineCorrection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/Correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/DecayAmplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/EquallySpacedAmplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/ModulatedAmplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/PeriodicAmplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/PsdDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/SmoothStepAmplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/SolutionDependentAmplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/SpectrumAmplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/TabularAmplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Amplitude/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.230048 abqpy-2023.5.2/src/abaqus/Animation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Animation/AVIOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Animation/AnimationController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Animation/AnimationOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Animation/AnimationSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Animation/ImageAnimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Animation/ImageAnimationOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Animation/Movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Animation/QuickTimeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Animation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.234048 abqpy-2023.5.2/src/abaqus/Annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Annotation/AnimationUserData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Annotation/Annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Annotation/AnnotationViewport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Annotation/AnnotationsToPlotArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17272 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Annotation/Arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Annotation/Text.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Annotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.238048 abqpy-2023.5.2/src/abaqus/Assembly/
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Assembly/Assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49193 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Assembly/AssemblyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Assembly/AssemblyFeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Assembly/AssemblyModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Assembly/ConnectorOrientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Assembly/ConnectorOrientationArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Assembly/ModelInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13780 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Assembly/PartInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Assembly/PartInstanceArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Assembly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.246048 abqpy-2023.5.2/src/abaqus/BasicGeometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/BasicGeometryPart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/Cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/CellArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/Edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/EdgeArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/Face.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/FaceArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/IgnoredEdge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/IgnoredEdgeArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/IgnoredVertex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/IgnoredVertexArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/InterestingPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/ModelDot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/ModelDotArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/ReferencePoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/ReferencePointArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/ReferencePoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/Transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/Vertex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/VertexArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BasicGeometry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.250048 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/ArbitraryProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/BeamSectionProfileModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15359 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/BeamSectionProfileOdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/BoxProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/CircularProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/GeneralizedProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/HexagonalProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/IProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/LProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/PipeProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/RectangularProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/TProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/TrapezoidalProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BeamSectionProfile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.266048 abqpy-2023.5.2/src/abaqus/BoundaryCondition/
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/AccelerationBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/AccelerationBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/AccelerationBaseMotionBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/AccelerationBaseMotionBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/AcousticPressureBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/AcousticPressureBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/BoundaryCondition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93767 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/BoundaryConditionModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/BoundaryConditionState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConcentrationBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConcentrationBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnAccelerationBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnAccelerationBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnDisplacementBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnDisplacementBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnVelocityBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnVelocityBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/DisplacementBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/DisplacementBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/DisplacementBaseMotionBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/DisplacementBaseMotionBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/ElectricPotentialBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/ElectricPotentialBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/EulerianBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/EulerianBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24508 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/EulerianMotionBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/EulerianMotionBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/FluidCavityPressureBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/FluidCavityPressureBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/MagneticVectorPotentialBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/MaterialFlowBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/MaterialFlowBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/PorePressureBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/PorePressureBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/RetainedNodalDofsBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/SecondaryBaseBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/SecondaryBaseBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/SubmodelBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/SubmodelBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/TemperatureBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/TemperatureBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/TypeBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/TypeBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/VelocityBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/VelocityBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/VelocityBaseMotionBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/VelocityBaseMotionBCState.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/BoundaryCondition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.266048 abqpy-2023.5.2/src/abaqus/Calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Calibration/Behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Calibration/Calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Calibration/CalibrationModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Calibration/DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Calibration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.270048 abqpy-2023.5.2/src/abaqus/Canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/AttributeColorMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/Canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/CanvasSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/Displayable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/DrawingArea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/Highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/ImageOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/Layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/MovieOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/Viewport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30234 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/ViewportBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Canvas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.274048 abqpy-2023.5.2/src/abaqus/Connector/
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/CDCTerm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/CDCTermArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorBehaviorOption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorBehaviorOptionArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20054 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorDamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorDamping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorElasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorFailure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17056 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorFriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorLock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorPlasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorPotential.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorPotentialArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39337 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/ConnectorStop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/DerivedComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/TangentialBehavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.278048 abqpy-2023.5.2/src/abaqus/Constraint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/AdjustPoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/ConstraintModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/Coupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/DisplayBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/EmbeddedRegion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/Equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/MultipointConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/RigidBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/ShellSolidCoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/Tie.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Constraint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.282048 abqpy-2023.5.2/src/abaqus/CustomKernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/CustomKernel/CommandRegister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/CustomKernel/RegisteredDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/CustomKernel/RegisteredList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/CustomKernel/RegisteredTuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/CustomKernel/RepositorySupport.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/CustomKernel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.282048 abqpy-2023.5.2/src/abaqus/Datum/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Datum/Datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Datum/DatumAxis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Datum/DatumCsys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Datum/DatumPlane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Datum/DatumPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Datum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.290048 abqpy-2023.5.2/src/abaqus/DisplayGroup/
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/DisplayGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/DisplayGroupArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/DisplayGroupInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/DisplayGroupInstanceRepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/DisplayGroupSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/Leaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromConstraintNames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromDatums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromDisplayGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromElementLabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromElementSets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromElementVarRange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromGeometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromInstanceElementLabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromInstanceNodeLabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromMeshElementLabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromMeshNodeLabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromMeshSurfaceSets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromModelElemLabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromModelNodeLabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromNodeLabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromNodeSets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromNodeVarRange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbEdgePick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementLayups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementMaterials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementPick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementPlies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementSections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbNodePick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromPartElementLabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromPartInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromPartNodeLabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromReferencePoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromSets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromSurfaceSets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromSurfaceVarRange.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayGroup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.298048 abqpy-2023.5.2/src/abaqus/DisplayOptions/
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/AssemblyDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/BCDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/ConstraintDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/EngineeringFeatureDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/GeometricRestrictionDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/GeometryDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/GraphicsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35297 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/GraphicsOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/InteractionDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/Light.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/LightArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/LightOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/LoadDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/MeshDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/OptimizationTaskDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/PartDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/PredefinedFieldDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/StopConditionDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/SymbolDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/ViewportAnnotationOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/DisplayOptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.298048 abqpy-2023.5.2/src/abaqus/EditMesh/
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EditMesh/MeshEditAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EditMesh/MeshEditOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25450 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EditMesh/MeshEditPart.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EditMesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.302049 abqpy-2023.5.2/src/abaqus/EngineeringFeature/
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/AssembledFastener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/ContourIntegral.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/Crack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/DataImperfection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/DebondVCCT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/DiscreteFastener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44363 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/EngineeringFeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/EngineeringFeatureBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/Fastener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/FileImperfection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/HeatCapacitance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/Imperfection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/Inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/InputImperfection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/NonstructuralMass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23813 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/PointFastener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/PointMassInertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/SpringDashpot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/SpringDashpotToGround.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/TwoPointSpringDashpot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/XFEMCrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/EngineeringFeature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.302049 abqpy-2023.5.2/src/abaqus/Feature/
+-rw-r--r--   0 runner    (1001) docker     (123)    80578 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Feature/Feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Feature/FeatureOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Feature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.306048 abqpy-2023.5.2/src/abaqus/Field/
+-rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Field/AnalyticalField.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Field/DataTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Field/DataTableArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Field/DiscreteField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Field/ExpressionField.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Field/Field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Field/FieldModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Field/FieldOdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Field/MappedField.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Field/OdbMeshRegionData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Field/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.306048 abqpy-2023.5.2/src/abaqus/FieldReport/
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/FieldReport/FieldReportOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/FieldReport/FieldReportSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/FieldReport/FreeBodyReportOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/FieldReport/OdbFieldVarList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/FieldReport/OdbModelFieldVarList.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/FieldReport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/FieldReport/writeFieldReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/FieldReport/writeFreeBodyReport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.310048 abqpy-2023.5.2/src/abaqus/Filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Filter/ButterworthFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Filter/Chebyshev1Filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Filter/Chebyshev2Filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Filter/Filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Filter/FilterModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Filter/FilterOdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Filter/OperatorFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.310048 abqpy-2023.5.2/src/abaqus/InputFileParser/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/InputFileParser/AbaqusNDarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/InputFileParser/InputFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/InputFileParser/Keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/InputFileParser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.334049 abqpy-2023.5.2/src/abaqus/Interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/AcousticImpedance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/AcousticImpedanceProp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/AcousticImpedanceState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ActuatorSensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ActuatorSensorProp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ActuatorSensorState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/CavityRadiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/CavityRadiationProp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/CavityRadiationState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/CohesiveBehavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ConcentratedFilmCondition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ConcentratedFilmConditionState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ConcentratedRadiationToAmbient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ConcentratedRadiationToAmbientState.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ContactControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ContactDamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ContactDamping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ContactExp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ContactInitialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35831 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ContactProperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ContactPropertyAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ContactStabilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ContactStd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ContactTangentialBehavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/CyclicSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/CyclicSymmetryState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ElasticFoundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ElasticFoundationState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ExpContactControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ExpInitialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FilmCondition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FilmConditionProp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FilmConditionState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FluidCavity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21420 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FluidCavityProperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FluidCavityState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FluidExchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FluidExchangeProperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FluidExchangeState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FluidInflator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FluidInflatorProperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FluidInflatorState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/FractureCriterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/GapElectricalConductance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/GapHeatGeneration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/GeometricProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/IncidentWave.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27503 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/IncidentWaveProperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/IncidentWaveState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/InitializationAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/Interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/InteractionContactControlModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/InteractionContactInitializationModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/InteractionContactStabilizationModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101262 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/InteractionModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/InteractionProperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33997 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/InteractionPropertyModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/InteractionState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/MainSecondaryAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ModelChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/NormalBehavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/PolarityAssignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/PressurePenetration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/PressurePenetrationState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/Radiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/RadiationToAmbient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/RadiationToAmbientState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/RegionPairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SelfContactExp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SelfContactExpState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SelfContactStd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SelfContactStdState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SlidingFormulationAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SlidingTransitionAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SmoothingAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/StabilizationAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20726 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/StdContactControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/StdInitialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/StdStabilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/StdXplCosimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/StdXplCosimulationState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SurfaceBeamSmoothingAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SurfaceCrushTriggerAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SurfaceFeatureAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SurfaceFrictionAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SurfaceOffsetAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SurfaceThicknessAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SurfaceToSurfaceContactExp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27980 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SurfaceToSurfaceContactStd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SurfaceToSurfaceExpState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SurfaceToSurfaceStdState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/SurfaceVertexCriteriaAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/ThermalConductance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/XFEMCrackGrowth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/XFEMCrackGrowthState.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Interaction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.338049 abqpy-2023.5.2/src/abaqus/Job/
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Job/Coexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Job/Job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19885 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Job/JobFromInputFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Job/JobMdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Job/JobSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Job/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Job/MessageArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Job/ModelJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Job/OptimizationProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Job/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.354049 abqpy-2023.5.2/src/abaqus/Load/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BodyCharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BodyChargeState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BodyConcentrationFlux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BodyConcentrationFluxState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BodyCurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BodyCurrentDensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BodyCurrentState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BodyForce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BodyForceState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BodyHeatFlux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BodyHeatFluxState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BoltLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/BoltLoadState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcCharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcConcFlux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcCurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcCurrentState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcPoreFluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcentratedChargeState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcentratedConcentrationFluxState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcentratedForce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcentratedForceState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcentratedHeatFlux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcentratedHeatFluxState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConcentratedPoreFluidState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConnectorForce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConnectorForceState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConnectorMoment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ConnectorMomentState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/CoriolisForce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/CoriolisForceState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/Gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/GravityState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/HydrostaticFluidFlowState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/InertiaRelief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/InertiaReliefState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/InwardVolAccel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/InwardVolAccelState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/LineLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/LineLoadState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/Load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/LoadCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88930 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/LoadModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/LoadState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/LoadStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/Moment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/MomentState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/PEGLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/PEGLoadState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/PipePressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/PipePressureState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/Pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/PressureState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/RotationalBodyForce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/RotationalBodyForceState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ShellEdgeLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/ShellEdgeLoadState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SubmodelSB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SubmodelSBState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SubstructureLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SubstructureLoadState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfaceCharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfaceChargeState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfaceConcentrationFlux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfaceConcentrationFluxState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfaceCurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfaceCurrentDensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfaceCurrentState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfaceHeatFlux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfaceHeatFluxState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfacePoreFluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfacePoreFluidState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfaceTraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/SurfaceTractionState.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Load/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.358049 abqpy-2023.5.2/src/abaqus/Material/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.358049 abqpy-2023.5.2/src/abaqus/Material/Acoustic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Acoustic/AcousticMedium.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Acoustic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.358049 abqpy-2023.5.2/src/abaqus/Material/Density/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Density/Density.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Density/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.358049 abqpy-2023.5.2/src/abaqus/Material/Elastic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.358049 abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.358049 abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/HyperFoam/
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/HyperFoam/Hyperfoam.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/HyperFoam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/Hyperelastic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.362049 abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/CombinedTestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/Hysteresis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/Viscoelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.362049 abqpy-2023.5.2/src/abaqus/Material/Elastic/HypoElastic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/HypoElastic/Hypoelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/HypoElastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.362049 abqpy-2023.5.2/src/abaqus/Material/Elastic/Linear/
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/Linear/Elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/Linear/FailStrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/Linear/FailStress.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/Linear/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.362049 abqpy-2023.5.2/src/abaqus/Material/Elastic/LowDensityFoam/
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/LowDensityFoam/LowDensityFoam.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/LowDensityFoam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.362049 abqpy-2023.5.2/src/abaqus/Material/Elastic/Porous/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/Porous/PorousElastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/Porous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.362049 abqpy-2023.5.2/src/abaqus/Material/Elastic/SuperElastic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/SuperElastic/SuperElasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/SuperElastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Elastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.362049 abqpy-2023.5.2/src/abaqus/Material/Electromagnetic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Electromagnetic/Dielectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Electromagnetic/ElectricalConductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Electromagnetic/MagneticPermeability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Electromagnetic/Piezoelectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Electromagnetic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.366049 abqpy-2023.5.2/src/abaqus/Material/Eos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Eos/DetonationPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Eos/Eos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Eos/EosCompaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.366049 abqpy-2023.5.2/src/abaqus/Material/Gap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Gap/GapConductance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Gap/GapConvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Gap/GapFlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Gap/GapRadiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Gap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.366049 abqpy-2023.5.2/src/abaqus/Material/Gasket/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Gasket/ContactArea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Gasket/GasketMembraneElastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Gasket/GasketThicknessBehavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Gasket/GasketTransverseShearElastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Gasket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.370049 abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/Conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/HeatGeneration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/InelasticHeatFraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/JouleHeatFraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/LatentHeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/SpecificHeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.370049 abqpy-2023.5.2/src/abaqus/Material/MassDiffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/MassDiffusion/Diffusivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/MassDiffusion/PressureEffect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/MassDiffusion/Solubility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/MassDiffusion/SoretEffect.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/MassDiffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154625 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/MaterialBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/MaterialModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/MaterialOdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.370049 abqpy-2023.5.2/src/abaqus/Material/Mechanical/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Mechanical/Damping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Mechanical/Expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Mechanical/PoreFluidExpansion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.370049 abqpy-2023.5.2/src/abaqus/Material/Mechanical/Viscosity/
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Mechanical/Viscosity/Trs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Mechanical/Viscosity/Viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Mechanical/Viscosity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Mechanical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.374049 abqpy-2023.5.2/src/abaqus/Material/Multiscale/
+-rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Multiscale/MeanFieldHomogenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Multiscale/MeanFieldInclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Multiscale/MeanFieldMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Multiscale/MeanFieldVoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Multiscale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.374049 abqpy-2023.5.2/src/abaqus/Material/Plastic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.378049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/BrittleCracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/BrittleFailure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/BrittleShear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/Concrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ConcreteCompressionDamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ConcreteCompressionHardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ConcreteDamagedPlasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ConcreteTensionDamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ConcreteTensionStiffening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/FailureRatios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ShearRetention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/TensionStiffening.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.378049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Creep/
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Creep/Creep.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Creep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.378049 abqpy-2023.5.2/src/abaqus/Material/Plastic/CriticalStateClay/
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/CriticalStateClay/ClayHardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/CriticalStateClay/ClayPlasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/CriticalStateClay/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.382049 abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushStress/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushStress/CrushStress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushStress/CrushStressVelocityFactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushStress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.382049 abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushableFoam/
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushableFoam/CrushableFoam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushableFoam/CrushableFoamHardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushableFoam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.382049 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.382049 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/Extended/
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPrager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPragerCreep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPragerHardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/Extended/TriaxialTestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/Extended/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.382049 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapCreepCohesion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapCreepConsolidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapHardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapPlasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.382049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.386049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Annealing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Annealing/AnnealTemperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Annealing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.386049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/CastIron/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/CastIron/CastIronCompressionHardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/CastIron/CastIronPlasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/CastIron/CastIronTensionHardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/CastIron/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.386049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Cyclic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Cyclic/CycledPlastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Cyclic/CyclicHardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Cyclic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.386049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Deformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Deformation/DeformationPlasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Deformation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.386049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/ORNL/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/ORNL/Ornl.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/ORNL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.386049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Porous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Porous/PorousFailureCriteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Porous/PorousMetalPlasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Porous/VoidNucleation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Porous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.386049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/RateDependent/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/RateDependent/RateDependent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/RateDependent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.390049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/TwoLayerViscoPlasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/TwoLayerViscoPlasticity/Viscous.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/TwoLayerViscoPlasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.390049 abqpy-2023.5.2/src/abaqus/Material/Plastic/MohrCoulomb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/MohrCoulomb/MohrCoulombHardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/MohrCoulomb/MohrCoulombPlasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/MohrCoulomb/TensionCutOff.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/MohrCoulomb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Plastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/PlasticityCorrection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Potential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.390049 abqpy-2023.5.2/src/abaqus/Material/Plastic/SuperElastic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/SuperElastic/SuperElasticHardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/SuperElastic/SuperElasticHardeningModifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/SuperElastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.390049 abqpy-2023.5.2/src/abaqus/Material/Plastic/Swelling/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Swelling/Swelling.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/Swelling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/TensileFailure.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Plastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.390049 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/FluidLeakoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Gel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.390049 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/MoistureSwelling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/MoistureSwelling/MoistureSwelling.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/MoistureSwelling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.394049 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Permeability/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Permeability/Permeability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Permeability/SaturationDependence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Permeability/VelocityDependence.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Permeability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/PorousBulkModuli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Sorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.394049 abqpy-2023.5.2/src/abaqus/Material/ProgressiveDamageFailure/
+-rw-r--r--   0 runner    (1001) docker     (123)    14495 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/ProgressiveDamageFailure/DamageEvolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76301 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/ProgressiveDamageFailure/DamageInitiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/ProgressiveDamageFailure/DamageStabilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/ProgressiveDamageFailure/DamageStabilizationCohesive.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/ProgressiveDamageFailure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Ratios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/Regularization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.398049 abqpy-2023.5.2/src/abaqus/Material/TestData/
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/TestData/BiaxialTestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/TestData/BiaxialTestDataArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/TestData/MullinsEffect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/TestData/PlanarTestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/TestData/PlanarTestDataArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/TestData/ShearTestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/TestData/SimpleShearTestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/TestData/UniaxialTestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/TestData/UniaxialTestDataArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/TestData/VolumetricTestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/TestData/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.398049 abqpy-2023.5.2/src/abaqus/Material/User/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/User/Depvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/User/UserDefinedField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/User/UserMaterial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/User/UserOutputVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/User/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Material/evaluateMaterial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.398049 abqpy-2023.5.2/src/abaqus/Mdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mdb/Mdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mdb/MdbBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mdb/MdbCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.402049 abqpy-2023.5.2/src/abaqus/Mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)    18075 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/ElemType.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54470 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MeshAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MeshEdge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MeshEdgeArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MeshElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MeshElementArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MeshFace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MeshFaceArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MeshNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MeshNodeArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55851 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MeshPart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MeshStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/MesherOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.402049 abqpy-2023.5.2/src/abaqus/Messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Messaging/DataObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Messaging/MonitorMgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.402049 abqpy-2023.5.2/src/abaqus/Model/
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Model/KeywordBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Model/Model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20842 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Model/ModelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.418049 abqpy-2023.5.2/src/abaqus/Odb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/AnalyticSurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/AnalyticSurfaceSegment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/BeamOrientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/BeamOrientationArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/FieldBulkData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/FieldLocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/FieldLocationArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31720 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/FieldOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/FieldValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/FieldValueArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/HistoryOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/HistoryPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/HistoryRegion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/JobData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/Odb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbAssemblyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbDatumCsys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbFrameArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbInstanceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbLoadCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbMeshElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbMeshElementArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbMeshNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbMeshNodeArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbPart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbPartBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbPretensionSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbPretensionSectionArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbRigidBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbRigidBodyArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbSequenceAnalyticSurfaceSegment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/OdbStepBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/RebarOrientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/RebarOrientationArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/ScratchOdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/SectionCategory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/SectionPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/SectionPointArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/SectorDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/UserData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/UserDataBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Odb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.418049 abqpy-2023.5.2/src/abaqus/OdbDisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/OdbDisplay/CommonOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21285 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/OdbDisplay/ContourOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/OdbDisplay/DefaultOdbDisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/OdbDisplay/DisplayBodyOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29603 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/OdbDisplay/OdbDisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/OdbDisplay/OrientationOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/OdbDisplay/SuperimposeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16333 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/OdbDisplay/SymbolOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/OdbDisplay/ViewCut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/OdbDisplay/ViewerOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/OdbDisplay/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.434049 abqpy-2023.5.2/src/abaqus/Optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/BeadFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/BeadFixedRegion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/BeadGrowth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/BeadPenetrationCheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/BeadPlanarSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/BeadPointSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/BeadRotationalSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/BeadTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/CombinedTermDesignResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/DesignDirection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/DesignResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/DrillControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/FixedRegion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/FrozenArea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/GeometricRestriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/Growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/LocalStopCondition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/ObjectiveFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/OptimizationConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/OptimizationObjective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/OptimizationObjectiveArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85890 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/OptimizationTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/OptimizationTaskBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36241 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/OptimizationTaskModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/PenetrationCheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/ShapeDemoldControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/ShapeMemberSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/ShapePlanarSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/ShapePointSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/ShapeRotationalSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36078 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/ShapeTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/SingleTermDesignResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/SizingClusterAreas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/SizingCyclicSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/SizingFrozenArea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/SizingMemberSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/SizingPlanarSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/SizingPointSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/SizingRotationalSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/SizingTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/SlideRegionControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/StampControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/StepOption.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/StepOptionArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/StopCondition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/TopologyCyclicSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/TopologyDemoldControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/TopologyMemberSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/TopologyMillingControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/TopologyOverhangControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/TopologyPlanarSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/TopologyPointSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/TopologyRibDesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/TopologyRotationalSymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/TopologyTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/TurnControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.434049 abqpy-2023.5.2/src/abaqus/Part/
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Part/AcisFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Part/AcisMdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Part/Part.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75046 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Part/PartBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105971 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Part/PartFeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Part/PartModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Part/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.434049 abqpy-2023.5.2/src/abaqus/Partition/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Partition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.438050 abqpy-2023.5.2/src/abaqus/PathAndProbe/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PathAndProbe/CurrentProbeValues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PathAndProbe/FreeBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PathAndProbe/NodeQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PathAndProbe/Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PathAndProbe/PathSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PathAndProbe/ProbeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PathAndProbe/ProbeReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PathAndProbe/SelectedProbeValues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PathAndProbe/Spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PathAndProbe/Stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PathAndProbe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.450050 abqpy-2023.5.2/src/abaqus/PlotOptions/
+-rw-r--r--   0 runner    (1001) docker     (123)    45429 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/BasicOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/CouplingConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/DGCommonOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/DGContourOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/DGDisplayBodyOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/DGOrientationOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/DGSuperimposeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/DGSymbolOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/DetailPlotOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/DisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/FreeBodyOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/HistoryVariable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/MdbData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/MdbDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/MdbDataFrameArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/MdbDataInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/MdbDataStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/MpcConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbAnalysisError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbAnalysisWarning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbAuxiliaryData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbContactDiagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataDatumCsys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataElementSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataFrameArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataMaterial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataNodeSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataSurfaceSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDiagnosticAttempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDiagnosticData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDiagnosticIncrement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDiagnosticStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDisplayOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbJobTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OdbNumericalProblemSummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/OptionArg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/PlyStackPlotOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/RigidBodyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/StreamOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/TieConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/ViewCutOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlotOptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.454050 abqpy-2023.5.2/src/abaqus/PlugInRegistration/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PlugInRegistration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.458050 abqpy-2023.5.2/src/abaqus/PredefinedField/
+-rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/Field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/FieldState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/FluidCavityPressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/IMAField.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/IMARegion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/InitialState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/KinematicHardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/MaterialAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/PorePressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/PredefinedField.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36889 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/PredefinedFieldModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/PredefinedFieldState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/Saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/Stress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/Temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/TemperatureState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/TiffOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/Velocity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/VoidsRatio.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/PredefinedField/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.462050 abqpy-2023.5.2/src/abaqus/Print/
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Print/EpsOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Print/PageSetupOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Print/PngOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Print/PrintOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Print/PsOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Print/SvgOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Print/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.466050 abqpy-2023.5.2/src/abaqus/Property/
+-rw-r--r--   0 runner    (1001) docker     (123)    29078 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/CompositeLayup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/CompositePly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/CompositePlyArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/MaterialOrientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/MaterialOrientationArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/PlyStackPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/Property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/PropertyAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/PropertyPart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/SectionAssignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/SectionAssignmentArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Property/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.466050 abqpy-2023.5.2/src/abaqus/Region/
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Region/Region.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Region/RegionArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Region/RegionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Region/RegionAssemblyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Region/RegionPart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Region/RegionPartBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Region/Set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Region/Skin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Region/Stringer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Region/Surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Region/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.478050 abqpy-2023.5.2/src/abaqus/Section/
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/AcousticInfiniteSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/AcousticInterfaceSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20316 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/BeamSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/CohesiveSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/CompositeShellSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/CompositeSolidSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22390 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/ConnectorSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/EulerianSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/GasketSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/GeneralStiffnessSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/GeometryShellSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/HomogeneousShellSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/HomogeneousSolidSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/LayerProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/LayerPropertiesArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/MPCSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/MembraneSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/PEGSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/RebarLayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/Section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/SectionBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/SectionLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/SectionLayerArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51672 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/SectionModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50473 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/SectionOdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/ShellSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/SolidSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/SurfaceSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/TransverseShearBeam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/TransverseShearShell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/TrussSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Section/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.482050 abqpy-2023.5.2/src/abaqus/Session/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Session/AutoColors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Session/Color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Session/Drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Session/Image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Session/JournalOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Session/MemoryReductionOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Session/NetworkDatabaseConnector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Session/NumberFormat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Session/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25463 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Session/SessionBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Session/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.482050 abqpy-2023.5.2/src/abaqus/Sketcher/
+-rw-r--r--   0 runner    (1001) docker     (123)    27746 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.486050 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/CoincidentConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/ConcentricConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/ConstrainedSketchConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/ConstrainedSketchConstraintModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualDistanceConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualLengthConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualRadiusConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/FixedConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/HorizontalConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/ParallelConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/PerpendicularConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/TangentConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/VerticalConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.486050 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/AngularDimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/ConstrainedSketchDimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/ConstrainedSketchDimensionModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/DistanceDimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/HorizontalDimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/ObliqueDimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/RadialDimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/VerticalDimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.494050 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/Arc3Points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ArcByCenterEnds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ArcByStartEndTangent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/CircleByCenterPerimeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometryArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12880 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometryModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstructionCircleByCenterPerimeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstructionLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/EllipseByCenterPerimeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/FilletByRadius.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/Line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/Spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/Spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/getPointAtDistance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.494050 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchOptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketchImageOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketchOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketcherOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchOptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.494050 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchParameter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchParameter/ConstrainedSketchParameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchParameter/ConstrainedSketchParameterModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchParameter/Parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchParameter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.494050 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchVertex/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertexArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertexModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchVertex/Spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchVertex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/SketchModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Sketcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.502050 abqpy-2023.5.2/src/abaqus/Step/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/AnalysisStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/AnnealStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/BuckleStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/ComplexFrequencyStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/CoupledTempDisplacementStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16566 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/CoupledThermalElectricStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/CoupledThermalElectricalStructuralStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/DirectCyclicStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/EmagTimeHarmonicStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14926 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/ExplicitDynamicsStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/FrequencyStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/GeostaticStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/HeatTransferStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/ImplicitDynamicsStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/InitialStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/MassDiffusionStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/ModalDynamicsStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/RandomResponseStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/ResponseSpectrumStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22799 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/SoilsStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/StaticLinearPerturbationStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/StaticRiksStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22372 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/StaticStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/SteadyStateDirectStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/SteadyStateModalStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/SteadyStateSubspaceStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/Step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/StepBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138090 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/StepModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/SubspaceDynamicsStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16766 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/SubstructureGenerateStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/TempDisplacementDynamicsStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20885 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/ViscoStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/Step/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.510050 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/CompositeDamping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/CompositeDampingComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/CompositeDampingComponentArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/Control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/DirectDamping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/DirectDampingByFrequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/DirectDampingByFrequencyComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/DirectDampingByFrequencyComponentArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/DirectDampingComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/DirectDampingComponentArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/EmagTimeHarmonicFrequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/EmagTimeHarmonicFrequencyArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/MassScaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/MassScalingArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RandomResponseFrequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RandomResponseFrequencyArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RayleighDamping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RayleighDampingByFrequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RayleighDampingByFrequencyComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RayleighDampingByFrequencyComponentArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RayleighDampingComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RayleighDampingComponentArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/ResponseSpectrumComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/ResponseSpectrumComponentArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SolverControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SteadyStateDirectFrequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SteadyStateDirectFrequencyArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SteadyStateModalFrequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SteadyStateModalFrequencyArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SteadyStateSubspaceFrequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SteadyStateSubspaceFrequencyArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/StructuralDamping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/StructuralDampingByFrequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/StructuralDampingByFrequencyComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/StructuralDampingByFrequencyComponentArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/StructuralDampingComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/StructuralDampingComponentArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SubstructureGenerateFrequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SubstructureGenerateFrequencyArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SubstructureGenerateModes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SubstructureGenerateModesArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepMiscellaneous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.514050 abqpy-2023.5.2/src/abaqus/StepOutput/
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/DiagnosticPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/FieldOutputRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/FieldOutputRequestState.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17487 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/HistoryOutputRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/HistoryOutputRequestState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/IntegratedOutputSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/OutputModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/OutputStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/Restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/TimePoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/StepOutput/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.518050 abqpy-2023.5.2/src/abaqus/TableCollection/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/ActivateElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/DataTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/DataTableArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/ElementProgressiveActivation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/EventSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/EventSeriesData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/EventSeriesType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/ParameterColumn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/ParameterColumnArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/ParameterTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/PropertyTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/PropertyTableData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/TableCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/TableCollectionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/TableCollectionModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/TableCollectionStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TableCollection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.518050 abqpy-2023.5.2/src/abaqus/TextRepresentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TextRepresentation/TextReprOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TextRepresentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TextRepresentation/redentABQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/TextRepresentation/textRepr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.522050 abqpy-2023.5.2/src/abaqus/UtilityAndView/
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/AbaqusBoolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/BackwardCompatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/Callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/Customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/Delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/Method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/Repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/Status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84660 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/SymbolicConstant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/Upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21795 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/View.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123933 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/UtilityAndView/abaqusConstants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.526050 abqpy-2023.5.2/src/abaqus/XY/
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/Area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/AreaStyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/Axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/AxisArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/AxisData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/Chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/DefaultChartOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/DefaultPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/Legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/LineStyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/QuantityType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/SymbolStyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/TextStyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/Title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/XYCurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/XYCurveArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40433 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/XYData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/XYPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/XYPlotBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/XYReportOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46541 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/XYSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/XYSessionBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/XY/writeXYReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/_OptionsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqus/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abaqusConstants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.530050 abqpy-2023.5.2/src/abqpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abqpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abqpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-24 15:24:22.000000 abqpy-2023.5.2/src/abqpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abqpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abqpy/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/abqpy/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.530050 abqpy-2023.5.2/src/abqpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-24 15:24:22.000000 abqpy-2023.5.2/src/abqpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    63794 2023-05-24 15:24:23.000000 abqpy-2023.5.2/src/abqpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:24:22.000000 abqpy-2023.5.2/src/abqpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 15:24:22.000000 abqpy-2023.5.2/src/abqpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-24 15:24:22.000000 abqpy-2023.5.2/src/abqpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 15:24:22.000000 abqpy-2023.5.2/src/abqpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/annotationToolset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/caeModules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/caePrefsAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/connectorBehavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/customKernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/deleteObjectCallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/displayGroupMdbToolset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/displayGroupOdbToolset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/driverUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/inpParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/meshEdit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/methodCallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/monitorManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/odbAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/odbConnectorBehavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/odbMaterial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/odbSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/part.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/redentABQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/regionToolset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/sketch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/symbolicConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/textRepr.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/upgradeScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28760 2023-05-24 15:24:03.000000 abqpy-2023.5.2/src/xyPlot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:24:23.530050 abqpy-2023.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-24 15:24:03.000000 abqpy-2023.5.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-24 15:24:03.000000 abqpy-2023.5.2/tests/test_mdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-24 15:24:03.000000 abqpy-2023.5.2/tests/test_odb.py
```

### Comparing `abqpy-2023.5.1/.github/CODE_OF_CONDUCT.md` & `abqpy-2023.5.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/CONTRIBUTING.md` & `abqpy-2023.5.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/ISSUE_TEMPLATE/bug_report.md` & `abqpy-2023.5.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/ISSUE_TEMPLATE/feature_request.md` & `abqpy-2023.5.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/PULL_REQUEST_TEMPLATE.md` & `abqpy-2023.5.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/dependabot.yml` & `abqpy-2023.5.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/keylabeler.yml` & `abqpy-2023.5.2/.github/keylabeler.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/mergify.yml` & `abqpy-2023.5.2/.github/mergify.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/release-drafter-2016.yml` & `abqpy-2023.5.2/.github/release-drafter-2016.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/release-drafter-2017.yml` & `abqpy-2023.5.2/.github/release-drafter-2017.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/release-drafter-2018.yml` & `abqpy-2023.5.2/.github/release-drafter-2018.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/release-drafter-2019.yml` & `abqpy-2023.5.2/.github/release-drafter-2019.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/release-drafter-2020.yml` & `abqpy-2023.5.2/.github/release-drafter-2020.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/release-drafter-2021.yml` & `abqpy-2023.5.2/.github/release-drafter-2021.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/release-drafter-2022.yml` & `abqpy-2023.5.2/.github/release-drafter-2022.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/release-drafter-2023.yml` & `abqpy-2023.5.2/.github/release-drafter-2023.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/workflows/changes.yml` & `abqpy-2023.5.2/.github/workflows/changes.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/workflows/conflicts.yml` & `abqpy-2023.5.2/.github/workflows/conflicts.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/workflows/docs.yml` & `abqpy-2023.5.2/.github/workflows/docs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 on:
   pull_request:
     branches:
     - 20**
     types: [opened, reopened, synchronize]
     paths:
     - 'src/**'
-    - 'requirements/docs.txt'
     - 'docs/source/**'
     - '.github/workflows/docs.yml'
     - 'pyproject.toml'
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
```

### Comparing `abqpy-2023.5.1/.github/workflows/release-drafter.yml` & `abqpy-2023.5.2/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/workflows/release.yml` & `abqpy-2023.5.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/workflows/rtd.yml` & `abqpy-2023.5.2/.github/workflows/rtd.yml`

 * *Files 14% similar despite different names*

```diff
@@ -29,19 +29,9 @@
       - name: Install Dependencies
         run: |
           python -m pip install --upgrade pip
           pip install fire requests
       - name: Activate Current Versions
         run: sh scripts/rtd.sh
         env:
-          MINOR_PATCH: ${{ github.event.inputs.current }}
-          ARGS: --active --nohidden
-      - name: Hide Previous Versions
-        run: sh scripts/rtd.sh
-        if: ${{ github.event.inputs.previous != '' }}
-        env:
-          MINOR_PATCH: ${{ github.event.inputs.previous }}
-          ARGS: --hidden
-      - name: Update Redirects
-        run: sh scripts/rtd.sh
-        env:
-          MINOR_PATCH: ${{ github.event.inputs.current }}
+          CURRENT_MINOR_PATCH: ${{ github.event.inputs.current }}
+          PREVIOUS_MINOR_PATCH: ${{ github.event.inputs.previous }}
```

### Comparing `abqpy-2023.5.1/.github/workflows/tests.yml` & `abqpy-2023.5.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.github/workflows/translations.yml` & `abqpy-2023.5.2/.github/workflows/translations.yml`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.gitignore` & `abqpy-2023.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/.readthedocs.yml` & `abqpy-2023.5.2/.readthedocs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 version: 2
 
 submodules:
   include: all
   recursive: true
 
 build:
-  os: ubuntu-20.04
+  os: ubuntu-22.04
   tools:
-    python: "3.10"
+    python: "3.11"
   jobs:
     # see https://github.com/readthedocs/readthedocs.org/pull/9649
     post_checkout:
       # Use `git log` to check if the latest commit contains "skip rtd",
       # in that case exit the command with 183 to skip the build
       - (git --no-pager log --pretty="tformat:%s -- %b" -1 | grep -viq "skip rtd") || exit 183
 
 sphinx:
   configuration: docs/source/conf.py
 
 formats: []
 
 python:
   install:
-    - requirements: requirements/docs.txt
     - method: pip
       path: .
+      extra_requirements:
+        - docs
```

### Comparing `abqpy-2023.5.1/LICENSE` & `abqpy-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/PKG-INFO` & `abqpy-2023.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: abqpy
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Type hints for Abaqus/Python scripting
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: Homepage, https://abqpy.com
 Project-URL: GitHub, https://github.com/haiiliin/abqpy
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Bug Tracker, https://github.com/haiiliin/abqpy/issues
 Project-URL: Read the Docs, https://readthedocs.org/projects/abqpy
 Project-URL: Documentation, https://docs.abqpy.com/en/stable/
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: jupyter
 Provides-Extra: dev
-Provides-Extra: juptyer
 Provides-Extra: docs
 License-File: LICENSE
 
 # abqpy 2023
 
 [![tests](https://github.com/haiiliin/abqpy/actions/workflows/tests.yml/badge.svg)](https://github.com/haiiliin/abqpy/actions/workflows/tests.yml)
 [![rtd](https://readthedocs.org/projects/abqpy/badge/?version=latest)](https://readthedocs.org/projects/abqpy/)
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: abqpy Version: 2023.5.1 Summary: Type hints for
+Metadata-Version: 2.1 Name: abqpy Version: 2023.5.2 Summary: Type hints for
 Abaqus/Python scripting Author-email: WANG Hailin
 wang@connect.polyu.hk> Project-URL: Homepage, https://abqpy.com Project-URL:
 GitHub, https://github.com/haiiliin/abqpy Project-URL: Bug Tracker, https://
-github.com/pypa/sampleproject/issues Project-URL: Read the Docs, https://
+github.com/haiiliin/abqpy/issues Project-URL: Read the Docs, https://
 readthedocs.org/projects/abqpy Project-URL: Documentation, https://
 docs.abqpy.com/en/stable/ Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev Provides-Extra: juptyer Provides-Extra: docs
+markdown Provides-Extra: jupyter Provides-Extra: dev Provides-Extra: docs
 License-File: LICENSE # abqpy 2023 [![tests](https://github.com/haiiliin/abqpy/
 actions/workflows/tests.yml/badge.svg)](https://github.com/haiiliin/abqpy/
 actions/workflows/tests.yml) [![rtd](https://readthedocs.org/projects/abqpy/
 badge/?version=latest)](https://readthedocs.org/projects/abqpy/) [![codecov]
 (https://codecov.io/gh/haiiliin/abqpy/branch/2023/graph/badge.svg)](https://
 app.codecov.io/gh/haiiliin/abqpy/tree/2023) [![python](https://img.shields.io/
 badge/Python-3.7%2B-brightgreen)](https://www.python.org/downloads/) [![abaqus]
```

### Comparing `abqpy-2023.5.1/README-zh-cn.md` & `abqpy-2023.5.2/README-zh-cn.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/README.md` & `abqpy-2023.5.2/README.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/Makefile` & `abqpy-2023.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/README.md` & `abqpy-2023.5.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/make.bat` & `abqpy-2023.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/CHANGES.md` & `abqpy-2023.5.2/docs/source/CHANGES.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/_autoapi_templates/python/class.rst` & `abqpy-2023.5.2/docs/source/_autoapi_templates/python/class.rst`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/_ext/automembers.py` & `abqpy-2023.5.2/docs/source/_ext/automembers.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/_ext/changes.py` & `abqpy-2023.5.2/docs/source/_ext/changes.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/_ext/classdocumenter.py` & `abqpy-2023.5.2/docs/source/_ext/classdocumenter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/_ext/version.py` & `abqpy-2023.5.2/docs/source/_ext/version.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/_static/3ds-dark.svg` & `abqpy-2023.5.2/docs/source/_static/3ds-dark.svg`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/_static/PyPI_logo.svg` & `abqpy-2023.5.2/docs/source/_static/PyPI_logo.svg`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/_static/rtd-logo-dark.svg` & `abqpy-2023.5.2/docs/source/_static/rtd-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/_static/rtd-logo-light.svg` & `abqpy-2023.5.2/docs/source/_static/rtd-logo-light.svg`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/cli.md` & `abqpy-2023.5.2/docs/source/cli.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/conf.py` & `abqpy-2023.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/envvars.md` & `abqpy-2023.5.2/docs/source/envvars.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/getting_started.md` & `abqpy-2023.5.2/docs/source/getting_started.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/acl-all-schematic-nls.png` & `abqpy-2023.5.2/docs/source/images/acl-all-schematic-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/afxI_messageArea.png` & `abqpy-2023.5.2/docs/source/images/afxI_messageArea.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-abstract-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-abstract-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-aexample-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-aexample-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-cae.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-cae.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-exception-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-exception-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-model-assembly-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-model-assembly-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-model-model-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-model-model-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-model-odb-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-model-odb-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-model-overview-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-model-overview-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-model-part-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-model-part-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-model-session-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-model-session-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-model-viewport-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-model-viewport-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-table-editor-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-table-editor-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-int-unix-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-int-unix-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-odb-api-acousticviz.png` & `abqpy-2023.5.2/docs/source/images/cmd-odb-api-acousticviz.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-pde-debugger-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-pde-debugger-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-pde-filemenu-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-pde-filemenu-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-pde-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-pde-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-pde-settingsmenu-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-pde-settingsmenu-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-righttoleft-nls.png` & `abqpy-2023.5.2/docs/source/images/cmd-righttoleft-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-skew-dim.png` & `abqpy-2023.5.2/docs/source/images/cmd-skew-dim.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/cmd-super.png` & `abqpy-2023.5.2/docs/source/images/cmd-super.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/compression.png` & `abqpy-2023.5.2/docs/source/images/compression.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/exxskew-quadmesh-nls.png` & `abqpy-2023.5.2/docs/source/images/exxskew-quadmesh-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/gst-beam.png` & `abqpy-2023.5.2/docs/source/images/gst-beam.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/ico_guiCli.png` & `abqpy-2023.5.2/docs/source/images/ico_guiCli.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/job_monitor.png` & `abqpy-2023.5.2/docs/source/images/job_monitor.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/model-code.gif` & `abqpy-2023.5.2/docs/source/images/model-code.gif`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/model-code.png` & `abqpy-2023.5.2/docs/source/images/model-code.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/model.png` & `abqpy-2023.5.2/docs/source/images/model.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/odb-field-nls.png` & `abqpy-2023.5.2/docs/source/images/odb-field-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/odb-history-nls.png` & `abqpy-2023.5.2/docs/source/images/odb-history-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/odb-model-nls.png` & `abqpy-2023.5.2/docs/source/images/odb-model-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/odb-overview-nls.png` & `abqpy-2023.5.2/docs/source/images/odb-overview-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/output-code.gif` & `abqpy-2023.5.2/docs/source/images/output-code.gif`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/output-code.png` & `abqpy-2023.5.2/docs/source/images/output-code.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/output.png` & `abqpy-2023.5.2/docs/source/images/output.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/utl-getinput-default-nls.png` & `abqpy-2023.5.2/docs/source/images/utl-getinput-default-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/utl-getinput-nls.png` & `abqpy-2023.5.2/docs/source/images/utl-getinput-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/utl-getinputs-nls.png` & `abqpy-2023.5.2/docs/source/images/utl-getinputs-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/images/utl-getwarningreply-nls.png` & `abqpy-2023.5.2/docs/source/images/utl-getwarningreply-nls.png`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/index.md` & `abqpy-2023.5.2/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/localization.md` & `abqpy-2023.5.2/docs/source/localization.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Documentation Localization
 
-The documentation is localized using [Sphinx](http://www.sphinx-doc.org/en/stable/),
-and translation files are placed in the [abqpy-locale](https://github.com/haiiliin/abqpy-locale) repository.
-The translation takes place at [Crowdin](https://crowdin.com/project/abqpy-locale).
-If you would like to help translate the documentation, please visit the
+The documentation is localized using [sphinx-intl](https://github.com/sphinx-doc/sphinx-intl),
+and the translation files are placed in the [abqpy-locale](https://github.com/haiiliin/abqpy-locale) repository.
+The translation takes place at [Crowdin](https://crowdin.com/project/abqpy-locale),
+if you would like to help translate the documentation, please visit the
 [Crowdin project](https://crowdin.com/project/abqpy-locale) and sign up for an
 account. Once you have an account, you can request to join the translation team.
 
 To add a new language, please open an issue on the [GitHub repository](https://github.com/haiiliin/abqpy/issues)
-or open a pull request with the new language code added to the `docs/update-locale.sh` script.
+or open a pull request with the new language code added to the 
+[`docs/update-locale.sh`](https://github.com/haiiliin/abqpy/blob/main/docs/update-locale.sh) script.
 
 ## Comments
 
 <script
    type="text/javascript"
    src="https://utteranc.es/client.js"
    async="async"
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_k9y87mws_/tmp0jzwfg7l_TarContainer/0/109.md", line 25, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_k9y87mws_/tmp0jzwfg7l_TarContainer/0/109.md", line 25, column 0: CDATA terminal not found*

```diff
@@ -1,10 +1,12 @@
-# Documentation Localization The documentation is localized using [Sphinx]
-(http://www.sphinx-doc.org/en/stable/), and translation files are placed in the
-[abqpy-locale](https://github.com/haiiliin/abqpy-locale) repository. The
-translation takes place at [Crowdin](https://crowdin.com/project/abqpy-locale).
-If you would like to help translate the documentation, please visit the
-[Crowdin project](https://crowdin.com/project/abqpy-locale) and sign up for an
-account. Once you have an account, you can request to join the translation
-team. To add a new language, please open an issue on the [GitHub repository]
-(https://github.com/haiiliin/abqpy/issues) or open a pull request with the new
-language code added to the `docs/update-locale.sh` script. ## Comments
+# Documentation Localization The documentation is localized using [sphinx-intl]
+(https://github.com/sphinx-doc/sphinx-intl), and the translation files are
+placed in the [abqpy-locale](https://github.com/haiiliin/abqpy-locale)
+repository. The translation takes place at [Crowdin](https://crowdin.com/
+project/abqpy-locale), if you would like to help translate the documentation,
+please visit the [Crowdin project](https://crowdin.com/project/abqpy-locale)
+and sign up for an account. Once you have an account, you can request to join
+the translation team. To add a new language, please open an issue on the
+[GitHub repository](https://github.com/haiiliin/abqpy/issues) or open a pull
+request with the new language code added to the [`docs/update-locale.sh`]
+(https://github.com/haiiliin/abqpy/blob/main/docs/update-locale.sh) script. ##
+Comments
```

### Comparing `abqpy-2023.5.1/docs/source/reference/index.md` & `abqpy-2023.5.2/docs/source/reference/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/kernel/kernel.md` & `abqpy-2023.5.2/docs/source/reference/kernel/kernel.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/kernel/table_collection.md` & `abqpy-2023.5.2/docs/source/reference/kernel/table_collection.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/kernel/utility.md` & `abqpy-2023.5.2/docs/source/reference/kernel/utility.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/annotation.md` & `abqpy-2023.5.2/docs/source/reference/mdb/annotation.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/edit_mesh.md` & `abqpy-2023.5.2/docs/source/reference/mdb/edit_mesh.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/index.md` & `abqpy-2023.5.2/docs/source/reference/mdb/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/job.md` & `abqpy-2023.5.2/docs/source/reference/mdb/job.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/adaptivity.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/adaptivity.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/amplitude.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/amplitude.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/bc.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/bc.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/field.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/field.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/filter.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/filter.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/index.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/interaction.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/interaction.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/load.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/load.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/material.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/material.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/optimization.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/optimization.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/output.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/output.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/assembly.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/assembly.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/datum.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/datum.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/feature.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/feature.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/part.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/part.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/part_assembly/region.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/part_assembly/region.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/predefined.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/predefined.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/profile.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/profile.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/property.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/property.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/section/index.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/section/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/sketcher.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/sketcher.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/mdb/model/step/index.md` & `abqpy-2023.5.2/docs/source/reference/mdb/model/step/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/odb.md` & `abqpy-2023.5.2/docs/source/reference/odb.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/session/canvas.md` & `abqpy-2023.5.2/docs/source/reference/session/canvas.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/session/index.md` & `abqpy-2023.5.2/docs/source/reference/session/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/reference/session/path.md` & `abqpy-2023.5.2/docs/source/reference/session/path.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/tutorials.md` & `abqpy-2023.5.2/docs/source/tutorials.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/about/examples/create-part.md` & `abqpy-2023.5.2/docs/source/user/about/examples/create-part.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/about/examples/index.md` & `abqpy-2023.5.2/docs/source/user/about/examples/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/about/examples/read-output.md` & `abqpy-2023.5.2/docs/source/user/about/examples/read-output.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/about/examples/summary.md` & `abqpy-2023.5.2/docs/source/user/about/examples/summary.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/about/index.md` & `abqpy-2023.5.2/docs/source/user/about/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/about/interact.md` & `abqpy-2023.5.2/docs/source/user/about/interact.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/about/interface.md` & `abqpy-2023.5.2/docs/source/user/about/interface.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/environment/about.md` & `abqpy-2023.5.2/docs/source/user/environment/about.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/environment/index.md` & `abqpy-2023.5.2/docs/source/user/environment/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/environment/pde-basics.md` & `abqpy-2023.5.2/docs/source/user/environment/pde-basics.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/environment/use-pde.md` & `abqpy-2023.5.2/docs/source/user/environment/use-pde.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/examples/cantilever.md` & `abqpy-2023.5.2/docs/source/user/examples/cantilever.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/examples/index.md` & `abqpy-2023.5.2/docs/source/user/examples/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/examples/plot.md` & `abqpy-2023.5.2/docs/source/user/examples/plot.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/examples/sensitivity.md` & `abqpy-2023.5.2/docs/source/user/examples/sensitivity.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/examples/settings.md` & `abqpy-2023.5.2/docs/source/user/examples/settings.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/index.md` & `abqpy-2023.5.2/docs/source/user/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/access.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/access.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/architecture.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/architecture.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/compile-link.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/compile-link.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/computations.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/computations.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/examples.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/examples.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/exceptions.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/exceptions.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/improve-efficiency.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/improve-efficiency.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/object-model.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/object-model.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/output-object-model.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/output-object-model.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/read.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/read.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/style.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/style.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/utility.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/utility.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/cpp/write.md` & `abqpy-2023.5.2/docs/source/user/output/cpp/write.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/index.md` & `abqpy-2023.5.2/docs/source/user/output/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/python/computations.md` & `abqpy-2023.5.2/docs/source/user/output/python/computations.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/python/examples.md` & `abqpy-2023.5.2/docs/source/user/output/python/examples.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/python/exceptions.md` & `abqpy-2023.5.2/docs/source/user/output/python/exceptions.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/python/execute-script.md` & `abqpy-2023.5.2/docs/source/user/output/python/execute-script.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/python/improve-efficiency.md` & `abqpy-2023.5.2/docs/source/user/output/python/improve-efficiency.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/python/need-what-to-understand.md` & `abqpy-2023.5.2/docs/source/user/output/python/need-what-to-understand.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/python/object-model.md` & `abqpy-2023.5.2/docs/source/user/output/python/object-model.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/python/output-object-model.md` & `abqpy-2023.5.2/docs/source/user/output/python/output-object-model.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/python/read.md` & `abqpy-2023.5.2/docs/source/user/output/python/read.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/output/python/write.md` & `abqpy-2023.5.2/docs/source/user/output/python/write.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/introduction/further-reading.md` & `abqpy-2023.5.2/docs/source/user/python/introduction/further-reading.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/introduction/index.md` & `abqpy-2023.5.2/docs/source/user/python/introduction/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/introduction/oop-basics.md` & `abqpy-2023.5.2/docs/source/user/python/introduction/oop-basics.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/introduction/programming.md` & `abqpy-2023.5.2/docs/source/user/python/introduction/programming.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/introduction/python-abaqus.md` & `abqpy-2023.5.2/docs/source/user/python/introduction/python-abaqus.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/introduction/python-basics.md` & `abqpy-2023.5.2/docs/source/user/python/introduction/python-basics.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/introduction/python-interpreter.md` & `abqpy-2023.5.2/docs/source/user/python/introduction/python-interpreter.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/introduction/python-resources.md` & `abqpy-2023.5.2/docs/source/user/python/introduction/python-resources.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/python-abaqus/errors.md` & `abqpy-2023.5.2/docs/source/user/python/python-abaqus/errors.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/python-abaqus/executing.md` & `abqpy-2023.5.2/docs/source/user/python/python-abaqus/executing.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/python-abaqus/extending.md` & `abqpy-2023.5.2/docs/source/user/python/python-abaqus/extending.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/python-abaqus/index.md` & `abqpy-2023.5.2/docs/source/user/python/python-abaqus/index.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/python-abaqus/oop.md` & `abqpy-2023.5.2/docs/source/user/python/python-abaqus/oop.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/python-abaqus/style.md` & `abqpy-2023.5.2/docs/source/user/python/python-abaqus/style.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/python-abaqus/types.md` & `abqpy-2023.5.2/docs/source/user/python/python-abaqus/types.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/use-scripts/environment-file.md` & `abqpy-2023.5.2/docs/source/user/python/use-scripts/environment-file.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/use-scripts/interact.md` & `abqpy-2023.5.2/docs/source/user/python/use-scripts/interact.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/use-scripts/modify-objects.md` & `abqpy-2023.5.2/docs/source/user/python/use-scripts/modify-objects.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/use-scripts/namespace.md` & `abqpy-2023.5.2/docs/source/user/python/use-scripts/namespace.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/use-scripts/object-model.md` & `abqpy-2023.5.2/docs/source/user/python/use-scripts/object-model.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/use-scripts/sequences.md` & `abqpy-2023.5.2/docs/source/user/python/use-scripts/sequences.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/use-scripts/specify-region.md` & `abqpy-2023.5.2/docs/source/user/python/use-scripts/specify-region.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/use-scripts/specify-viewport.md` & `abqpy-2023.5.2/docs/source/user/python/use-scripts/specify-viewport.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/docs/source/user/python/use-scripts/user-input.md` & `abqpy-2023.5.2/docs/source/user/python/use-scripts/user-input.md`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/examples/Abaqus/cantilever.py` & `abqpy-2023.5.2/examples/Abaqus/cantilever.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/examples/Abaqus/skewExample.py` & `abqpy-2023.5.2/examples/Abaqus/skewExample.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/examples/Abaqus/viewerOpenOdbAndContour.py` & `abqpy-2023.5.2/examples/Abaqus/viewerOpenOdbAndContour.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/examples/Abaqus/viewerPrintContours.py` & `abqpy-2023.5.2/examples/Abaqus/viewerPrintContours.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/examples/Compression/compression-output.py` & `abqpy-2023.5.2/examples/Compression/compression-output.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/examples/Compression/compression.py` & `abqpy-2023.5.2/examples/Compression/compression.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/examples/Parameter-Identification/compression.py` & `abqpy-2023.5.2/examples/Parameter-Identification/compression.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/examples/Parameter-Identification/optimize.py` & `abqpy-2023.5.2/examples/Parameter-Identification/optimize.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/pyproject.toml` & `abqpy-2023.5.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -7,33 +7,77 @@
 [project]
 name = "abqpy"
 authors = [
   { name="WANG Hailin", email="hailin.wang@connect.polyu.hk" },
 ]
 description = "Type hints for Abaqus/Python scripting"
 readme = "README.md"
-dynamic = ["version", "dependencies", "optional-dependencies"]
+dynamic = ["version"]
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "auto-all",
+    "fire",
+    "typing-extensions",
+]
+
+[project.optional-dependencies]
+jupyter = [
+    "ipynbname",
+    "nbconvert",
+]
+dev = [
+    "black",
+    "coverage",
+    "crowdin-api-client",
+    "docformatter",
+    "flake8",
+    "numpy",
+    "pofmt",
+    "pre-commit",
+    "polib",
+    "pytest",
+    "pytest-cov",
+]
+docs = [
+    "autoclasstoc",
+    "myst-parser",
+    "pandas",
+    "pillow",
+    "sphinx",
+    "sphinx-autoapi",
+    "sphinx-toolbox",
+    "sphinx-autodoc-typehints",
+    "sphinx-copybutton",
+    "sphinx-comments",
+    "sphinx-design",
+    "sphinx-gallery",
+    "sphinx-hoverxref",
+    "sphinx-intl",
+    "sphinx-codeautolink",
+    "sphinx-rtd-theme",
+    "sphinx-togglebutton",
+    "sphinxcontrib-programoutput",
+]
 
 [project.urls]
 "Homepage" = "https://abqpy.com"
 "GitHub" = "https://github.com/haiiliin/abqpy"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+"Bug Tracker" = "https://github.com/haiiliin/abqpy/issues"
 "Read the Docs" = "https://readthedocs.org/projects/abqpy"
 "Documentation" = "https://docs.abqpy.com/en/stable/"
 
 [project.scripts]
 abqpy = "abqpy.__main__:main"
 
 [tool.setuptools]
@@ -46,22 +90,14 @@
     "meshEdit", "methodCallback", "monitorManager", "odbAccess",
     "odbConnectorBehavior", "odbMaterial", "odbSection", "part", 
     "redentABQ", "section","symbolicConstants", "textRepr", 
     "upgradeScript", "visualization", "regionToolset", "step", 
     "load", "optimization", "job", "sketch", "xyPlot",
 ]
 
-[tool.setuptools.dynamic.dependencies]
-file = ["requirements/deps.txt"]
-
-[tool.setuptools.dynamic.optional-dependencies]
-dev.file = ["requirements/dev.txt"]
-juptyer.file = ["requirements/jupyter.txt"]
-docs.file = ["requirements/docs.txt"]
-
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools_scm]
 root = "."
 relative_to = "__file__"
 version_scheme = "post-release"
```

### Comparing `abqpy-2023.5.1/scripts/conflicts.py` & `abqpy-2023.5.2/scripts/conflicts.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/scripts/rtd.py` & `abqpy-2023.5.2/scripts/rtd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 import os
 import re
 
 import fire
 import requests
-from requests import Response
 
 
 class ReadTheDocsAPI:
     """ReadTheDocs API client"""
 
     def __init__(self, project: str = "abqpy", token: str = None):
         self.project = project
         self.TOKEN = token or os.environ.get("RTD_TOKEN")
         self.HEADERS = {"Authorization": f"token {self.TOKEN}"}
 
 
 class ReadTheDocsVersion(ReadTheDocsAPI):
     """Manage versions of a project"""
 
-    def update(self, version: str, *, active: bool = None, hidden: bool = None, privacy_level: str = None) -> Response:
+    def build(self, version: str):
+        """Build a version
+
+        Parameters
+        ----------
+        version : str
+            Version to build
+        """
+        URL = f"https://readthedocs.org/api/v3/projects/{self.project}/versions/{version}/builds/"
+        print(requests.post(URL, headers=self.HEADERS))
+
+    def update(self, version: str, *, active: bool = None, hidden: bool = None, privacy_level: str = None):
         """Update status of a version
 
         Parameters
         ----------
         version : str
             Version to update
         active : bool, optional
             Whether the version is active
         hidden : bool, optional
             Whether the version is hidden
         privacy_level : str, optional
             Privacy level of the version
-
-        Returns
-        -------
-        Response from the API
         """
         URL = f"https://readthedocs.org/api/v3/projects/{self.project}/versions/{version}/"
         data = {}
         for option in ("active", "hidden", "privacy_level"):
             if locals()[option] is not None:
                 data[option] = locals()[option]
-        return requests.patch(URL, json=data, headers=self.HEADERS)
+        print(requests.patch(URL, json=data, headers=self.HEADERS))
 
 
 class ReadTheDocsRedirect(ReadTheDocsAPI):
     """Manage redirects of a project"""
 
-    def lists(self) -> requests.Response:
+    def _lists(self) -> requests.Response:
         """List redirects
 
         Returns
         -------
         Response from the API
         """
         URL = f"https://readthedocs.org/api/v3/projects/{self.project}/redirects/"
         return requests.get(URL, headers=self.HEADERS)
 
-    def update(self, minor_patch: str) -> list[requests.Response]:
+    def update(self, minor_patch: str):
         """Update a redirect from /{lang}/{major} to the latest /{lang}/{major}.{minor}.{patch} version
 
         Parameters
         ----------
         minor_patch : str
             {minor}.{patch} version to update
-
-        Returns
-        -------
-        A list of responses from the API
         """
         URL = f"https://readthedocs.org/api/v3/projects/{self.project}/redirects/{{pk}}/"
-        responses = []
-        for redirect in self.lists().json()["results"]:
+        for redirect in self._lists().json()["results"]:
             url = URL.format(pk=redirect["pk"])
             from_url, to_url = redirect["from_url"], redirect["to_url"]
-            lang, prefix, major, minor, patch = re.match(r"/(\w+)?/([vV]?)(\d+)\.(\d+)\.(\d+)/?", to_url).groups()
-            data = dict(url=url, from_url=from_url, to_url=f"/{lang}/{prefix}{major}.{minor_patch}", type="exact")
-            responses.append(requests.put(url, json=data, headers=self.HEADERS))
-        return responses
+            lang, pfx, major, minor, patch, sfx = re.match(r"/(\w+)?/([vV]?)(\d+)\.(\d+)\.(\d+)(.+?)", to_url).groups()
+            data = dict(url=url, from_url=from_url, to_url=f"/{lang}/{pfx}{major}.{minor_patch}{sfx}", type="exact")
+            print(requests.put(url, json=data, headers=self.HEADERS))
 
 
 class ReadTheDocs(ReadTheDocsAPI):
     """Manage a project on ReadTheDocs"""
 
     def __init__(self, project: str = "abqpy", token: str = None):
         super().__init__(project, token)
```

### Comparing `abqpy-2023.5.1/src/ababltin.py` & `abqpy-2023.5.2/src/ababltin.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/AbaqusCAEDisplayPreferences/CaeGuiPrefs.py` & `abqpy-2023.5.2/src/abaqus/AbaqusCAEDisplayPreferences/CaeGuiPrefs.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/AbaqusCAEDisplayPreferences/CaeKerPrefs.py` & `abqpy-2023.5.2/src/abaqus/AbaqusCAEDisplayPreferences/CaeKerPrefs.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/AbaqusCAEDisplayPreferences/caePrefsAccess.py` & `abqpy-2023.5.2/src/abaqus/AbaqusCAEDisplayPreferences/caePrefsAccess.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptiveMeshConstraint.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptiveMeshConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptiveMeshConstraintState.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptiveMeshConstraintState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptiveMeshControl.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptiveMeshControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptiveMeshDomain.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptiveMeshDomain.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptivityIteration.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptivityIteration.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptivityModel.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptivityModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptivityProcess.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptivityProcess.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/AdaptivityStep.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/AdaptivityStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/DisplacementAdaptiveMeshConstraint.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/DisplacementAdaptiveMeshConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/DisplacementAdaptiveMeshConstraintState.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/DisplacementAdaptiveMeshConstraintState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/ErrorIndicatorResult.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/ErrorIndicatorResult.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/RemeshingRule.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/RemeshingRule.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/RuleResult.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/RuleResult.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/VelocityAdaptiveMeshConstraint.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/VelocityAdaptiveMeshConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Adaptivity/VelocityAdaptiveMeshConstraintState.py` & `abqpy-2023.5.2/src/abaqus/Adaptivity/VelocityAdaptiveMeshConstraintState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/ActuatorAmplitude.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/ActuatorAmplitude.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/Amplitude.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/Amplitude.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/AmplitudeModel.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/AmplitudeModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/AmplitudeOdb.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/AmplitudeOdb.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/BaselineCorrection.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/BaselineCorrection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/Correlation.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/Correlation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/DecayAmplitude.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/DecayAmplitude.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/EquallySpacedAmplitude.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/EquallySpacedAmplitude.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/ModulatedAmplitude.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/ModulatedAmplitude.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/PeriodicAmplitude.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/PeriodicAmplitude.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/PsdDefinition.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/PsdDefinition.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/SmoothStepAmplitude.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/SmoothStepAmplitude.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/SolutionDependentAmplitude.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/SolutionDependentAmplitude.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/SpectrumAmplitude.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/SpectrumAmplitude.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Amplitude/TabularAmplitude.py` & `abqpy-2023.5.2/src/abaqus/Amplitude/TabularAmplitude.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Animation/AVIOptions.py` & `abqpy-2023.5.2/src/abaqus/Animation/AVIOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Animation/AnimationController.py` & `abqpy-2023.5.2/src/abaqus/Animation/AnimationController.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Animation/AnimationOptions.py` & `abqpy-2023.5.2/src/abaqus/Animation/AnimationOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Animation/AnimationSession.py` & `abqpy-2023.5.2/src/abaqus/Animation/AnimationSession.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Animation/ImageAnimation.py` & `abqpy-2023.5.2/src/abaqus/Animation/ImageAnimation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Animation/ImageAnimationOptions.py` & `abqpy-2023.5.2/src/abaqus/Animation/ImageAnimationOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Animation/Movie.py` & `abqpy-2023.5.2/src/abaqus/Animation/Movie.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Animation/QuickTimeOptions.py` & `abqpy-2023.5.2/src/abaqus/Animation/QuickTimeOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Annotation/AnimationUserData.py` & `abqpy-2023.5.2/src/abaqus/Annotation/AnimationUserData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Annotation/Annotation.py` & `abqpy-2023.5.2/src/abaqus/Annotation/Annotation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Annotation/AnnotationViewport.py` & `abqpy-2023.5.2/src/abaqus/Annotation/AnnotationViewport.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Annotation/AnnotationsToPlotArray.py` & `abqpy-2023.5.2/src/abaqus/Annotation/AnnotationsToPlotArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Annotation/Arrow.py` & `abqpy-2023.5.2/src/abaqus/Annotation/Arrow.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Annotation/Text.py` & `abqpy-2023.5.2/src/abaqus/Annotation/Text.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Assembly/Assembly.py` & `abqpy-2023.5.2/src/abaqus/Assembly/Assembly.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Assembly/AssemblyBase.py` & `abqpy-2023.5.2/src/abaqus/Assembly/AssemblyBase.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,24 @@
 from ..Mesh.MeshNodeArray import MeshNodeArray
 from ..Part.Part import Part
 from ..Property.SectionAssignmentArray import SectionAssignmentArray
 from ..Region.Set import Set
 from ..Region.Skin import Skin
 from ..Region.Stringer import Stringer
 from ..Region.Surface import Surface
-from ..UtilityAndView.abaqusConstants import ALL_EDGES, LOW, OFF, ON, Boolean
+from ..UtilityAndView.abaqusConstants import (
+    ALL_EDGES,
+    BOUNDARY_ONLY,
+    GEOMETRY,
+    LOW,
+    OFF,
+    ON,
+    SUPPRESS,
+    Boolean,
+)
 from ..UtilityAndView.abaqusConstants import abaqusConstants as C
 from .AssemblyFeature import AssemblyFeature
 from .AssemblyModel import AssemblyModel
 from .ConnectorOrientationArray import ConnectorOrientationArray
 from .ModelInstance import ModelInstance
 from .PartInstance import PartInstance
 
@@ -226,14 +235,202 @@
             instance = ModelInstance(name, *args, **kwargs)
             self.modelInstances[name] = instance
         self.instances[name] = instance
         self.allInstances[name] = instance
         return instance
 
     @abaqus_method_doc
+    def InstanceFromBooleanCut(
+        self,
+        name: str,
+        instanceToBeCut: PartInstance,
+        cuttingInstances: Sequence["PartInstance"],
+        originalInstances: Literal[C.SUPPRESS, C.DELETE] = SUPPRESS,
+    ) -> PartInstance:
+        """This method creates a PartInstance in the instances repository after subtracting or cutting the
+        geometries of a group of part instances from that of a base part instance.
+
+        .. note::
+            This function can be accessed by::
+
+                mdb.models[name].rootAssembly.InstanceFromBooleanCut
+
+        Parameters
+        ----------
+        name
+            A String specifying the repository key. The name must be a valid Abaqus object name.
+        instanceToBeCut
+            A PartInstance specifying the base instance from which to cut other instances.
+        cuttingInstances
+            A sequence of PartInstance objects specifying the instances with which to cut the base
+            instance.
+        originalInstances
+            A SymbolicConstant specifying whether the original instances should be suppressed or
+            deleted after the merge operation. Possible values are SUPPRESS or DELETE. The default
+            value is SUPPRESS.
+
+        Returns
+        -------
+        PartInstance
+            A PartInstance object.
+        """
+        return PartInstance(name, Part())
+
+    @abaqus_method_doc
+    def InstanceFromBooleanMerge(
+        self,
+        name: str,
+        instances: Sequence["PartInstance"],
+        keepIntersections: Boolean = False,
+        originalInstances: Literal[C.SUPPRESS, C.DELETE] = SUPPRESS,
+        domain: Literal[C.MESH, C.BOTH, C.GEOMETRY] = GEOMETRY,
+        mergeNodes: Literal[C.MESH, C.ALL, C.BOUNDARY_ONLY, C.NONE] = BOUNDARY_ONLY,
+        nodeMergingTolerance: Optional[float] = None,
+        removeDuplicateElements: Boolean = True,
+    ):
+        """This method creates a PartInstance in the instances repository after merging two or more part
+        instances.
+
+        .. note::
+            This function can be accessed by::
+
+                mdb.models[name].rootAssembly.InstanceFromBooleanMerge
+
+        Parameters
+        ----------
+        name
+            A String specifying the repository key. The name must be a valid Abaqus object name.
+        instances
+            A sequence of PartInstance objects specifying the part instances to merge.
+        keepIntersections
+            A Boolean specifying whether the boundary intersections of Abaqus native part instances
+            should be retained after the merge operation. The default value is False.
+        originalInstances
+            A SymbolicConstant specifying whether the original instances should be suppressed or
+            deleted after the merge operation. Possible values are SUPPRESS or DELETE. The default
+            value is SUPPRESS.
+        domain
+            A SymbolicConstant specifying whether geometry or mesh of the specified part instances
+            is to be merged. Possible values are GEOMETRY, MESH or BOTH. The default value is
+            GEOMETRY.
+        mergeNodes
+            A SymbolicConstant specifying which nodes of the specified part instances should be
+            considered for merging. This argument is only applicable if **domain** is MESH. Possible
+            values are BOUNDARY_ONLY, ALL, or NONE. The default value is BOUNDARY_ONLY.
+        nodeMergingTolerance
+            A Float specifying the maximum distance between nodes of the specified part instances
+            that will be merged and replaced with a single node in the new part. The location of the
+            new node is the average position of the deleted nodes. This argument is only applicable
+            if **domain** is MESH. The default value is 10⁻⁶.
+        removeDuplicateElements
+            A Boolean specifying whether elements with the same connectivity in the new part will be
+            merged into a single element. This argument is only applicable if **domain** is MESH. The
+            default value is True.
+
+        Returns
+        -------
+        PartInstance
+            A PartInstance object.
+        """
+        return PartInstance(name, Part())
+
+    @abaqus_method_doc
+    def LinearInstancePattern(
+        self,
+        instanceList: tuple,
+        number1: int,
+        spacing1: float,
+        number2: int,
+        spacing2: float,
+        direction1: tuple = (),
+        direction2: tuple = (),
+    ) -> Sequence["PartInstance"]:
+        """This method creates multiple PartInstance objects in a linear pattern and puts them into the
+        instances repository.
+
+        .. note::
+            This function can be accessed by::
+
+                mdb.models[name].rootAssembly.LinearInstancePattern
+
+        Parameters
+        ----------
+        instanceList
+            A sequence of Strings specifying the names of instances to pattern.
+        number1
+            An Int specifying the total number of instances, including the original instances, that
+            appear along the first direction in the pattern.
+        spacing1
+            A Float specifying the spacing between instances along the first direction in the
+            pattern.
+        number2
+            An Int specifying the total number of instances, including the original instances, that
+            appear along the second direction in the pattern.
+        spacing2
+            A Float specifying the spacing between instances along the second direction in the
+            pattern.
+        direction1
+            A sequence of three Floats specifying a vector along the first direction. The default
+            value is (1.0, 0.0, 0.0).
+        direction2
+            A sequence of three Floats specifying a vector along the second direction. The default
+            value is (0.0, 1.0, 0.0).
+
+        Returns
+        -------
+        Sequence[PartInstance]
+            A sequence of PartInstance objects.
+        """
+        return [PartInstance(name, Part()) for name in instanceList]
+
+    @abaqus_method_doc
+    def RadialInstancePattern(
+        self,
+        instanceList: tuple,
+        number: int,
+        totalAngle: float,
+        point: Sequence[float] = (),
+        axis: Sequence[float] = (),
+    ) -> Sequence["PartInstance"]:
+        """This method creates multiple PartInstance objects in a radial pattern and puts them into the
+        instances repository.
+
+        .. note::
+            This function can be accessed by::
+
+                mdb.models[name].rootAssembly.RadialInstancePattern
+
+        Parameters
+        ----------
+        instanceList
+            A sequence of Strings specifying the names of instances to pattern.
+        number
+            An Int specifying the total number of instances, including the original instances, that
+            appear in the radial pattern.
+        totalAngle
+            A Float specifying the total angle in degrees between the first and last instance in the
+            pattern. A positive angle corresponds to a counter-clockwise direction. The values 360°
+            and -360° represent a special case where the pattern makes a full circle. In this case,
+            because the copy would overlay the original, the copy is not placed at the last
+            position. Possible values are -360.0 ≤ **totalAngle** ≤ 360.0.
+        point
+            A sequence of three Floats specifying the center of the radial pattern. The default
+            value is (0.0, 0.0, 0.0).
+        axis
+            A sequence of three Floats specifying the central axis of the radial pattern. The
+            default value is (0.0, 0.0, 1.0).
+
+        Returns
+        -------
+        Sequence[PartInstance]
+            A sequence of PartInstance objects.
+        """
+        return [PartInstance(name, Part()) for name in instanceList]
+
+    @abaqus_method_doc
     def backup(self):
         """This method makes a backup copy of the features in the assembly.
 
         The backup() method is used in conjunction with the restore() method.
         """
         ...
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `abqpy-2023.5.1/src/abaqus/Assembly/AssemblyFeature.py` & `abqpy-2023.5.2/src/abaqus/Assembly/AssemblyFeature.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Assembly/AssemblyModel.py` & `abqpy-2023.5.2/src/abaqus/Assembly/AssemblyModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Assembly/ConnectorOrientation.py` & `abqpy-2023.5.2/src/abaqus/Assembly/ConnectorOrientation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Assembly/ModelInstance.py` & `abqpy-2023.5.2/src/abaqus/Assembly/ModelInstance.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Assembly/PartInstance.py` & `abqpy-2023.5.2/src/abaqus/Model/ModelBase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,554 +1,510 @@
-from typing import Dict, List, Optional, Sequence, Tuple
+from typing import Dict, Optional
 
 from typing_extensions import Literal
 
 from abqpy.decorators import abaqus_class_doc, abaqus_method_doc
 
-from ..BasicGeometry.CellArray import CellArray
-from ..BasicGeometry.EdgeArray import EdgeArray
-from ..BasicGeometry.FaceArray import FaceArray
-from ..BasicGeometry.IgnoredEdgeArray import IgnoredEdgeArray
-from ..BasicGeometry.IgnoredVertexArray import IgnoredVertexArray
-from ..BasicGeometry.ReferencePoint import ReferencePoint
-from ..BasicGeometry.VertexArray import VertexArray
-from ..Datum.Datum import Datum
-from ..Mesh.MeshEdge import MeshEdge
-from ..Mesh.MeshEdgeArray import MeshEdgeArray
-from ..Mesh.MeshElementArray import MeshElementArray
-from ..Mesh.MeshFace import MeshFace
-from ..Mesh.MeshFaceArray import MeshFaceArray
-from ..Mesh.MeshNodeArray import MeshNodeArray
+from ..Adaptivity.AdaptiveMeshConstraint import AdaptiveMeshConstraint
+from ..Adaptivity.AdaptiveMeshControl import AdaptiveMeshControl
+from ..Adaptivity.RemeshingRule import RemeshingRule
+from ..Amplitude.Amplitude import Amplitude
+from ..Assembly.Assembly import Assembly
+from ..BeamSectionProfile.Profile import Profile
+from ..BoundaryCondition.BoundaryCondition import BoundaryCondition
+from ..Calibration.Calibration import Calibration
+from ..Constraint.Constraint import Constraint
+from ..Feature.FeatureOptions import FeatureOptions
+from ..Field.AnalyticalField import AnalyticalField
+from ..Field.DiscreteField import DiscreteField
+from ..Filter.Filter import Filter
+from ..Interaction.ContactControl import ContactControl
+from ..Interaction.ContactInitialization import ContactInitialization
+from ..Interaction.ContactProperty import ContactProperty
+from ..Interaction.ContactStabilization import ContactStabilization
+from ..Interaction.Interaction import Interaction
+from ..Load.Load import Load
+from ..Material.Material import Material
+from ..Optimization.OptimizationTask import OptimizationTask
 from ..Part.Part import Part
-from ..Region.Set import Set
-from ..Region.Skin import Skin
-from ..Region.Stringer import Stringer
-from ..Region.Surface import Surface
+from ..PredefinedField.PredefinedField import PredefinedField
+from ..Section.Section import Section
+from ..Sketcher.ConstrainedSketch import ConstrainedSketch
+from ..Step.InitialStep import InitialStep
+from ..Step.Step import Step
+from ..StepOutput.FieldOutputRequest import FieldOutputRequest
+from ..StepOutput.HistoryOutputRequest import HistoryOutputRequest
+from ..StepOutput.IntegratedOutputSection import IntegratedOutputSection
+from ..StepOutput.TimePoint import TimePoint
+from ..TableCollection.EventSeriesData import EventSeriesData
+from ..TableCollection.EventSeriesType import EventSeriesType
+from ..TableCollection.TableCollection import TableCollection
 from ..UtilityAndView.abaqusConstants import (
-    BOUNDARY_ONLY,
-    GEOMETRY,
+    B31,
+    C3D8I,
+    C3D10,
+    NOT_SET,
     OFF,
-    SUPPRESS,
+    ON,
+    PRESERVE_SECTION,
+    S4,
+    STANDARD_EXPLICIT,
     Boolean,
     SymbolicConstant,
 )
 from ..UtilityAndView.abaqusConstants import abaqusConstants as C
+from .KeywordBlock import KeywordBlock
 
 
 @abaqus_class_doc
-class PartInstance:
-    """A PartInstance object is an instance of a Part object.
+class ModelBase:
+    """Abaqus creates a Model object named `Model-1` when a session is started.
 
     .. note::
         This object can be accessed by::
 
-            import assembly
-            mdb.models[name].rootAssembly.allInstances[name]
-            mdb.models[name].rootAssembly.instances[name]
+            mdb.models[name]
+
+        The corresponding analysis keywords are:
+
+        - PHYSICAL CONSTANTS
     """
 
-    #: A String specifying the repository key. The name must be a valid Abaqus object name.
+    #: A String specifying the repository key.
     name: str = ""
 
-    #: A Boolean specifying whether the part instance is dependent or independent. If
-    #: **dependent** = OFF, the part instance is independent. The default value is OFF.
-    dependent: Boolean = OFF
+    #: None or a Float specifying the Stefan-Boltzmann constant. The default value is None.
+    stefanBoltzmann: Optional[float] = None
 
-    #: A Boolean specifying whether the part instance is excluded from the simulation. If
-    #: **excludedFromSimulation** = ON, the part instance is excluded from the simulation. The
-    #: default value is OFF.
-    excludedFromSimulation: Boolean = OFF
+    #: None or a Float specifying the absolute zero constant. The default value is None.
+    absoluteZero: Optional[float] = None
 
-    #: A Boolean specifying the validity of the geometry of the instance. The value is
-    #: computed, but it can be set to ON to perform feature and mesh operations on an invalid
-    #: instance. There is no guarantee that such operations will work if the instance was
-    #: originally invalid.
-    geometryValidity: Boolean = OFF
+    #: A SymbolicConstant specifying the type of incident wave formulation to be used in
+    #: acoustic problems. Possible values are NOT_SET, SCATTERED, and TOTAL. The default value
+    #: is NOT_SET.
+    waveFormulation: SymbolicConstant = NOT_SET
 
-    #: A SymbolicConstant specifying the part type. Possible values are DEFORMABLE_BODY,
-    #: EULERIAN, DISCRETE_RIGID_SURFACE, and ANALYTIC_RIGID_SURFACE.
-    analysisType: Optional[SymbolicConstant] = None
+    #: None or a Float specifying the universal gas constant. The default value is None.
+    universalGas: Optional[float] = None
 
-    #: An Int specifying the reference node number. This member is valid only if
-    #: **analysisType** = DISCRETE_RIGID_SURFACE or ANALYTIC_RIGID_SURFACE.
-    referenceNode: Optional[int] = None
+    #: A Boolean specifying whether an input file should be written without parts and
+    #: assemblies. The default value is OFF.
+    noPartsInputFile: Boolean = OFF
 
-    #: A Part object specifying the instanced part.
-    part: Optional[Part] = None
+    #: An Int specifying the increment, interval, iteration or cycle where the restart analysis
+    #: will start. To select the end of the step use the SymbolicConstant STEP_END.
+    restartIncrement: Optional[SymbolicConstant] = None
 
-    #: A repository of Set objects specifying the sets created on the part. For more
-    #: information, see Region commands.
-    sets: Dict[str, Set] = {}
+    #: A Boolean specifying that the step specified by **restartStep** should be terminated at
+    #: the increment specified by **restartIncrement**.
+    endRestartStep: Boolean = OFF
 
-    #: A repository of Surface objects specifying the surfaces created on the part. For more
-    #: information, see Region commands.
-    surfaces: Dict[str, Surface] = {}
+    #: A Boolean specifying that a shell global model drives a solid submodel.
+    shellToSolid: Boolean = OFF
 
-    #: A repository of Skin objects specifying the skins created on the part. For more
-    #: information, see Region commands.
-    skins: Dict[str, Skin] = {}
+    #: A Float specifying the time stamp that indicates when the model was last changed.
+    lastChangedCount: Optional[float] = None
 
-    #: A repository of Stringer objects specifying the stringers created on the part. For more
-    #: information, see Region commands.
-    stringers: Dict[str, Stringer] = {}
+    #: A String specifying the purpose and contents of the Model object. The default value is
+    #: an empty string.
+    description: str = ""
 
-    #: A VertexArray object.
-    vertices: VertexArray = VertexArray([])
+    #: A String specifying the name of the job that generated the restart data.
+    restartJob: str = ""
 
-    #: An IgnoredVertexArray object.
-    ignoredVertices: IgnoredVertexArray = []
+    #: A String specifying the name of the step where the restart analysis will start.
+    restartStep: str = ""
 
-    #: An EdgeArray object.
-    edges: EdgeArray = EdgeArray([])
+    #: A String specifying the name of the job that generated the results for the global model.
+    globalJob: str = ""
 
-    #: An IgnoredEdgeArray object.
-    ignoredEdges: IgnoredEdgeArray = []
+    #: A boolean specifying the status of constraints created in a model, in the model which
+    #: instances this model.
+    copyConstraints: Boolean = OFF
 
-    #: A FaceArray object.
-    faces: FaceArray = FaceArray([])
+    #: A boolean specifying the status of connectors created in a model, in the model which
+    #: instances this model.
+    copyConnectors: Boolean = OFF
 
-    #: A CellArray object.
-    cells: CellArray = CellArray([])
+    #: A boolean specifying the status of interactions created in a model, in the model which
+    #: instances this model.
+    copyInteractions: Boolean = OFF
 
-    #: A repository of Datum objects.
-    datums: List[Datum] = []
+    #: A KeywordBlock object.
+    keywordBlock: KeywordBlock = KeywordBlock()
 
-    #: A MeshElementArray object.
-    elements: MeshElementArray = MeshElementArray([])
+    #: An Assembly object.
+    rootAssembly: Assembly = Assembly()
 
-    #: A MeshNodeArray object.
-    nodes: MeshNodeArray = MeshNodeArray([])
+    #: A repository of Amplitude objects.
+    amplitudes: Dict[str, Amplitude] = {}
 
-    #: A repository of MeshFace objects specifying all the element faces in the part instance.
-    #: For a given element and a given face index within that element, the corresponding
-    #: MeshFace object can be retrieved from the repository by using the key calculated as
-    # (i*8 + j), where i and j are zero-based element and face indices, respectively.
-    elemFaces: Dict[str, MeshFace] = {}
+    #: A repository of Profile objects.
+    profiles: Dict[str, Profile] = {}
 
-    #: A MeshFaceArray object.
-    elementFaces: MeshFaceArray = MeshFaceArray([])
+    #: A repository of BoundaryCondition objects.
+    boundaryConditions: Dict[str, BoundaryCondition] = {}
 
-    #: A repository of MeshEdge objects specifying all the element edges in the part instance.
-    #: For a given element and a given edge index on a given face within that element, the
-    #: corresponding MeshEdge object can be retrieved from the repository by using the key
-    #: calculated as (i*32 + j*4 + k), where i, j, and k are zero-based element, face, and edge
-    #: indices, respectively.
-    elemEdges: Dict[str, MeshEdge] = {}
+    #: A repository of ConstrainedSketchConstraint objects.
+    constraints: Dict[str, Constraint] = {}
 
-    #: A MeshEdgeArray object.
-    elementEdges: MeshEdgeArray = MeshEdgeArray([])
+    #: A repository of AnalyticalField objects.
+    analyticalFields: Dict[str, AnalyticalField] = {}
 
-    #: A repository of ReferencePoint objects.
-    referencePoints: Dict[str, ReferencePoint] = {}
+    #: A repository of DiscreteField objects.
+    discreteFields: Dict[str, DiscreteField] = {}
 
-    #: A String specifying the name of the part from which the instance was created.
-    partName: str = ""
+    #: A repository of PredefinedField objects.
+    predefinedFields: Dict[str, PredefinedField] = {}
 
-    @abaqus_method_doc
-    def __init__(self, name: str, part: Part, autoOffset: Boolean = OFF, dependent: Boolean = OFF):
-        """This method creates a PartInstance object and puts it into the instances repository.
+    #: A repository of Interaction objects.
+    interactions: Dict[str, Interaction] = {}
 
-        .. note::
-            This function can be accessed by::
+    #: A repository of InteractionProperty objects.
+    interactionProperties: Dict[str, ContactProperty] = {}
 
-                mdb.models[name].rootAssembly.Instance
+    #: A repository of ContactControl objects.
+    contactControls: Dict[str, ContactControl] = {}
 
-        Parameters
-        ----------
-        name
-            A String specifying the repository key. The name must be a valid Abaqus object name.
-        part
-            A Part object to be instanced. If the part does not exist, no PartInstance object is
-            created.
-        autoOffset
-            A Boolean specifying whether to apply an auto offset to the new part instance that will
-            offset it from existing part instances. The default value is OFF.
-        dependent
-            A Boolean specifying whether the part instance is dependent or independent. If
-            **dependent** = OFF, the part instance is independent. The default value is OFF.
+    #: A repository of ContactInitialization objects.
+    contactInitializations: Dict[str, ContactInitialization] = {}
 
-        Returns
-        -------
-        PartInstance
-            A PartInstance object.
-        """
-        self.vertices = part.vertices
-        self.ignoredEdges = part.ignoredEdges
-        self.faces = part.faces
-        self.cells = part.cells
-        self.datums = part.datums
-        self.elements = part.elements
-        self.elemFaces = part.elemFaces
-        self.elementFaces = part.elementFaces
-        self.nodes = part.nodes
-        self.sets = part.sets
-        self.surfaces = part.surfaces
-        self.skins = part.skins
-        self.stringers = part.stringers
-        self.referencePoints = part.referencePoints
-        self.elemEdges = part.elemEdges
-        self.elementEdges = part.elementEdges
+    #: A repository of ContactStabilization objects.
+    contactStabilizations: Dict[str, ContactStabilization] = {}
 
-    @abaqus_method_doc
-    def InstanceFromBooleanCut(
-        self,
-        name: str,
-        instanceToBeCut: str,
-        cuttingInstances: Sequence["PartInstance"],
-        originalInstances: Literal[C.SUPPRESS, C.DELETE] = SUPPRESS,
-    ):
-        """This method creates a PartInstance in the instances repository after subtracting or cutting the
-        geometries of a group of part instances from that of a base part instance.
+    #: A tuple of tuples of Strings specifying the linked child PartInstance name in the
+    #: current model to the corresponding parent PartInstance name in a different model.
+    linkedInstances: tuple = ()
 
-        .. note::
-            This function can be accessed by::
+    #: A tuple of tuples of Strings specifying the linked child Part name in the current model
+    #: to the corresponding parent Part name in a different model.
+    linkedParts: tuple = ()
 
-                mdb.models[name].rootAssembly.Instance
+    #: A repository of Load objects.
+    loads: Dict[str, Load] = {}
 
-        Parameters
-        ----------
-        name
-            A String specifying the repository key. The name must be a valid Abaqus object name.
-        instanceToBeCut
-            A PartInstance specifying the base instance from which to cut other instances.
-        cuttingInstances
-            A sequence of PartInstance objects specifying the instances with which to cut the base
-            instance.
-        originalInstances
-            A SymbolicConstant specifying whether the original instances should be suppressed or
-            deleted after the merge operation. Possible values are SUPPRESS or DELETE. The default
-            value is SUPPRESS.
+    #: A repository of Material objects.
+    materials: Dict[str, Material] = {}
 
-        Returns
-        -------
-        PartInstance
-            A PartInstance object.
-        """
-        ...
+    #: A repository of Calibration objects.
+    calibrations: Dict[str, Calibration] = {}
 
-    @abaqus_method_doc
-    def InstanceFromBooleanMerge(
-        self,
-        name: str,
-        instances: Sequence["PartInstance"],
-        keepIntersections: Boolean = False,
-        originalInstances: Literal[C.SUPPRESS, C.DELETE] = SUPPRESS,
-        domain: Literal[C.MESH, C.BOTH, C.GEOMETRY] = GEOMETRY,
-        mergeNodes: Literal[C.MESH, C.ALL, C.BOUNDARY_ONLY, C.NONE] = BOUNDARY_ONLY,
-        nodeMergingTolerance: Optional[float] = None,
-        removeDuplicateElements: Boolean = True,
-    ):
-        """This method creates a PartInstance in the instances repository after merging two or more part
-        instances.
+    #: A repository of Section objects.
+    sections: Dict[str, Section] = {}
 
-        .. note::
-            This function can be accessed by::
+    #: A repository of RemeshingRule objects.
+    remeshingRules: Dict[str, RemeshingRule] = {}
 
-                mdb.models[name].rootAssembly.Instance
+    #: A repository of ConstrainedSketch objects.
+    sketches: Dict[str, ConstrainedSketch] = {}
 
-        Parameters
-        ----------
-        name
-            A String specifying the repository key. The name must be a valid Abaqus object name.
-        instances
-            A sequence of PartInstance objects specifying the part instances to merge.
-        keepIntersections
-            A Boolean specifying whether the boundary intersections of Abaqus native part instances
-            should be retained after the merge operation. The default value is False.
-        originalInstances
-            A SymbolicConstant specifying whether the original instances should be suppressed or
-            deleted after the merge operation. Possible values are SUPPRESS or DELETE. The default
-            value is SUPPRESS.
-        domain
-            A SymbolicConstant specifying whether geometry or mesh of the specified part instances
-            is to be merged. Possible values are GEOMETRY, MESH or BOTH. The default value is
-            GEOMETRY.
-        mergeNodes
-            A SymbolicConstant specifying which nodes of the specified part instances should be
-            considered for merging. This argument is only applicable if **domain** is MESH. Possible
-            values are BOUNDARY_ONLY, ALL, or NONE. The default value is BOUNDARY_ONLY.
-        nodeMergingTolerance
-            A Float specifying the maximum distance between nodes of the specified part instances
-            that will be merged and replaced with a single node in the new part. The location of the
-            new node is the average position of the deleted nodes. This argument is only applicable
-            if **domain** is MESH. The default value is 10⁻⁶.
-        removeDuplicateElements
-            A Boolean specifying whether elements with the same connectivity in the new part will be
-            merged into a single element. This argument is only applicable if **domain** is MESH. The
-            default value is True.
+    #: A repository of Part objects.
+    parts: Dict[str, Part] = {}
 
-        Returns
-        -------
-        PartInstance
-            A PartInstance object.
-        """
-        ...
+    #: A repository of Step objects.
+    steps: Dict[str, Step] = {}
 
-    @abaqus_method_doc
-    def LinearInstancePattern(
-        self,
-        instanceList: tuple,
-        number1: int,
-        spacing1: float,
-        number2: int,
-        spacing2: float,
-        direction1: tuple = (),
-        direction2: tuple = (),
-    ) -> Sequence["PartInstance"]:
-        """This method creates multiple PartInstance objects in a linear pattern and puts them into the
-        instances repository.
+    #: A FeatureOptions object.
+    featureOptions: FeatureOptions = FeatureOptions()
 
-        .. note::
-            This function can be accessed by::
+    #: A repository of AdaptiveMeshConstraint objects.
+    adaptiveMeshConstraints: Dict[str, AdaptiveMeshConstraint] = {}
 
-                mdb.models[name].rootAssembly.Instance
+    #: A repository of AdaptiveMeshControl objects.
+    adaptiveMeshControls: Dict[str, AdaptiveMeshControl] = {}
 
-        Parameters
-        ----------
-        instanceList
-            A sequence of Strings specifying the names of instances to pattern.
-        number1
-            An Int specifying the total number of instances, including the original instances, that
-            appear along the first direction in the pattern.
-        spacing1
-            A Float specifying the spacing between instances along the first direction in the
-            pattern.
-        number2
-            An Int specifying the total number of instances, including the original instances, that
-            appear along the second direction in the pattern.
-        spacing2
-            A Float specifying the spacing between instances along the second direction in the
-            pattern.
-        direction1
-            A sequence of three Floats specifying a vector along the first direction. The default
-            value is (1.0, 0.0, 0.0).
-        direction2
-            A sequence of three Floats specifying a vector along the second direction. The default
-            value is (0.0, 1.0, 0.0).
+    #: A repository of TimePoint objects.
+    timePoints: Dict[str, TimePoint] = {}
 
-        Returns
-        -------
-        Sequence[PartInstance]
-            A sequence of PartInstance objects.
-        """
-        ...
+    #: A repository of Filter objects.
+    filters: Dict[str, Filter] = {}
+
+    #: A repository of IntegratedOutputSection objects.
+    integratedOutputSections: Dict[str, IntegratedOutputSection] = {}
+
+    #: A repository of FieldOutputRequest objects.
+    fieldOutputRequests: Dict[str, FieldOutputRequest] = {}
+
+    #: A repository of HistoryOutputRequest objects.
+    historyOutputRequests: Dict[str, HistoryOutputRequest] = {}
+
+    #: A repository of OptimizationTask objects.
+    optimizationTasks: Dict[str, OptimizationTask] = {}
+
+    #: A repository of TableCollection objects.
+    #:
+    #: .. versionadded:: 2020
+    #:     The ``tableCollections`` attribute was added.
+    tableCollections: Dict[str, TableCollection] = {}
+
+    #: A repository of EventSeriesType objects.
+    #:
+    #: .. versionadded:: 2020
+    #:     The ``eventSeriesTypes`` attribute was added.
+    eventSeriesTypes: Dict[str, EventSeriesType] = {}
+
+    #: A repository of EventSeriesData objects.
+    #:
+    #: .. versionadded:: 2020
+    #:     The ``eventSeriesDatas`` attribute was added.
+    eventSeriesDatas: Dict[str, EventSeriesData] = {}
 
     @abaqus_method_doc
-    def RadialInstancePattern(
+    def __init__(
         self,
-        instanceList: tuple,
-        number: int,
-        totalAngle: float,
-        point: Sequence[float] = (),
-        axis: Sequence[float] = (),
+        name: str,
+        description: str = "",
+        stefanBoltzmann: Optional[float] = None,
+        absoluteZero: Optional[float] = None,
+        waveFormulation: Literal[C.SCATTERED, C.NOT_SET, C.TOTAL] = NOT_SET,
+        modelType: Literal[C.STANDARD_EXPLICIT, C.ELECTROMAGNETIC] = STANDARD_EXPLICIT,
+        universalGas: Optional[float] = None,
+        copyConstraints: Boolean = ON,
+        copyConnectors: Boolean = ON,
+        copyInteractions: Boolean = ON,
     ):
-        """This method creates multiple PartInstance objects in a radial pattern and puts them into the
-        instances repository.
+        """This method creates a Model object.
 
         .. note::
             This function can be accessed by::
 
-                mdb.models[name].rootAssembly.Instance
+                mdb.Model
 
         Parameters
         ----------
-        instanceList
-            A sequence of Strings specifying the names of instances to pattern.
-        number
-            An Int specifying the total number of instances, including the original instances, that
-            appear in the radial pattern.
-        totalAngle
-            A Float specifying the total angle in degrees between the first and last instance in the
-            pattern. A positive angle corresponds to a counter-clockwise direction. The values 360°
-            and -360° represent a special case where the pattern makes a full circle. In this case,
-            because the copy would overlay the original, the copy is not placed at the last
-            position. Possible values are -360.0 ≤ **totalAngle** ≤ 360.0.
-        point
-            A sequence of three Floats specifying the center of the radial pattern. The default
-            value is (0.0, 0.0, 0.0).
-        axis
-            A sequence of three Floats specifying the central axis of the radial pattern. The
-            default value is (0.0, 0.0, 1.0).
+        name
+            A String specifying the repository key.
+        description
+            A String specifying the purpose and contents of the Model object. The default value is
+            an empty string.
+        stefanBoltzmann
+            None or a Float specifying the Stefan-Boltzmann constant. The default value is None.
+        absoluteZero
+            None or a Float specifying the absolute zero constant. The default value is None.
+        waveFormulation
+            A SymbolicConstant specifying the type of incident wave formulation to be used in
+            acoustic problems. Possible values are NOT_SET, SCATTERED, and TOTAL. The default value
+            is NOT_SET.
+        modelType
+            A SymbolicConstant specifying the analysis model type. Possible values are
+            STANDARD_EXPLICIT and ELECTROMAGNETIC. The default is STANDARD_EXPLICIT.
+        universalGas
+            None or a Float specifying the universal gas constant. The default value is None.
+        copyConstraints
+            A boolean specifying whether to copy the constraints created in the model to the model
+            that instances this model. The default value is ON.
+        copyConnectors
+            A boolean specifying whether to copy the connectors created in the model to the model
+            that instances this model. The default value is ON.
+        copyInteractions
+            A boolean specifying whether to copy the interactions created in the model to the model
+            that instances this model. The default value is ON.
 
         Returns
         -------
-        Sequence[PartInstance]
-            A sequence of PartInstance objects.
+        Model
+            A Model object.
         """
-        ...
+        self.steps["Initial"] = InitialStep()
 
     @abaqus_method_doc
-    def checkGeometry(self, detailed: Boolean = OFF, level: Optional[int] = None):
-        """This method checks the validity of the geometry of the part instance and prints a count of all
-        topological entities on the part instance (faces, edges, vertices, etc.).
+    def ModelFromInputFile(self, name: str, inputFileName: str):
+        """This method creates a Model object by reading the keywords in an input file and creating the
+        corresponding Abaqus/CAE objects.
 
-        Parameters
-        ----------
-        detailed
-            A Boolean specifying whether detailed output will be printed to the replay file. The
-            default value is OFF.
-        level
-            An Int specifying which level of checking is performed. Values can range from 20 to 70,
-            with higher values reporting less and less important errors. The default value is 20,
-            which reports all critical errors. When the default value is used, the stored validity
-            status is updated to agree with the result of this check.
-
-        Raises
-        ------
-        Exception
-            An exception is thrown if this is a dependent part instance and **level** was either not
-            specified or was set to 20, because the validity status cannot be updated for a
-            dependent part instance. In this case, this command should be called on the Part
-            instead. The geometry of dependent part instances cannot be changed.
-        """
-        ...
+        .. note::
+            This function can be accessed by::
 
-    @abaqus_method_doc
-    def Contact(
-        self,
-        movableList: tuple,
-        fixedList: tuple,
-        direction: tuple,
-        clearance: float,
-        isFaceEdges: Boolean = OFF,
-    ):
-        """This method translates an instance along the specified direction until it is in contact with a fixed
-        instance.
+                mdb.Model
 
         Parameters
         ----------
-        movableList
-            A sequence of Face or Edge objects on the part instance to be moved.
-        fixedList
-            A sequence of Face or Edge objects on the part instance to remain fixed.
-        direction
-            A sequence of three Floats specifying the direction of contact.
-        clearance
-            A Float specifying the distance between the two faces along the direction of contact.
-        isFaceEdges
-            A Boolean specifying how Abaqus calculates the contact. If **isFaceEdges** is OFF, contact
-            is computed from the movable face to the fixed face. If **isFaceEdges** is ON, contact is
-            computed using only the edges of the movable face and not its interior. The default
-            value is OFF.
+        name
+            A String specifying the repository key.
+        inputFileName
+            A String specifying the name of the input file (including the .inp extension) to be
+            parsed into the new model. This String can also be the full path to the input file if it
+            is located in another directory.
 
         Returns
         -------
-        feature: Feature
-            A Feature object
+        Model
+            A Model object.
         """
         ...
 
     @abaqus_method_doc
-    def ConvertConstraints(self):
-        """This method converts the position constraints of an instance to absolute positions.
+    def ModelFromOdbFile(self, name: str, odbFileName: str):
+        """This method creates a Model object by reading an output database and creating any corresponding
+        Abaqus/CAE objects.
 
-        The method deletes the constraint features on the instance but preserves the position in space.
-        """
-        ...
-
-    @abaqus_method_doc
-    def getPosition(self):
-        """This method prints the sum of the translations and rotations applied to the PartInstance object."""
-        ...
-
-    @abaqus_method_doc
-    def getRotation(self):
-        """This method returns a tuple including the point of rotation, axis of rotation, and rotation angle (in
-        degrees).
+        .. note::
+            This function can be accessed by::
 
-        Returns
-        -------
-        tuple
-            A tuple including the point of rotation, axis of rotation, and rotation angle (in
-            degrees).
-        """
-        ...
+                mdb.Model
 
-    @abaqus_method_doc
-    def getTranslation(self) -> Tuple[float, float, float]:
-        """This method returns a tuple of three Floats representing translation in the **X**, **Y**, and **Z**
-        directions.
+        Parameters
+        ----------
+        name
+            A String specifying the repository key.
+        odbFileName
+            A String specifying the name of the output database file (including the .odb extension)
+            to be read into the new model. This String can also be the full path to the output
+            database file if it is located in another directory.
 
         Returns
         -------
-        Tuple[float, float, float]
-            A tuple of three Floats representing the translation.
+        Model
+            A Model object.
         """
         ...
 
     @abaqus_method_doc
-    def replace(self, instanceOf: Part, applyConstraints: Boolean = True):
-        """This method replaces one instance with an instance of another part.
+    def ModelFromNastranFile(
+        self,
+        modelName: str,
+        inputFileName: str,
+        sectionConsolidation: Literal[C.PRESERVE_SECTION, C.GROUP_BY_MATERIAL, C.NONE] = PRESERVE_SECTION,
+        preIntegratedShell: Boolean = OFF,
+        weightMassScaling: Boolean = ON,
+        loadCases: Boolean = ON,
+        coupleBeamOffsets: Boolean = ON,
+        cbar: str = B31,
+        cquad4: str = S4,
+        chexa: str = C3D8I,
+        ctetra: str = C3D10,
+        keepTranslatedFiles: Boolean = ON,
+    ):
+        """This method creates a Model object by reading the keywords in a Nastran bulk data file or Nastran
+        input file and creating any corresponding Abaqus/CAE objects. The default values is discussed in
+        following and can be defined alternatively in the Abaqus environment file as the one used for the
+        translator from Nastran to Abaqus. For more information, see Translating Nastran data to Abaqus files.
 
-        Parameters
-        ----------
-        instanceOf
-            A Part object specifying which Part will be instanced in place of the original Part.
-        applyConstraints
-            A Boolean specifying whether to apply existing constraints on the new instance or to
-            position the new instance in the same place as the original instance. The default value
-            is True. A value of False indicates that constraints applies to the instance are deleted
-            will be deleted from the feature list.
-        """
-        ...
+        .. note::
+            This function can be accessed by::
 
-    @abaqus_method_doc
-    def rotateAboutAxis(self, axisPoint: Sequence[float], axisDirection: Sequence[float], angle: float):
-        """This method translates an instance by the specified amount.
+                mdb.Model
 
         Parameters
         ----------
-        axisPoint
-            A sequence of three Floats specifying the **X**, **Y**, and **Z** coordinates of a point on
-            the axis.
-        axisDirection
-            A sequence of three Floats specifying the direction vector of the axis.
-        angle
-            A Float specifying the rotation angle in degrees. Use the right-hand rule to determine
-            the direction.
-        """
-        ...
+        modelName
+            A String specifying the repository key.
+        inputFileName
+            A String specifying the name of the Nastran input file (including the .bdf, .dat, .nas,
+            .nastran, .blk, .bulk extension) to be read into the new model. This String can also be
+            the full path to the Nastran input file if it is located in another directory.
+        sectionConsolidation
+            A SymbolicConstant specifying the method used to create shell section. Possible values
+            are PRESERVE_SECTION, GROUP_BY_MATERIAL, and NONE. If PRESERVE_SECTION is used, an
+            Abaqus section is created corresponding to each shell property ID. If GROUP_BY_MATERIAL
+            is used, a single Abaqus section is created for all homogeneous elements referencing the
+            same material. In both cases, material orientations and offsets are created using
+            discrete fields. If NONE is used, a separate shell section is created for each
+            combination of orientation, material offset, and/or thickness. The default is
+            PRESERVE_SECTION.
+        preIntegratedShell
+            A Boolean specifying whether the pre-integrated shell section is created in default for
+            shell element. The default value is OFF.
+        weightMassScaling
+            A Boolean specifying whether the value on the Nastran data line PARAM, WTMASS is used as
+            a multiplier for all density, mass, and rotary inertia values created in the Abaqus
+            input file. The default value is ON.
+        loadCases
+            A Boolean specifying whether each SUBCASE for linear static analyses is translated to a
+            LOAD CASE option, and all such LOAD CASE options are grouped in a single STEP option.
+            The default value is ON.
+        coupleBeamOffsets
+            A Boolean specifying whether to translate the beam element connectivity to newly created
+            nodes at the offset location and rigidly coupling the new and original nodes. If not,
+            beam element offsets are translated to the CENTROID and SHEAR CENTER options, which are
+            suboptions of the BEAM GENERAL SECTION option. The default value is ON. When the beam
+            element references a PBARL or PBEAML property or if the beam offset has a significant
+            component in the direction of the beam axis, the setting for this argument is always ON.
+        cbar
+            A String specifying the 2-node beam that is created from CBAR and CBEAM elements.
+            Possible values are B31 and B33. The default is B31.
+        cquad4
+            A String specifying the 4-node shell that is created from CQUAD4 elements. Possible
+            values are S4 and S4R. The default is S4. If a reduced-integration element is chosen,
+            the enhanced hourglass formulation is applied automatically.
+        chexa
+            A String specifying the 8-node brick that is created from CHEXA elements. Possible
+            values are C3D8I, C3D8 and C3D8R. The default is C3D8I. If a reduced-integration element
+            is chosen, the enhanced hourglass formulation is applied automatically.
+        ctetra
+            A String specifying the 10-node tetrahedron that is created from CTETRA elements.
+            Possible values are C3D10 and C3D10M. The default is C3D10.
+        keepTranslatedFiles
+            A Boolean specifying whether to keep the generated Abaqus input file after the model is
+            created from the Nastran input file. The default value is ON.
 
-    @abaqus_method_doc
-    def translate(self, vector: tuple):
-        """This method translates an instance by the specified amount.
-
-        Parameters
-        ----------
-        vector
-            A sequence of three Floats specifying a translation vector.
+        Returns
+        -------
+        Model
+            A Model object.
         """
         ...
 
     @abaqus_method_doc
-    def translateTo(
+    def setValues(
         self,
-        movableList: tuple,
-        fixedList: tuple,
-        direction: tuple,
-        clearance: float,
-        vector: tuple = (),
+        description: str = "",
+        noPartsInputFile: Boolean = OFF,
+        absoluteZero: Optional[float] = None,
+        stefanBoltzmann: Optional[float] = None,
+        waveFormulation: Literal[C.SCATTERED, C.NOT_SET, C.TOTAL] = NOT_SET,
+        universalGas: Optional[float] = None,
+        restartJob: str = "",
+        restartStep: str = "",
+        restartIncrement: Optional[Literal[C.STEP_END]] = None,
+        endRestartStep: Boolean = OFF,
+        globalJob: str = "",
+        shellToSolid: Boolean = OFF,
+        copyConstraints: Boolean = OFF,
+        copyConnectors: Boolean = OFF,
+        copyInteractions: Boolean = OFF,
     ):
-        """This method translates an instance along the specified direction until it is in contact with a fixed
-        instance.
+        """This method modifies the Model object.
 
         Parameters
         ----------
-        movableList
-            A sequence of Face or Edge objects on the part instance to be moved.
-        fixedList
-            A sequence of Face or Edge objects on the part instances to remain fixed.
-        direction
-            A sequence of three Floats specifying the direction of contact.
-        clearance
-            A Float specifying the distance between the two faces along the direction of contact.
-        vector
-            A sequence of three Floats specifying a translation vector. If this argument is
-            specified, the movable instance will be translated by the specified amount without
-            solving for the actual contact.
-
-        Returns
-        -------
-        feature: Feature
-            A Feature object
+        description
+            A String specifying the purpose and contents of the Model object. The default value is
+            an empty string.
+        noPartsInputFile
+            A Boolean specifying whether an input file should be written without parts and
+            assemblies. The default value is OFF.
+        absoluteZero
+            None or a Float specifying the absolute zero constant. The default value is None.
+        stefanBoltzmann
+            None or a Float specifying the Stefan-Boltzmann constant. The default value is None.
+        waveFormulation
+            A SymbolicConstant specifying the type of incident wave formulation to be used in
+            acoustic problems. Possible values are NOT_SET, SCATTERED, and TOTAL. The default value
+            is NOT_SET.
+        universalGas
+            None or a Float specifying the universal gas constant. The default value is None.
+        restartJob
+            A String specifying the name of the job that generated the restart data.
+        restartStep
+            A String specifying the name of the step where the restart analysis will start.
+        restartIncrement
+            An Int specifying the increment, interval, iteration or cycle where the restart analysis
+            will start. To select the end of the step use the SymbolicConstant STEP_END.
+        endRestartStep
+            A Boolean specifying that the step specified by **restartStep** should be terminated at
+            the increment specified by **restartIncrement**.
+        globalJob
+            A String specifying the name of the job that generated the results for the global model.
+        shellToSolid
+            A Boolean specifying that a shell global model drives a solid submodel.
+        copyConstraints
+            A Boolean specifying whether to copy the constraints created in the model to the model
+            that instances this model.
+        copyConnectors
+            A Boolean specifying whether to copy the connectors created in the model to the model
+            that instances this model
+        copyInteractions
+            A Boolean specifying whether to copy the interactions created in the model to the model
+            that instances this model.
         """
         ...
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/BasicGeometryPart.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/BasicGeometryPart.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/Cell.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/Cell.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/CellArray.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/CellArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/Edge.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/Edge.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/EdgeArray.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/EdgeArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/Face.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/Face.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/FaceArray.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/FaceArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/IgnoredEdge.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/IgnoredEdge.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/IgnoredEdgeArray.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/IgnoredEdgeArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/IgnoredVertex.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/IgnoredVertex.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/IgnoredVertexArray.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/IgnoredVertexArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/InterestingPoint.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/InterestingPoint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/ReferencePoint.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/ReferencePoint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/Transform.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/Transform.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/Vertex.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/Vertex.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BasicGeometry/VertexArray.py` & `abqpy-2023.5.2/src/abaqus/BasicGeometry/VertexArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/ArbitraryProfile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/ArbitraryProfile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/BeamSectionProfileModel.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/BeamSectionProfileModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/BeamSectionProfileOdb.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/BeamSectionProfileOdb.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/BoxProfile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/BoxProfile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/CircularProfile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/CircularProfile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/GeneralizedProfile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/GeneralizedProfile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/HexagonalProfile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/HexagonalProfile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/IProfile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/IProfile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/LProfile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/LProfile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/PipeProfile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/PipeProfile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/Profile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/Profile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/RectangularProfile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/RectangularProfile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/TProfile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/TProfile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BeamSectionProfile/TrapezoidalProfile.py` & `abqpy-2023.5.2/src/abaqus/BeamSectionProfile/TrapezoidalProfile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/AccelerationBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/AccelerationBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/AccelerationBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/AccelerationBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/AccelerationBaseMotionBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/AccelerationBaseMotionBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/AccelerationBaseMotionBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/AccelerationBaseMotionBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/AcousticPressureBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/AcousticPressureBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/AcousticPressureBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/AcousticPressureBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/BoundaryCondition.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/BoundaryCondition.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/BoundaryConditionModel.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/BoundaryConditionModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/BoundaryConditionState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/BoundaryConditionState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConcentrationBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConcentrationBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConcentrationBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConcentrationBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnAccelerationBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnAccelerationBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnAccelerationBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnAccelerationBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnDisplacementBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnDisplacementBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnDisplacementBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnDisplacementBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnVelocityBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnVelocityBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/ConnVelocityBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/ConnVelocityBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/DisplacementBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/DisplacementBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/DisplacementBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/DisplacementBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/DisplacementBaseMotionBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/DisplacementBaseMotionBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/DisplacementBaseMotionBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/DisplacementBaseMotionBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/ElectricPotentialBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/ElectricPotentialBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/ElectricPotentialBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/ElectricPotentialBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/EulerianBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/EulerianBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/EulerianBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/EulerianBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/EulerianMotionBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/EulerianMotionBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/EulerianMotionBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/EulerianMotionBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/FluidCavityPressureBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/FluidCavityPressureBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/FluidCavityPressureBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/FluidCavityPressureBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/MagneticVectorPotentialBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/MagneticVectorPotentialBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/MaterialFlowBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/MaterialFlowBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/MaterialFlowBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/MaterialFlowBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/PorePressureBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/PorePressureBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/PorePressureBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/PorePressureBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/RetainedNodalDofsBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/RetainedNodalDofsBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/SecondaryBaseBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/SecondaryBaseBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/SecondaryBaseBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/SecondaryBaseBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/SubmodelBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/SubmodelBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/SubmodelBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/SubmodelBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/TemperatureBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/TemperatureBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/TemperatureBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/TemperatureBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/TypeBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/TypeBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/TypeBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/TypeBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/VelocityBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/VelocityBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/VelocityBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/VelocityBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/VelocityBaseMotionBC.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/VelocityBaseMotionBC.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/BoundaryCondition/VelocityBaseMotionBCState.py` & `abqpy-2023.5.2/src/abaqus/BoundaryCondition/VelocityBaseMotionBCState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Calibration/Behavior.py` & `abqpy-2023.5.2/src/abaqus/Calibration/Behavior.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Calibration/Calibration.py` & `abqpy-2023.5.2/src/abaqus/Calibration/Calibration.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Calibration/CalibrationModel.py` & `abqpy-2023.5.2/src/abaqus/Calibration/CalibrationModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Calibration/DataSet.py` & `abqpy-2023.5.2/src/abaqus/Calibration/DataSet.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Canvas/AttributeColorMap.py` & `abqpy-2023.5.2/src/abaqus/Canvas/AttributeColorMap.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Canvas/CanvasSession.py` & `abqpy-2023.5.2/src/abaqus/Canvas/CanvasSession.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Canvas/DrawingArea.py` & `abqpy-2023.5.2/src/abaqus/Canvas/DrawingArea.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Canvas/Highlight.py` & `abqpy-2023.5.2/src/abaqus/Canvas/Highlight.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Canvas/ImageOptions.py` & `abqpy-2023.5.2/src/abaqus/Canvas/ImageOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Canvas/Layer.py` & `abqpy-2023.5.2/src/abaqus/Canvas/Layer.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Canvas/MovieOptions.py` & `abqpy-2023.5.2/src/abaqus/Canvas/MovieOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Canvas/Viewport.py` & `abqpy-2023.5.2/src/abaqus/Canvas/Viewport.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Canvas/ViewportBase.py` & `abqpy-2023.5.2/src/abaqus/Canvas/ViewportBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/CDCTerm.py` & `abqpy-2023.5.2/src/abaqus/Connector/CDCTerm.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorBehaviorOption.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorBehaviorOption.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorDamage.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorDamage.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorDamping.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorDamping.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorElasticity.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorElasticity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorFailure.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorFailure.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorFriction.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorFriction.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorLock.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorLock.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorOptions.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorPlasticity.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorPlasticity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorPotential.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorPotential.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorSection.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/ConnectorStop.py` & `abqpy-2023.5.2/src/abaqus/Connector/ConnectorStop.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/DerivedComponent.py` & `abqpy-2023.5.2/src/abaqus/Connector/DerivedComponent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Connector/TangentialBehavior.py` & `abqpy-2023.5.2/src/abaqus/Connector/TangentialBehavior.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Constraint/AdjustPoints.py` & `abqpy-2023.5.2/src/abaqus/Constraint/AdjustPoints.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Constraint/Constraint.py` & `abqpy-2023.5.2/src/abaqus/Constraint/Constraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Constraint/ConstraintModel.py` & `abqpy-2023.5.2/src/abaqus/Constraint/ConstraintModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Constraint/Coupling.py` & `abqpy-2023.5.2/src/abaqus/Constraint/Coupling.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Constraint/DisplayBody.py` & `abqpy-2023.5.2/src/abaqus/Constraint/DisplayBody.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Constraint/EmbeddedRegion.py` & `abqpy-2023.5.2/src/abaqus/Constraint/EmbeddedRegion.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Constraint/Equation.py` & `abqpy-2023.5.2/src/abaqus/Constraint/Equation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Constraint/MultipointConstraint.py` & `abqpy-2023.5.2/src/abaqus/Constraint/MultipointConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Constraint/RigidBody.py` & `abqpy-2023.5.2/src/abaqus/Constraint/RigidBody.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Constraint/ShellSolidCoupling.py` & `abqpy-2023.5.2/src/abaqus/Constraint/ShellSolidCoupling.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Constraint/Tie.py` & `abqpy-2023.5.2/src/abaqus/Constraint/Tie.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/CustomKernel/CommandRegister.py` & `abqpy-2023.5.2/src/abaqus/CustomKernel/CommandRegister.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/CustomKernel/RegisteredDictionary.py` & `abqpy-2023.5.2/src/abaqus/CustomKernel/RegisteredDictionary.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/CustomKernel/RegisteredList.py` & `abqpy-2023.5.2/src/abaqus/CustomKernel/RegisteredList.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/CustomKernel/RegisteredTuple.py` & `abqpy-2023.5.2/src/abaqus/CustomKernel/RegisteredTuple.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/CustomKernel/RepositorySupport.py` & `abqpy-2023.5.2/src/abaqus/CustomKernel/RepositorySupport.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Datum/Datum.py` & `abqpy-2023.5.2/src/abaqus/Datum/Datum.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Datum/DatumAxis.py` & `abqpy-2023.5.2/src/abaqus/Datum/DatumAxis.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Datum/DatumCsys.py` & `abqpy-2023.5.2/src/abaqus/Datum/DatumCsys.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Datum/DatumPlane.py` & `abqpy-2023.5.2/src/abaqus/Datum/DatumPlane.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Datum/DatumPoint.py` & `abqpy-2023.5.2/src/abaqus/Datum/DatumPoint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/DisplayGroup.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/DisplayGroup.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/DisplayGroupInstance.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/DisplayGroupInstance.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/DisplayGroupInstanceRepository.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/DisplayGroupInstanceRepository.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/DisplayGroupSession.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/DisplayGroupSession.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/Leaf.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/Leaf.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromConstraintNames.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromConstraintNames.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromDatums.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromDatums.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromDisplayGroup.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromDisplayGroup.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromElementLabels.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromElementLabels.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromElementSets.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromElementSets.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromElementVarRange.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromElementVarRange.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromGeometry.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromGeometry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromInstance.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromInstance.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromInstanceElementLabels.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromInstanceElementLabels.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromInstanceNodeLabels.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromInstanceNodeLabels.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromMeshElementLabels.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromMeshElementLabels.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromMeshNodeLabels.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromMeshNodeLabels.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromMeshSurfaceSets.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromMeshSurfaceSets.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromModelElemLabels.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromModelElemLabels.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromModelNodeLabels.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromModelNodeLabels.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromNodeLabels.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromNodeLabels.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromNodeSets.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromNodeSets.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromNodeVarRange.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromNodeVarRange.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbEdgePick.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbEdgePick.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementLayups.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementLayups.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementMaterials.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementMaterials.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementPick.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementPick.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementPlies.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementPlies.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementSections.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementSections.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbElementTypes.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbElementTypes.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromOdbNodePick.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromOdbNodePick.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromPartElementLabels.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromPartElementLabels.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromPartInstance.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromPartInstance.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromPartNodeLabels.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromPartNodeLabels.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromReferencePoint.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromReferencePoint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromSets.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromSets.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromSurfaceSets.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromSurfaceSets.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayGroup/LeafFromSurfaceVarRange.py` & `abqpy-2023.5.2/src/abaqus/DisplayGroup/LeafFromSurfaceVarRange.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/AssemblyDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/AssemblyDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/BCDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/BCDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/ConstraintDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/ConstraintDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/EngineeringFeatureDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/EngineeringFeatureDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/GeometricRestrictionDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/GeometricRestrictionDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/GeometryDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/GeometryDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/GraphicsInfo.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/GraphicsInfo.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/GraphicsOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/GraphicsOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/InteractionDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/InteractionDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/Light.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/Light.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/LightOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/LightOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/LoadDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/LoadDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/MeshDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/MeshDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/OptimizationTaskDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/OptimizationTaskDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/PartDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/PartDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/PredefinedFieldDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/PredefinedFieldDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/StopConditionDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/StopConditionDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/SymbolDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/SymbolDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/DisplayOptions/ViewportAnnotationOptions.py` & `abqpy-2023.5.2/src/abaqus/DisplayOptions/ViewportAnnotationOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EditMesh/MeshEditAssembly.py` & `abqpy-2023.5.2/src/abaqus/EditMesh/MeshEditAssembly.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EditMesh/MeshEditOptions.py` & `abqpy-2023.5.2/src/abaqus/EditMesh/MeshEditOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EditMesh/MeshEditPart.py` & `abqpy-2023.5.2/src/abaqus/EditMesh/MeshEditPart.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/AssembledFastener.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/AssembledFastener.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/ContourIntegral.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/ContourIntegral.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/Crack.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/Crack.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/DataImperfection.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/DataImperfection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/DebondVCCT.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/DebondVCCT.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/DiscreteFastener.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/DiscreteFastener.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/EngineeringFeature.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/EngineeringFeature.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/EngineeringFeatureBase.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/EngineeringFeatureBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/Fastener.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/Fastener.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/FileImperfection.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/FileImperfection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/HeatCapacitance.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/HeatCapacitance.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/Imperfection.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/Imperfection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/Inertia.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/Inertia.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/InputImperfection.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/InputImperfection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/NonstructuralMass.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/NonstructuralMass.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/PointFastener.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/PointFastener.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/PointMassInertia.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/PointMassInertia.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/SpringDashpot.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/SpringDashpot.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/SpringDashpotToGround.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/SpringDashpotToGround.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/TwoPointSpringDashpot.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/TwoPointSpringDashpot.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/EngineeringFeature/XFEMCrack.py` & `abqpy-2023.5.2/src/abaqus/EngineeringFeature/XFEMCrack.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Feature/Feature.py` & `abqpy-2023.5.2/src/abaqus/Feature/Feature.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Feature/FeatureOptions.py` & `abqpy-2023.5.2/src/abaqus/Feature/FeatureOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Field/AnalyticalField.py` & `abqpy-2023.5.2/src/abaqus/Field/AnalyticalField.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Field/DataTable.py` & `abqpy-2023.5.2/src/abaqus/Field/DataTable.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Field/DiscreteField.py` & `abqpy-2023.5.2/src/abaqus/Field/DiscreteField.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Field/ExpressionField.py` & `abqpy-2023.5.2/src/abaqus/Field/ExpressionField.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Field/Field.py` & `abqpy-2023.5.2/src/abaqus/Field/Field.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Field/FieldModel.py` & `abqpy-2023.5.2/src/abaqus/Field/FieldModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Field/MappedField.py` & `abqpy-2023.5.2/src/abaqus/Field/MappedField.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Field/OdbMeshRegionData.py` & `abqpy-2023.5.2/src/abaqus/Field/OdbMeshRegionData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/FieldReport/FieldReportOptions.py` & `abqpy-2023.5.2/src/abaqus/FieldReport/FieldReportOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/FieldReport/FieldReportSession.py` & `abqpy-2023.5.2/src/abaqus/FieldReport/FieldReportSession.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/FieldReport/FreeBodyReportOptions.py` & `abqpy-2023.5.2/src/abaqus/FieldReport/FreeBodyReportOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/FieldReport/OdbFieldVarList.py` & `abqpy-2023.5.2/src/abaqus/FieldReport/OdbFieldVarList.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/FieldReport/writeFieldReport.py` & `abqpy-2023.5.2/src/abaqus/FieldReport/writeFieldReport.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/FieldReport/writeFreeBodyReport.py` & `abqpy-2023.5.2/src/abaqus/FieldReport/writeFreeBodyReport.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Filter/ButterworthFilter.py` & `abqpy-2023.5.2/src/abaqus/Filter/ButterworthFilter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Filter/Chebyshev1Filter.py` & `abqpy-2023.5.2/src/abaqus/Filter/Chebyshev1Filter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Filter/Chebyshev2Filter.py` & `abqpy-2023.5.2/src/abaqus/Filter/Chebyshev2Filter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Filter/Filter.py` & `abqpy-2023.5.2/src/abaqus/Filter/Filter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Filter/FilterModel.py` & `abqpy-2023.5.2/src/abaqus/Filter/FilterModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Filter/FilterOdb.py` & `abqpy-2023.5.2/src/abaqus/Filter/FilterOdb.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Filter/OperatorFilter.py` & `abqpy-2023.5.2/src/abaqus/Filter/OperatorFilter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/InputFileParser/AbaqusNDarray.py` & `abqpy-2023.5.2/src/abaqus/InputFileParser/AbaqusNDarray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/InputFileParser/InputFile.py` & `abqpy-2023.5.2/src/abaqus/InputFileParser/InputFile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/InputFileParser/Keyword.py` & `abqpy-2023.5.2/src/abaqus/InputFileParser/Keyword.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/AcousticImpedance.py` & `abqpy-2023.5.2/src/abaqus/Interaction/AcousticImpedance.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/AcousticImpedanceProp.py` & `abqpy-2023.5.2/src/abaqus/Interaction/AcousticImpedanceProp.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/AcousticImpedanceState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/AcousticImpedanceState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ActuatorSensor.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ActuatorSensor.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ActuatorSensorProp.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ActuatorSensorProp.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ActuatorSensorState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ActuatorSensorState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/CavityRadiation.py` & `abqpy-2023.5.2/src/abaqus/Interaction/CavityRadiation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/CavityRadiationProp.py` & `abqpy-2023.5.2/src/abaqus/Interaction/CavityRadiationProp.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/CavityRadiationState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/CavityRadiationState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/CohesiveBehavior.py` & `abqpy-2023.5.2/src/abaqus/Interaction/CohesiveBehavior.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ConcentratedFilmCondition.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ConcentratedFilmCondition.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ConcentratedFilmConditionState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ConcentratedFilmConditionState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ConcentratedRadiationToAmbient.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ConcentratedRadiationToAmbient.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ConcentratedRadiationToAmbientState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ConcentratedRadiationToAmbientState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ContactDamage.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ContactDamage.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ContactDamping.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ContactDamping.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ContactExp.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ContactExp.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ContactProperty.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ContactProperty.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ContactPropertyAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ContactPropertyAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ContactStd.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ContactStd.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ContactTangentialBehavior.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ContactTangentialBehavior.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/CyclicSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Interaction/CyclicSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/CyclicSymmetryState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/CyclicSymmetryState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ElasticFoundation.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ElasticFoundation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ElasticFoundationState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ElasticFoundationState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ExpContactControl.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ExpContactControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ExpInitialization.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ExpInitialization.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FilmCondition.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FilmCondition.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FilmConditionProp.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FilmConditionProp.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FilmConditionState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FilmConditionState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FluidCavity.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FluidCavity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FluidCavityProperty.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FluidCavityProperty.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FluidCavityState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FluidCavityState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FluidExchange.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FluidExchange.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FluidExchangeProperty.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FluidExchangeProperty.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FluidExchangeState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FluidExchangeState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FluidInflator.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FluidInflator.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FluidInflatorProperty.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FluidInflatorProperty.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FluidInflatorState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FluidInflatorState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/FractureCriterion.py` & `abqpy-2023.5.2/src/abaqus/Interaction/FractureCriterion.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/GapElectricalConductance.py` & `abqpy-2023.5.2/src/abaqus/Interaction/GapElectricalConductance.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/GapHeatGeneration.py` & `abqpy-2023.5.2/src/abaqus/Interaction/GapHeatGeneration.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/GeometricProperties.py` & `abqpy-2023.5.2/src/abaqus/Interaction/GeometricProperties.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/IncidentWave.py` & `abqpy-2023.5.2/src/abaqus/Interaction/IncidentWave.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/IncidentWaveProperty.py` & `abqpy-2023.5.2/src/abaqus/Interaction/IncidentWaveProperty.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/IncidentWaveState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/IncidentWaveState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/InitializationAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/InitializationAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/Interaction.py` & `abqpy-2023.5.2/src/abaqus/Interaction/Interaction.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/InteractionContactControlModel.py` & `abqpy-2023.5.2/src/abaqus/Interaction/InteractionContactControlModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/InteractionContactInitializationModel.py` & `abqpy-2023.5.2/src/abaqus/Interaction/InteractionContactInitializationModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/InteractionContactStabilizationModel.py` & `abqpy-2023.5.2/src/abaqus/Interaction/InteractionContactStabilizationModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/InteractionModel.py` & `abqpy-2023.5.2/src/abaqus/Interaction/InteractionModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/InteractionPropertyModel.py` & `abqpy-2023.5.2/src/abaqus/Interaction/InteractionPropertyModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/InteractionState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/InteractionState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/MainSecondaryAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/MainSecondaryAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ModelChange.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ModelChange.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/NormalBehavior.py` & `abqpy-2023.5.2/src/abaqus/Interaction/NormalBehavior.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/PolarityAssignments.py` & `abqpy-2023.5.2/src/abaqus/Interaction/PolarityAssignments.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/PressurePenetration.py` & `abqpy-2023.5.2/src/abaqus/Interaction/PressurePenetration.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/PressurePenetrationState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/PressurePenetrationState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/Radiation.py` & `abqpy-2023.5.2/src/abaqus/Interaction/Radiation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/RadiationToAmbient.py` & `abqpy-2023.5.2/src/abaqus/Interaction/RadiationToAmbient.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/RadiationToAmbientState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/RadiationToAmbientState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/RegionPairs.py` & `abqpy-2023.5.2/src/abaqus/Interaction/RegionPairs.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SelfContactExp.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SelfContactExp.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SelfContactExpState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SelfContactExpState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SelfContactStd.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SelfContactStd.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SelfContactStdState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SelfContactStdState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SlidingFormulationAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SlidingFormulationAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SlidingTransitionAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SlidingTransitionAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SmoothingAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SmoothingAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/StabilizationAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/StabilizationAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/StdContactControl.py` & `abqpy-2023.5.2/src/abaqus/Interaction/StdContactControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/StdInitialization.py` & `abqpy-2023.5.2/src/abaqus/Interaction/StdInitialization.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/StdStabilization.py` & `abqpy-2023.5.2/src/abaqus/Interaction/StdStabilization.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/StdXplCosimulation.py` & `abqpy-2023.5.2/src/abaqus/Interaction/StdXplCosimulation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/StdXplCosimulationState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/StdXplCosimulationState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SurfaceBeamSmoothingAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SurfaceBeamSmoothingAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SurfaceCrushTriggerAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SurfaceCrushTriggerAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SurfaceFeatureAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SurfaceFeatureAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SurfaceFrictionAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SurfaceFrictionAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SurfaceOffsetAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SurfaceOffsetAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SurfaceThicknessAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SurfaceThicknessAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SurfaceToSurfaceContactExp.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SurfaceToSurfaceContactExp.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SurfaceToSurfaceContactStd.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SurfaceToSurfaceContactStd.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SurfaceToSurfaceExpState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SurfaceToSurfaceExpState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SurfaceToSurfaceStdState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SurfaceToSurfaceStdState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/SurfaceVertexCriteriaAssignment.py` & `abqpy-2023.5.2/src/abaqus/Interaction/SurfaceVertexCriteriaAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/ThermalConductance.py` & `abqpy-2023.5.2/src/abaqus/Interaction/ThermalConductance.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/XFEMCrackGrowth.py` & `abqpy-2023.5.2/src/abaqus/Interaction/XFEMCrackGrowth.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Interaction/XFEMCrackGrowthState.py` & `abqpy-2023.5.2/src/abaqus/Interaction/XFEMCrackGrowthState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Job/Coexecution.py` & `abqpy-2023.5.2/src/abaqus/Job/Coexecution.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Job/Job.py` & `abqpy-2023.5.2/src/abaqus/Job/Job.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Job/JobFromInputFile.py` & `abqpy-2023.5.2/src/abaqus/Job/JobFromInputFile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Job/JobMdb.py` & `abqpy-2023.5.2/src/abaqus/Job/JobMdb.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Job/JobSession.py` & `abqpy-2023.5.2/src/abaqus/Job/JobSession.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Job/Message.py` & `abqpy-2023.5.2/src/abaqus/Job/Message.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Job/ModelJob.py` & `abqpy-2023.5.2/src/abaqus/Job/ModelJob.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Job/OptimizationProcess.py` & `abqpy-2023.5.2/src/abaqus/Job/OptimizationProcess.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Job/Queue.py` & `abqpy-2023.5.2/src/abaqus/Job/Queue.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BodyCharge.py` & `abqpy-2023.5.2/src/abaqus/Load/BodyCharge.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BodyChargeState.py` & `abqpy-2023.5.2/src/abaqus/Load/BodyChargeState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BodyConcentrationFlux.py` & `abqpy-2023.5.2/src/abaqus/Load/BodyConcentrationFlux.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BodyConcentrationFluxState.py` & `abqpy-2023.5.2/src/abaqus/Load/BodyConcentrationFluxState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BodyCurrent.py` & `abqpy-2023.5.2/src/abaqus/Load/BodyCurrent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BodyCurrentDensity.py` & `abqpy-2023.5.2/src/abaqus/Load/BodyCurrentDensity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BodyCurrentState.py` & `abqpy-2023.5.2/src/abaqus/Load/BodyCurrentState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BodyForce.py` & `abqpy-2023.5.2/src/abaqus/Load/BodyForce.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BodyForceState.py` & `abqpy-2023.5.2/src/abaqus/Load/BodyForceState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BodyHeatFlux.py` & `abqpy-2023.5.2/src/abaqus/Load/BodyHeatFlux.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BodyHeatFluxState.py` & `abqpy-2023.5.2/src/abaqus/Load/BodyHeatFluxState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BoltLoad.py` & `abqpy-2023.5.2/src/abaqus/Load/BoltLoad.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/BoltLoadState.py` & `abqpy-2023.5.2/src/abaqus/Load/BoltLoadState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcCharge.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcCharge.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcConcFlux.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcConcFlux.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcCurrent.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcCurrent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcCurrentState.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcCurrentState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcPoreFluid.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcPoreFluid.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcentratedChargeState.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcentratedChargeState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcentratedConcentrationFluxState.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcentratedConcentrationFluxState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcentratedForce.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcentratedForce.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcentratedForceState.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcentratedForceState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcentratedHeatFlux.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcentratedHeatFlux.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcentratedHeatFluxState.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcentratedHeatFluxState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConcentratedPoreFluidState.py` & `abqpy-2023.5.2/src/abaqus/Load/ConcentratedPoreFluidState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConnectorForce.py` & `abqpy-2023.5.2/src/abaqus/Load/ConnectorForce.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConnectorForceState.py` & `abqpy-2023.5.2/src/abaqus/Load/ConnectorForceState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConnectorMoment.py` & `abqpy-2023.5.2/src/abaqus/Load/ConnectorMoment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ConnectorMomentState.py` & `abqpy-2023.5.2/src/abaqus/Load/ConnectorMomentState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/CoriolisForce.py` & `abqpy-2023.5.2/src/abaqus/Load/CoriolisForce.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/CoriolisForceState.py` & `abqpy-2023.5.2/src/abaqus/Load/CoriolisForceState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/Gravity.py` & `abqpy-2023.5.2/src/abaqus/Load/Gravity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/GravityState.py` & `abqpy-2023.5.2/src/abaqus/Load/GravityState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/HydrostaticFluidFlowState.py` & `abqpy-2023.5.2/src/abaqus/Load/HydrostaticFluidFlowState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/InertiaRelief.py` & `abqpy-2023.5.2/src/abaqus/Load/InertiaRelief.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/InertiaReliefState.py` & `abqpy-2023.5.2/src/abaqus/Load/InertiaReliefState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/InwardVolAccel.py` & `abqpy-2023.5.2/src/abaqus/Load/InwardVolAccel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/InwardVolAccelState.py` & `abqpy-2023.5.2/src/abaqus/Load/InwardVolAccelState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/LineLoad.py` & `abqpy-2023.5.2/src/abaqus/Load/LineLoad.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/LineLoadState.py` & `abqpy-2023.5.2/src/abaqus/Load/LineLoadState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/Load.py` & `abqpy-2023.5.2/src/abaqus/Load/Load.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/LoadCase.py` & `abqpy-2023.5.2/src/abaqus/Load/LoadCase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/LoadModel.py` & `abqpy-2023.5.2/src/abaqus/Load/LoadModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/LoadState.py` & `abqpy-2023.5.2/src/abaqus/Load/LoadState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/LoadStep.py` & `abqpy-2023.5.2/src/abaqus/Load/LoadStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/Moment.py` & `abqpy-2023.5.2/src/abaqus/Load/Moment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/MomentState.py` & `abqpy-2023.5.2/src/abaqus/Load/MomentState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/PEGLoad.py` & `abqpy-2023.5.2/src/abaqus/Load/PEGLoad.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/PEGLoadState.py` & `abqpy-2023.5.2/src/abaqus/Load/PEGLoadState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/PipePressure.py` & `abqpy-2023.5.2/src/abaqus/Load/PipePressure.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/PipePressureState.py` & `abqpy-2023.5.2/src/abaqus/Load/PipePressureState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/Pressure.py` & `abqpy-2023.5.2/src/abaqus/Load/Pressure.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/PressureState.py` & `abqpy-2023.5.2/src/abaqus/Load/PressureState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/RotationalBodyForce.py` & `abqpy-2023.5.2/src/abaqus/Load/RotationalBodyForce.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/RotationalBodyForceState.py` & `abqpy-2023.5.2/src/abaqus/Load/RotationalBodyForceState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ShellEdgeLoad.py` & `abqpy-2023.5.2/src/abaqus/Load/ShellEdgeLoad.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/ShellEdgeLoadState.py` & `abqpy-2023.5.2/src/abaqus/Load/ShellEdgeLoadState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SubmodelSB.py` & `abqpy-2023.5.2/src/abaqus/Load/SubmodelSB.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SubmodelSBState.py` & `abqpy-2023.5.2/src/abaqus/Load/SubmodelSBState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SubstructureLoad.py` & `abqpy-2023.5.2/src/abaqus/Load/SubstructureLoad.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SubstructureLoadState.py` & `abqpy-2023.5.2/src/abaqus/Load/SubstructureLoadState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfaceCharge.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfaceCharge.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfaceChargeState.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfaceChargeState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfaceConcentrationFlux.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfaceConcentrationFlux.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfaceConcentrationFluxState.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfaceConcentrationFluxState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfaceCurrent.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfaceCurrent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfaceCurrentDensity.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfaceCurrentDensity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfaceCurrentState.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfaceCurrentState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfaceHeatFlux.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfaceHeatFlux.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfaceHeatFluxState.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfaceHeatFluxState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfacePoreFluid.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfacePoreFluid.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfacePoreFluidState.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfacePoreFluidState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfaceTraction.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfaceTraction.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Load/SurfaceTractionState.py` & `abqpy-2023.5.2/src/abaqus/Load/SurfaceTractionState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Acoustic/AcousticMedium.py` & `abqpy-2023.5.2/src/abaqus/Material/Acoustic/AcousticMedium.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Density/Density.py` & `abqpy-2023.5.2/src/abaqus/Material/Density/Density.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/HyperFoam/Hyperfoam.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/HyperFoam/Hyperfoam.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/Hyperelastic.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/Hyperelastic.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/CombinedTestData.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/CombinedTestData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/Hysteresis.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/Hysteresis.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/Viscoelastic.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/HyperElastic/ViscoElastic/Viscoelastic.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/HypoElastic/Hypoelastic.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/HypoElastic/Hypoelastic.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/Linear/Elastic.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/Linear/Elastic.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/Linear/FailStrain.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/Linear/FailStrain.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/Linear/FailStress.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/Linear/FailStress.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/LowDensityFoam/LowDensityFoam.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/LowDensityFoam/LowDensityFoam.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/Porous/PorousElastic.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/Porous/PorousElastic.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Elastic/SuperElastic/SuperElasticity.py` & `abqpy-2023.5.2/src/abaqus/Material/Elastic/SuperElastic/SuperElasticity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Electromagnetic/Dielectric.py` & `abqpy-2023.5.2/src/abaqus/Material/Electromagnetic/Dielectric.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Electromagnetic/ElectricalConductivity.py` & `abqpy-2023.5.2/src/abaqus/Material/Electromagnetic/ElectricalConductivity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Electromagnetic/MagneticPermeability.py` & `abqpy-2023.5.2/src/abaqus/Material/Electromagnetic/MagneticPermeability.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Electromagnetic/Piezoelectric.py` & `abqpy-2023.5.2/src/abaqus/Material/Electromagnetic/Piezoelectric.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Eos/DetonationPoint.py` & `abqpy-2023.5.2/src/abaqus/Material/Eos/DetonationPoint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Eos/Eos.py` & `abqpy-2023.5.2/src/abaqus/Material/Eos/Eos.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Eos/EosCompaction.py` & `abqpy-2023.5.2/src/abaqus/Material/Eos/EosCompaction.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Gap/GapConductance.py` & `abqpy-2023.5.2/src/abaqus/Material/Gap/GapConductance.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Gap/GapConvection.py` & `abqpy-2023.5.2/src/abaqus/Material/Gap/GapConvection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Gap/GapFlow.py` & `abqpy-2023.5.2/src/abaqus/Material/Gap/GapFlow.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Gap/GapRadiation.py` & `abqpy-2023.5.2/src/abaqus/Material/Gap/GapRadiation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Gasket/ContactArea.py` & `abqpy-2023.5.2/src/abaqus/Material/Gasket/ContactArea.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Gasket/GasketMembraneElastic.py` & `abqpy-2023.5.2/src/abaqus/Material/Gasket/GasketMembraneElastic.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Gasket/GasketThicknessBehavior.py` & `abqpy-2023.5.2/src/abaqus/Material/Gasket/GasketThicknessBehavior.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Gasket/GasketTransverseShearElastic.py` & `abqpy-2023.5.2/src/abaqus/Material/Gasket/GasketTransverseShearElastic.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/Conductivity.py` & `abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/Conductivity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/HeatGeneration.py` & `abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/HeatGeneration.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/InelasticHeatFraction.py` & `abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/InelasticHeatFraction.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/JouleHeatFraction.py` & `abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/JouleHeatFraction.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/LatentHeat.py` & `abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/LatentHeat.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/HeatTransfer/SpecificHeat.py` & `abqpy-2023.5.2/src/abaqus/Material/HeatTransfer/SpecificHeat.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/MassDiffusion/Diffusivity.py` & `abqpy-2023.5.2/src/abaqus/Material/MassDiffusion/Diffusivity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/MassDiffusion/PressureEffect.py` & `abqpy-2023.5.2/src/abaqus/Material/MassDiffusion/PressureEffect.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/MassDiffusion/Solubility.py` & `abqpy-2023.5.2/src/abaqus/Material/MassDiffusion/Solubility.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/MassDiffusion/SoretEffect.py` & `abqpy-2023.5.2/src/abaqus/Material/MassDiffusion/SoretEffect.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Material.py` & `abqpy-2023.5.2/src/abaqus/Material/Material.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/MaterialBase.py` & `abqpy-2023.5.2/src/abaqus/Material/MaterialBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/MaterialModel.py` & `abqpy-2023.5.2/src/abaqus/Material/MaterialModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/MaterialOdb.py` & `abqpy-2023.5.2/src/abaqus/Material/MaterialOdb.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Mechanical/Damping.py` & `abqpy-2023.5.2/src/abaqus/Material/Mechanical/Damping.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Mechanical/Expansion.py` & `abqpy-2023.5.2/src/abaqus/Material/Mechanical/Expansion.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Mechanical/PoreFluidExpansion.py` & `abqpy-2023.5.2/src/abaqus/Material/Mechanical/PoreFluidExpansion.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Mechanical/Viscosity/Trs.py` & `abqpy-2023.5.2/src/abaqus/Material/Mechanical/Viscosity/Trs.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Mechanical/Viscosity/Viscosity.py` & `abqpy-2023.5.2/src/abaqus/Material/Mechanical/Viscosity/Viscosity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Multiscale/MeanFieldHomogenization.py` & `abqpy-2023.5.2/src/abaqus/Material/Multiscale/MeanFieldHomogenization.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Multiscale/MeanFieldInclusion.py` & `abqpy-2023.5.2/src/abaqus/Material/Multiscale/MeanFieldInclusion.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Multiscale/MeanFieldMatrix.py` & `abqpy-2023.5.2/src/abaqus/Material/Multiscale/MeanFieldMatrix.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Multiscale/MeanFieldVoid.py` & `abqpy-2023.5.2/src/abaqus/Material/Multiscale/MeanFieldVoid.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/BrittleCracking.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/BrittleCracking.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/BrittleFailure.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/BrittleFailure.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/BrittleShear.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/BrittleShear.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/Concrete.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/Concrete.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ConcreteCompressionDamage.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ConcreteCompressionDamage.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ConcreteCompressionHardening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ConcreteCompressionHardening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ConcreteDamagedPlasticity.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ConcreteDamagedPlasticity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ConcreteTensionDamage.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ConcreteTensionDamage.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ConcreteTensionStiffening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ConcreteTensionStiffening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/FailureRatios.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/FailureRatios.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/ShearRetention.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/ShearRetention.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Concrete/TensionStiffening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Concrete/TensionStiffening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Creep/Creep.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Creep/Creep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/CriticalStateClay/ClayHardening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/CriticalStateClay/ClayHardening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/CriticalStateClay/ClayPlasticity.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/CriticalStateClay/ClayPlasticity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushStress/CrushStress.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushStress/CrushStress.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushStress/CrushStressVelocityFactor.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushStress/CrushStressVelocityFactor.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushableFoam/CrushableFoam.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushableFoam/CrushableFoam.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/CrushableFoam/CrushableFoamHardening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/CrushableFoam/CrushableFoamHardening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPrager.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPrager.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPragerCreep.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPragerCreep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPragerHardening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/Extended/DruckerPragerHardening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/Extended/TriaxialTestData.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/Extended/TriaxialTestData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapCreepCohesion.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapCreepCohesion.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapCreepConsolidation.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapCreepConsolidation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapHardening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapHardening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapPlasticity.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/DruckerPrager/ModifiedCap/CapPlasticity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Annealing/AnnealTemperature.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Annealing/AnnealTemperature.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/CastIron/CastIronCompressionHardening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/CastIron/CastIronCompressionHardening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/CastIron/CastIronPlasticity.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/CastIron/CastIronPlasticity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/CastIron/CastIronTensionHardening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/CastIron/CastIronTensionHardening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Cyclic/CycledPlastic.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Cyclic/CycledPlastic.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Cyclic/CyclicHardening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Cyclic/CyclicHardening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Deformation/DeformationPlasticity.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Deformation/DeformationPlasticity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/ORNL/Ornl.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/ORNL/Ornl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Porous/PorousFailureCriteria.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Porous/PorousFailureCriteria.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Porous/PorousMetalPlasticity.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Porous/PorousMetalPlasticity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/Porous/VoidNucleation.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/Porous/VoidNucleation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/RateDependent/RateDependent.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/RateDependent/RateDependent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Metal/TwoLayerViscoPlasticity/Viscous.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Metal/TwoLayerViscoPlasticity/Viscous.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/MohrCoulomb/MohrCoulombHardening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/MohrCoulomb/MohrCoulombHardening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/MohrCoulomb/MohrCoulombPlasticity.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/MohrCoulomb/MohrCoulombPlasticity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/MohrCoulomb/TensionCutOff.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/MohrCoulomb/TensionCutOff.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Plastic.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Plastic.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/PlasticityCorrection.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/PlasticityCorrection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Potential.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Potential.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/SuperElastic/SuperElasticHardening.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/SuperElastic/SuperElasticHardening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/SuperElastic/SuperElasticHardeningModifications.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/SuperElastic/SuperElasticHardeningModifications.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/Swelling/Swelling.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/Swelling/Swelling.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Plastic/TensileFailure.py` & `abqpy-2023.5.2/src/abaqus/Material/Plastic/TensileFailure.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/FluidLeakoff.py` & `abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/FluidLeakoff.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Gel.py` & `abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Gel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/MoistureSwelling/MoistureSwelling.py` & `abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/MoistureSwelling/MoistureSwelling.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Permeability/Permeability.py` & `abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Permeability/Permeability.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Permeability/SaturationDependence.py` & `abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Permeability/SaturationDependence.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Permeability/VelocityDependence.py` & `abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Permeability/VelocityDependence.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/PorousBulkModuli.py` & `abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/PorousBulkModuli.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/PoreFluidFlow/Sorption.py` & `abqpy-2023.5.2/src/abaqus/Material/PoreFluidFlow/Sorption.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/ProgressiveDamageFailure/DamageEvolution.py` & `abqpy-2023.5.2/src/abaqus/Material/ProgressiveDamageFailure/DamageEvolution.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/ProgressiveDamageFailure/DamageInitiation.py` & `abqpy-2023.5.2/src/abaqus/Material/ProgressiveDamageFailure/DamageInitiation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/ProgressiveDamageFailure/DamageStabilization.py` & `abqpy-2023.5.2/src/abaqus/Material/ProgressiveDamageFailure/DamageStabilization.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/ProgressiveDamageFailure/DamageStabilizationCohesive.py` & `abqpy-2023.5.2/src/abaqus/Material/ProgressiveDamageFailure/DamageStabilizationCohesive.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Ratios.py` & `abqpy-2023.5.2/src/abaqus/Material/Ratios.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/Regularization.py` & `abqpy-2023.5.2/src/abaqus/Material/Regularization.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/TestData/BiaxialTestData.py` & `abqpy-2023.5.2/src/abaqus/Material/TestData/BiaxialTestData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/TestData/MullinsEffect.py` & `abqpy-2023.5.2/src/abaqus/Material/TestData/MullinsEffect.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/TestData/PlanarTestData.py` & `abqpy-2023.5.2/src/abaqus/Material/TestData/PlanarTestData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/TestData/ShearTestData.py` & `abqpy-2023.5.2/src/abaqus/Material/TestData/ShearTestData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/TestData/SimpleShearTestData.py` & `abqpy-2023.5.2/src/abaqus/Material/TestData/SimpleShearTestData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/TestData/UniaxialTestData.py` & `abqpy-2023.5.2/src/abaqus/Material/TestData/UniaxialTestData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/TestData/VolumetricTestData.py` & `abqpy-2023.5.2/src/abaqus/Material/TestData/VolumetricTestData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/User/Depvar.py` & `abqpy-2023.5.2/src/abaqus/Material/User/Depvar.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/User/UserDefinedField.py` & `abqpy-2023.5.2/src/abaqus/Material/User/UserDefinedField.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/User/UserMaterial.py` & `abqpy-2023.5.2/src/abaqus/Material/User/UserMaterial.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/User/UserOutputVariables.py` & `abqpy-2023.5.2/src/abaqus/Material/User/UserOutputVariables.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Material/evaluateMaterial.py` & `abqpy-2023.5.2/src/abaqus/Material/evaluateMaterial.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mdb/Mdb.py` & `abqpy-2023.5.2/src/abaqus/Mdb/Mdb.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mdb/MdbBase.py` & `abqpy-2023.5.2/src/abaqus/Mdb/MdbBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mdb/MdbCommands.py` & `abqpy-2023.5.2/src/abaqus/Mdb/MdbCommands.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/ElemType.py` & `abqpy-2023.5.2/src/abaqus/Mesh/ElemType.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MeshAssembly.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MeshAssembly.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MeshEdge.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MeshEdge.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MeshEdgeArray.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MeshEdgeArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MeshElement.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MeshElement.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MeshElementArray.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MeshElementArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MeshFace.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MeshFace.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MeshFaceArray.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MeshFaceArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MeshNode.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MeshNode.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MeshNodeArray.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MeshNodeArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MeshPart.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MeshPart.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MeshStats.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MeshStats.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Mesh/MesherOptions.py` & `abqpy-2023.5.2/src/abaqus/Mesh/MesherOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Messaging/DataObject.py` & `abqpy-2023.5.2/src/abaqus/Messaging/DataObject.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Messaging/MonitorMgr.py` & `abqpy-2023.5.2/src/abaqus/Messaging/MonitorMgr.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Model/KeywordBlock.py` & `abqpy-2023.5.2/src/abaqus/Model/KeywordBlock.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Model/Model.py` & `abqpy-2023.5.2/src/abaqus/Model/Model.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Model/ModelBase.py` & `abqpy-2023.5.2/src/abaqus/Step/StaticRiksStep.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,510 +1,448 @@
 from typing import Dict, Optional
 
 from typing_extensions import Literal
 
 from abqpy.decorators import abaqus_class_doc, abaqus_method_doc
 
-from ..Adaptivity.AdaptiveMeshConstraint import AdaptiveMeshConstraint
-from ..Adaptivity.AdaptiveMeshControl import AdaptiveMeshControl
-from ..Adaptivity.RemeshingRule import RemeshingRule
-from ..Amplitude.Amplitude import Amplitude
-from ..Assembly.Assembly import Assembly
-from ..BeamSectionProfile.Profile import Profile
-from ..BoundaryCondition.BoundaryCondition import BoundaryCondition
-from ..Calibration.Calibration import Calibration
-from ..Constraint.Constraint import Constraint
-from ..Feature.FeatureOptions import FeatureOptions
-from ..Field.AnalyticalField import AnalyticalField
-from ..Field.DiscreteField import DiscreteField
-from ..Filter.Filter import Filter
-from ..Interaction.ContactControl import ContactControl
-from ..Interaction.ContactInitialization import ContactInitialization
-from ..Interaction.ContactProperty import ContactProperty
-from ..Interaction.ContactStabilization import ContactStabilization
-from ..Interaction.Interaction import Interaction
-from ..Load.Load import Load
-from ..Material.Material import Material
-from ..Optimization.OptimizationTask import OptimizationTask
-from ..Part.Part import Part
-from ..PredefinedField.PredefinedField import PredefinedField
-from ..Section.Section import Section
-from ..Sketcher.ConstrainedSketch import ConstrainedSketch
-from ..Step.InitialStep import InitialStep
-from ..Step.Step import Step
-from ..StepOutput.FieldOutputRequest import FieldOutputRequest
-from ..StepOutput.HistoryOutputRequest import HistoryOutputRequest
-from ..StepOutput.IntegratedOutputSection import IntegratedOutputSection
-from ..StepOutput.TimePoint import TimePoint
-from ..TableCollection.EventSeriesData import EventSeriesData
-from ..TableCollection.EventSeriesType import EventSeriesType
-from ..TableCollection.TableCollection import TableCollection
+from ..Adaptivity.AdaptiveMeshConstraintState import AdaptiveMeshConstraintState
+from ..Adaptivity.AdaptiveMeshDomain import AdaptiveMeshDomain
+from ..BoundaryCondition.BoundaryConditionState import BoundaryConditionState
+from ..Load.LoadCase import LoadCase
+from ..Load.LoadState import LoadState
+from ..PredefinedField.PredefinedFieldState import PredefinedFieldState
+from ..Region.Region import Region
+from ..StepMiscellaneous.Control import Control
+from ..StepMiscellaneous.SolverControl import SolverControl
+from ..StepOutput.DiagnosticPrint import DiagnosticPrint
+from ..StepOutput.FieldOutputRequestState import FieldOutputRequestState
+from ..StepOutput.HistoryOutputRequestState import HistoryOutputRequestState
+from ..StepOutput.Monitor import Monitor
+from ..StepOutput.Restart import Restart
 from ..UtilityAndView.abaqusConstants import (
-    B31,
-    C3D8I,
-    C3D10,
-    NOT_SET,
+    AUTOMATIC,
+    LINEAR,
     OFF,
-    ON,
-    PRESERVE_SECTION,
-    S4,
-    STANDARD_EXPLICIT,
+    PROPAGATED,
+    SOLVER_DEFAULT,
     Boolean,
     SymbolicConstant,
 )
 from ..UtilityAndView.abaqusConstants import abaqusConstants as C
-from .KeywordBlock import KeywordBlock
+from .AnalysisStep import AnalysisStep
 
 
 @abaqus_class_doc
-class ModelBase:
-    """Abaqus creates a Model object named `Model-1` when a session is started.
+class StaticRiksStep(AnalysisStep):
+    """The StaticRiksStep object is used to indicate that the step should be analyzed as a static load step
+    using the modified Riks method for proportional loading cases. The StaticRiksStep object is derived from the
+    AnalysisStep object.
 
     .. note::
         This object can be accessed by::
 
-            mdb.models[name]
+            import step
+            mdb.models[name].steps[name]
 
         The corresponding analysis keywords are:
 
-        - PHYSICAL CONSTANTS
+        - STATIC
+        - STEP
     """
 
     #: A String specifying the repository key.
     name: str = ""
 
-    #: None or a Float specifying the Stefan-Boltzmann constant. The default value is None.
-    stefanBoltzmann: Optional[float] = None
+    #: A Boolean specifying whether to allow for geometric nonlinearity. The default value is
+    #: OFF.
+    nlgeom: Boolean = OFF
+
+    #: A Boolean specifying whether to perform an adiabatic stress analysis. The default value
+    #: is OFF.
+    adiabatic: Boolean = OFF
+
+    #: None or a Float specifying the maximum value of the load proportionality factor. The
+    #: default value is None.
+    maxLPF: Optional[float] = None
+
+    #: A Boolean specifying whether to monitor the finishing displacement value at a node. The
+    #: default value is OFF.
+    nodeOn: Boolean = OFF
+
+    #: A Float specifying the value of the total displacement (or rotation) at the node and
+    #: degree of freedom that, if crossed during an increment, ends the step at the current
+    #: increment. This argument is required when **nodeOn** = ON. The default value is 0.0.
+    maximumDisplacement: float = 0
+
+    #: An Int specifying the degree of freedom being monitored. This argument is required when
+    #: **nodeOn** = ON. The default value is 0.
+    dof: int = 0
+
+    #: A SymbolicConstant specifying the time incrementation method to be used. Possible values
+    #: are FIXED and AUTOMATIC. The default value is AUTOMATIC.
+    timeIncrementationMethod: SymbolicConstant = AUTOMATIC
+
+    #: An Int specifying the maximum number of increments in a step. The default value is 100.
+    maxNumInc: int = 100
+
+    #: A Float specifying the total load proportionality factor associated with the load in
+    #: this step. The default value is 1.0.
+    totalArcLength: float = 1
+
+    #: A Float specifying the initial load proportionality factor. The default value is the
+    #: total load proportionality factor for the step.
+    initialArcInc: Optional[float] = None
+
+    #: A Float specifying the minimum arc length increment allowed. The default value is the
+    #: smaller of the suggested initial load proportionality factor or 10−5 times the total
+    #: load proportionality factor for the step.
+    minArcInc: Optional[float] = None
+
+    #: A Float specifying the maximum arc length increment allowed. The default value is the
+    #: total load proportionality factor for the step.
+    maxArcInc: Optional[float] = None
+
+    #: A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
+    #: UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
+    matrixStorage: SymbolicConstant = SOLVER_DEFAULT
+
+    #: A SymbolicConstant specifying the type of extrapolation to use in determining the
+    #: incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
+    #: PARABOLIC. The default value is LINEAR.
+    extrapolation: SymbolicConstant = LINEAR
+
+    #: A Boolean specifying whether to accept the solution to an increment after the maximum
+    #: number of iterations allowed have been completed, even if the equilibrium tolerances are
+    #: not satisfied. The default value is OFF.Warning:You should set **noStop** = ON only in
+    #: special cases when you have a thorough understanding of how to interpret the results.
+    noStop: Boolean = OFF
+
+    #: A Boolean specifying wether to obtain the fully relaxed long-term elastic solution with
+    #: time-domain viscoelasticity or the long-term elastic-Plastic solution for two-layer
+    #: viscoplasticity. The default value is OFF.
+    useLongTermSolution: Boolean = OFF
+
+    #: A SymbolicConstant specifying whether to force a new iteration if severe discontinuities
+    #: occur during an iteration. Possible values are PROPAGATED, CONVERT_SDI_OFF, and
+    #: CONVERT_SDI_ON. The default value is PROPAGATED.
+    convertSDI: SymbolicConstant = PROPAGATED
+
+    #: A String specifying the name of the previous step. The new step appears after this step
+    #: in the list of analysis steps.
+    previous: str = ""
 
-    #: None or a Float specifying the absolute zero constant. The default value is None.
-    absoluteZero: Optional[float] = None
-
-    #: A SymbolicConstant specifying the type of incident wave formulation to be used in
-    #: acoustic problems. Possible values are NOT_SET, SCATTERED, and TOTAL. The default value
-    #: is NOT_SET.
-    waveFormulation: SymbolicConstant = NOT_SET
-
-    #: None or a Float specifying the universal gas constant. The default value is None.
-    universalGas: Optional[float] = None
-
-    #: A Boolean specifying whether an input file should be written without parts and
-    #: assemblies. The default value is OFF.
-    noPartsInputFile: Boolean = OFF
-
-    #: An Int specifying the increment, interval, iteration or cycle where the restart analysis
-    #: will start. To select the end of the step use the SymbolicConstant STEP_END.
-    restartIncrement: Optional[SymbolicConstant] = None
-
-    #: A Boolean specifying that the step specified by **restartStep** should be terminated at
-    #: the increment specified by **restartIncrement**.
-    endRestartStep: Boolean = OFF
-
-    #: A Boolean specifying that a shell global model drives a solid submodel.
-    shellToSolid: Boolean = OFF
-
-    #: A Float specifying the time stamp that indicates when the model was last changed.
-    lastChangedCount: Optional[float] = None
-
-    #: A String specifying the purpose and contents of the Model object. The default value is
-    #: an empty string.
+    #: A String specifying a description of the new step. The default value is an empty string.
     description: str = ""
 
-    #: A String specifying the name of the job that generated the restart data.
-    restartJob: str = ""
-
-    #: A String specifying the name of the step where the restart analysis will start.
-    restartStep: str = ""
-
-    #: A String specifying the name of the job that generated the results for the global model.
-    globalJob: str = ""
-
-    #: A boolean specifying the status of constraints created in a model, in the model which
-    #: instances this model.
-    copyConstraints: Boolean = OFF
-
-    #: A boolean specifying the status of connectors created in a model, in the model which
-    #: instances this model.
-    copyConnectors: Boolean = OFF
-
-    #: A boolean specifying the status of interactions created in a model, in the model which
-    #: instances this model.
-    copyInteractions: Boolean = OFF
-
-    #: A KeywordBlock object.
-    keywordBlock: KeywordBlock = KeywordBlock()
-
-    #: An Assembly object.
-    rootAssembly: Assembly = Assembly()
-
-    #: A repository of Amplitude objects.
-    amplitudes: Dict[str, Amplitude] = {}
-
-    #: A repository of Profile objects.
-    profiles: Dict[str, Profile] = {}
-
-    #: A repository of BoundaryCondition objects.
-    boundaryConditions: Dict[str, BoundaryCondition] = {}
-
-    #: A repository of ConstrainedSketchConstraint objects.
-    constraints: Dict[str, Constraint] = {}
-
-    #: A repository of AnalyticalField objects.
-    analyticalFields: Dict[str, AnalyticalField] = {}
-
-    #: A repository of DiscreteField objects.
-    discreteFields: Dict[str, DiscreteField] = {}
-
-    #: A repository of PredefinedField objects.
-    predefinedFields: Dict[str, PredefinedField] = {}
-
-    #: A repository of Interaction objects.
-    interactions: Dict[str, Interaction] = {}
-
-    #: A repository of InteractionProperty objects.
-    interactionProperties: Dict[str, ContactProperty] = {}
+    #: A String specifying the name of the region being monitored for fully Plastic behavior.
+    #: The default value is an empty string.
+    fullyPlastic: str = ""
 
-    #: A repository of ContactControl objects.
-    contactControls: Dict[str, ContactControl] = {}
+    #: A Region object specifying the vertex at which the finishing displacement value is being
+    #: monitored. This argument is required when **nodeOn** = ON.
+    region: Region = Region()
 
-    #: A repository of ContactInitialization objects.
-    contactInitializations: Dict[str, ContactInitialization] = {}
+    #: A SymbolicConstant specifying whether the step has an explicit procedure type
+    #: (*procedureType* = ANNEAL, DYNAMIC_EXPLICIT, or DYNAMIC_TEMP_DISPLACEMENT).
+    explicit: Optional[SymbolicConstant] = None
 
-    #: A repository of ContactStabilization objects.
-    contactStabilizations: Dict[str, ContactStabilization] = {}
+    #: A Boolean specifying whether the step has a perturbation procedure type.
+    perturbation: Boolean = OFF
 
-    #: A tuple of tuples of Strings specifying the linked child PartInstance name in the
-    #: current model to the corresponding parent PartInstance name in a different model.
-    linkedInstances: tuple = ()
+    #: A Boolean specifying whether the step has a mechanical procedure type.
+    nonmechanical: Boolean = OFF
 
-    #: A tuple of tuples of Strings specifying the linked child Part name in the current model
-    #: to the corresponding parent Part name in a different model.
-    linkedParts: tuple = ()
-
-    #: A repository of Load objects.
-    loads: Dict[str, Load] = {}
-
-    #: A repository of Material objects.
-    materials: Dict[str, Material] = {}
-
-    #: A repository of Calibration objects.
-    calibrations: Dict[str, Calibration] = {}
-
-    #: A repository of Section objects.
-    sections: Dict[str, Section] = {}
-
-    #: A repository of RemeshingRule objects.
-    remeshingRules: Dict[str, RemeshingRule] = {}
-
-    #: A repository of ConstrainedSketch objects.
-    sketches: Dict[str, ConstrainedSketch] = {}
-
-    #: A repository of Part objects.
-    parts: Dict[str, Part] = {}
-
-    #: A repository of Step objects.
-    steps: Dict[str, Step] = {}
-
-    #: A FeatureOptions object.
-    featureOptions: FeatureOptions = FeatureOptions()
-
-    #: A repository of AdaptiveMeshConstraint objects.
-    adaptiveMeshConstraints: Dict[str, AdaptiveMeshConstraint] = {}
-
-    #: A repository of AdaptiveMeshControl objects.
-    adaptiveMeshControls: Dict[str, AdaptiveMeshControl] = {}
-
-    #: A repository of TimePoint objects.
-    timePoints: Dict[str, TimePoint] = {}
-
-    #: A repository of Filter objects.
-    filters: Dict[str, Filter] = {}
-
-    #: A repository of IntegratedOutputSection objects.
-    integratedOutputSections: Dict[str, IntegratedOutputSection] = {}
-
-    #: A repository of FieldOutputRequest objects.
-    fieldOutputRequests: Dict[str, FieldOutputRequest] = {}
-
-    #: A repository of HistoryOutputRequest objects.
-    historyOutputRequests: Dict[str, HistoryOutputRequest] = {}
-
-    #: A repository of OptimizationTask objects.
-    optimizationTasks: Dict[str, OptimizationTask] = {}
-
-    #: A repository of TableCollection objects.
+    #: A SymbolicConstant specifying the Abaqus procedure. Possible values are:
     #:
-    #: .. versionadded:: 2020
-    #:     The ``tableCollections`` attribute was added.
-    tableCollections: Dict[str, TableCollection] = {}
+    #: - ANNEAL
+    #: - BUCKLE
+    #: - COMPLEX_FREQUENCY
+    #: - COUPLED_TEMP_DISPLACEMENT
+    #: - COUPLED_THERMAL_ELECTRIC
+    #: - DIRECT_CYCLIC
+    #: - DYNAMIC_IMPLICIT
+    #: - DYNAMIC_EXPLICIT
+    #: - DYNAMIC_SUBSPACE
+    #: - DYNAMIC_TEMP_DISPLACEMENT
+    #: - COUPLED_THERMAL_ELECTRICAL_STRUCTURAL
+    #: - FREQUENCY
+    #: - GEOSTATIC
+    #: - HEAT_TRANSFER
+    #: - MASS_DIFFUSION
+    #: - MODAL_DYNAMICS
+    #: - RANDOM_RESPONSE
+    #: - RESPONSE_SPECTRUM
+    #: - SOILS
+    #: - STATIC_GENERAL
+    #: - STATIC_LINEAR_PERTURBATION
+    #: - STATIC_RIKS
+    #: - STEADY_STATE_DIRECT
+    #: - STEADY_STATE_MODAL
+    #: - STEADY_STATE_SUBSPACE
+    #: - VISCO
+    procedureType: Optional[SymbolicConstant] = None
+
+    #: A Boolean specifying whether the step is suppressed or not. The default value is OFF.
+    suppressed: Boolean = OFF
+
+    #: A repository of FieldOutputRequestState objects.
+    fieldOutputRequestState: Dict[str, FieldOutputRequestState] = {}
+
+    #: A repository of HistoryOutputRequestState objects.
+    historyOutputRequestState: Dict[str, HistoryOutputRequestState] = {}
+
+    #: A DiagnosticPrint object.
+    diagnosticPrint: DiagnosticPrint = DiagnosticPrint()
+
+    #: A Monitor object.
+    monitor: Optional[Monitor] = None
+
+    #: A Restart object.
+    restart: Restart = Restart()
+
+    #: A repository of AdaptiveMeshConstraintState objects.
+    adaptiveMeshConstraintStates: Dict[str, AdaptiveMeshConstraintState] = {}
+
+    #: A repository of AdaptiveMeshDomain objects.
+    adaptiveMeshDomains: Dict[str, AdaptiveMeshDomain] = {}
+
+    #: A Control object.
+    control: Control = Control()
+
+    #: A SolverControl object.
+    solverControl: SolverControl = SolverControl()
+
+    #: A repository of BoundaryConditionState objects.
+    boundaryConditionStates: Dict[str, BoundaryConditionState] = {}
+
+    #: A repository of InteractionState objects.
+    interactionStates: Optional[int] = None
 
-    #: A repository of EventSeriesType objects.
-    #:
-    #: .. versionadded:: 2020
-    #:     The ``eventSeriesTypes`` attribute was added.
-    eventSeriesTypes: Dict[str, EventSeriesType] = {}
+    #: A repository of LoadState objects.
+    loadStates: Dict[str, LoadState] = {}
 
-    #: A repository of EventSeriesData objects.
-    #:
-    #: .. versionadded:: 2020
-    #:     The ``eventSeriesDatas`` attribute was added.
-    eventSeriesDatas: Dict[str, EventSeriesData] = {}
+    #: A repository of LoadCase objects.
+    loadCases: Dict[str, LoadCase] = {}
+
+    #: A repository of PredefinedFieldState objects.
+    predefinedFieldStates: Dict[str, PredefinedFieldState] = {}
 
     @abaqus_method_doc
     def __init__(
         self,
         name: str,
+        previous: str,
         description: str = "",
-        stefanBoltzmann: Optional[float] = None,
-        absoluteZero: Optional[float] = None,
-        waveFormulation: Literal[C.SCATTERED, C.NOT_SET, C.TOTAL] = NOT_SET,
-        modelType: Literal[C.STANDARD_EXPLICIT, C.ELECTROMAGNETIC] = STANDARD_EXPLICIT,
-        universalGas: Optional[float] = None,
-        copyConstraints: Boolean = ON,
-        copyConnectors: Boolean = ON,
-        copyInteractions: Boolean = ON,
+        nlgeom: Boolean = OFF,
+        adiabatic: Boolean = OFF,
+        maxLPF: Optional[float] = None,
+        nodeOn: Boolean = OFF,
+        maximumDisplacement: float = 0,
+        dof: int = 0,
+        region: Optional[Region] = None,
+        timeIncrementationMethod: Literal[C.AUTOMATIC, C.FIXED] = AUTOMATIC,
+        maxNumInc: int = 100,
+        totalArcLength: float = 1,
+        initialArcInc: Optional[float] = None,
+        minArcInc: Optional[float] = None,
+        maxArcInc: Optional[float] = None,
+        matrixStorage: Literal[C.SYMMETRIC, C.SOLVER_DEFAULT, C.UNSYMMETRIC] = SOLVER_DEFAULT,
+        extrapolation: Literal[C.PARABOLIC, C.NONE, C.LINEAR] = LINEAR,
+        fullyPlastic: str = "",
+        noStop: Boolean = OFF,
+        maintainAttributes: Boolean = False,
+        useLongTermSolution: Boolean = OFF,
+        convertSDI: Literal[C.CONVERT_SDI_OFF, C.PROPAGATED, C.CONVERT_SDI_ON] = PROPAGATED,
     ):
-        """This method creates a Model object.
+        """This method creates a StaticRiksStep object.
 
         .. note::
             This function can be accessed by::
 
-                mdb.Model
+                mdb.models[name].StaticRiksStep
 
         Parameters
         ----------
         name
             A String specifying the repository key.
+        previous
+            A String specifying the name of the previous step. The new step appears after this step
+            in the list of analysis steps.
         description
-            A String specifying the purpose and contents of the Model object. The default value is
-            an empty string.
-        stefanBoltzmann
-            None or a Float specifying the Stefan-Boltzmann constant. The default value is None.
-        absoluteZero
-            None or a Float specifying the absolute zero constant. The default value is None.
-        waveFormulation
-            A SymbolicConstant specifying the type of incident wave formulation to be used in
-            acoustic problems. Possible values are NOT_SET, SCATTERED, and TOTAL. The default value
-            is NOT_SET.
-        modelType
-            A SymbolicConstant specifying the analysis model type. Possible values are
-            STANDARD_EXPLICIT and ELECTROMAGNETIC. The default is STANDARD_EXPLICIT.
-        universalGas
-            None or a Float specifying the universal gas constant. The default value is None.
-        copyConstraints
-            A boolean specifying whether to copy the constraints created in the model to the model
-            that instances this model. The default value is ON.
-        copyConnectors
-            A boolean specifying whether to copy the connectors created in the model to the model
-            that instances this model. The default value is ON.
-        copyInteractions
-            A boolean specifying whether to copy the interactions created in the model to the model
-            that instances this model. The default value is ON.
+            A String specifying a description of the new step. The default value is an empty string.
+        nlgeom
+            A Boolean specifying whether to allow for geometric nonlinearity. The default value is
+            OFF.
+        adiabatic
+            A Boolean specifying whether to perform an adiabatic stress analysis. The default value
+            is OFF.
+        maxLPF
+            None or a Float specifying the maximum value of the load proportionality factor. The
+            default value is None.
+        nodeOn
+            A Boolean specifying whether to monitor the finishing displacement value at a node. The
+            default value is OFF.
+        maximumDisplacement
+            A Float specifying the value of the total displacement (or rotation) at the node and
+            degree of freedom that, if crossed during an increment, ends the step at the current
+            increment. This argument is required when **nodeOn** = ON. The default value is 0.0.
+        dof
+            An Int specifying the degree of freedom being monitored. This argument is required when
+            **nodeOn** = ON. The default value is 0.
+        region
+            A Region object specifying the vertex at which the finishing displacement value is being
+            monitored. This argument is required when **nodeOn** = ON.
+        timeIncrementationMethod
+            A SymbolicConstant specifying the time incrementation method to be used. Possible values
+            are FIXED and AUTOMATIC. The default value is AUTOMATIC.
+        maxNumInc
+            An Int specifying the maximum number of increments in a step. The default value is 100.
+        totalArcLength
+            A Float specifying the total load proportionality factor associated with the load in
+            this step. The default value is 1.0.
+        initialArcInc
+            A Float specifying the initial load proportionality factor. The default value is the
+            total load proportionality factor for the step.
+        minArcInc
+            A Float specifying the minimum arc length increment allowed. The default value is the
+            smaller of the suggested initial load proportionality factor or 10−5 times the total
+            load proportionality factor for the step.
+        maxArcInc
+            A Float specifying the maximum arc length increment allowed. The default value is the
+            total load proportionality factor for the step.
+        matrixStorage
+            A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
+            UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
+        extrapolation
+            A SymbolicConstant specifying the type of extrapolation to use in determining the
+            incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
+            PARABOLIC. The default value is LINEAR.
+        fullyPlastic
+            A String specifying the name of the region being monitored for fully Plastic behavior.
+            The default value is an empty string.
+        noStop
+            A Boolean specifying whether to accept the solution to an increment after the maximum
+            number of iterations allowed have been completed, even if the equilibrium tolerances are
+            not satisfied. The default value is OFF.Warning:You should set **noStop** = ON only in
+            special cases when you have a thorough understanding of how to interpret the results.
+        maintainAttributes
+            A Boolean specifying whether to retain attributes from an existing step with the same
+            name. The default value is False.
+        useLongTermSolution
+            A Boolean specifying wether to obtain the fully relaxed long-term elastic solution with
+            time-domain viscoelasticity or the long-term elastic-Plastic solution for two-layer
+            viscoplasticity. The default value is OFF.
+        convertSDI
+            A SymbolicConstant specifying whether to force a new iteration if severe discontinuities
+            occur during an iteration. Possible values are PROPAGATED, CONVERT_SDI_OFF, and
+            CONVERT_SDI_ON. The default value is PROPAGATED.
 
         Returns
         -------
-        Model
-            A Model object.
-        """
-        self.steps["Initial"] = InitialStep()
+        StaticRiksStep
+            A StaticRiksStep object.
 
-    @abaqus_method_doc
-    def ModelFromInputFile(self, name: str, inputFileName: str):
-        """This method creates a Model object by reading the keywords in an input file and creating the
-        corresponding Abaqus/CAE objects.
-
-        .. note::
-            This function can be accessed by::
-
-                mdb.Model
-
-        Parameters
-        ----------
-        name
-            A String specifying the repository key.
-        inputFileName
-            A String specifying the name of the input file (including the .inp extension) to be
-            parsed into the new model. This String can also be the full path to the input file if it
-            is located in another directory.
-
-        Returns
-        -------
-        Model
-            A Model object.
-        """
-        ...
-
-    @abaqus_method_doc
-    def ModelFromOdbFile(self, name: str, odbFileName: str):
-        """This method creates a Model object by reading an output database and creating any corresponding
-        Abaqus/CAE objects.
-
-        .. note::
-            This function can be accessed by::
-
-                mdb.Model
-
-        Parameters
-        ----------
-        name
-            A String specifying the repository key.
-        odbFileName
-            A String specifying the name of the output database file (including the .odb extension)
-            to be read into the new model. This String can also be the full path to the output
-            database file if it is located in another directory.
-
-        Returns
-        -------
-        Model
-            A Model object.
+        Raises
+        ------
+        RangeError
         """
-        ...
-
-    @abaqus_method_doc
-    def ModelFromNastranFile(
-        self,
-        modelName: str,
-        inputFileName: str,
-        sectionConsolidation: Literal[C.PRESERVE_SECTION, C.GROUP_BY_MATERIAL, C.NONE] = PRESERVE_SECTION,
-        preIntegratedShell: Boolean = OFF,
-        weightMassScaling: Boolean = ON,
-        loadCases: Boolean = ON,
-        coupleBeamOffsets: Boolean = ON,
-        cbar: str = B31,
-        cquad4: str = S4,
-        chexa: str = C3D8I,
-        ctetra: str = C3D10,
-        keepTranslatedFiles: Boolean = ON,
-    ):
-        """This method creates a Model object by reading the keywords in a Nastran bulk data file or Nastran
-        input file and creating any corresponding Abaqus/CAE objects. The default values is discussed in
-        following and can be defined alternatively in the Abaqus environment file as the one used for the
-        translator from Nastran to Abaqus. For more information, see Translating Nastran data to Abaqus files.
-
-        .. note::
-            This function can be accessed by::
-
-                mdb.Model
-
-        Parameters
-        ----------
-        modelName
-            A String specifying the repository key.
-        inputFileName
-            A String specifying the name of the Nastran input file (including the .bdf, .dat, .nas,
-            .nastran, .blk, .bulk extension) to be read into the new model. This String can also be
-            the full path to the Nastran input file if it is located in another directory.
-        sectionConsolidation
-            A SymbolicConstant specifying the method used to create shell section. Possible values
-            are PRESERVE_SECTION, GROUP_BY_MATERIAL, and NONE. If PRESERVE_SECTION is used, an
-            Abaqus section is created corresponding to each shell property ID. If GROUP_BY_MATERIAL
-            is used, a single Abaqus section is created for all homogeneous elements referencing the
-            same material. In both cases, material orientations and offsets are created using
-            discrete fields. If NONE is used, a separate shell section is created for each
-            combination of orientation, material offset, and/or thickness. The default is
-            PRESERVE_SECTION.
-        preIntegratedShell
-            A Boolean specifying whether the pre-integrated shell section is created in default for
-            shell element. The default value is OFF.
-        weightMassScaling
-            A Boolean specifying whether the value on the Nastran data line PARAM, WTMASS is used as
-            a multiplier for all density, mass, and rotary inertia values created in the Abaqus
-            input file. The default value is ON.
-        loadCases
-            A Boolean specifying whether each SUBCASE for linear static analyses is translated to a
-            LOAD CASE option, and all such LOAD CASE options are grouped in a single STEP option.
-            The default value is ON.
-        coupleBeamOffsets
-            A Boolean specifying whether to translate the beam element connectivity to newly created
-            nodes at the offset location and rigidly coupling the new and original nodes. If not,
-            beam element offsets are translated to the CENTROID and SHEAR CENTER options, which are
-            suboptions of the BEAM GENERAL SECTION option. The default value is ON. When the beam
-            element references a PBARL or PBEAML property or if the beam offset has a significant
-            component in the direction of the beam axis, the setting for this argument is always ON.
-        cbar
-            A String specifying the 2-node beam that is created from CBAR and CBEAM elements.
-            Possible values are B31 and B33. The default is B31.
-        cquad4
-            A String specifying the 4-node shell that is created from CQUAD4 elements. Possible
-            values are S4 and S4R. The default is S4. If a reduced-integration element is chosen,
-            the enhanced hourglass formulation is applied automatically.
-        chexa
-            A String specifying the 8-node brick that is created from CHEXA elements. Possible
-            values are C3D8I, C3D8 and C3D8R. The default is C3D8I. If a reduced-integration element
-            is chosen, the enhanced hourglass formulation is applied automatically.
-        ctetra
-            A String specifying the 10-node tetrahedron that is created from CTETRA elements.
-            Possible values are C3D10 and C3D10M. The default is C3D10.
-        keepTranslatedFiles
-            A Boolean specifying whether to keep the generated Abaqus input file after the model is
-            created from the Nastran input file. The default value is ON.
-
-        Returns
-        -------
-        Model
-            A Model object.
-        """
-        ...
+        super().__init__()
 
     @abaqus_method_doc
     def setValues(
         self,
         description: str = "",
-        noPartsInputFile: Boolean = OFF,
-        absoluteZero: Optional[float] = None,
-        stefanBoltzmann: Optional[float] = None,
-        waveFormulation: Literal[C.SCATTERED, C.NOT_SET, C.TOTAL] = NOT_SET,
-        universalGas: Optional[float] = None,
-        restartJob: str = "",
-        restartStep: str = "",
-        restartIncrement: Optional[Literal[C.STEP_END]] = None,
-        endRestartStep: Boolean = OFF,
-        globalJob: str = "",
-        shellToSolid: Boolean = OFF,
-        copyConstraints: Boolean = OFF,
-        copyConnectors: Boolean = OFF,
-        copyInteractions: Boolean = OFF,
+        nlgeom: Boolean = OFF,
+        adiabatic: Boolean = OFF,
+        maxLPF: Optional[float] = None,
+        nodeOn: Boolean = OFF,
+        maximumDisplacement: float = 0,
+        dof: int = 0,
+        region: Optional[Region] = None,
+        timeIncrementationMethod: Literal[C.AUTOMATIC, C.FIXED] = AUTOMATIC,
+        maxNumInc: int = 100,
+        totalArcLength: float = 1,
+        initialArcInc: Optional[float] = None,
+        minArcInc: Optional[float] = None,
+        maxArcInc: Optional[float] = None,
+        matrixStorage: Literal[C.SYMMETRIC, C.SOLVER_DEFAULT, C.UNSYMMETRIC] = SOLVER_DEFAULT,
+        extrapolation: Literal[C.PARABOLIC, C.NONE, C.LINEAR] = LINEAR,
+        fullyPlastic: str = "",
+        noStop: Boolean = OFF,
+        useLongTermSolution: Boolean = OFF,
+        convertSDI: Literal[C.CONVERT_SDI_OFF, C.PROPAGATED, C.CONVERT_SDI_ON] = PROPAGATED,
     ):
-        """This method modifies the Model object.
+        """This method modifies the StaticRiksStep object.
 
         Parameters
         ----------
         description
-            A String specifying the purpose and contents of the Model object. The default value is
-            an empty string.
-        noPartsInputFile
-            A Boolean specifying whether an input file should be written without parts and
-            assemblies. The default value is OFF.
-        absoluteZero
-            None or a Float specifying the absolute zero constant. The default value is None.
-        stefanBoltzmann
-            None or a Float specifying the Stefan-Boltzmann constant. The default value is None.
-        waveFormulation
-            A SymbolicConstant specifying the type of incident wave formulation to be used in
-            acoustic problems. Possible values are NOT_SET, SCATTERED, and TOTAL. The default value
-            is NOT_SET.
-        universalGas
-            None or a Float specifying the universal gas constant. The default value is None.
-        restartJob
-            A String specifying the name of the job that generated the restart data.
-        restartStep
-            A String specifying the name of the step where the restart analysis will start.
-        restartIncrement
-            An Int specifying the increment, interval, iteration or cycle where the restart analysis
-            will start. To select the end of the step use the SymbolicConstant STEP_END.
-        endRestartStep
-            A Boolean specifying that the step specified by **restartStep** should be terminated at
-            the increment specified by **restartIncrement**.
-        globalJob
-            A String specifying the name of the job that generated the results for the global model.
-        shellToSolid
-            A Boolean specifying that a shell global model drives a solid submodel.
-        copyConstraints
-            A Boolean specifying whether to copy the constraints created in the model to the model
-            that instances this model.
-        copyConnectors
-            A Boolean specifying whether to copy the connectors created in the model to the model
-            that instances this model
-        copyInteractions
-            A Boolean specifying whether to copy the interactions created in the model to the model
-            that instances this model.
+            A String specifying a description of the new step. The default value is an empty string.
+        nlgeom
+            A Boolean specifying whether to allow for geometric nonlinearity. The default value is
+            OFF.
+        adiabatic
+            A Boolean specifying whether to perform an adiabatic stress analysis. The default value
+            is OFF.
+        maxLPF
+            None or a Float specifying the maximum value of the load proportionality factor. The
+            default value is None.
+        nodeOn
+            A Boolean specifying whether to monitor the finishing displacement value at a node. The
+            default value is OFF.
+        maximumDisplacement
+            A Float specifying the value of the total displacement (or rotation) at the node and
+            degree of freedom that, if crossed during an increment, ends the step at the current
+            increment. This argument is required when **nodeOn** = ON. The default value is 0.0.
+        dof
+            An Int specifying the degree of freedom being monitored. This argument is required when
+            **nodeOn** = ON. The default value is 0.
+        region
+            A Region object specifying the vertex at which the finishing displacement value is being
+            monitored. This argument is required when **nodeOn** = ON.
+        timeIncrementationMethod
+            A SymbolicConstant specifying the time incrementation method to be used. Possible values
+            are FIXED and AUTOMATIC. The default value is AUTOMATIC.
+        maxNumInc
+            An Int specifying the maximum number of increments in a step. The default value is 100.
+        totalArcLength
+            A Float specifying the total load proportionality factor associated with the load in
+            this step. The default value is 1.0.
+        initialArcInc
+            A Float specifying the initial load proportionality factor. The default value is the
+            total load proportionality factor for the step.
+        minArcInc
+            A Float specifying the minimum arc length increment allowed. The default value is the
+            smaller of the suggested initial load proportionality factor or 10−5 times the total
+            load proportionality factor for the step.
+        maxArcInc
+            A Float specifying the maximum arc length increment allowed. The default value is the
+            total load proportionality factor for the step.
+        matrixStorage
+            A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
+            UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
+        extrapolation
+            A SymbolicConstant specifying the type of extrapolation to use in determining the
+            incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
+            PARABOLIC. The default value is LINEAR.
+        fullyPlastic
+            A String specifying the name of the region being monitored for fully Plastic behavior.
+            The default value is an empty string.
+        noStop
+            A Boolean specifying whether to accept the solution to an increment after the maximum
+            number of iterations allowed have been completed, even if the equilibrium tolerances are
+            not satisfied. The default value is OFF.Warning:You should set **noStop** = ON only in
+            special cases when you have a thorough understanding of how to interpret the results.
+        useLongTermSolution
+            A Boolean specifying wether to obtain the fully relaxed long-term elastic solution with
+            time-domain viscoelasticity or the long-term elastic-Plastic solution for two-layer
+            viscoplasticity. The default value is OFF.
+        convertSDI
+            A SymbolicConstant specifying whether to force a new iteration if severe discontinuities
+            occur during an iteration. Possible values are PROPAGATED, CONVERT_SDI_OFF, and
+            CONVERT_SDI_ON. The default value is PROPAGATED.
+
+        Raises
+        ------
+        RangeError
         """
         ...
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/AnalyticSurface.py` & `abqpy-2023.5.2/src/abaqus/Odb/AnalyticSurface.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/AnalyticSurfaceSegment.py` & `abqpy-2023.5.2/src/abaqus/Odb/AnalyticSurfaceSegment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/BeamOrientation.py` & `abqpy-2023.5.2/src/abaqus/Odb/BeamOrientation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/FieldBulkData.py` & `abqpy-2023.5.2/src/abaqus/Odb/FieldBulkData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/FieldLocation.py` & `abqpy-2023.5.2/src/abaqus/Odb/FieldLocation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/FieldOutput.py` & `abqpy-2023.5.2/src/abaqus/Odb/FieldOutput.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/FieldValue.py` & `abqpy-2023.5.2/src/abaqus/Odb/FieldValue.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/HistoryOutput.py` & `abqpy-2023.5.2/src/abaqus/Odb/HistoryOutput.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/HistoryPoint.py` & `abqpy-2023.5.2/src/abaqus/Odb/HistoryPoint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/HistoryRegion.py` & `abqpy-2023.5.2/src/abaqus/Odb/HistoryRegion.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/JobData.py` & `abqpy-2023.5.2/src/abaqus/Odb/JobData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/Odb.py` & `abqpy-2023.5.2/src/abaqus/Odb/Odb.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbAssembly.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbAssembly.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbAssemblyBase.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbAssemblyBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbBase.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbCommands.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbCommands.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbDatumCsys.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbDatumCsys.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbFrame.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbFrame.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbInstance.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbInstance.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbInstanceBase.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbInstanceBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbLoadCase.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbLoadCase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbMeshElement.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbMeshElement.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbMeshNode.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbMeshNode.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbPart.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbPart.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbPartBase.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbPartBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbPretensionSection.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbPretensionSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbRigidBody.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbRigidBody.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbSequenceAnalyticSurfaceSegment.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbSequenceAnalyticSurfaceSegment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbSession.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbSession.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbSet.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbSet.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbStep.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/OdbStepBase.py` & `abqpy-2023.5.2/src/abaqus/Odb/OdbStepBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/RebarOrientation.py` & `abqpy-2023.5.2/src/abaqus/Odb/RebarOrientation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/ScratchOdb.py` & `abqpy-2023.5.2/src/abaqus/Odb/ScratchOdb.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/SectionCategory.py` & `abqpy-2023.5.2/src/abaqus/Odb/SectionCategory.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/SectionPoint.py` & `abqpy-2023.5.2/src/abaqus/Odb/SectionPoint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/SectorDefinition.py` & `abqpy-2023.5.2/src/abaqus/Odb/SectorDefinition.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Odb/UserDataBase.py` & `abqpy-2023.5.2/src/abaqus/Odb/UserDataBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/OdbDisplay/CommonOptions.py` & `abqpy-2023.5.2/src/abaqus/OdbDisplay/CommonOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/OdbDisplay/ContourOptions.py` & `abqpy-2023.5.2/src/abaqus/OdbDisplay/ContourOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/OdbDisplay/DefaultOdbDisplay.py` & `abqpy-2023.5.2/src/abaqus/OdbDisplay/DefaultOdbDisplay.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/OdbDisplay/DisplayBodyOptions.py` & `abqpy-2023.5.2/src/abaqus/OdbDisplay/DisplayBodyOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/OdbDisplay/OdbDisplay.py` & `abqpy-2023.5.2/src/abaqus/OdbDisplay/OdbDisplay.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/OdbDisplay/OrientationOptions.py` & `abqpy-2023.5.2/src/abaqus/OdbDisplay/OrientationOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/OdbDisplay/SuperimposeOptions.py` & `abqpy-2023.5.2/src/abaqus/OdbDisplay/SuperimposeOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/OdbDisplay/SymbolOptions.py` & `abqpy-2023.5.2/src/abaqus/OdbDisplay/SymbolOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/OdbDisplay/ViewCut.py` & `abqpy-2023.5.2/src/abaqus/OdbDisplay/ViewCut.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/OdbDisplay/ViewerOptions.py` & `abqpy-2023.5.2/src/abaqus/OdbDisplay/ViewerOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/BeadFilter.py` & `abqpy-2023.5.2/src/abaqus/Optimization/BeadFilter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/BeadFixedRegion.py` & `abqpy-2023.5.2/src/abaqus/Optimization/BeadFixedRegion.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/BeadGrowth.py` & `abqpy-2023.5.2/src/abaqus/Optimization/BeadGrowth.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/BeadPenetrationCheck.py` & `abqpy-2023.5.2/src/abaqus/Optimization/BeadPenetrationCheck.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/BeadPlanarSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/BeadPlanarSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/BeadPointSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/BeadPointSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/BeadRotationalSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/BeadRotationalSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/BeadTask.py` & `abqpy-2023.5.2/src/abaqus/Optimization/BeadTask.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/CombinedTermDesignResponse.py` & `abqpy-2023.5.2/src/abaqus/Optimization/CombinedTermDesignResponse.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/DesignDirection.py` & `abqpy-2023.5.2/src/abaqus/Optimization/DesignDirection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/DesignResponse.py` & `abqpy-2023.5.2/src/abaqus/Optimization/DesignResponse.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/DrillControl.py` & `abqpy-2023.5.2/src/abaqus/Optimization/DrillControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/FixedRegion.py` & `abqpy-2023.5.2/src/abaqus/Optimization/FixedRegion.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/FrozenArea.py` & `abqpy-2023.5.2/src/abaqus/Optimization/FrozenArea.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/GeometricRestriction.py` & `abqpy-2023.5.2/src/abaqus/Optimization/GeometricRestriction.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/Growth.py` & `abqpy-2023.5.2/src/abaqus/Optimization/Growth.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/LocalStopCondition.py` & `abqpy-2023.5.2/src/abaqus/Optimization/LocalStopCondition.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/ObjectiveFunction.py` & `abqpy-2023.5.2/src/abaqus/Optimization/ObjectiveFunction.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/OptimizationConstraint.py` & `abqpy-2023.5.2/src/abaqus/Optimization/OptimizationConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/OptimizationObjective.py` & `abqpy-2023.5.2/src/abaqus/Optimization/OptimizationObjective.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/OptimizationTask.py` & `abqpy-2023.5.2/src/abaqus/Optimization/OptimizationTask.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/OptimizationTaskBase.py` & `abqpy-2023.5.2/src/abaqus/Optimization/OptimizationTaskBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/OptimizationTaskModel.py` & `abqpy-2023.5.2/src/abaqus/Optimization/OptimizationTaskModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/PenetrationCheck.py` & `abqpy-2023.5.2/src/abaqus/Optimization/PenetrationCheck.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/ShapeDemoldControl.py` & `abqpy-2023.5.2/src/abaqus/Optimization/ShapeDemoldControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/ShapeMemberSize.py` & `abqpy-2023.5.2/src/abaqus/Optimization/ShapeMemberSize.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/ShapePlanarSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/ShapePlanarSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/ShapePointSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/ShapePointSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/ShapeRotationalSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/ShapeRotationalSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/ShapeTask.py` & `abqpy-2023.5.2/src/abaqus/Optimization/ShapeTask.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/SingleTermDesignResponse.py` & `abqpy-2023.5.2/src/abaqus/Optimization/SingleTermDesignResponse.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/SizingClusterAreas.py` & `abqpy-2023.5.2/src/abaqus/Optimization/SizingClusterAreas.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/SizingCyclicSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/SizingCyclicSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/SizingFrozenArea.py` & `abqpy-2023.5.2/src/abaqus/Optimization/SizingFrozenArea.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/SizingMemberSize.py` & `abqpy-2023.5.2/src/abaqus/Optimization/SizingMemberSize.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/SizingPlanarSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/SizingPlanarSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/SizingPointSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/SizingPointSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/SizingRotationalSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/SizingRotationalSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/SizingTask.py` & `abqpy-2023.5.2/src/abaqus/Optimization/SizingTask.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/SlideRegionControl.py` & `abqpy-2023.5.2/src/abaqus/Optimization/SlideRegionControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/StampControl.py` & `abqpy-2023.5.2/src/abaqus/Optimization/StampControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/StepOption.py` & `abqpy-2023.5.2/src/abaqus/Optimization/StepOption.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/StopCondition.py` & `abqpy-2023.5.2/src/abaqus/Optimization/StopCondition.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/TopologyCyclicSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/TopologyCyclicSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/TopologyDemoldControl.py` & `abqpy-2023.5.2/src/abaqus/Optimization/TopologyDemoldControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/TopologyMemberSize.py` & `abqpy-2023.5.2/src/abaqus/Optimization/TopologyMemberSize.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/TopologyMillingControl.py` & `abqpy-2023.5.2/src/abaqus/Optimization/TopologyMillingControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/TopologyOverhangControl.py` & `abqpy-2023.5.2/src/abaqus/Optimization/TopologyOverhangControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/TopologyPlanarSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/TopologyPlanarSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/TopologyPointSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/TopologyPointSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/TopologyRibDesign.py` & `abqpy-2023.5.2/src/abaqus/Optimization/TopologyRibDesign.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/TopologyRotationalSymmetry.py` & `abqpy-2023.5.2/src/abaqus/Optimization/TopologyRotationalSymmetry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/TopologyTask.py` & `abqpy-2023.5.2/src/abaqus/Optimization/TopologyTask.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Optimization/TurnControl.py` & `abqpy-2023.5.2/src/abaqus/Optimization/TurnControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Part/AcisFile.py` & `abqpy-2023.5.2/src/abaqus/Part/AcisFile.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Part/AcisMdb.py` & `abqpy-2023.5.2/src/abaqus/Part/AcisMdb.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Part/Part.py` & `abqpy-2023.5.2/src/abaqus/Part/Part.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Part/PartBase.py` & `abqpy-2023.5.2/src/abaqus/Part/PartBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Part/PartFeature.py` & `abqpy-2023.5.2/src/abaqus/Part/PartFeature.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Part/PartModel.py` & `abqpy-2023.5.2/src/abaqus/Part/PartModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PathAndProbe/CurrentProbeValues.py` & `abqpy-2023.5.2/src/abaqus/PathAndProbe/CurrentProbeValues.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PathAndProbe/FreeBody.py` & `abqpy-2023.5.2/src/abaqus/PathAndProbe/FreeBody.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PathAndProbe/NodeQuery.py` & `abqpy-2023.5.2/src/abaqus/PathAndProbe/NodeQuery.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PathAndProbe/Path.py` & `abqpy-2023.5.2/src/abaqus/PathAndProbe/Path.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PathAndProbe/PathSession.py` & `abqpy-2023.5.2/src/abaqus/PathAndProbe/PathSession.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PathAndProbe/ProbeOptions.py` & `abqpy-2023.5.2/src/abaqus/PathAndProbe/ProbeOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PathAndProbe/ProbeReport.py` & `abqpy-2023.5.2/src/abaqus/PathAndProbe/ProbeReport.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PathAndProbe/SelectedProbeValues.py` & `abqpy-2023.5.2/src/abaqus/PathAndProbe/SelectedProbeValues.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PathAndProbe/Spectrum.py` & `abqpy-2023.5.2/src/abaqus/PathAndProbe/Spectrum.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PathAndProbe/Stream.py` & `abqpy-2023.5.2/src/abaqus/PathAndProbe/Stream.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/BasicOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/BasicOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/CouplingConstraint.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/CouplingConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/DGCommonOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/DGCommonOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/DGContourOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/DGContourOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/DGDisplayBodyOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/DGDisplayBodyOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/DGOrientationOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/DGOrientationOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/DGSuperimposeOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/DGSuperimposeOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/DGSymbolOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/DGSymbolOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/DetailPlotOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/DetailPlotOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/DisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/DisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/FreeBodyOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/FreeBodyOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/HistoryVariable.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/HistoryVariable.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/MdbData.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/MdbData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/MdbDataStep.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/MdbDataStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/MpcConstraint.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/MpcConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbAnalysisError.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbAnalysisError.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbAuxiliaryData.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbAuxiliaryData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbContactDiagnostics.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbContactDiagnostics.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbData.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataDatumCsys.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataDatumCsys.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataElementSet.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataElementSet.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataFrame.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataFrame.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataMaterial.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataMaterial.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataSection.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataStep.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDataSurfaceSet.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDataSurfaceSet.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDiagnosticAttempt.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDiagnosticAttempt.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDiagnosticData.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDiagnosticData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDiagnosticIncrement.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDiagnosticIncrement.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDiagnosticStep.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDiagnosticStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbDisplayOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbDisplayOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbJobTime.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbJobTime.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OdbNumericalProblemSummary.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OdbNumericalProblemSummary.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/OptionArg.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/OptionArg.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/PlyStackPlotOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/PlyStackPlotOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/RigidBodyConstraint.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/RigidBodyConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/StreamOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/StreamOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/TieConstraint.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/TieConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PlotOptions/ViewCutOptions.py` & `abqpy-2023.5.2/src/abaqus/PlotOptions/ViewCutOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/Field.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/Field.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/FieldState.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/FieldState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/FluidCavityPressure.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/FluidCavityPressure.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/IMAField.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/IMAField.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/IMARegion.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/IMARegion.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/InitialState.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/InitialState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/KinematicHardening.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/KinematicHardening.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/MaterialAssignment.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/MaterialAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/PorePressure.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/PorePressure.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/PredefinedField.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/PredefinedField.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/PredefinedFieldModel.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/PredefinedFieldModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/PredefinedFieldState.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/PredefinedFieldState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/Saturation.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/Saturation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/Stress.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/Stress.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/Temperature.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/Temperature.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/TemperatureState.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/TemperatureState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/TiffOptions.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/TiffOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/Velocity.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/Velocity.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/PredefinedField/VoidsRatio.py` & `abqpy-2023.5.2/src/abaqus/PredefinedField/VoidsRatio.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Print/EpsOptions.py` & `abqpy-2023.5.2/src/abaqus/Print/EpsOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Print/PageSetupOptions.py` & `abqpy-2023.5.2/src/abaqus/Print/PageSetupOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Print/PngOptions.py` & `abqpy-2023.5.2/src/abaqus/Print/PngOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Print/PrintOptions.py` & `abqpy-2023.5.2/src/abaqus/Print/PrintOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Print/PsOptions.py` & `abqpy-2023.5.2/src/abaqus/Print/PsOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Print/SvgOptions.py` & `abqpy-2023.5.2/src/abaqus/Print/SvgOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Property/CompositeLayup.py` & `abqpy-2023.5.2/src/abaqus/Property/CompositeLayup.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Property/CompositePly.py` & `abqpy-2023.5.2/src/abaqus/Property/CompositePly.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Property/MaterialOrientation.py` & `abqpy-2023.5.2/src/abaqus/Property/MaterialOrientation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Property/PlyStackPlot.py` & `abqpy-2023.5.2/src/abaqus/Property/PlyStackPlot.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Property/Property.py` & `abqpy-2023.5.2/src/abaqus/Property/Property.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Property/PropertyAssembly.py` & `abqpy-2023.5.2/src/abaqus/Property/PropertyAssembly.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Property/PropertyPart.py` & `abqpy-2023.5.2/src/abaqus/Property/PropertyPart.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Property/SectionAssignment.py` & `abqpy-2023.5.2/src/abaqus/Property/SectionAssignment.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Region/Region.py` & `abqpy-2023.5.2/src/abaqus/Region/Region.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Region/RegionAssembly.py` & `abqpy-2023.5.2/src/abaqus/Region/RegionAssembly.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Region/RegionAssemblyBase.py` & `abqpy-2023.5.2/src/abaqus/Region/RegionAssemblyBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Region/RegionPart.py` & `abqpy-2023.5.2/src/abaqus/Region/RegionPart.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Region/RegionPartBase.py` & `abqpy-2023.5.2/src/abaqus/Region/RegionPartBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Region/Set.py` & `abqpy-2023.5.2/src/abaqus/Region/Set.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Region/Skin.py` & `abqpy-2023.5.2/src/abaqus/Region/Skin.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Region/Stringer.py` & `abqpy-2023.5.2/src/abaqus/Region/Stringer.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Region/Surface.py` & `abqpy-2023.5.2/src/abaqus/Region/Surface.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/AcousticInfiniteSection.py` & `abqpy-2023.5.2/src/abaqus/Section/AcousticInfiniteSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/AcousticInterfaceSection.py` & `abqpy-2023.5.2/src/abaqus/Section/AcousticInterfaceSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/BeamSection.py` & `abqpy-2023.5.2/src/abaqus/Section/BeamSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/CohesiveSection.py` & `abqpy-2023.5.2/src/abaqus/Section/CohesiveSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/CompositeShellSection.py` & `abqpy-2023.5.2/src/abaqus/Section/CompositeShellSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/CompositeSolidSection.py` & `abqpy-2023.5.2/src/abaqus/Section/CompositeSolidSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/ConnectorSection.py` & `abqpy-2023.5.2/src/abaqus/Section/ConnectorSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/EulerianSection.py` & `abqpy-2023.5.2/src/abaqus/Section/EulerianSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/GasketSection.py` & `abqpy-2023.5.2/src/abaqus/Section/GasketSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/GeneralStiffnessSection.py` & `abqpy-2023.5.2/src/abaqus/Section/GeneralStiffnessSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/GeometryShellSection.py` & `abqpy-2023.5.2/src/abaqus/Section/GeometryShellSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/HomogeneousShellSection.py` & `abqpy-2023.5.2/src/abaqus/Section/HomogeneousShellSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/HomogeneousSolidSection.py` & `abqpy-2023.5.2/src/abaqus/Section/HomogeneousSolidSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/LayerProperties.py` & `abqpy-2023.5.2/src/abaqus/Section/LayerProperties.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/MPCSection.py` & `abqpy-2023.5.2/src/abaqus/Section/MPCSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/MembraneSection.py` & `abqpy-2023.5.2/src/abaqus/Section/MembraneSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/PEGSection.py` & `abqpy-2023.5.2/src/abaqus/Section/PEGSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/RebarLayers.py` & `abqpy-2023.5.2/src/abaqus/Section/RebarLayers.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/Section.py` & `abqpy-2023.5.2/src/abaqus/Section/Section.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/SectionBase.py` & `abqpy-2023.5.2/src/abaqus/Section/SectionBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/SectionLayer.py` & `abqpy-2023.5.2/src/abaqus/Section/SectionLayer.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/SectionModel.py` & `abqpy-2023.5.2/src/abaqus/Section/SectionModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/SectionOdb.py` & `abqpy-2023.5.2/src/abaqus/Section/SectionOdb.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/ShellSection.py` & `abqpy-2023.5.2/src/abaqus/Section/ShellSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/SolidSection.py` & `abqpy-2023.5.2/src/abaqus/Section/SolidSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/SurfaceSection.py` & `abqpy-2023.5.2/src/abaqus/Section/SurfaceSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/TransverseShearBeam.py` & `abqpy-2023.5.2/src/abaqus/Section/TransverseShearBeam.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/TransverseShearShell.py` & `abqpy-2023.5.2/src/abaqus/Section/TransverseShearShell.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Section/TrussSection.py` & `abqpy-2023.5.2/src/abaqus/Section/TrussSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Session/AutoColors.py` & `abqpy-2023.5.2/src/abaqus/Session/AutoColors.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Session/Color.py` & `abqpy-2023.5.2/src/abaqus/Session/Color.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Session/Drawing.py` & `abqpy-2023.5.2/src/abaqus/Session/Drawing.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Session/Image.py` & `abqpy-2023.5.2/src/abaqus/Session/Image.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Session/JournalOptions.py` & `abqpy-2023.5.2/src/abaqus/Session/JournalOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Session/MemoryReductionOptions.py` & `abqpy-2023.5.2/src/abaqus/Session/MemoryReductionOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Session/NetworkDatabaseConnector.py` & `abqpy-2023.5.2/src/abaqus/Session/NetworkDatabaseConnector.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Session/NumberFormat.py` & `abqpy-2023.5.2/src/abaqus/Session/NumberFormat.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Session/Session.py` & `abqpy-2023.5.2/src/abaqus/Session/Session.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Session/SessionBase.py` & `abqpy-2023.5.2/src/abaqus/Session/SessionBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketch.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketch.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchBase.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/CoincidentConstraint.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/CoincidentConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/ConcentricConstraint.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/ConcentricConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/ConstrainedSketchConstraintModel.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/ConstrainedSketchConstraintModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualDistanceConstraint.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualDistanceConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualLengthConstraint.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualLengthConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualRadiusConstraint.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/EqualRadiusConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/FixedConstraint.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/FixedConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/HorizontalConstraint.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/HorizontalConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/ParallelConstraint.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/ParallelConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/PerpendicularConstraint.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/PerpendicularConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/TangentConstraint.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/TangentConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchConstraint/VerticalConstraint.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchConstraint/VerticalConstraint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/AngularDimension.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/AngularDimension.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/ConstrainedSketchDimensionModel.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/ConstrainedSketchDimensionModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/DistanceDimension.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/DistanceDimension.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/HorizontalDimension.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/HorizontalDimension.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/ObliqueDimension.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/ObliqueDimension.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/RadialDimension.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/RadialDimension.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchDimension/VerticalDimension.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchDimension/VerticalDimension.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/Arc3Points.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/Arc3Points.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ArcByCenterEnds.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ArcByCenterEnds.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ArcByStartEndTangent.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ArcByStartEndTangent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/CircleByCenterPerimeter.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/CircleByCenterPerimeter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometry.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometry.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometryArray.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometryArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometryModel.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstrainedSketchGeometryModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstructionCircleByCenterPerimeter.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstructionCircleByCenterPerimeter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstructionLine.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/ConstructionLine.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/EllipseByCenterPerimeter.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/EllipseByCenterPerimeter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/FilletByRadius.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/FilletByRadius.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/Line.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/Line.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/Spline.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/Spline.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/Spot.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/Spot.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchGeometry/getPointAtDistance.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchGeometry/getPointAtDistance.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketchImageOptions.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketchImageOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketchOptions.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketchOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketcherOptions.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchOptions/ConstrainedSketcherOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchParameter/ConstrainedSketchParameter.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchParameter/ConstrainedSketchParameter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchParameter/ConstrainedSketchParameterModel.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchParameter/ConstrainedSketchParameterModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchParameter/Parameter.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchParameter/Parameter.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertex.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertex.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertexArray.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertexArray.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertexModel.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchVertex/ConstrainedSketchVertexModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/ConstrainedSketchVertex/Spot.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/ConstrainedSketchVertex/Spot.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Sketcher/SketchModel.py` & `abqpy-2023.5.2/src/abaqus/Sketcher/SketchModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/AnalysisStep.py` & `abqpy-2023.5.2/src/abaqus/Step/AnalysisStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/AnnealStep.py` & `abqpy-2023.5.2/src/abaqus/Step/AnnealStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/BuckleStep.py` & `abqpy-2023.5.2/src/abaqus/Step/BuckleStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/ComplexFrequencyStep.py` & `abqpy-2023.5.2/src/abaqus/Step/ComplexFrequencyStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/CoupledTempDisplacementStep.py` & `abqpy-2023.5.2/src/abaqus/Step/CoupledTempDisplacementStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/CoupledThermalElectricStep.py` & `abqpy-2023.5.2/src/abaqus/Step/CoupledThermalElectricStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/CoupledThermalElectricalStructuralStep.py` & `abqpy-2023.5.2/src/abaqus/Step/CoupledThermalElectricalStructuralStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/DirectCyclicStep.py` & `abqpy-2023.5.2/src/abaqus/Step/DirectCyclicStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/EmagTimeHarmonicStep.py` & `abqpy-2023.5.2/src/abaqus/Step/EmagTimeHarmonicStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/ExplicitDynamicsStep.py` & `abqpy-2023.5.2/src/abaqus/Step/ExplicitDynamicsStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/FrequencyStep.py` & `abqpy-2023.5.2/src/abaqus/Step/FrequencyStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/GeostaticStep.py` & `abqpy-2023.5.2/src/abaqus/Step/GeostaticStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/HeatTransferStep.py` & `abqpy-2023.5.2/src/abaqus/Step/HeatTransferStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/ImplicitDynamicsStep.py` & `abqpy-2023.5.2/src/abaqus/Step/ImplicitDynamicsStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/InitialStep.py` & `abqpy-2023.5.2/src/abaqus/Step/InitialStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/MassDiffusionStep.py` & `abqpy-2023.5.2/src/abaqus/Step/MassDiffusionStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/ModalDynamicsStep.py` & `abqpy-2023.5.2/src/abaqus/Step/ModalDynamicsStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/RandomResponseStep.py` & `abqpy-2023.5.2/src/abaqus/Step/RandomResponseStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/ResponseSpectrumStep.py` & `abqpy-2023.5.2/src/abaqus/Step/ResponseSpectrumStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/SoilsStep.py` & `abqpy-2023.5.2/src/abaqus/Step/SoilsStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/StaticLinearPerturbationStep.py` & `abqpy-2023.5.2/src/abaqus/Step/StaticLinearPerturbationStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/StaticRiksStep.py` & `abqpy-2023.5.2/src/abaqus/Step/StaticStep.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,40 +6,42 @@
 
 from ..Adaptivity.AdaptiveMeshConstraintState import AdaptiveMeshConstraintState
 from ..Adaptivity.AdaptiveMeshDomain import AdaptiveMeshDomain
 from ..BoundaryCondition.BoundaryConditionState import BoundaryConditionState
 from ..Load.LoadCase import LoadCase
 from ..Load.LoadState import LoadState
 from ..PredefinedField.PredefinedFieldState import PredefinedFieldState
-from ..Region.Region import Region
 from ..StepMiscellaneous.Control import Control
 from ..StepMiscellaneous.SolverControl import SolverControl
 from ..StepOutput.DiagnosticPrint import DiagnosticPrint
 from ..StepOutput.FieldOutputRequestState import FieldOutputRequestState
 from ..StepOutput.HistoryOutputRequestState import HistoryOutputRequestState
 from ..StepOutput.Monitor import Monitor
 from ..StepOutput.Restart import Restart
 from ..UtilityAndView.abaqusConstants import (
     AUTOMATIC,
+    DIRECT,
+    FULL_NEWTON,
     LINEAR,
+    NONE,
     OFF,
     PROPAGATED,
+    RAMP,
     SOLVER_DEFAULT,
     Boolean,
     SymbolicConstant,
 )
 from ..UtilityAndView.abaqusConstants import abaqusConstants as C
 from .AnalysisStep import AnalysisStep
 
 
 @abaqus_class_doc
-class StaticRiksStep(AnalysisStep):
-    """The StaticRiksStep object is used to indicate that the step should be analyzed as a static load step
-    using the modified Riks method for proportional loading cases. The StaticRiksStep object is derived from the
-    AnalysisStep object.
+class StaticStep(AnalysisStep):
+    """The StaticStep object is used to indicate that the step should be analyzed as a static load step. The
+    StaticStep object is derived from the AnalysisStep object.
 
     .. note::
         This object can be accessed by::
 
             import step
             mdb.models[name].steps[name]
 
@@ -48,103 +50,115 @@
         - STATIC
         - STEP
     """
 
     #: A String specifying the repository key.
     name: str = ""
 
+    #: A Float specifying the total time period. The default value is 1.0.
+    timePeriod: float = 1
+
     #: A Boolean specifying whether to allow for geometric nonlinearity. The default value is
     #: OFF.
     nlgeom: Boolean = OFF
 
+    #: A SymbolicConstant specifying the stabilization type. Possible values are NONE,
+    #: DISSIPATED_ENERGY_FRACTION, and DAMPING_FACTOR. The default value is NONE.
+    stabilizationMethod: SymbolicConstant = NONE
+
+    #: A Float specifying the damping intensity of the automatic damping algorithm if the
+    #: problem is expected to be unstable, and **stabilizationMethod** is not NONE. The default
+    #: value is 2x10⁻⁴.
+    stabilizationMagnitude: Optional[float] = None
+
     #: A Boolean specifying whether to perform an adiabatic stress analysis. The default value
     #: is OFF.
     adiabatic: Boolean = OFF
 
-    #: None or a Float specifying the maximum value of the load proportionality factor. The
-    #: default value is None.
-    maxLPF: Optional[float] = None
-
-    #: A Boolean specifying whether to monitor the finishing displacement value at a node. The
-    #: default value is OFF.
-    nodeOn: Boolean = OFF
-
-    #: A Float specifying the value of the total displacement (or rotation) at the node and
-    #: degree of freedom that, if crossed during an increment, ends the step at the current
-    #: increment. This argument is required when **nodeOn** = ON. The default value is 0.0.
-    maximumDisplacement: float = 0
-
-    #: An Int specifying the degree of freedom being monitored. This argument is required when
-    #: **nodeOn** = ON. The default value is 0.
-    dof: int = 0
-
     #: A SymbolicConstant specifying the time incrementation method to be used. Possible values
     #: are FIXED and AUTOMATIC. The default value is AUTOMATIC.
     timeIncrementationMethod: SymbolicConstant = AUTOMATIC
 
     #: An Int specifying the maximum number of increments in a step. The default value is 100.
     maxNumInc: int = 100
 
-    #: A Float specifying the total load proportionality factor associated with the load in
-    #: this step. The default value is 1.0.
-    totalArcLength: float = 1
-
-    #: A Float specifying the initial load proportionality factor. The default value is the
-    #: total load proportionality factor for the step.
-    initialArcInc: Optional[float] = None
-
-    #: A Float specifying the minimum arc length increment allowed. The default value is the
-    #: smaller of the suggested initial load proportionality factor or 10−5 times the total
-    #: load proportionality factor for the step.
-    minArcInc: Optional[float] = None
-
-    #: A Float specifying the maximum arc length increment allowed. The default value is the
-    #: total load proportionality factor for the step.
-    maxArcInc: Optional[float] = None
+    #: A Float specifying the initial time increment. The default value is the total time
+    #: period for the step.
+    initialInc: Optional[float] = None
+
+    #: A Float specifying the minimum time increment allowed. The default value is the smaller
+    #: of the suggested initial time increment or 10⁻⁵ times the total time period.
+    minInc: Optional[float] = None
+
+    #: A Float specifying the maximum time increment allowed. The default value is the total
+    #: time period for the step.
+    maxInc: Optional[float] = None
+
+    #: A SymbolicConstant specifying the type of solver. Possible values are DIRECT and
+    #: ITERATIVE. The default value is DIRECT.
+    matrixSolver: SymbolicConstant = DIRECT
 
     #: A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
     #: UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
     matrixStorage: SymbolicConstant = SOLVER_DEFAULT
 
+    #: A SymbolicConstant specifying the amplitude variation for loading magnitudes during the
+    #: step. Possible values are STEP and RAMP. The default value is RAMP.
+    amplitude: SymbolicConstant = RAMP
+
     #: A SymbolicConstant specifying the type of extrapolation to use in determining the
     #: incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
     #: PARABOLIC. The default value is LINEAR.
     extrapolation: SymbolicConstant = LINEAR
 
     #: A Boolean specifying whether to accept the solution to an increment after the maximum
-    #: number of iterations allowed have been completed, even if the equilibrium tolerances are
+    #: number of iterations allowed has been completed, even if the equilibrium tolerances are
     #: not satisfied. The default value is OFF.Warning:You should set **noStop** = ON only in
     #: special cases when you have a thorough understanding of how to interpret the results.
     noStop: Boolean = OFF
 
     #: A Boolean specifying wether to obtain the fully relaxed long-term elastic solution with
     #: time-domain viscoelasticity or the long-term elastic-Plastic solution for two-layer
     #: viscoplasticity. The default value is OFF.
     useLongTermSolution: Boolean = OFF
 
+    #: A SymbolicConstant specifying the technique used to for solving nonlinear equations.
+    #: Possible values are FULL_NEWTON and QUASI_NEWTON. The default value is FULL_NEWTON.
+    solutionTechnique: SymbolicConstant = FULL_NEWTON
+
+    #: An Int specifying the number of quasi-Newton iterations allowed before the kernel matrix
+    #: is reformed.. The default value is 8.
+    reformKernel: int = 8
+
     #: A SymbolicConstant specifying whether to force a new iteration if severe discontinuities
     #: occur during an iteration. Possible values are PROPAGATED, CONVERT_SDI_OFF, and
     #: CONVERT_SDI_ON. The default value is PROPAGATED.
     convertSDI: SymbolicConstant = PROPAGATED
 
+    #: A Float specifying the maximum allowable ratio of the stabilization energy to the total
+    #: strain energy and can be used only if **stabilizationMethod** is not NONE. The default
+    #: value is 0.05.
+    adaptiveDampingRatio: float = 0
+
+    #: A Boolean specifying whether this step will carry over the damping factors from the
+    #: results of the preceding general step. This parameter must be used in conjunction with
+    #: the **adaptiveDampingRatio** parameter. The default value is OFF.
+    continueDampingFactors: Boolean = OFF
+
     #: A String specifying the name of the previous step. The new step appears after this step
     #: in the list of analysis steps.
     previous: str = ""
 
     #: A String specifying a description of the new step. The default value is an empty string.
     description: str = ""
 
-    #: A String specifying the name of the region being monitored for fully Plastic behavior.
-    #: The default value is an empty string.
+    #: A String specifying the region being monitored for fully Plastic behavior. The default
+    #: value is an empty string.
     fullyPlastic: str = ""
 
-    #: A Region object specifying the vertex at which the finishing displacement value is being
-    #: monitored. This argument is required when **nodeOn** = ON.
-    region: Region = Region()
-
     #: A SymbolicConstant specifying whether the step has an explicit procedure type
     #: (*procedureType* = ANNEAL, DYNAMIC_EXPLICIT, or DYNAMIC_TEMP_DISPLACEMENT).
     explicit: Optional[SymbolicConstant] = None
 
     #: A Boolean specifying whether the step has a perturbation procedure type.
     perturbation: Boolean = OFF
 
@@ -228,221 +242,245 @@
 
     @abaqus_method_doc
     def __init__(
         self,
         name: str,
         previous: str,
         description: str = "",
+        timePeriod: float = 1,
         nlgeom: Boolean = OFF,
+        stabilizationMethod: Literal[C.DAMPING_FACTOR, C.DISSIPATED_ENERGY_FRACTION, C.NONE] = NONE,
+        stabilizationMagnitude: Optional[float] = None,
         adiabatic: Boolean = OFF,
-        maxLPF: Optional[float] = None,
-        nodeOn: Boolean = OFF,
-        maximumDisplacement: float = 0,
-        dof: int = 0,
-        region: Optional[Region] = None,
         timeIncrementationMethod: Literal[C.AUTOMATIC, C.FIXED] = AUTOMATIC,
         maxNumInc: int = 100,
-        totalArcLength: float = 1,
-        initialArcInc: Optional[float] = None,
-        minArcInc: Optional[float] = None,
-        maxArcInc: Optional[float] = None,
+        initialInc: Optional[float] = None,
+        minInc: Optional[float] = None,
+        maxInc: Optional[float] = None,
+        matrixSolver: Literal[C.DIRECT, C.ITERATIVE] = DIRECT,
         matrixStorage: Literal[C.SYMMETRIC, C.SOLVER_DEFAULT, C.UNSYMMETRIC] = SOLVER_DEFAULT,
+        amplitude: Literal[C.STEP, C.RAMP] = RAMP,
         extrapolation: Literal[C.PARABOLIC, C.NONE, C.LINEAR] = LINEAR,
         fullyPlastic: str = "",
         noStop: Boolean = OFF,
         maintainAttributes: Boolean = False,
         useLongTermSolution: Boolean = OFF,
+        solutionTechnique: Literal[C.QUASI_NEWTON, C.FULL_NEWTON] = FULL_NEWTON,
+        reformKernel: int = 8,
         convertSDI: Literal[C.CONVERT_SDI_OFF, C.PROPAGATED, C.CONVERT_SDI_ON] = PROPAGATED,
+        adaptiveDampingRatio: float = 0,
+        continueDampingFactors: Boolean = OFF,
     ):
-        """This method creates a StaticRiksStep object.
+        """This method creates a StaticStep object.
 
         .. note::
             This function can be accessed by::
 
-                mdb.models[name].StaticRiksStep
+                mdb.models[name].StaticStep
 
         Parameters
         ----------
         name
             A String specifying the repository key.
         previous
             A String specifying the name of the previous step. The new step appears after this step
             in the list of analysis steps.
         description
             A String specifying a description of the new step. The default value is an empty string.
+        timePeriod
+            A Float specifying the total time period. The default value is 1.0.
         nlgeom
             A Boolean specifying whether to allow for geometric nonlinearity. The default value is
             OFF.
+        stabilizationMethod
+            A SymbolicConstant specifying the stabilization type. Possible values are NONE,
+            DISSIPATED_ENERGY_FRACTION, and DAMPING_FACTOR. The default value is NONE.
+        stabilizationMagnitude
+            A Float specifying the damping intensity of the automatic damping algorithm if the
+            problem is expected to be unstable, and **stabilizationMethod** is not NONE. The default
+            value is 2x10⁻⁴.
         adiabatic
             A Boolean specifying whether to perform an adiabatic stress analysis. The default value
             is OFF.
-        maxLPF
-            None or a Float specifying the maximum value of the load proportionality factor. The
-            default value is None.
-        nodeOn
-            A Boolean specifying whether to monitor the finishing displacement value at a node. The
-            default value is OFF.
-        maximumDisplacement
-            A Float specifying the value of the total displacement (or rotation) at the node and
-            degree of freedom that, if crossed during an increment, ends the step at the current
-            increment. This argument is required when **nodeOn** = ON. The default value is 0.0.
-        dof
-            An Int specifying the degree of freedom being monitored. This argument is required when
-            **nodeOn** = ON. The default value is 0.
-        region
-            A Region object specifying the vertex at which the finishing displacement value is being
-            monitored. This argument is required when **nodeOn** = ON.
         timeIncrementationMethod
             A SymbolicConstant specifying the time incrementation method to be used. Possible values
             are FIXED and AUTOMATIC. The default value is AUTOMATIC.
         maxNumInc
             An Int specifying the maximum number of increments in a step. The default value is 100.
-        totalArcLength
-            A Float specifying the total load proportionality factor associated with the load in
-            this step. The default value is 1.0.
-        initialArcInc
-            A Float specifying the initial load proportionality factor. The default value is the
-            total load proportionality factor for the step.
-        minArcInc
-            A Float specifying the minimum arc length increment allowed. The default value is the
-            smaller of the suggested initial load proportionality factor or 10−5 times the total
-            load proportionality factor for the step.
-        maxArcInc
-            A Float specifying the maximum arc length increment allowed. The default value is the
-            total load proportionality factor for the step.
+        initialInc
+            A Float specifying the initial time increment. The default value is the total time
+            period for the step.
+        minInc
+            A Float specifying the minimum time increment allowed. The default value is the smaller
+            of the suggested initial time increment or 10⁻⁵ times the total time period.
+        maxInc
+            A Float specifying the maximum time increment allowed. The default value is the total
+            time period for the step.
+        matrixSolver
+            A SymbolicConstant specifying the type of solver. Possible values are DIRECT and
+            ITERATIVE. The default value is DIRECT.
         matrixStorage
             A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
             UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
+        amplitude
+            A SymbolicConstant specifying the amplitude variation for loading magnitudes during the
+            step. Possible values are STEP and RAMP. The default value is RAMP.
         extrapolation
             A SymbolicConstant specifying the type of extrapolation to use in determining the
             incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
             PARABOLIC. The default value is LINEAR.
         fullyPlastic
-            A String specifying the name of the region being monitored for fully Plastic behavior.
-            The default value is an empty string.
+            A String specifying the region being monitored for fully Plastic behavior. The default
+            value is an empty string.
         noStop
             A Boolean specifying whether to accept the solution to an increment after the maximum
-            number of iterations allowed have been completed, even if the equilibrium tolerances are
+            number of iterations allowed has been completed, even if the equilibrium tolerances are
             not satisfied. The default value is OFF.Warning:You should set **noStop** = ON only in
             special cases when you have a thorough understanding of how to interpret the results.
         maintainAttributes
             A Boolean specifying whether to retain attributes from an existing step with the same
             name. The default value is False.
         useLongTermSolution
             A Boolean specifying wether to obtain the fully relaxed long-term elastic solution with
             time-domain viscoelasticity or the long-term elastic-Plastic solution for two-layer
             viscoplasticity. The default value is OFF.
+        solutionTechnique
+            A SymbolicConstant specifying the technique used to for solving nonlinear equations.
+            Possible values are FULL_NEWTON and QUASI_NEWTON. The default value is FULL_NEWTON.
+        reformKernel
+            An Int specifying the number of quasi-Newton iterations allowed before the kernel matrix
+            is reformed.. The default value is 8.
         convertSDI
             A SymbolicConstant specifying whether to force a new iteration if severe discontinuities
             occur during an iteration. Possible values are PROPAGATED, CONVERT_SDI_OFF, and
             CONVERT_SDI_ON. The default value is PROPAGATED.
+        adaptiveDampingRatio
+            A Float specifying the maximum allowable ratio of the stabilization energy to the total
+            strain energy and can be used only if **stabilizationMethod** is not NONE. The default
+            value is 0.05.
+        continueDampingFactors
+            A Boolean specifying whether this step will carry over the damping factors from the
+            results of the preceding general step. This parameter must be used in conjunction with
+            the **adaptiveDampingRatio** parameter. The default value is OFF.
 
         Returns
         -------
-        StaticRiksStep
-            A StaticRiksStep object.
+        StaticStep
+            A StaticStep object.
 
         Raises
         ------
         RangeError
         """
         super().__init__()
 
     @abaqus_method_doc
     def setValues(
         self,
         description: str = "",
+        timePeriod: float = 1,
         nlgeom: Boolean = OFF,
+        stabilizationMethod: Literal[C.DAMPING_FACTOR, C.DISSIPATED_ENERGY_FRACTION, C.NONE] = NONE,
+        stabilizationMagnitude: Optional[float] = None,
         adiabatic: Boolean = OFF,
-        maxLPF: Optional[float] = None,
-        nodeOn: Boolean = OFF,
-        maximumDisplacement: float = 0,
-        dof: int = 0,
-        region: Optional[Region] = None,
         timeIncrementationMethod: Literal[C.AUTOMATIC, C.FIXED] = AUTOMATIC,
         maxNumInc: int = 100,
-        totalArcLength: float = 1,
-        initialArcInc: Optional[float] = None,
-        minArcInc: Optional[float] = None,
-        maxArcInc: Optional[float] = None,
+        initialInc: Optional[float] = None,
+        minInc: Optional[float] = None,
+        maxInc: Optional[float] = None,
+        matrixSolver: Literal[C.DIRECT, C.ITERATIVE] = DIRECT,
         matrixStorage: Literal[C.SYMMETRIC, C.SOLVER_DEFAULT, C.UNSYMMETRIC] = SOLVER_DEFAULT,
+        amplitude: Literal[C.STEP, C.RAMP] = RAMP,
         extrapolation: Literal[C.PARABOLIC, C.NONE, C.LINEAR] = LINEAR,
         fullyPlastic: str = "",
         noStop: Boolean = OFF,
         useLongTermSolution: Boolean = OFF,
+        solutionTechnique: Literal[C.QUASI_NEWTON, C.FULL_NEWTON] = FULL_NEWTON,
+        reformKernel: int = 8,
         convertSDI: Literal[C.CONVERT_SDI_OFF, C.PROPAGATED, C.CONVERT_SDI_ON] = PROPAGATED,
+        adaptiveDampingRatio: float = 0,
+        continueDampingFactors: Boolean = OFF,
     ):
-        """This method modifies the StaticRiksStep object.
+        """This method modifies the StaticStep object.
 
         Parameters
         ----------
         description
             A String specifying a description of the new step. The default value is an empty string.
+        timePeriod
+            A Float specifying the total time period. The default value is 1.0.
         nlgeom
             A Boolean specifying whether to allow for geometric nonlinearity. The default value is
             OFF.
+        stabilizationMethod
+            A SymbolicConstant specifying the stabilization type. Possible values are NONE,
+            DISSIPATED_ENERGY_FRACTION, and DAMPING_FACTOR. The default value is NONE.
+        stabilizationMagnitude
+            A Float specifying the damping intensity of the automatic damping algorithm if the
+            problem is expected to be unstable, and **stabilizationMethod** is not NONE. The default
+            value is 2x10⁻⁴.
         adiabatic
             A Boolean specifying whether to perform an adiabatic stress analysis. The default value
             is OFF.
-        maxLPF
-            None or a Float specifying the maximum value of the load proportionality factor. The
-            default value is None.
-        nodeOn
-            A Boolean specifying whether to monitor the finishing displacement value at a node. The
-            default value is OFF.
-        maximumDisplacement
-            A Float specifying the value of the total displacement (or rotation) at the node and
-            degree of freedom that, if crossed during an increment, ends the step at the current
-            increment. This argument is required when **nodeOn** = ON. The default value is 0.0.
-        dof
-            An Int specifying the degree of freedom being monitored. This argument is required when
-            **nodeOn** = ON. The default value is 0.
-        region
-            A Region object specifying the vertex at which the finishing displacement value is being
-            monitored. This argument is required when **nodeOn** = ON.
         timeIncrementationMethod
             A SymbolicConstant specifying the time incrementation method to be used. Possible values
             are FIXED and AUTOMATIC. The default value is AUTOMATIC.
         maxNumInc
             An Int specifying the maximum number of increments in a step. The default value is 100.
-        totalArcLength
-            A Float specifying the total load proportionality factor associated with the load in
-            this step. The default value is 1.0.
-        initialArcInc
-            A Float specifying the initial load proportionality factor. The default value is the
-            total load proportionality factor for the step.
-        minArcInc
-            A Float specifying the minimum arc length increment allowed. The default value is the
-            smaller of the suggested initial load proportionality factor or 10−5 times the total
-            load proportionality factor for the step.
-        maxArcInc
-            A Float specifying the maximum arc length increment allowed. The default value is the
-            total load proportionality factor for the step.
+        initialInc
+            A Float specifying the initial time increment. The default value is the total time
+            period for the step.
+        minInc
+            A Float specifying the minimum time increment allowed. The default value is the smaller
+            of the suggested initial time increment or 10⁻⁵ times the total time period.
+        maxInc
+            A Float specifying the maximum time increment allowed. The default value is the total
+            time period for the step.
+        matrixSolver
+            A SymbolicConstant specifying the type of solver. Possible values are DIRECT and
+            ITERATIVE. The default value is DIRECT.
         matrixStorage
             A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
             UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
+        amplitude
+            A SymbolicConstant specifying the amplitude variation for loading magnitudes during the
+            step. Possible values are STEP and RAMP. The default value is RAMP.
         extrapolation
             A SymbolicConstant specifying the type of extrapolation to use in determining the
             incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
             PARABOLIC. The default value is LINEAR.
         fullyPlastic
-            A String specifying the name of the region being monitored for fully Plastic behavior.
-            The default value is an empty string.
+            A String specifying the region being monitored for fully Plastic behavior. The default
+            value is an empty string.
         noStop
             A Boolean specifying whether to accept the solution to an increment after the maximum
-            number of iterations allowed have been completed, even if the equilibrium tolerances are
+            number of iterations allowed has been completed, even if the equilibrium tolerances are
             not satisfied. The default value is OFF.Warning:You should set **noStop** = ON only in
             special cases when you have a thorough understanding of how to interpret the results.
         useLongTermSolution
             A Boolean specifying wether to obtain the fully relaxed long-term elastic solution with
             time-domain viscoelasticity or the long-term elastic-Plastic solution for two-layer
             viscoplasticity. The default value is OFF.
+        solutionTechnique
+            A SymbolicConstant specifying the technique used to for solving nonlinear equations.
+            Possible values are FULL_NEWTON and QUASI_NEWTON. The default value is FULL_NEWTON.
+        reformKernel
+            An Int specifying the number of quasi-Newton iterations allowed before the kernel matrix
+            is reformed.. The default value is 8.
         convertSDI
             A SymbolicConstant specifying whether to force a new iteration if severe discontinuities
             occur during an iteration. Possible values are PROPAGATED, CONVERT_SDI_OFF, and
             CONVERT_SDI_ON. The default value is PROPAGATED.
+        adaptiveDampingRatio
+            A Float specifying the maximum allowable ratio of the stabilization energy to the total
+            strain energy and can be used only if **stabilizationMethod** is not NONE. The default
+            value is 0.05.
+        continueDampingFactors
+            A Boolean specifying whether this step will carry over the damping factors from the
+            results of the preceding general step. This parameter must be used in conjunction with
+            the **adaptiveDampingRatio** parameter. The default value is OFF.
 
         Raises
         ------
         RangeError
         """
         ...
```

### Comparing `abqpy-2023.5.1/src/abaqus/Step/StaticStep.py` & `abqpy-2023.5.2/src/abaqus/Step/ViscoStep.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,41 +17,43 @@
 from ..StepOutput.HistoryOutputRequestState import HistoryOutputRequestState
 from ..StepOutput.Monitor import Monitor
 from ..StepOutput.Restart import Restart
 from ..UtilityAndView.abaqusConstants import (
     AUTOMATIC,
     DIRECT,
     FULL_NEWTON,
+    IMPLICIT_EXPLICIT,
     LINEAR,
     NONE,
     OFF,
     PROPAGATED,
-    RAMP,
     SOLVER_DEFAULT,
+    STEP,
     Boolean,
     SymbolicConstant,
 )
 from ..UtilityAndView.abaqusConstants import abaqusConstants as C
 from .AnalysisStep import AnalysisStep
 
 
 @abaqus_class_doc
-class StaticStep(AnalysisStep):
-    """The StaticStep object is used to indicate that the step should be analyzed as a static load step. The
-    StaticStep object is derived from the AnalysisStep object.
+class ViscoStep(AnalysisStep):
+    """The ViscoStep object is used to obtain a transient static response in an analysis with time-dependent
+    material behavior (creep, swelling, and viscoelasticity). The ViscoStep object is derived from the
+    AnalysisStep object.
 
     .. note::
         This object can be accessed by::
 
             import step
             mdb.models[name].steps[name]
 
         The corresponding analysis keywords are:
 
-        - STATIC
+        - VISCO
         - STEP
     """
 
     #: A String specifying the repository key.
     name: str = ""
 
     #: A Float specifying the total time period. The default value is 1.0.
@@ -66,65 +68,60 @@
     stabilizationMethod: SymbolicConstant = NONE
 
     #: A Float specifying the damping intensity of the automatic damping algorithm if the
     #: problem is expected to be unstable, and **stabilizationMethod** is not NONE. The default
     #: value is 2x10⁻⁴.
     stabilizationMagnitude: Optional[float] = None
 
-    #: A Boolean specifying whether to perform an adiabatic stress analysis. The default value
-    #: is OFF.
-    adiabatic: Boolean = OFF
-
     #: A SymbolicConstant specifying the time incrementation method to be used. Possible values
     #: are FIXED and AUTOMATIC. The default value is AUTOMATIC.
     timeIncrementationMethod: SymbolicConstant = AUTOMATIC
 
-    #: An Int specifying the maximum number of increments in a step. The default value is 100.
-    maxNumInc: int = 100
+    #: A SymbolicConstant specifying the type of solver. Possible values are DIRECT and
+    #: ITERATIVE. The default value is DIRECT.
+    matrixSolver: SymbolicConstant = DIRECT
+
+    #: A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
+    #: UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
+    matrixStorage: SymbolicConstant = SOLVER_DEFAULT
 
     #: A Float specifying the initial time increment. The default value is the total time
     #: period for the step.
     initialInc: Optional[float] = None
 
+    #: An Int specifying the maximum number of increments in a step. The default value is 100.
+    maxNumInc: int = 100
+
     #: A Float specifying the minimum time increment allowed. The default value is the smaller
-    #: of the suggested initial time increment or 10⁻⁵ times the total time period.
+    #: of the suggested initial time increment or 10−5 times the total time period.
     minInc: Optional[float] = None
 
-    #: A Float specifying the maximum time increment allowed. The default value is the total
-    #: time period for the step.
-    maxInc: Optional[float] = None
-
-    #: A SymbolicConstant specifying the type of solver. Possible values are DIRECT and
-    #: ITERATIVE. The default value is DIRECT.
-    matrixSolver: SymbolicConstant = DIRECT
-
-    #: A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
-    #: UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
-    matrixStorage: SymbolicConstant = SOLVER_DEFAULT
+    #: A Float specifying the maximum time increment allowed. The default is the total time
+    #: period for the step. The default value is 1.0.
+    maxInc: float = 1
+
+    #: A SymbolicConstant specifying which type of integration to use throughout the step.
+    #: Possible values are IMPLICIT_EXPLICIT and EXPLICIT_ONLY. The default value is
+    #: IMPLICIT_EXPLICIT.
+    integration: SymbolicConstant = IMPLICIT_EXPLICIT
+
+    #: A Float specifying the maximum difference in the creep strain increment calculated from
+    #: the creep strain rates at the beginning and end of the increment. The default value is
+    #: 0.0.
+    cetol: float = 0
 
     #: A SymbolicConstant specifying the amplitude variation for loading magnitudes during the
-    #: step. Possible values are STEP and RAMP. The default value is RAMP.
-    amplitude: SymbolicConstant = RAMP
+    #: step. Possible values are STEP and RAMP. The default value is STEP.
+    amplitude: SymbolicConstant = STEP
 
     #: A SymbolicConstant specifying the type of extrapolation to use in determining the
     #: incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
     #: PARABOLIC. The default value is LINEAR.
     extrapolation: SymbolicConstant = LINEAR
 
-    #: A Boolean specifying whether to accept the solution to an increment after the maximum
-    #: number of iterations allowed has been completed, even if the equilibrium tolerances are
-    #: not satisfied. The default value is OFF.Warning:You should set **noStop** = ON only in
-    #: special cases when you have a thorough understanding of how to interpret the results.
-    noStop: Boolean = OFF
-
-    #: A Boolean specifying wether to obtain the fully relaxed long-term elastic solution with
-    #: time-domain viscoelasticity or the long-term elastic-Plastic solution for two-layer
-    #: viscoplasticity. The default value is OFF.
-    useLongTermSolution: Boolean = OFF
-
     #: A SymbolicConstant specifying the technique used to for solving nonlinear equations.
     #: Possible values are FULL_NEWTON and QUASI_NEWTON. The default value is FULL_NEWTON.
     solutionTechnique: SymbolicConstant = FULL_NEWTON
 
     #: An Int specifying the number of quasi-Newton iterations allowed before the kernel matrix
     #: is reformed.. The default value is 8.
     reformKernel: int = 8
@@ -147,18 +144,14 @@
     #: A String specifying the name of the previous step. The new step appears after this step
     #: in the list of analysis steps.
     previous: str = ""
 
     #: A String specifying a description of the new step. The default value is an empty string.
     description: str = ""
 
-    #: A String specifying the region being monitored for fully Plastic behavior. The default
-    #: value is an empty string.
-    fullyPlastic: str = ""
-
     #: A SymbolicConstant specifying whether the step has an explicit procedure type
     #: (*procedureType* = ANNEAL, DYNAMIC_EXPLICIT, or DYNAMIC_TEMP_DISPLACEMENT).
     explicit: Optional[SymbolicConstant] = None
 
     #: A Boolean specifying whether the step has a perturbation procedure type.
     perturbation: Boolean = OFF
 
@@ -246,40 +239,38 @@
         name: str,
         previous: str,
         description: str = "",
         timePeriod: float = 1,
         nlgeom: Boolean = OFF,
         stabilizationMethod: Literal[C.DAMPING_FACTOR, C.DISSIPATED_ENERGY_FRACTION, C.NONE] = NONE,
         stabilizationMagnitude: Optional[float] = None,
-        adiabatic: Boolean = OFF,
         timeIncrementationMethod: Literal[C.AUTOMATIC, C.FIXED] = AUTOMATIC,
-        maxNumInc: int = 100,
-        initialInc: Optional[float] = None,
-        minInc: Optional[float] = None,
-        maxInc: Optional[float] = None,
         matrixSolver: Literal[C.DIRECT, C.ITERATIVE] = DIRECT,
         matrixStorage: Literal[C.SYMMETRIC, C.SOLVER_DEFAULT, C.UNSYMMETRIC] = SOLVER_DEFAULT,
-        amplitude: Literal[C.STEP, C.RAMP] = RAMP,
+        initialInc: Optional[float] = None,
+        maxNumInc: int = 100,
+        minInc: Optional[float] = None,
+        maxInc: float = 1,
+        integration: Literal[C.EXPLICIT_ONLY, C.IMPLICIT_EXPLICIT] = IMPLICIT_EXPLICIT,
+        cetol: float = 0,
+        amplitude: Literal[C.STEP, C.RAMP] = STEP,
         extrapolation: Literal[C.PARABOLIC, C.NONE, C.LINEAR] = LINEAR,
-        fullyPlastic: str = "",
-        noStop: Boolean = OFF,
         maintainAttributes: Boolean = False,
-        useLongTermSolution: Boolean = OFF,
         solutionTechnique: Literal[C.QUASI_NEWTON, C.FULL_NEWTON] = FULL_NEWTON,
         reformKernel: int = 8,
         convertSDI: Literal[C.CONVERT_SDI_OFF, C.PROPAGATED, C.CONVERT_SDI_ON] = PROPAGATED,
         adaptiveDampingRatio: float = 0,
         continueDampingFactors: Boolean = OFF,
     ):
-        """This method creates a StaticStep object.
+        """This method creates a ViscoStep object.
 
         .. note::
             This function can be accessed by::
 
-                mdb.models[name].StaticStep
+                mdb.models[name].ViscoStep
 
         Parameters
         ----------
         name
             A String specifying the repository key.
         previous
             A String specifying the name of the previous step. The new step appears after this step
@@ -294,59 +285,52 @@
         stabilizationMethod
             A SymbolicConstant specifying the stabilization type. Possible values are NONE,
             DISSIPATED_ENERGY_FRACTION, and DAMPING_FACTOR. The default value is NONE.
         stabilizationMagnitude
             A Float specifying the damping intensity of the automatic damping algorithm if the
             problem is expected to be unstable, and **stabilizationMethod** is not NONE. The default
             value is 2x10⁻⁴.
-        adiabatic
-            A Boolean specifying whether to perform an adiabatic stress analysis. The default value
-            is OFF.
         timeIncrementationMethod
             A SymbolicConstant specifying the time incrementation method to be used. Possible values
             are FIXED and AUTOMATIC. The default value is AUTOMATIC.
-        maxNumInc
-            An Int specifying the maximum number of increments in a step. The default value is 100.
-        initialInc
-            A Float specifying the initial time increment. The default value is the total time
-            period for the step.
-        minInc
-            A Float specifying the minimum time increment allowed. The default value is the smaller
-            of the suggested initial time increment or 10⁻⁵ times the total time period.
-        maxInc
-            A Float specifying the maximum time increment allowed. The default value is the total
-            time period for the step.
         matrixSolver
             A SymbolicConstant specifying the type of solver. Possible values are DIRECT and
             ITERATIVE. The default value is DIRECT.
         matrixStorage
             A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
             UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
+        initialInc
+            A Float specifying the initial time increment. The default value is the total time
+            period for the step.
+        maxNumInc
+            An Int specifying the maximum number of increments in a step. The default value is 100.
+        minInc
+            A Float specifying the minimum time increment allowed. The default value is the smaller
+            of the suggested initial time increment or 10−5 times the total time period.
+        maxInc
+            A Float specifying the maximum time increment allowed. The default is the total time
+            period for the step. The default value is 1.0.
+        integration
+            A SymbolicConstant specifying which type of integration to use throughout the step.
+            Possible values are IMPLICIT_EXPLICIT and EXPLICIT_ONLY. The default value is
+            IMPLICIT_EXPLICIT.
+        cetol
+            A Float specifying the maximum difference in the creep strain increment calculated from
+            the creep strain rates at the beginning and end of the increment. The default value is
+            0.0.
         amplitude
             A SymbolicConstant specifying the amplitude variation for loading magnitudes during the
-            step. Possible values are STEP and RAMP. The default value is RAMP.
+            step. Possible values are STEP and RAMP. The default value is STEP.
         extrapolation
             A SymbolicConstant specifying the type of extrapolation to use in determining the
             incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
             PARABOLIC. The default value is LINEAR.
-        fullyPlastic
-            A String specifying the region being monitored for fully Plastic behavior. The default
-            value is an empty string.
-        noStop
-            A Boolean specifying whether to accept the solution to an increment after the maximum
-            number of iterations allowed has been completed, even if the equilibrium tolerances are
-            not satisfied. The default value is OFF.Warning:You should set **noStop** = ON only in
-            special cases when you have a thorough understanding of how to interpret the results.
         maintainAttributes
             A Boolean specifying whether to retain attributes from an existing step with the same
             name. The default value is False.
-        useLongTermSolution
-            A Boolean specifying wether to obtain the fully relaxed long-term elastic solution with
-            time-domain viscoelasticity or the long-term elastic-Plastic solution for two-layer
-            viscoplasticity. The default value is OFF.
         solutionTechnique
             A SymbolicConstant specifying the technique used to for solving nonlinear equations.
             Possible values are FULL_NEWTON and QUASI_NEWTON. The default value is FULL_NEWTON.
         reformKernel
             An Int specifying the number of quasi-Newton iterations allowed before the kernel matrix
             is reformed.. The default value is 8.
         convertSDI
@@ -360,16 +344,16 @@
         continueDampingFactors
             A Boolean specifying whether this step will carry over the damping factors from the
             results of the preceding general step. This parameter must be used in conjunction with
             the **adaptiveDampingRatio** parameter. The default value is OFF.
 
         Returns
         -------
-        StaticStep
-            A StaticStep object.
+        ViscoStep
+            A ViscoStep object.
 
         Raises
         ------
         RangeError
         """
         super().__init__()
 
@@ -377,34 +361,32 @@
     def setValues(
         self,
         description: str = "",
         timePeriod: float = 1,
         nlgeom: Boolean = OFF,
         stabilizationMethod: Literal[C.DAMPING_FACTOR, C.DISSIPATED_ENERGY_FRACTION, C.NONE] = NONE,
         stabilizationMagnitude: Optional[float] = None,
-        adiabatic: Boolean = OFF,
         timeIncrementationMethod: Literal[C.AUTOMATIC, C.FIXED] = AUTOMATIC,
-        maxNumInc: int = 100,
-        initialInc: Optional[float] = None,
-        minInc: Optional[float] = None,
-        maxInc: Optional[float] = None,
         matrixSolver: Literal[C.DIRECT, C.ITERATIVE] = DIRECT,
         matrixStorage: Literal[C.SYMMETRIC, C.SOLVER_DEFAULT, C.UNSYMMETRIC] = SOLVER_DEFAULT,
-        amplitude: Literal[C.STEP, C.RAMP] = RAMP,
+        initialInc: Optional[float] = None,
+        maxNumInc: int = 100,
+        minInc: Optional[float] = None,
+        maxInc: float = 1,
+        integration: Literal[C.EXPLICIT_ONLY, C.IMPLICIT_EXPLICIT] = IMPLICIT_EXPLICIT,
+        cetol: float = 0,
+        amplitude: Literal[C.STEP, C.RAMP] = STEP,
         extrapolation: Literal[C.PARABOLIC, C.NONE, C.LINEAR] = LINEAR,
-        fullyPlastic: str = "",
-        noStop: Boolean = OFF,
-        useLongTermSolution: Boolean = OFF,
         solutionTechnique: Literal[C.QUASI_NEWTON, C.FULL_NEWTON] = FULL_NEWTON,
         reformKernel: int = 8,
         convertSDI: Literal[C.CONVERT_SDI_OFF, C.PROPAGATED, C.CONVERT_SDI_ON] = PROPAGATED,
         adaptiveDampingRatio: float = 0,
         continueDampingFactors: Boolean = OFF,
     ):
-        """This method modifies the StaticStep object.
+        """This method modifies the ViscoStep object.
 
         Parameters
         ----------
         description
             A String specifying a description of the new step. The default value is an empty string.
         timePeriod
             A Float specifying the total time period. The default value is 1.0.
@@ -414,56 +396,49 @@
         stabilizationMethod
             A SymbolicConstant specifying the stabilization type. Possible values are NONE,
             DISSIPATED_ENERGY_FRACTION, and DAMPING_FACTOR. The default value is NONE.
         stabilizationMagnitude
             A Float specifying the damping intensity of the automatic damping algorithm if the
             problem is expected to be unstable, and **stabilizationMethod** is not NONE. The default
             value is 2x10⁻⁴.
-        adiabatic
-            A Boolean specifying whether to perform an adiabatic stress analysis. The default value
-            is OFF.
         timeIncrementationMethod
             A SymbolicConstant specifying the time incrementation method to be used. Possible values
             are FIXED and AUTOMATIC. The default value is AUTOMATIC.
-        maxNumInc
-            An Int specifying the maximum number of increments in a step. The default value is 100.
-        initialInc
-            A Float specifying the initial time increment. The default value is the total time
-            period for the step.
-        minInc
-            A Float specifying the minimum time increment allowed. The default value is the smaller
-            of the suggested initial time increment or 10⁻⁵ times the total time period.
-        maxInc
-            A Float specifying the maximum time increment allowed. The default value is the total
-            time period for the step.
         matrixSolver
             A SymbolicConstant specifying the type of solver. Possible values are DIRECT and
             ITERATIVE. The default value is DIRECT.
         matrixStorage
             A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
             UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
+        initialInc
+            A Float specifying the initial time increment. The default value is the total time
+            period for the step.
+        maxNumInc
+            An Int specifying the maximum number of increments in a step. The default value is 100.
+        minInc
+            A Float specifying the minimum time increment allowed. The default value is the smaller
+            of the suggested initial time increment or 10−5 times the total time period.
+        maxInc
+            A Float specifying the maximum time increment allowed. The default is the total time
+            period for the step. The default value is 1.0.
+        integration
+            A SymbolicConstant specifying which type of integration to use throughout the step.
+            Possible values are IMPLICIT_EXPLICIT and EXPLICIT_ONLY. The default value is
+            IMPLICIT_EXPLICIT.
+        cetol
+            A Float specifying the maximum difference in the creep strain increment calculated from
+            the creep strain rates at the beginning and end of the increment. The default value is
+            0.0.
         amplitude
             A SymbolicConstant specifying the amplitude variation for loading magnitudes during the
-            step. Possible values are STEP and RAMP. The default value is RAMP.
+            step. Possible values are STEP and RAMP. The default value is STEP.
         extrapolation
             A SymbolicConstant specifying the type of extrapolation to use in determining the
             incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
             PARABOLIC. The default value is LINEAR.
-        fullyPlastic
-            A String specifying the region being monitored for fully Plastic behavior. The default
-            value is an empty string.
-        noStop
-            A Boolean specifying whether to accept the solution to an increment after the maximum
-            number of iterations allowed has been completed, even if the equilibrium tolerances are
-            not satisfied. The default value is OFF.Warning:You should set **noStop** = ON only in
-            special cases when you have a thorough understanding of how to interpret the results.
-        useLongTermSolution
-            A Boolean specifying wether to obtain the fully relaxed long-term elastic solution with
-            time-domain viscoelasticity or the long-term elastic-Plastic solution for two-layer
-            viscoplasticity. The default value is OFF.
         solutionTechnique
             A SymbolicConstant specifying the technique used to for solving nonlinear equations.
             Possible values are FULL_NEWTON and QUASI_NEWTON. The default value is FULL_NEWTON.
         reformKernel
             An Int specifying the number of quasi-Newton iterations allowed before the kernel matrix
             is reformed.. The default value is 8.
         convertSDI
```

### Comparing `abqpy-2023.5.1/src/abaqus/Step/SteadyStateDirectStep.py` & `abqpy-2023.5.2/src/abaqus/Step/SteadyStateDirectStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/SteadyStateModalStep.py` & `abqpy-2023.5.2/src/abaqus/Step/SteadyStateModalStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/SteadyStateSubspaceStep.py` & `abqpy-2023.5.2/src/abaqus/Step/SteadyStateSubspaceStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/Step.py` & `abqpy-2023.5.2/src/abaqus/Step/Step.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/StepBase.py` & `abqpy-2023.5.2/src/abaqus/Step/StepBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/StepModel.py` & `abqpy-2023.5.2/src/abaqus/Step/StepModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/SubspaceDynamicsStep.py` & `abqpy-2023.5.2/src/abaqus/Step/SubspaceDynamicsStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/SubstructureGenerateStep.py` & `abqpy-2023.5.2/src/abaqus/Step/SubstructureGenerateStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/TempDisplacementDynamicsStep.py` & `abqpy-2023.5.2/src/abaqus/Step/TempDisplacementDynamicsStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/Step/ViscoStep.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/View.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,461 +1,513 @@
-from typing import Dict, Optional
+from __future__ import annotations
+
+from typing import Optional, Sequence, Tuple
 
 from typing_extensions import Literal
 
 from abqpy.decorators import abaqus_class_doc, abaqus_method_doc
 
-from ..Adaptivity.AdaptiveMeshConstraintState import AdaptiveMeshConstraintState
-from ..Adaptivity.AdaptiveMeshDomain import AdaptiveMeshDomain
-from ..BoundaryCondition.BoundaryConditionState import BoundaryConditionState
-from ..Load.LoadCase import LoadCase
-from ..Load.LoadState import LoadState
-from ..PredefinedField.PredefinedFieldState import PredefinedFieldState
-from ..StepMiscellaneous.Control import Control
-from ..StepMiscellaneous.SolverControl import SolverControl
-from ..StepOutput.DiagnosticPrint import DiagnosticPrint
-from ..StepOutput.FieldOutputRequestState import FieldOutputRequestState
-from ..StepOutput.HistoryOutputRequestState import HistoryOutputRequestState
-from ..StepOutput.Monitor import Monitor
-from ..StepOutput.Restart import Restart
-from ..UtilityAndView.abaqusConstants import (
-    AUTOMATIC,
-    DIRECT,
-    FULL_NEWTON,
-    IMPLICIT_EXPLICIT,
-    LINEAR,
-    NONE,
-    OFF,
-    PROPAGATED,
-    SOLVER_DEFAULT,
-    STEP,
-    Boolean,
-    SymbolicConstant,
-)
+from ..UtilityAndView.abaqusConstants import ABSOLUTE, MODEL, OFF, Boolean
 from ..UtilityAndView.abaqusConstants import abaqusConstants as C
-from .AnalysisStep import AnalysisStep
 
 
 @abaqus_class_doc
-class ViscoStep(AnalysisStep):
-    """The ViscoStep object is used to obtain a transient static response in an analysis with time-dependent
-    material behavior (creep, swelling, and viscoelasticity). The ViscoStep object is derived from the
-    AnalysisStep object.
+class View:
+    """The Session and Viewport View objects store view settings for custom (both predefined and user-defined)
+    views. The paradigm used to define a view is based on a camera analogy. Similar to taking a photograph with
+    a camera, features such as camera position, view direction, orientation, depth of field, and projection are
+    specified to transform three-dimensional views to the screen. The Layer View objects store a transformation
+    matrix used to position the contents of the Layer within a viewport.
 
     .. note::
         This object can be accessed by::
 
-            import step
-            mdb.models[name].steps[name]
-
-        The corresponding analysis keywords are:
-
-        - VISCO
-        - STEP
+            session.viewports[name].layers[name].view
+            session.viewports[name].view
+            session.views[name]
     """
 
-    #: A String specifying the repository key.
-    name: str = ""
-
-    #: A Float specifying the total time period. The default value is 1.0.
-    timePeriod: float = 1
+    #: A Float specifying the width in viewport millimeters of the bounding rectangle around
+    #: the viewport contents. This value does not include annotations or symbols and it is not
+    #: clipped to the size of the viewport window.
+    displayedObjectScreenWidth: Optional[float] = None
+
+    #: A Float specifying the height in viewport millimeters of the bounding rectangle around
+    #: the viewport contents. This value does not include annotations or symbols and it is not
+    #: clipped to the size of the viewport window.
+    displayedObjectScreenHeight: Optional[float] = None
+
+    #: A tuple of Floats specifying a transformation matrix used to position the contents of
+    #: the Layer within a viewport.
+    layerTransform: Optional[float] = None
+
+    #: A String specifying the name of the view (also used as the repository key). Possible
+    #: values are 'Front', 'Back', 'Top', 'Bottom', 'Left', 'Right', 'Iso', 'User-1', 'User-2',
+    #: 'User-3', and 'User-4'. The object member associated with this argument is a
+    #: SymbolicConstant. Possible values of the **name** member are: FRONT, BACK, TOP, BOTTOM,
+    #: LEFT, RIGHT, ISO, USER1, USER2, USER3, and USER4.
+    name: str
+
+    #: A Float specifying the distance from the camera to the near clipping plane. Possible
+    #: values are **nearPlane** > 0.0.
+    nearPlane: float
+
+    #: A Float specifying the distance from the camera to the far clipping plane when
+    #: **farPlaneMode** =SPECIFY. Possible values are **farPlane** > **nearPlane**.
+    farPlane: float
 
-    #: A Boolean specifying whether to allow for geometric nonlinearity. The default value is
-    #: OFF.
-    nlgeom: Boolean = OFF
-
-    #: A SymbolicConstant specifying the stabilization type. Possible values are NONE,
-    #: DISSIPATED_ENERGY_FRACTION, and DAMPING_FACTOR. The default value is NONE.
-    stabilizationMethod: SymbolicConstant = NONE
-
-    #: A Float specifying the damping intensity of the automatic damping algorithm if the
-    #: problem is expected to be unstable, and **stabilizationMethod** is not NONE. The default
-    #: value is 2x10⁻⁴.
-    stabilizationMagnitude: Optional[float] = None
-
-    #: A SymbolicConstant specifying the time incrementation method to be used. Possible values
-    #: are FIXED and AUTOMATIC. The default value is AUTOMATIC.
-    timeIncrementationMethod: SymbolicConstant = AUTOMATIC
-
-    #: A SymbolicConstant specifying the type of solver. Possible values are DIRECT and
-    #: ITERATIVE. The default value is DIRECT.
-    matrixSolver: SymbolicConstant = DIRECT
-
-    #: A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
-    #: UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
-    matrixStorage: SymbolicConstant = SOLVER_DEFAULT
-
-    #: A Float specifying the initial time increment. The default value is the total time
-    #: period for the step.
-    initialInc: Optional[float] = None
-
-    #: An Int specifying the maximum number of increments in a step. The default value is 100.
-    maxNumInc: int = 100
-
-    #: A Float specifying the minimum time increment allowed. The default value is the smaller
-    #: of the suggested initial time increment or 10−5 times the total time period.
-    minInc: Optional[float] = None
-
-    #: A Float specifying the maximum time increment allowed. The default is the total time
-    #: period for the step. The default value is 1.0.
-    maxInc: float = 1
-
-    #: A SymbolicConstant specifying which type of integration to use throughout the step.
-    #: Possible values are IMPLICIT_EXPLICIT and EXPLICIT_ONLY. The default value is
-    #: IMPLICIT_EXPLICIT.
-    integration: SymbolicConstant = IMPLICIT_EXPLICIT
-
-    #: A Float specifying the maximum difference in the creep strain increment calculated from
-    #: the creep strain rates at the beginning and end of the increment. The default value is
+    #: A Float specifying the width of the front clipping plane. Possible values are **width** >
     #: 0.0.
-    cetol: float = 0
-
-    #: A SymbolicConstant specifying the amplitude variation for loading magnitudes during the
-    #: step. Possible values are STEP and RAMP. The default value is STEP.
-    amplitude: SymbolicConstant = STEP
-
-    #: A SymbolicConstant specifying the type of extrapolation to use in determining the
-    #: incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
-    #: PARABOLIC. The default value is LINEAR.
-    extrapolation: SymbolicConstant = LINEAR
-
-    #: A SymbolicConstant specifying the technique used to for solving nonlinear equations.
-    #: Possible values are FULL_NEWTON and QUASI_NEWTON. The default value is FULL_NEWTON.
-    solutionTechnique: SymbolicConstant = FULL_NEWTON
-
-    #: An Int specifying the number of quasi-Newton iterations allowed before the kernel matrix
-    #: is reformed.. The default value is 8.
-    reformKernel: int = 8
-
-    #: A SymbolicConstant specifying whether to force a new iteration if severe discontinuities
-    #: occur during an iteration. Possible values are PROPAGATED, CONVERT_SDI_OFF, and
-    #: CONVERT_SDI_ON. The default value is PROPAGATED.
-    convertSDI: SymbolicConstant = PROPAGATED
-
-    #: A Float specifying the maximum allowable ratio of the stabilization energy to the total
-    #: strain energy and can be used only if **stabilizationMethod** is not NONE. The default
-    #: value is 0.05.
-    adaptiveDampingRatio: float = 0
-
-    #: A Boolean specifying whether this step will carry over the damping factors from the
-    #: results of the preceding general step. This parameter must be used in conjunction with
-    #: the **adaptiveDampingRatio** parameter. The default value is OFF.
-    continueDampingFactors: Boolean = OFF
-
-    #: A String specifying the name of the previous step. The new step appears after this step
-    #: in the list of analysis steps.
-    previous: str = ""
-
-    #: A String specifying a description of the new step. The default value is an empty string.
-    description: str = ""
-
-    #: A SymbolicConstant specifying whether the step has an explicit procedure type
-    #: (*procedureType* = ANNEAL, DYNAMIC_EXPLICIT, or DYNAMIC_TEMP_DISPLACEMENT).
-    explicit: Optional[SymbolicConstant] = None
-
-    #: A Boolean specifying whether the step has a perturbation procedure type.
-    perturbation: Boolean = OFF
-
-    #: A Boolean specifying whether the step has a mechanical procedure type.
-    nonmechanical: Boolean = OFF
-
-    #: A SymbolicConstant specifying the Abaqus procedure. Possible values are:
-    #:
-    #: - ANNEAL
-    #: - BUCKLE
-    #: - COMPLEX_FREQUENCY
-    #: - COUPLED_TEMP_DISPLACEMENT
-    #: - COUPLED_THERMAL_ELECTRIC
-    #: - DIRECT_CYCLIC
-    #: - DYNAMIC_IMPLICIT
-    #: - DYNAMIC_EXPLICIT
-    #: - DYNAMIC_SUBSPACE
-    #: - DYNAMIC_TEMP_DISPLACEMENT
-    #: - COUPLED_THERMAL_ELECTRICAL_STRUCTURAL
-    #: - FREQUENCY
-    #: - GEOSTATIC
-    #: - HEAT_TRANSFER
-    #: - MASS_DIFFUSION
-    #: - MODAL_DYNAMICS
-    #: - RANDOM_RESPONSE
-    #: - RESPONSE_SPECTRUM
-    #: - SOILS
-    #: - STATIC_GENERAL
-    #: - STATIC_LINEAR_PERTURBATION
-    #: - STATIC_RIKS
-    #: - STEADY_STATE_DIRECT
-    #: - STEADY_STATE_MODAL
-    #: - STEADY_STATE_SUBSPACE
-    #: - VISCO
-    procedureType: Optional[SymbolicConstant] = None
-
-    #: A Boolean specifying whether the step is suppressed or not. The default value is OFF.
-    suppressed: Boolean = OFF
-
-    #: A repository of FieldOutputRequestState objects.
-    fieldOutputRequestState: Dict[str, FieldOutputRequestState] = {}
-
-    #: A repository of HistoryOutputRequestState objects.
-    historyOutputRequestState: Dict[str, HistoryOutputRequestState] = {}
-
-    #: A DiagnosticPrint object.
-    diagnosticPrint: DiagnosticPrint = DiagnosticPrint()
-
-    #: A Monitor object.
-    monitor: Optional[Monitor] = None
-
-    #: A Restart object.
-    restart: Restart = Restart()
-
-    #: A repository of AdaptiveMeshConstraintState objects.
-    adaptiveMeshConstraintStates: Dict[str, AdaptiveMeshConstraintState] = {}
-
-    #: A repository of AdaptiveMeshDomain objects.
-    adaptiveMeshDomains: Dict[str, AdaptiveMeshDomain] = {}
-
-    #: A Control object.
-    control: Control = Control()
-
-    #: A SolverControl object.
-    solverControl: SolverControl = SolverControl()
-
-    #: A repository of BoundaryConditionState objects.
-    boundaryConditionStates: Dict[str, BoundaryConditionState] = {}
-
-    #: A repository of InteractionState objects.
-    interactionStates: Optional[int] = None
+    width: float
 
-    #: A repository of LoadState objects.
-    loadStates: Dict[str, LoadState] = {}
+    #: A Float specifying the height of the front clipping plane. Possible values are **height**
+    #: > 0.0.
+    height: float
+
+    #: A SymbolicConstant specifying the projection mode. Possible values are PERSPECTIVE and
+    #: PARALLEL.
+    projection: Literal[C.PERSPECTIVE, C.PARALLEL]
+
+    #: A sequence of three Floats specifying the camera position.
+    cameraPosition: Tuple[float, float, float]
+
+    #: A sequence of three Floats specifying the camera's up vector (the screen's positive
+    #: **Y** axis). The initial value is (0, 0, 0).
+    cameraUpVector: Tuple[float, float, float]
+
+    #: A sequence of three Floats specifying the center of the scene.
+    cameraTarget: Tuple[float, float, float]
+
+    #: A Float specifying the amount to pan the model in the screen **X** direction as a fraction
+    #: of the viewport width. A positive value pans the model to the right. A negative value
+    #: pans the model to the left. The *viewOffsetX* and **viewOffsetY** arguments allow you to pan
+    #: the view without changing the position of the camera or the target (*cameraPosition* and
+    #: **cameraTarget** arguments to the View method). The resulting change in the view allows
+    #: you to pan a perspective display without producing an apparent rotation of the model.
+    viewOffsetX: float
+
+    #: A Float specifying the amount to pan the model in the screen **Y** direction as a fraction
+    #: of the viewport height. A positive value pans the model upward. A negative value pans
+    #: the model downward.
+    viewOffsetY: float
 
-    #: A repository of LoadCase objects.
-    loadCases: Dict[str, LoadCase] = {}
+    #: A Boolean specifying whether the view is auto-fit when applied.
+    autoFit: Boolean
 
-    #: A repository of PredefinedFieldState objects.
-    predefinedFieldStates: Dict[str, PredefinedFieldState] = {}
+    #: A Boolean specifying whether or not the camera is in movie mode. The default value is
+    #: OFF.
+    movieMode: Boolean = OFF
 
     @abaqus_method_doc
     def __init__(
         self,
         name: str,
-        previous: str,
-        description: str = "",
-        timePeriod: float = 1,
-        nlgeom: Boolean = OFF,
-        stabilizationMethod: Literal[C.DAMPING_FACTOR, C.DISSIPATED_ENERGY_FRACTION, C.NONE] = NONE,
-        stabilizationMagnitude: Optional[float] = None,
-        timeIncrementationMethod: Literal[C.AUTOMATIC, C.FIXED] = AUTOMATIC,
-        matrixSolver: Literal[C.DIRECT, C.ITERATIVE] = DIRECT,
-        matrixStorage: Literal[C.SYMMETRIC, C.SOLVER_DEFAULT, C.UNSYMMETRIC] = SOLVER_DEFAULT,
-        initialInc: Optional[float] = None,
-        maxNumInc: int = 100,
-        minInc: Optional[float] = None,
-        maxInc: float = 1,
-        integration: Literal[C.EXPLICIT_ONLY, C.IMPLICIT_EXPLICIT] = IMPLICIT_EXPLICIT,
-        cetol: float = 0,
-        amplitude: Literal[C.STEP, C.RAMP] = STEP,
-        extrapolation: Literal[C.PARABOLIC, C.NONE, C.LINEAR] = LINEAR,
-        maintainAttributes: Boolean = False,
-        solutionTechnique: Literal[C.QUASI_NEWTON, C.FULL_NEWTON] = FULL_NEWTON,
-        reformKernel: int = 8,
-        convertSDI: Literal[C.CONVERT_SDI_OFF, C.PROPAGATED, C.CONVERT_SDI_ON] = PROPAGATED,
-        adaptiveDampingRatio: float = 0,
-        continueDampingFactors: Boolean = OFF,
+        nearPlane: float,
+        farPlane: float,
+        width: float,
+        height: float,
+        projection: Literal[C.PERSPECTIVE, C.PARALLEL],
+        cameraPosition: Tuple[float, float, float],
+        cameraUpVector: Tuple[float, float, float],
+        cameraTarget: Tuple[float, float, float],
+        viewOffsetX: float,
+        viewOffsetY: float,
+        autoFit: Boolean,
+        movieMode: Boolean = OFF,
     ):
-        """This method creates a ViscoStep object.
+        """This method creates a View object. Note:All dimensions and coordinates are specified in the model
+        coordinate system. Note:This method cannot be used to create a View for a Layer object.
 
         .. note::
             This function can be accessed by::
 
-                mdb.models[name].ViscoStep
+                session.View
 
         Parameters
         ----------
         name
-            A String specifying the repository key.
-        previous
-            A String specifying the name of the previous step. The new step appears after this step
-            in the list of analysis steps.
-        description
-            A String specifying a description of the new step. The default value is an empty string.
-        timePeriod
-            A Float specifying the total time period. The default value is 1.0.
-        nlgeom
-            A Boolean specifying whether to allow for geometric nonlinearity. The default value is
-            OFF.
-        stabilizationMethod
-            A SymbolicConstant specifying the stabilization type. Possible values are NONE,
-            DISSIPATED_ENERGY_FRACTION, and DAMPING_FACTOR. The default value is NONE.
-        stabilizationMagnitude
-            A Float specifying the damping intensity of the automatic damping algorithm if the
-            problem is expected to be unstable, and **stabilizationMethod** is not NONE. The default
-            value is 2x10⁻⁴.
-        timeIncrementationMethod
-            A SymbolicConstant specifying the time incrementation method to be used. Possible values
-            are FIXED and AUTOMATIC. The default value is AUTOMATIC.
-        matrixSolver
-            A SymbolicConstant specifying the type of solver. Possible values are DIRECT and
-            ITERATIVE. The default value is DIRECT.
-        matrixStorage
-            A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
-            UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
-        initialInc
-            A Float specifying the initial time increment. The default value is the total time
-            period for the step.
-        maxNumInc
-            An Int specifying the maximum number of increments in a step. The default value is 100.
-        minInc
-            A Float specifying the minimum time increment allowed. The default value is the smaller
-            of the suggested initial time increment or 10−5 times the total time period.
-        maxInc
-            A Float specifying the maximum time increment allowed. The default is the total time
-            period for the step. The default value is 1.0.
-        integration
-            A SymbolicConstant specifying which type of integration to use throughout the step.
-            Possible values are IMPLICIT_EXPLICIT and EXPLICIT_ONLY. The default value is
-            IMPLICIT_EXPLICIT.
-        cetol
-            A Float specifying the maximum difference in the creep strain increment calculated from
-            the creep strain rates at the beginning and end of the increment. The default value is
+            A String specifying the name of the view (also used as the repository key). Possible
+            values are 'Front', 'Back', 'Top', 'Bottom', 'Left', 'Right', 'Iso', 'User-1', 'User-2',
+            'User-3', and 'User-4'. The object member associated with this argument is a
+            SymbolicConstant. Possible values of the **name** member are:FRONT, BACK, TOP, BOTTOM,
+            LEFT, RIGHT, ISO, USER1, USER2, USER3, and USER4.
+        nearPlane
+            A Float specifying the distance from the camera to the near clipping plane. Possible
+            values are **nearPlane** > 0.0.
+        farPlane
+            A Float specifying the distance from the camera to the far clipping plane when
+            **farPlaneMode** =SPECIFY. Possible values are **farPlane** > **nearPlane**.
+        width
+            A Float specifying the width of the front clipping plane. Possible values are **width** >
             0.0.
-        amplitude
-            A SymbolicConstant specifying the amplitude variation for loading magnitudes during the
-            step. Possible values are STEP and RAMP. The default value is STEP.
-        extrapolation
-            A SymbolicConstant specifying the type of extrapolation to use in determining the
-            incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
-            PARABOLIC. The default value is LINEAR.
-        maintainAttributes
-            A Boolean specifying whether to retain attributes from an existing step with the same
-            name. The default value is False.
-        solutionTechnique
-            A SymbolicConstant specifying the technique used to for solving nonlinear equations.
-            Possible values are FULL_NEWTON and QUASI_NEWTON. The default value is FULL_NEWTON.
-        reformKernel
-            An Int specifying the number of quasi-Newton iterations allowed before the kernel matrix
-            is reformed.. The default value is 8.
-        convertSDI
-            A SymbolicConstant specifying whether to force a new iteration if severe discontinuities
-            occur during an iteration. Possible values are PROPAGATED, CONVERT_SDI_OFF, and
-            CONVERT_SDI_ON. The default value is PROPAGATED.
-        adaptiveDampingRatio
-            A Float specifying the maximum allowable ratio of the stabilization energy to the total
-            strain energy and can be used only if **stabilizationMethod** is not NONE. The default
-            value is 0.05.
-        continueDampingFactors
-            A Boolean specifying whether this step will carry over the damping factors from the
-            results of the preceding general step. This parameter must be used in conjunction with
-            the **adaptiveDampingRatio** parameter. The default value is OFF.
+        height
+            A Float specifying the height of the front clipping plane. Possible values are **height**
+            > 0.0.
+        projection
+            A SymbolicConstant specifying the projection mode. Possible values are PERSPECTIVE and
+            PARALLEL.
+        cameraPosition
+            A sequence of three Floats specifying the camera position.
+        cameraUpVector
+            A sequence of three Floats specifying the camera's up vector (the screen's positive
+            **Y** axis). The initial value is (0, 0, 0).
+        cameraTarget
+            A sequence of three Floats specifying the center of the scene.
+        viewOffsetX
+            A Float specifying the amount to pan the model in the screen **X** direction as a fraction
+            of the viewport width. A positive value pans the model to the right. A negative value
+            pans the model to the left. The *viewOffsetX* and **viewOffsetY** arguments allow you to pan
+            the view without changing the position of the camera or the target (*cameraPosition* and
+            **cameraTarget** arguments to the View method). The resulting change in the view allows
+            you to pan a perspective display without producing an apparent rotation of the model.
+        viewOffsetY
+            A Float specifying the amount to pan the model in the screen **Y** direction as a fraction
+            of the viewport height. A positive value pans the model upward. A negative value pans
+            the model downward.
+        autoFit
+            A Boolean specifying whether the view is auto-fit when applied.
+        movieMode
+            A Boolean specifying whether or not the camera is in movie mode. The default value is
+            OFF.
 
         Returns
         -------
-        ViscoStep
-            A ViscoStep object.
+        View
+            A View object.
 
         Raises
         ------
         RangeError
         """
-        super().__init__()
+        ...
+
+    @abaqus_method_doc
+    def fitView(self, drawImmediately: Boolean = False):
+        """This method scales the displayable object (such as a part, the assembly, or an **X - Y**
+        plot) to fit the viewport.
+
+        Parameters
+        ----------
+        drawImmediately
+            A Boolean specifying the viewport should refresh immediately after the command is
+            processed. This is typically only used when writing a script and it is desirable to show
+            intermediate results before the script completes. The default value is False.
+        """
+        ...
+
+    @abaqus_method_doc
+    def next(self, drawImmediately: Boolean = False):
+        """This method restores the view in the viewport to the next view setting in the list. (There is a list
+        of eight views stored for each viewport.) If there is no next view, no action is taken. Note:This method
+        is not available for a Layer View.
+
+        Parameters
+        ----------
+        drawImmediately
+            A Boolean specifying the viewport should refresh immediately after the command is
+            processed. This is typically only used when writing a script and it is desirable to show
+            intermediate results before the script completes. The default value is False.
+        """
+        ...
+
+    @abaqus_method_doc
+    def pan(
+        self,
+        xFraction: float = 0,
+        yFraction: float = 0,
+        asMovie: Boolean = OFF,
+        drawImmediately: Boolean = False,
+    ):
+        """This method pans the view in the viewport using absolute, not relative, mode.
+
+        Parameters
+        ----------
+        xFraction
+            A Float specifying the amount to pan the model in the screen **X** direction as a fraction
+            of the viewport width. A positive value pans the model to the right. A negative value
+            pans the model to the left. The default value is 0.0.
+        yFraction
+            A Float specifying the amount to pan the model in the screen **Y** direction as a fraction
+            of the viewport height. A positive value pans the model upward. A negative value pans
+            the model downward. The default value is 0.0.
+        asMovie
+            A Boolean specifying the alternate mode of the pan view manipulation should be used. The
+            default value is OFF. This argument is ignored for a Layer View.
+        drawImmediately
+            A Boolean specifying the viewport should refresh immediately after the command is
+            processed. This argument is typically used only when writing a script and it is
+            desirable to show intermediate results before the script completes. The default value is
+            False.
+        """
+        ...
+
+    @abaqus_method_doc
+    def previous(self, drawImmediately: Boolean = False):
+        """This method restores the view in the viewport to the previous view setting in the list. (There is a
+        list of eight views stored for each viewport.) If there is no previous view, no action is taken.
+        Note:This method is not available for a Layer View.
+
+        Parameters
+        ----------
+        drawImmediately
+            A Boolean specifying the viewport should refresh immediately after the command is
+            processed. This argument is typically used only when writing a script and it is
+            desirable to show intermediate results before the script completes. The default value is
+            False.
+        """
+        ...
+
+    @abaqus_method_doc
+    def rotate(
+        self,
+        xAngle: float = 0,
+        yAngle: float = 0,
+        zAngle: float = 0,
+        mode: Literal[C.TOTAL, C.SCREEN, C.MODEL] = MODEL,
+        asMovie: Boolean = OFF,
+        drawImmediately: Boolean = False,
+    ):
+        """This method rotates the view in the viewport. If a center of rotation has been previously specified
+        and **asMovie** is OFF then this method will honor that rotation center.
+
+        Parameters
+        ----------
+        xAngle
+            A Float specifying the degrees to rotate about the **X** axis. The default value is 0.0.
+        yAngle
+            A Float specifying the degrees to rotate about the **Y** axis. The default value is 0.0.
+        zAngle
+            A Float specifying the degrees to rotate about the*Z*-axis. The default value is 0.0.
+        mode
+            A SymbolicConstant specifying the rotation mode. Possible values are:
+
+            * TOTAL : Set the view to (0, 0, 1), then rotate about the screen's axes (an absolute rotation).
+            * SCREEN : Rotate incrementally about the screen's axes (a relative rotation).
+            * MODEL : Rotate incrementally about the model's axes (a relative rotation).
+
+            The default value is MODEL.
+        asMovie
+            A Boolean specifying the alternate mode of the rotate view manipulation should be used.
+            The default value is OFF.
+        drawImmediately
+            A Boolean specifying the viewport should refresh immediately after the command is
+            processed. This argument is typically used only when writing a script and it is
+            desirable to show intermediate results before the script completes. The default value is
+            False.
+        """
+        ...
+
+    @abaqus_method_doc
+    def setLayerTransform(
+        self,
+        layerTransform: tuple = (),
+        options: Optional["View"] = None,
+        drawImmediately: Boolean = False,
+    ):
+        """This method modifies the transformation used to position a Layer. Note:This method is not available
+        for Session and Viewport Views.
+
+        Parameters
+        ----------
+        layerTransform
+            A sequence of 16 Floats specifying the transformation matrix.
+        options
+            A View object from which the view settings are to be copied. If the **layerTransform**
+            argument is also supplied to setLayerTransform, it will override the values in the View
+            object specified by **view**.
+        drawImmediately
+            A Boolean specifying the viewport should refresh immediately after the command is
+            processed. This argument is typically used only when writing a script and it is
+            desirable to show intermediate results before the script completes. The default value is
+            False.
+        """
+        ...
+
+    @abaqus_method_doc
+    def setProjection(self, projection: Literal[C.PARALLEL, C.PERSPECTIVE], drawImmediately: Boolean = False):
+        """This method modifies the appearance of three-dimensional models in the viewport. Choosing PERSPECTIVE
+        makes a model appear more realistic by decreasing the apparent size of features that are farther away
+        from the viewing point. Note:This method is not available for a Layer View.
+
+        Parameters
+        ----------
+        projection
+            A SymbolicConstant specifying the projection mode. Possible values are PERSPECTIVE and
+            PARALLEL.
+        drawImmediately
+            A Boolean specifying the viewport should refresh immediately after the command is
+            processed. This argument is typically used only when writing a script and it is
+            desirable to show intermediate results before the script completes. The default value is
+            False.
+
+        Raises
+        ------
+        RangeError
+        """
+        ...
+
+    @abaqus_method_doc
+    def setRotationCenter(self, rotationCenter: tuple):
+        """This method sets the center of rotation to the specified location.
+
+        Parameters
+        ----------
+        rotationCenter
+            A sequence of a String and an Int specifying a part instance name and a node label or a
+            sequence of 3 Floats specifying a point.
+
+        Raises
+        ------
+        TypeError
+            rotationCenter cannot be set using a part instance and node label unless the
+            displayed object is an ODB.
+        """
+        ...
 
     @abaqus_method_doc
     def setValues(
         self,
-        description: str = "",
-        timePeriod: float = 1,
-        nlgeom: Boolean = OFF,
-        stabilizationMethod: Literal[C.DAMPING_FACTOR, C.DISSIPATED_ENERGY_FRACTION, C.NONE] = NONE,
-        stabilizationMagnitude: Optional[float] = None,
-        timeIncrementationMethod: Literal[C.AUTOMATIC, C.FIXED] = AUTOMATIC,
-        matrixSolver: Literal[C.DIRECT, C.ITERATIVE] = DIRECT,
-        matrixStorage: Literal[C.SYMMETRIC, C.SOLVER_DEFAULT, C.UNSYMMETRIC] = SOLVER_DEFAULT,
-        initialInc: Optional[float] = None,
-        maxNumInc: int = 100,
-        minInc: Optional[float] = None,
-        maxInc: float = 1,
-        integration: Literal[C.EXPLICIT_ONLY, C.IMPLICIT_EXPLICIT] = IMPLICIT_EXPLICIT,
-        cetol: float = 0,
-        amplitude: Literal[C.STEP, C.RAMP] = STEP,
-        extrapolation: Literal[C.PARABOLIC, C.NONE, C.LINEAR] = LINEAR,
-        solutionTechnique: Literal[C.QUASI_NEWTON, C.FULL_NEWTON] = FULL_NEWTON,
-        reformKernel: int = 8,
-        convertSDI: Literal[C.CONVERT_SDI_OFF, C.PROPAGATED, C.CONVERT_SDI_ON] = PROPAGATED,
-        adaptiveDampingRatio: float = 0,
-        continueDampingFactors: Boolean = OFF,
+        options: View = ...,
+        drawImmediately: Boolean = False,
+        fieldOfViewAngle: float = ...,
+        farPlaneMode: Literal[C.AUTOCOMPUTE, C.SPECIFY] = ...,
+        nearPlane: float = ...,
+        farPlane: float = ...,
+        width: float = ...,
+        height: float = ...,
+        projection: Literal[C.PERSPECTIVE, C.PARALLEL] = ...,
+        cameraPosition: Tuple[float, float, float] = ...,
+        cameraUpVector: Tuple[float, float, float] = ...,
+        cameraTarget: Tuple[float, float, float] = ...,
+        viewOffsetX: float = ...,
+        viewOffsetY: float = ...,
+        movieMode: Boolean = OFF,
+    ) -> None:
+        """This method modifies the View object.
+
+        .. note::
+            This method is not available for a Layer View.
+
+        The optional arguments to ``setValues`` are the same as the arguments to the
+        View method, except for the ``name``
+        and ``autoFit`` arguments. In addition, ``setValues`` has the following optional
+        arguments:
+
+        Parameters
+        ----------
+        options
+            A View object from which the view settings are to be copied. If other
+            arguments are also supplied to ``setValues``, they will override the values
+            in the View object specified by ``view``.
+
+        drawImmediately
+            A Boolean specifying the viewport should refresh immediately after the
+            command is processed. This argument is typically used only when writing a
+            script and it is desirable to show intermediate results before the script
+            completes. The default value is False.
+
+        fieldOfViewAngle
+            A Float specifying the viewing angle of the camera. Possible values are
+            0.0 < filedOfViewAngle < 180.0.
+
+        farPlaneMode
+            A SymbolicConstant specifying how the distance from the camera to the far
+            clipping plane is set. Possible values are AUTOCOMPUTE and SPECIFY.
+
+        Returns
+        -------
+        None.
+
+        Raises
+        ------
+        RangeError
+        """
+        ...
+
+    @abaqus_method_doc
+    def setViewpoint(
+        self,
+        viewVector: tuple,
+        cameraUpVector: tuple = (),
+        drawImmediately: Boolean = False,
     ):
-        """This method modifies the ViscoStep object.
+        """This method sets the camera's position in the viewport. Note:This method is not available for a Layer
+        View.
 
         Parameters
         ----------
-        description
-            A String specifying a description of the new step. The default value is an empty string.
-        timePeriod
-            A Float specifying the total time period. The default value is 1.0.
-        nlgeom
-            A Boolean specifying whether to allow for geometric nonlinearity. The default value is
-            OFF.
-        stabilizationMethod
-            A SymbolicConstant specifying the stabilization type. Possible values are NONE,
-            DISSIPATED_ENERGY_FRACTION, and DAMPING_FACTOR. The default value is NONE.
-        stabilizationMagnitude
-            A Float specifying the damping intensity of the automatic damping algorithm if the
-            problem is expected to be unstable, and **stabilizationMethod** is not NONE. The default
-            value is 2x10⁻⁴.
-        timeIncrementationMethod
-            A SymbolicConstant specifying the time incrementation method to be used. Possible values
-            are FIXED and AUTOMATIC. The default value is AUTOMATIC.
-        matrixSolver
-            A SymbolicConstant specifying the type of solver. Possible values are DIRECT and
-            ITERATIVE. The default value is DIRECT.
-        matrixStorage
-            A SymbolicConstant specifying the type of matrix storage. Possible values are SYMMETRIC,
-            UNSYMMETRIC, and SOLVER_DEFAULT. The default value is SOLVER_DEFAULT.
-        initialInc
-            A Float specifying the initial time increment. The default value is the total time
-            period for the step.
-        maxNumInc
-            An Int specifying the maximum number of increments in a step. The default value is 100.
-        minInc
-            A Float specifying the minimum time increment allowed. The default value is the smaller
-            of the suggested initial time increment or 10−5 times the total time period.
-        maxInc
-            A Float specifying the maximum time increment allowed. The default is the total time
-            period for the step. The default value is 1.0.
-        integration
-            A SymbolicConstant specifying which type of integration to use throughout the step.
-            Possible values are IMPLICIT_EXPLICIT and EXPLICIT_ONLY. The default value is
-            IMPLICIT_EXPLICIT.
-        cetol
-            A Float specifying the maximum difference in the creep strain increment calculated from
-            the creep strain rates at the beginning and end of the increment. The default value is
-            0.0.
-        amplitude
-            A SymbolicConstant specifying the amplitude variation for loading magnitudes during the
-            step. Possible values are STEP and RAMP. The default value is STEP.
-        extrapolation
-            A SymbolicConstant specifying the type of extrapolation to use in determining the
-            incremental solution for a nonlinear analysis. Possible values are NONE, LINEAR, and
-            PARABOLIC. The default value is LINEAR.
-        solutionTechnique
-            A SymbolicConstant specifying the technique used to for solving nonlinear equations.
-            Possible values are FULL_NEWTON and QUASI_NEWTON. The default value is FULL_NEWTON.
-        reformKernel
-            An Int specifying the number of quasi-Newton iterations allowed before the kernel matrix
-            is reformed.. The default value is 8.
-        convertSDI
-            A SymbolicConstant specifying whether to force a new iteration if severe discontinuities
-            occur during an iteration. Possible values are PROPAGATED, CONVERT_SDI_OFF, and
-            CONVERT_SDI_ON. The default value is PROPAGATED.
-        adaptiveDampingRatio
-            A Float specifying the maximum allowable ratio of the stabilization energy to the total
-            strain energy and can be used only if **stabilizationMethod** is not NONE. The default
-            value is 0.05.
-        continueDampingFactors
-            A Boolean specifying whether this step will carry over the damping factors from the
-            results of the preceding general step. This parameter must be used in conjunction with
-            the **adaptiveDampingRatio** parameter. The default value is OFF.
+        viewVector
+            A sequence of three Floats specifying the viewing vector (from the camera to the origin
+            of the model).
+        cameraUpVector
+            A sequence of three Floats specifying the camera's up vector (the screen's positive
+            **Y** axis). The initial value is (0, 0, 0).
+        drawImmediately
+            A Boolean specifying the viewport should refresh immediately after the command is
+            processed. This argument is typically used only when writing a script and it is
+            desirable to show intermediate results before the script completes. The default value is
+            False.
+        """
+        ...
+
+    @abaqus_method_doc
+    def zoom(
+        self,
+        zoomFactor: float,
+        mode: Literal[C.ABSOLUTE, C.RELATIVE] = ABSOLUTE,
+        asMovie: Boolean = OFF,
+        drawImmediately: Boolean = False,
+    ):
+        """This method magnifies the view in the viewport.
+
+        Parameters
+        ----------
+        zoomFactor
+            A Float specifying the amount to zoom. Possible values are 0.000001 ≤ **zoomFactor** ≤
+            1000000. A **zoomFactor** less than one reduces the image. A **zoomFactor** greater than one
+            enlarges the image.
+        mode
+            A SymbolicConstant specifying the way the zoom is executed. Possible values are:
+
+            * ABSOLUTE : Execute fitView, then zoom.
+            * RELATIVE : Zoom from the current camera settings.
+
+            The default value is ABSOLUTE.
+        asMovie
+            A Boolean specifying the alternate mode of the zoom view manipulation should be used.
+            The default value is OFF. This argument is ignored for a Layer View.
+        drawImmediately
+            A Boolean specifying the viewport should refresh immediately after the command is
+            processed. This argument is typically used only when writing a script and it is
+            desirable to show intermediate results before the script completes. The default value is
+            False.
 
         Raises
         ------
         RangeError
         """
         ...
+
+    @abaqus_method_doc
+    def zoomRectangle(
+        self,
+        point1: Sequence[float],
+        point2: Sequence[float],
+        drawImmediately: Boolean = False,
+    ):
+        """This method fills the viewport with the graphics located within the given rectangle.
+
+        Parameters
+        ----------
+        point1
+            A pair of Floats specifying the*X*- and **Y** coordinates of one corner of the rectangle
+            in fractions of the viewport width and height.
+        point2
+            A pair of Floats specifying the*X*- and **Y** coordinates of the other corner of the
+            rectangle in fractions of the viewport width and height.
+        drawImmediately
+            A Boolean specifying the viewport should refresh immediately after the command is
+            processed. This argument is typically used only when writing a script and it is
+            desirable to show intermediate results before the script completes. The default value is
+            False.
+        """
+        ...
```

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/CompositeDampingComponent.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/CompositeDampingComponent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/Control.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/Control.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/DirectDampingByFrequency.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/DirectDampingByFrequency.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/DirectDampingByFrequencyComponent.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/DirectDampingByFrequencyComponent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/DirectDampingComponent.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/DirectDampingComponent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/EmagTimeHarmonicFrequency.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/EmagTimeHarmonicFrequency.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/MassScaling.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/MassScaling.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RandomResponseFrequency.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RandomResponseFrequency.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RayleighDampingByFrequency.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RayleighDampingByFrequency.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RayleighDampingByFrequencyComponent.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RayleighDampingByFrequencyComponent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/RayleighDampingComponent.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/RayleighDampingComponent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/ResponseSpectrumComponent.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/ResponseSpectrumComponent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SolverControl.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SolverControl.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SteadyStateDirectFrequency.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SteadyStateDirectFrequency.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SteadyStateModalFrequency.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SteadyStateModalFrequency.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SteadyStateSubspaceFrequency.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SteadyStateSubspaceFrequency.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/StructuralDampingByFrequency.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/StructuralDampingByFrequency.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/StructuralDampingByFrequencyComponent.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/StructuralDampingByFrequencyComponent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/StructuralDampingComponent.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/StructuralDampingComponent.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SubstructureGenerateFrequency.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SubstructureGenerateFrequency.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepMiscellaneous/SubstructureGenerateModes.py` & `abqpy-2023.5.2/src/abaqus/StepMiscellaneous/SubstructureGenerateModes.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepOutput/DiagnosticPrint.py` & `abqpy-2023.5.2/src/abaqus/StepOutput/DiagnosticPrint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepOutput/FieldOutputRequest.py` & `abqpy-2023.5.2/src/abaqus/StepOutput/FieldOutputRequest.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepOutput/FieldOutputRequestState.py` & `abqpy-2023.5.2/src/abaqus/StepOutput/FieldOutputRequestState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepOutput/HistoryOutputRequest.py` & `abqpy-2023.5.2/src/abaqus/StepOutput/HistoryOutputRequest.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepOutput/HistoryOutputRequestState.py` & `abqpy-2023.5.2/src/abaqus/StepOutput/HistoryOutputRequestState.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepOutput/IntegratedOutputSection.py` & `abqpy-2023.5.2/src/abaqus/StepOutput/IntegratedOutputSection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepOutput/Monitor.py` & `abqpy-2023.5.2/src/abaqus/StepOutput/Monitor.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepOutput/OutputModel.py` & `abqpy-2023.5.2/src/abaqus/StepOutput/OutputModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepOutput/OutputStep.py` & `abqpy-2023.5.2/src/abaqus/StepOutput/OutputStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepOutput/Restart.py` & `abqpy-2023.5.2/src/abaqus/StepOutput/Restart.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/StepOutput/TimePoint.py` & `abqpy-2023.5.2/src/abaqus/StepOutput/TimePoint.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/ActivateElements.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/ActivateElements.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/DataTable.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/DataTable.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/ElementProgressiveActivation.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/ElementProgressiveActivation.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/EventSeries.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/EventSeries.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/EventSeriesType.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/EventSeriesType.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/ParameterColumn.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/ParameterColumn.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/ParameterTable.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/ParameterTable.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/PropertyTable.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/PropertyTable.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/PropertyTableData.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/PropertyTableData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/TableCollection.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/TableCollection.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/TableCollectionAssembly.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/TableCollectionAssembly.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/TableCollectionModel.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/TableCollectionModel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TableCollection/TableCollectionStep.py` & `abqpy-2023.5.2/src/abaqus/TableCollection/TableCollectionStep.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TextRepresentation/TextReprOptions.py` & `abqpy-2023.5.2/src/abaqus/TextRepresentation/TextReprOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TextRepresentation/redentABQ.py` & `abqpy-2023.5.2/src/abaqus/TextRepresentation/redentABQ.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/TextRepresentation/textRepr.py` & `abqpy-2023.5.2/src/abaqus/TextRepresentation/textRepr.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/AbaqusBoolean.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/AbaqusBoolean.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/BackwardCompatibility.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/BackwardCompatibility.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/Callback.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/Callback.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/Customization.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/Customization.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/Delete.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/Delete.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/Method.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/Method.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/Repository.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/Repository.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/Status.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/Status.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/SymbolicConstant.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/SymbolicConstant.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/Upgrade.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/Upgrade.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/User.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/User.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/UtilityAndView/abaqusConstants.py` & `abqpy-2023.5.2/src/abaqus/UtilityAndView/abaqusConstants.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/Area.py` & `abqpy-2023.5.2/src/abaqus/XY/Area.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/AreaStyle.py` & `abqpy-2023.5.2/src/abaqus/XY/AreaStyle.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/Axis.py` & `abqpy-2023.5.2/src/abaqus/XY/Axis.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/AxisData.py` & `abqpy-2023.5.2/src/abaqus/XY/AxisData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/Chart.py` & `abqpy-2023.5.2/src/abaqus/XY/Chart.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/DefaultChartOptions.py` & `abqpy-2023.5.2/src/abaqus/XY/DefaultChartOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/DefaultPlot.py` & `abqpy-2023.5.2/src/abaqus/XY/DefaultPlot.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/Legend.py` & `abqpy-2023.5.2/src/abaqus/XY/Legend.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/LineStyle.py` & `abqpy-2023.5.2/src/abaqus/XY/LineStyle.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/QuantityType.py` & `abqpy-2023.5.2/src/abaqus/XY/QuantityType.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/SymbolStyle.py` & `abqpy-2023.5.2/src/abaqus/XY/SymbolStyle.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/TextStyle.py` & `abqpy-2023.5.2/src/abaqus/XY/TextStyle.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/Title.py` & `abqpy-2023.5.2/src/abaqus/XY/Title.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/XYCurve.py` & `abqpy-2023.5.2/src/abaqus/XY/XYCurve.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/XYData.py` & `abqpy-2023.5.2/src/abaqus/XY/XYData.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/XYPlot.py` & `abqpy-2023.5.2/src/abaqus/XY/XYPlot.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/XYPlotBase.py` & `abqpy-2023.5.2/src/abaqus/XY/XYPlotBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/XYReportOptions.py` & `abqpy-2023.5.2/src/abaqus/XY/XYReportOptions.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/XYSession.py` & `abqpy-2023.5.2/src/abaqus/XY/XYSession.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/XYSessionBase.py` & `abqpy-2023.5.2/src/abaqus/XY/XYSessionBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/XY/writeXYReport.py` & `abqpy-2023.5.2/src/abaqus/XY/writeXYReport.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/_OptionsBase.py` & `abqpy-2023.5.2/src/abaqus/_OptionsBase.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/__init__.py` & `abqpy-2023.5.2/src/abaqus/__init__.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abaqus/builtin.py` & `abqpy-2023.5.2/src/abaqus/builtin.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abqpy/__init__.py` & `abqpy-2023.5.2/src/abqpy/__init__.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abqpy/cli.py` & `abqpy-2023.5.2/src/abqpy/cli.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abqpy/decorators.py` & `abqpy-2023.5.2/src/abqpy/decorators.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abqpy/run.py` & `abqpy-2023.5.2/src/abqpy/run.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/abqpy.egg-info/PKG-INFO` & `abqpy-2023.5.2/src/abqpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: abqpy
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Type hints for Abaqus/Python scripting
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: Homepage, https://abqpy.com
 Project-URL: GitHub, https://github.com/haiiliin/abqpy
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Bug Tracker, https://github.com/haiiliin/abqpy/issues
 Project-URL: Read the Docs, https://readthedocs.org/projects/abqpy
 Project-URL: Documentation, https://docs.abqpy.com/en/stable/
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: jupyter
 Provides-Extra: dev
-Provides-Extra: juptyer
 Provides-Extra: docs
 License-File: LICENSE
 
 # abqpy 2023
 
 [![tests](https://github.com/haiiliin/abqpy/actions/workflows/tests.yml/badge.svg)](https://github.com/haiiliin/abqpy/actions/workflows/tests.yml)
 [![rtd](https://readthedocs.org/projects/abqpy/badge/?version=latest)](https://readthedocs.org/projects/abqpy/)
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: abqpy Version: 2023.5.1 Summary: Type hints for
+Metadata-Version: 2.1 Name: abqpy Version: 2023.5.2 Summary: Type hints for
 Abaqus/Python scripting Author-email: WANG Hailin
 wang@connect.polyu.hk> Project-URL: Homepage, https://abqpy.com Project-URL:
 GitHub, https://github.com/haiiliin/abqpy Project-URL: Bug Tracker, https://
-github.com/pypa/sampleproject/issues Project-URL: Read the Docs, https://
+github.com/haiiliin/abqpy/issues Project-URL: Read the Docs, https://
 readthedocs.org/projects/abqpy Project-URL: Documentation, https://
 docs.abqpy.com/en/stable/ Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev Provides-Extra: juptyer Provides-Extra: docs
+markdown Provides-Extra: jupyter Provides-Extra: dev Provides-Extra: docs
 License-File: LICENSE # abqpy 2023 [![tests](https://github.com/haiiliin/abqpy/
 actions/workflows/tests.yml/badge.svg)](https://github.com/haiiliin/abqpy/
 actions/workflows/tests.yml) [![rtd](https://readthedocs.org/projects/abqpy/
 badge/?version=latest)](https://readthedocs.org/projects/abqpy/) [![codecov]
 (https://codecov.io/gh/haiiliin/abqpy/branch/2023/graph/badge.svg)](https://
 app.codecov.io/gh/haiiliin/abqpy/tree/2023) [![python](https://img.shields.io/
 badge/Python-3.7%2B-brightgreen)](https://www.python.org/downloads/) [![abaqus]
```

### Comparing `abqpy-2023.5.1/src/abqpy.egg-info/SOURCES.txt` & `abqpy-2023.5.2/src/abqpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 .github/workflows/release.yml
 .github/workflows/rtd.yml
 .github/workflows/tests.yml
 .github/workflows/translations.yml
 docs/Makefile
 docs/README.md
 docs/make.bat
-docs/requirements.txt
 docs/update-locale.sh
 docs/source/CHANGES.md
 docs/source/cli.md
 docs/source/conf.py
 docs/source/envvars.md
 docs/source/getting_started.md
 docs/source/index.md
@@ -234,18 +233,14 @@
 examples/Abaqus/viewerPrintContours.py
 examples/Compression/README.rst
 examples/Compression/compression-output.py
 examples/Compression/compression.py
 examples/Parameter-Identification/README.rst
 examples/Parameter-Identification/compression.py
 examples/Parameter-Identification/optimize.py
-requirements/deps.txt
-requirements/dev.txt
-requirements/docs.txt
-requirements/jupyter.txt
 scripts/conflicts.py
 scripts/rtd.py
 scripts/rtd.sh
 src/ababltin.py
 src/abaqusConstants.py
 src/animation.py
 src/annotationToolset.py
```

### Comparing `abqpy-2023.5.1/src/connectorBehavior.py` & `abqpy-2023.5.2/src/connectorBehavior.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/customKernel.py` & `abqpy-2023.5.2/src/customKernel.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/displayGroupMdbToolset.py` & `abqpy-2023.5.2/src/displayGroupMdbToolset.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/displayGroupOdbToolset.py` & `abqpy-2023.5.2/src/displayGroupOdbToolset.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/job.py` & `abqpy-2023.5.2/src/job.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/load.py` & `abqpy-2023.5.2/src/load.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/odbConnectorBehavior.py` & `abqpy-2023.5.2/src/odbConnectorBehavior.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/optimization.py` & `abqpy-2023.5.2/src/optimization.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/symbolicConstants.py` & `abqpy-2023.5.2/src/symbolicConstants.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/src/xyPlot.py` & `abqpy-2023.5.2/src/xyPlot.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/tests/conftest.py` & `abqpy-2023.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/tests/test_mdb.py` & `abqpy-2023.5.2/tests/test_mdb.py`

 * *Files identical despite different names*

### Comparing `abqpy-2023.5.1/tests/test_odb.py` & `abqpy-2023.5.2/tests/test_odb.py`

 * *Files identical despite different names*

