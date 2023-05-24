# Comparing `tmp/zalando-aws-cli-1.2.7.35.tar.gz` & `tmp/zalando-aws-cli-1.2.9.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zalando-aws-cli-1.2.7.35.tar", last modified: Wed Dec 30 11:34:35 2020, max compression
+gzip compressed data, was "zalando-aws-cli-1.2.9.40.tar", last modified: Wed May 24 15:55:15 2023, max compression
```

## Comparing `zalando-aws-cli-1.2.7.35.tar` & `zalando-aws-cli-1.2.9.40.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/
--rw-r--r--   0 root         (0) root         (0)       38 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       91 2020-12-30 11:34:00.000000 zalando-aws-cli-1.2.7.35/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1542 2020-12-30 11:34:00.000000 zalando-aws-cli-1.2.7.35/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)       16 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       51 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      386 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     2848 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli/
--rw-rw-rw-   0 root         (0) root         (0)       76 2020-12-30 11:34:00.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     9996 2020-12-30 11:34:00.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       76 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4153 2020-12-30 11:34:00.000000 zalando-aws-cli-1.2.7.35/zalando_aws_cli/api.py
--rw-rw-rw-   0 root         (0) root         (0)     4525 2020-12-30 11:34:00.000000 zalando-aws-cli-1.2.7.35/setup.py
--rw-r--r--   0 root         (0) root         (0)     2848 2020-12-30 11:34:35.000000 zalando-aws-cli-1.2.7.35/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      101 2020-12-30 11:34:00.000000 zalando-aws-cli-1.2.7.35/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:55:15.686179 zalando-aws-cli-1.2.9.40/
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-24 15:54:47.000000 zalando-aws-cli-1.2.9.40/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-24 15:54:47.000000 zalando-aws-cli-1.2.9.40/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-05-24 15:55:15.686179 zalando-aws-cli-1.2.9.40/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2023-05-24 15:54:47.000000 zalando-aws-cli-1.2.9.40/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-24 15:54:47.000000 zalando-aws-cli-1.2.9.40/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 15:55:15.686179 zalando-aws-cli-1.2.9.40/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4525 2023-05-24 15:54:47.000000 zalando-aws-cli-1.2.9.40/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:55:15.682179 zalando-aws-cli-1.2.9.40/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-24 15:54:47.000000 zalando-aws-cli-1.2.9.40/tests/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:55:15.686179 zalando-aws-cli-1.2.9.40/zalando_aws_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-24 15:55:12.000000 zalando-aws-cli-1.2.9.40/zalando_aws_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-24 15:54:47.000000 zalando-aws-cli-1.2.9.40/zalando_aws_cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4153 2023-05-24 15:54:47.000000 zalando-aws-cli-1.2.9.40/zalando_aws_cli/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     9996 2023-05-24 15:54:47.000000 zalando-aws-cli-1.2.9.40/zalando_aws_cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:55:15.686179 zalando-aws-cli-1.2.9.40/zalando_aws_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-05-24 15:55:15.000000 zalando-aws-cli-1.2.9.40/zalando_aws_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2023-05-24 15:55:15.000000 zalando-aws-cli-1.2.9.40/zalando_aws_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 15:55:15.000000 zalando-aws-cli-1.2.9.40/zalando_aws_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-24 15:55:15.000000 zalando-aws-cli-1.2.9.40/zalando_aws_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-24 15:55:15.000000 zalando-aws-cli-1.2.9.40/zalando_aws_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-24 15:55:15.000000 zalando-aws-cli-1.2.9.40/zalando_aws_cli.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zalando-aws-cli-1.2.7.35/README.rst` & `zalando-aws-cli-1.2.9.40/README.rst`

 * *Files identical despite different names*

### Comparing `zalando-aws-cli-1.2.7.35/zalando_aws_cli/cli.py` & `zalando-aws-cli-1.2.9.40/zalando_aws_cli/cli.py`

 * *Files identical despite different names*

### Comparing `zalando-aws-cli-1.2.7.35/zalando_aws_cli/api.py` & `zalando-aws-cli-1.2.9.40/zalando_aws_cli/api.py`

 * *Files identical despite different names*

### Comparing `zalando-aws-cli-1.2.7.35/setup.py` & `zalando-aws-cli-1.2.9.40/setup.py`

 * *Files identical despite different names*

