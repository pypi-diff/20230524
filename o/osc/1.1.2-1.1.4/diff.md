# Comparing `tmp/osc-1.1.2.tar.gz` & `tmp/osc-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc-1.1.2.tar", last modified: Wed May  3 08:14:07 2023, max compression
+gzip compressed data, was "osc-1.1.4.tar", last modified: Wed May 24 07:04:25 2023, max compression
```

## Comparing `osc-1.1.2.tar` & `osc-1.1.4.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.947695 osc-1.1.2/
--rw-r--r--   0 dmach     (1000) dmach     (1000)      480 2023-05-03 08:03:10.000000 osc-1.1.2/AUTHORS
--rw-r--r--   0 dmach     (1000) dmach     (1000)    18092 2023-05-03 08:03:10.000000 osc-1.1.2/COPYING
--rw-r--r--   0 dmach     (1000) dmach     (1000)       63 2023-05-03 08:03:10.000000 osc-1.1.2/MANIFEST.in
--rw-r--r--   0 dmach     (1000) dmach     (1000)     6939 2023-05-03 08:10:41.000000 osc-1.1.2/NEWS
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1420 2023-05-03 08:14:07.947695 osc-1.1.2/PKG-INFO
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5632 2023-05-03 08:03:10.000000 osc-1.1.2/README.md
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.943695 osc-1.1.2/osc/
--rw-r--r--   0 dmach     (1000) dmach     (1000)    13406 2023-05-03 08:03:10.000000 osc-1.1.2/osc/OscConfigParser.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      259 2023-05-03 08:03:30.000000 osc-1.1.2/osc/__init__.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.943695 osc-1.1.2/osc/_private/
--rw-r--r--   0 dmach     (1000) dmach     (1000)      692 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/__init__.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5770 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/api.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2338 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/api_build.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      381 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/api_configuration.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3347 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/api_source.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1525 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/common.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3623 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1207 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/request.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8318 2023-05-03 08:03:10.000000 osc-1.1.2/osc/babysitter.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    63226 2023-05-03 08:03:10.000000 osc-1.1.2/osc/build.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3211 2023-05-03 08:03:10.000000 osc-1.1.2/osc/checker.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    10121 2023-05-03 08:03:10.000000 osc-1.1.2/osc/cmdln.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)   440150 2023-05-03 08:03:10.000000 osc-1.1.2/osc/commandline.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.943695 osc-1.1.2/osc/commands/
--rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:03:10.000000 osc-1.1.2/osc/commands/__init__.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    40770 2023-05-03 08:03:10.000000 osc-1.1.2/osc/conf.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    25246 2023-05-03 08:03:10.000000 osc-1.1.2/osc/connection.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)   331036 2023-05-03 08:03:10.000000 osc-1.1.2/osc/core.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    11240 2023-05-03 08:03:10.000000 osc-1.1.2/osc/credentials.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    17821 2023-05-03 08:03:10.000000 osc-1.1.2/osc/fetch.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1411 2023-05-03 08:03:10.000000 osc-1.1.2/osc/grabber.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2076 2023-05-03 08:03:10.000000 osc-1.1.2/osc/meter.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5923 2023-05-03 08:03:10.000000 osc-1.1.2/osc/oscerr.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     6840 2023-05-03 08:03:10.000000 osc-1.1.2/osc/oscssl.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:03:10.000000 osc-1.1.2/osc/py.typed
--rw-r--r--   0 dmach     (1000) dmach     (1000)     9989 2023-05-03 08:03:10.000000 osc-1.1.2/osc/store.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.943695 osc-1.1.2/osc/util/
--rw-r--r--   0 dmach     (1000) dmach     (1000)       79 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/__init__.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     7084 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/ar.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     7225 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/archquery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8208 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/cpio.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     9258 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/debquery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2728 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/git_version.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1886 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/helper.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5499 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/packagequery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     6788 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/repodata.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    13167 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/rpmquery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      809 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/safewriter.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.943695 osc-1.1.2/osc.egg-info/
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1420 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/PKG-INFO
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1593 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/SOURCES.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)        1 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/dependency_links.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)       44 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/entry_points.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)       52 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/requires.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)        4 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/top_level.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1574 2023-05-03 08:14:07.947695 osc-1.1.2/setup.cfg
--rwxr-xr-x   0 dmach     (1000) dmach     (1000)       95 2023-05-03 08:03:10.000000 osc-1.1.2/setup.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.947695 osc-1.1.2/tests/
--rw-r--r--   0 dmach     (1000) dmach     (1000)      788 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test__private_api.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     4912 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test__private_package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3168 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_addfiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    29754 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_commandline.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    21957 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_commit.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1451 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_conf.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      578 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_config_parser.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1783 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_core.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8446 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_core_package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      877 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_core_request.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8656 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_deletefiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    11258 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_difffiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2320 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_doc_plugins.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      926 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_helpers.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     4605 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_init_package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3431 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_init_project.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3094 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_package_status.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8779 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_prdiff.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5829 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_project_status.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    10407 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_repairwc.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    24512 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_request.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2307 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_results.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3277 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_revertfiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     4891 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_setlinkrev.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8298 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_store.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    15545 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_update.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.964644 osc-1.1.4/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      480 2023-05-24 07:04:23.000000 osc-1.1.4/AUTHORS
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    18092 2023-05-24 07:04:23.000000 osc-1.1.4/COPYING
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       63 2023-05-24 07:04:23.000000 osc-1.1.4/MANIFEST.in
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     7756 2023-05-24 07:04:23.000000 osc-1.1.4/NEWS
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1420 2023-05-24 07:04:25.964644 osc-1.1.4/PKG-INFO
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5632 2023-05-24 07:04:23.000000 osc-1.1.4/README.md
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.960644 osc-1.1.4/osc/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    13406 2023-05-24 07:04:23.000000 osc-1.1.4/osc/OscConfigParser.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      259 2023-05-24 07:04:23.000000 osc-1.1.4/osc/__init__.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.960644 osc-1.1.4/osc/_private/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      692 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5770 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/api.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2338 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/api_build.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      381 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/api_configuration.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3347 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/api_source.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1525 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/common.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3623 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1207 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8977 2023-05-24 07:04:23.000000 osc-1.1.4/osc/babysitter.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    63492 2023-05-24 07:04:23.000000 osc-1.1.4/osc/build.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3211 2023-05-24 07:04:23.000000 osc-1.1.4/osc/checker.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    10121 2023-05-24 07:04:23.000000 osc-1.1.4/osc/cmdln.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)   440457 2023-05-24 07:04:23.000000 osc-1.1.4/osc/commandline.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.960644 osc-1.1.4/osc/commands/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:23.000000 osc-1.1.4/osc/commands/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    40770 2023-05-24 07:04:23.000000 osc-1.1.4/osc/conf.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    25246 2023-05-24 07:04:23.000000 osc-1.1.4/osc/connection.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)   332241 2023-05-24 07:04:23.000000 osc-1.1.4/osc/core.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    11240 2023-05-24 07:04:23.000000 osc-1.1.4/osc/credentials.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    17821 2023-05-24 07:04:23.000000 osc-1.1.4/osc/fetch.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1611 2023-05-24 07:04:23.000000 osc-1.1.4/osc/grabber.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2076 2023-05-24 07:04:23.000000 osc-1.1.4/osc/meter.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5923 2023-05-24 07:04:23.000000 osc-1.1.4/osc/oscerr.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     6840 2023-05-24 07:04:23.000000 osc-1.1.4/osc/oscssl.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:23.000000 osc-1.1.4/osc/py.typed
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     9989 2023-05-24 07:04:23.000000 osc-1.1.4/osc/store.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.960644 osc-1.1.4/osc/util/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       79 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     7084 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/ar.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     7225 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/archquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8208 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/cpio.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     9258 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/debquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2728 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/git_version.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1886 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/helper.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5499 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/packagequery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     6788 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/repodata.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    13167 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/rpmquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      809 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/safewriter.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.960644 osc-1.1.4/osc.egg-info/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1420 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/PKG-INFO
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1635 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/SOURCES.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        1 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/dependency_links.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       44 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/entry_points.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       52 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/requires.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        4 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/top_level.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1574 2023-05-24 07:04:25.964644 osc-1.1.4/setup.cfg
+-rwxr-xr-x   0 dmach     (1000) dmach     (1000)       95 2023-05-24 07:04:23.000000 osc-1.1.4/setup.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.964644 osc-1.1.4/tests/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      788 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test__private_api.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4912 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test__private_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3168 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_addfiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1416 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_build.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    29754 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_commandline.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    21957 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_commit.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1451 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_conf.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      578 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_config_parser.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1783 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_core.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8446 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_core_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      877 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_core_request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8656 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_deletefiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    11258 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_difffiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2320 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_doc_plugins.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      856 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_grabber.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      926 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_helpers.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4605 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_init_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3431 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_init_project.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3094 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_package_status.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8779 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_prdiff.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5829 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_project_status.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    10407 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_repairwc.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    24512 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2307 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_results.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3277 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_revertfiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4891 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_setlinkrev.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8298 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_store.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    15545 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_update.py
```

### Comparing `osc-1.1.2/COPYING` & `osc-1.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/NEWS` & `osc-1.1.4/NEWS`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+- 1.1.4
+  - Command-line:
+    - Change 'review list' command to display open requests (state: new, review, declined)
+    - Fix running osc in an AppImage by switching to the correct working directory
+    - Handle ProtocolError exception
+  - Library:
+    - Add 'req_states' parameter to osc.core.get_review_list()
+  - Connection:
+    - Fix grabber to work with old urllib3 versions that do not contain URLSchemeUnknown exception
+
+- 1.1.3
+  - Command-line:
+    - Backup edited messages and notify user about them when osc errors out
+    - Consider only open requests when listing requests with a given review state
+    - Fix 'diff' command when no files are specified
+  - Configuration:
+    - Add glob support to the 'trusted_prj' config option
+  - Library:
+    - Fix core.xmlindent() to work with ElementTree objects
+
 - 1.1.2
   - Command-line:
     - Add '--buildtool-opt' option passing options to underlying rpmbuild to the 'build' command
     - Fix 'diff' command to support diffing selected files only
     - Identify inherited packages in the 'dependson' command output
     - Bring the '--debug' option back to the 'buildinfo' command
     - Fix 'buildhistory' command by setting the type of the '--limit' option to int
```

### Comparing `osc-1.1.2/PKG-INFO` & `osc-1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc
-Version: 1.1.2
+Version: 1.1.4
 Summary: openSUSE commander
 Home-page: http://en.opensuse.org/openSUSE:OSC
 Download-URL: https://github.com/openSUSE/osc
 Author: openSUSE project
 Author-email: opensuse-buildservice@opensuse.org
 License: GPLv2+
 Keywords: openSUSE,SUSE,RPM,build,buildservice,command-line
```

### Comparing `osc-1.1.2/README.md` & `osc-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/OscConfigParser.py` & `osc-1.1.4/osc/OscConfigParser.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/_private/__init__.py` & `osc-1.1.4/osc/_private/__init__.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/_private/api.py` & `osc-1.1.4/osc/_private/api.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/_private/api_build.py` & `osc-1.1.4/osc/_private/api_build.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/_private/api_source.py` & `osc-1.1.4/osc/_private/api_source.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/_private/common.py` & `osc-1.1.4/osc/_private/common.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/_private/package.py` & `osc-1.1.4/osc/_private/package.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/_private/request.py` & `osc-1.1.4/osc/_private/request.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/babysitter.py` & `osc-1.1.4/osc/babysitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from urllib.error import URLError, HTTPError
 
 import urllib3.exceptions
 
 from . import _private
 from . import commandline
 from . import conf as osc_conf
+from . import core as osc_core
 from . import oscerr
 from .OscConfigParser import configparser
 from .oscssl import CertVerificationError
 from .util.cpio import CpioError
 from .util.helper import decode_it
 from .util.packagequery import PackageError
 
@@ -188,18 +189,25 @@
         print(e, file=sys.stderr)
     except KeyringLocked as e:
         print(e, file=sys.stderr)
     except CertVerificationError as e:
         print(e, file=sys.stderr)
     except urllib3.exceptions.MaxRetryError as e:
         print(e.reason, file=sys.stderr)
+    except urllib3.exceptions.ProtocolError as e:
+        print(e.args[0], file=sys.stderr)
     except CpioError as e:
         print(e, file=sys.stderr)
     except oscerr.OscBaseError as e:
         print('*** Error:', e, file=sys.stderr)
+    if osc_core.MESSAGE_BACKUPS:
+        print()
+        print("If you lost any edited commit messages due to an error, you may find them here:")
+        for path in osc_core.MESSAGE_BACKUPS:
+            print(f"  - {path}")
     return 1
 
 
 def main():
     # avoid buffering output on pipes (bnc#930137) Basically,
     # a "print('foo')" call is translated to a corresponding
     # fwrite call that writes to the stdout stream (cf.
@@ -214,10 +222,17 @@
     # support setvbuf - if setvbuf is not supported, the stream
     # remains fully buffered (see PyFile_SetBufSize
     # (Objects/fileobject.c))).
     if not os.isatty(sys.stdout.fileno()):
         sys.stdout = os.fdopen(sys.stdout.fileno(), sys.stdout.mode, 1)
         sys.stderr = os.fdopen(sys.stderr.fileno(), sys.stderr.mode, 1)
 
+    appimage = os.getenv("APPIMAGE", None)
+    owd = os.getenv("OWD", None)
+    if appimage and owd:
+        # OWD stands for Original Working Directory and we need to switch there when running in an AppImage
+        # https://docs.appimage.org/packaging-guide/environment-variables.html
+        os.chdir(owd)
+
     sys.exit(run(commandline.OscMainCommand()))
 
 # vim: sw=4 et
```

### Comparing `osc-1.1.2/osc/build.py` & `osc-1.1.4/osc/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (C) 2006 Novell Inc.  All rights reserved.
 # This program is free software; it may be used, copied, modified
 # and distributed under the terms of the GNU General Public Licence,
 # either version 2, or (at your option) any later version.
 
+import fnmatch
 import glob
 import os
 import re
 import shutil
 import subprocess
 import sys
 
@@ -544,22 +545,32 @@
 trustprompt = """Would you like to ...
 0 - quit (default)
 1 - always trust packages from '%(project)s'
 2 - trust packages just this time
 ? """
 
 
-def check_trusted_projects(apiurl, projects):
+def check_trusted_projects(apiurl, projects, interactive=True):
     trusted = conf.config['api_host_options'][apiurl]['trusted_prj']
     tlen = len(trusted)
     for prj in projects:
-        if prj not in trusted:
+        is_trusted = False
+        for pattern in trusted:
+            if fnmatch.fnmatch(prj, pattern):
+                is_trusted = True
+                break
+        if not is_trusted:
             print("\nThe build root needs packages from project '%s'." % prj)
             print("Note that malicious packages can compromise the build result or even your system.")
-            r = raw_input(trustprompt % {'project': prj})
+
+            if interactive:
+                r = raw_input(trustprompt % {'project': prj})
+            else:
+                r = "0"
+
             if r == '1':
                 print("adding '%s' to oscrc: ['%s']['trusted_prj']" % (prj, apiurl))
                 trusted.append(prj)
             elif r != '2':
                 print("Well, goodbye then :-)")
                 raise oscerr.UserAbort()
```

### Comparing `osc-1.1.2/osc/checker.py` & `osc-1.1.4/osc/checker.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/cmdln.py` & `osc-1.1.4/osc/cmdln.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/commandline.py` & `osc-1.1.4/osc/commandline.py`

 * *Files 1% similar despite different names*

```diff
@@ -3250,15 +3250,15 @@
                 # FIXME -B not implemented!
                 if opts.bugowner:
                     self._debug('list: option --bugowner ignored: not impl.')
 
                 if subcmd == 'review':
                     # FIXME: do the review list for the user and for all groups he belong to
                     results = get_review_list(apiurl, project, package, who, opts.group, opts.project, opts.package, state_list,
-                                              opts.type)
+                                              opts.type, req_states=("new", "review", "declined"))
                 else:
                     if opts.involved_projects:
                         who = who or conf.get_apiurl_usr(apiurl)
                         results = get_user_projpkgs_request_list(apiurl, who, req_state=state_list,
                                                                  req_type=opts.type, exclude_projects=opts.exclude_target_project or [])
                     else:
                         roles = ["creator"] if opts.mine else None
@@ -4642,15 +4642,20 @@
             rev1, rev2 = parseRevisionOption(opts.revision)
         diff = b''
         for pac in pacs:
             if not rev2:
                 for i in pac.get_diff(rev1):
                     diff += b''.join(i)
             else:
-                files = args
+                if args == ["."]:
+                    # parseargs() returns ["."] (list with workdir) if no args are specified
+                    # "." is illegal filename that causes server to return 400
+                    files = None
+                else:
+                    files = args
                 diff += server_diff_noex(pac.apiurl, pac.prjname, pac.name, rev1,
                                          pac.prjname, pac.name, rev2,
                                          not opts.plain, opts.missingok, opts.meta, not opts.unexpand, files=files)
         run_pager(diff)
 
     @cmdln.option('--issues-only', action='store_true',
                   help='show only issues in diff')
```

### Comparing `osc-1.1.2/osc/conf.py` & `osc-1.1.4/osc/conf.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/connection.py` & `osc-1.1.4/osc/connection.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/core.py` & `osc-1.1.4/osc/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,14 +632,16 @@
         return self.error is not None
 
 # http://effbot.org/zone/element-lib.htm#prettyprint
 
 
 def xmlindent(elem, level=0):
     i = "\n" + level * "  "
+    if isinstance(elem, ET.ElementTree):
+        elem = elem.getroot()
     if len(elem):
         if not elem.text or not elem.text.strip():
             elem.text = i + "  "
         for e in elem:
             xmlindent(e, level + 1)
             if not e.tail or not e.tail.strip():
                 e.tail = i + "  "
@@ -4404,14 +4406,19 @@
     try:
         cmd = shlex.split(editor)
     except SyntaxError:
         cmd = editor.split()
     return cmd
 
 
+# list of files with message backups
+# we'll show this list when osc errors out
+MESSAGE_BACKUPS = []
+
+
 def _edit_message_open_editor(filename, data, orig_mtime):
     editor = _editor_command()
     mtime = os.stat(filename).st_mtime
     if isinstance(data, str):
         data = bytes(data, 'utf-8')
     if mtime == orig_mtime:
         # prepare file for editors
@@ -4424,15 +4431,42 @@
         else:
             with open(filename, 'wb') as f:
                 f.write(data)
             orig_mtime = os.stat(filename).st_mtime
             run_editor(filename)
     else:
         run_editor(filename)
-    return os.stat(filename).st_mtime != orig_mtime
+
+    if os.stat(filename).st_mtime != orig_mtime:
+        # file has changed
+
+        cache_dir = os.path.expanduser("~/.cache/osc/edited-messages")
+        try:
+            os.makedirs(cache_dir, mode=0o700)
+        except FileExistsError:
+            pass
+
+        # remove any stored messages older than 1 day
+        now = datetime.datetime.now()
+        epoch = datetime.datetime.timestamp(now - datetime.timedelta(days=1))
+        for fn in os.listdir(cache_dir):
+            path = os.path.join(cache_dir, fn)
+            if not os.path.isfile(path):
+                continue
+            mtime = os.path.getmtime(path)
+            if mtime < epoch:
+                os.unlink(path)
+
+        # store the current message's backup to the cache dir
+        message_backup_path = os.path.join(cache_dir, str(now).replace(" ", "_"))
+        shutil.copyfile(filename, message_backup_path)
+        MESSAGE_BACKUPS.append(message_backup_path)
+        return True
+
+    return False
 
 
 def edit_message(footer='', template='', templatelen=30):
     delim = '--This line, and those below, will be ignored--\n'
     data = ''
     if template != '':
         if templatelen is not None:
@@ -4666,15 +4700,15 @@
         return tmpl % data
     except KeyError as e:
         print('error: cannot interpolate \'%s\' in \'%s\'' % (e.args[0], tmpl_name), file=sys.stderr)
         return ''
 
 
 def get_review_list(
-    apiurl: str, project="", package="", byuser="", bygroup="", byproject="", bypackage="", states=(), req_type=""
+    apiurl: str, project="", package="", byuser="", bygroup="", byproject="", bypackage="", states=(), req_type="", req_states=("review",)
 ):
     # this is so ugly...
     def build_by(xpath, val):
         if 'all' in states:
             return xpath_join(xpath, 'review/%s' % val, op='and')
         elif states:
             s_xp = ''
@@ -4684,17 +4718,22 @@
             return xpath_join(xpath, 'review[%s and (%s)]' % (val, s_xp), op='and')
         else:
             # default case
             return xpath_join(xpath, 'review[%s and @state=\'new\']' % val, op='and')
         return ''
 
     xpath = ''
+
+    # By default we're interested only in reviews of requests that are in state review.
+    for req_state in req_states:
+        xpath = xpath_join(xpath, "state/@name='%s'" % req_state, inner=True)
+
+    xpath = "(%s)" % xpath
+
     if states == ():
-        # default: requests which are still open and have reviews in "new" state
-        xpath = xpath_join('', 'state/@name=\'review\'', op='and')
         xpath = xpath_join(xpath, 'review/@state=\'new\'', op='and')
     if byuser:
         xpath = build_by(xpath, '@by_user=\'%s\'' % byuser)
     if bygroup:
         xpath = build_by(xpath, '@by_group=\'%s\'' % bygroup)
     if bypackage:
         xpath = build_by(xpath, '@by_project=\'%s\' and @by_package=\'%s\'' % (byproject, bypackage))
```

### Comparing `osc-1.1.2/osc/credentials.py` & `osc-1.1.4/osc/credentials.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/fetch.py` & `osc-1.1.4/osc/fetch.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/grabber.py` & `osc-1.1.4/osc/grabber.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 
 import os
 from urllib.request import HTTPError
 from urllib.parse import urlparse
 from urllib.parse import unquote
 from urllib.error import URLError
 
-import urllib3.exceptions
+try:
+    from urllib3.exceptions import URLSchemeUnknown
+except ImportError:
+    class URLSchemeUnknown(Exception):
+        pass
 
 from .core import streamfile
 
 
 class OscFileGrabber:
     def __init__(self, progress_obj=None):
         self.progress_obj = progress_obj
@@ -35,12 +39,13 @@
         self._mirrors = mirrors
 
     def urlgrab(self, url, filename=None, text=None):
         for mirror in self._mirrors:
             try:
                 self._grabber.urlgrab(mirror, filename, text)
                 return True
-            except (HTTPError, URLError, urllib3.exceptions.URLSchemeUnknown) as e:
+            except (HTTPError, URLError, URLSchemeUnknown, KeyError) as e:
+                # urllib3 1.25.10 throws a KeyError: pool_key_constructor = self.key_fn_by_scheme[scheme]
                 # try next mirror
                 pass
 
         return False
```

### Comparing `osc-1.1.2/osc/meter.py` & `osc-1.1.4/osc/meter.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/oscerr.py` & `osc-1.1.4/osc/oscerr.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/oscssl.py` & `osc-1.1.4/osc/oscssl.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/store.py` & `osc-1.1.4/osc/store.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/util/ar.py` & `osc-1.1.4/osc/util/ar.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/util/archquery.py` & `osc-1.1.4/osc/util/archquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/util/cpio.py` & `osc-1.1.4/osc/util/cpio.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/util/debquery.py` & `osc-1.1.4/osc/util/debquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/util/git_version.py` & `osc-1.1.4/osc/util/git_version.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/util/helper.py` & `osc-1.1.4/osc/util/helper.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/util/packagequery.py` & `osc-1.1.4/osc/util/packagequery.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/util/repodata.py` & `osc-1.1.4/osc/util/repodata.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/util/rpmquery.py` & `osc-1.1.4/osc/util/rpmquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc/util/safewriter.py` & `osc-1.1.4/osc/util/safewriter.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/osc.egg-info/PKG-INFO` & `osc-1.1.4/osc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc
-Version: 1.1.2
+Version: 1.1.4
 Summary: openSUSE commander
 Home-page: http://en.opensuse.org/openSUSE:OSC
 Download-URL: https://github.com/openSUSE/osc
 Author: openSUSE project
 Author-email: opensuse-buildservice@opensuse.org
 License: GPLv2+
 Keywords: openSUSE,SUSE,RPM,build,buildservice,command-line
```

### Comparing `osc-1.1.2/osc.egg-info/SOURCES.txt` & `osc-1.1.4/osc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -48,24 +48,26 @@
 osc/util/packagequery.py
 osc/util/repodata.py
 osc/util/rpmquery.py
 osc/util/safewriter.py
 tests/test__private_api.py
 tests/test__private_package.py
 tests/test_addfiles.py
+tests/test_build.py
 tests/test_commandline.py
 tests/test_commit.py
 tests/test_conf.py
 tests/test_config_parser.py
 tests/test_core.py
 tests/test_core_package.py
 tests/test_core_request.py
 tests/test_deletefiles.py
 tests/test_difffiles.py
 tests/test_doc_plugins.py
+tests/test_grabber.py
 tests/test_helpers.py
 tests/test_init_package.py
 tests/test_init_project.py
 tests/test_package_status.py
 tests/test_prdiff.py
 tests/test_project_status.py
 tests/test_repairwc.py
```

### Comparing `osc-1.1.2/setup.cfg` & `osc-1.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test__private_api.py` & `osc-1.1.4/tests/test__private_api.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test__private_package.py` & `osc-1.1.4/tests/test__private_package.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_addfiles.py` & `osc-1.1.4/tests/test_addfiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_commandline.py` & `osc-1.1.4/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_commit.py` & `osc-1.1.4/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_conf.py` & `osc-1.1.4/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_config_parser.py` & `osc-1.1.4/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_core.py` & `osc-1.1.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_core_package.py` & `osc-1.1.4/tests/test_core_package.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_core_request.py` & `osc-1.1.4/tests/test_core_request.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_deletefiles.py` & `osc-1.1.4/tests/test_deletefiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_difffiles.py` & `osc-1.1.4/tests/test_difffiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_doc_plugins.py` & `osc-1.1.4/tests/test_doc_plugins.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_helpers.py` & `osc-1.1.4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_init_package.py` & `osc-1.1.4/tests/test_init_package.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_init_project.py` & `osc-1.1.4/tests/test_init_project.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_package_status.py` & `osc-1.1.4/tests/test_package_status.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_prdiff.py` & `osc-1.1.4/tests/test_prdiff.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_project_status.py` & `osc-1.1.4/tests/test_project_status.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_repairwc.py` & `osc-1.1.4/tests/test_repairwc.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_request.py` & `osc-1.1.4/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_results.py` & `osc-1.1.4/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_revertfiles.py` & `osc-1.1.4/tests/test_revertfiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_setlinkrev.py` & `osc-1.1.4/tests/test_setlinkrev.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_store.py` & `osc-1.1.4/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.2/tests/test_update.py` & `osc-1.1.4/tests/test_update.py`

 * *Files identical despite different names*

