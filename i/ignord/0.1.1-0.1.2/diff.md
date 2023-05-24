# Comparing `tmp/ignord-0.1.1.tar.gz` & `tmp/ignord-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignord-0.1.1.tar", last modified: Wed May 24 09:23:59 2023, max compression
+gzip compressed data, was "ignord-0.1.2.tar", last modified: Wed May 24 09:32:30 2023, max compression
```

## Comparing `ignord-0.1.1.tar` & `ignord-0.1.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.413304 ignord-0.1.1/
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      731 2023-05-24 09:10:29.000000 ignord-0.1.1/.bumpversion.cfg
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      174 2023-05-24 09:10:29.000000 ignord-0.1.1/.coveragerc
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      353 2023-05-23 12:14:06.000000 ignord-0.1.1/.editorconfig
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.409304 ignord-0.1.1/.github/
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.411304 ignord-0.1.1/.github/workflows/
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2585 2023-05-23 12:14:15.000000 ignord-0.1.1/.github/workflows/github-actions.yml
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      684 2023-05-23 12:14:06.000000 ignord-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      231 2023-05-23 12:14:06.000000 ignord-0.1.1/.readthedocs.yml
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       55 2023-05-23 12:14:06.000000 ignord-0.1.1/AUTHORS.rst
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      147 2023-05-24 09:10:27.000000 ignord-0.1.1/CHANGELOG.rst
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2333 2023-05-23 12:14:06.000000 ignord-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)    43648 2023-05-23 12:40:10.000000 ignord-0.1.1/LICENSE
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      427 2023-05-23 12:14:06.000000 ignord-0.1.1/MANIFEST.in
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2389 2023-05-24 09:23:59.413304 ignord-0.1.1/PKG-INFO
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2207 2023-05-24 09:12:07.000000 ignord-0.1.1/README.rst
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.411304 ignord-0.1.1/ci/
--rwxr-xr-x   0 grafuls   (1000) grafuls   (1000)     2867 2023-05-23 12:14:06.000000 ignord-0.1.1/ci/bootstrap.py
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       72 2023-05-23 12:14:06.000000 ignord-0.1.1/ci/requirements.txt
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.409304 ignord-0.1.1/ci/templates/
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.409304 ignord-0.1.1/ci/templates/.github/
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.411304 ignord-0.1.1/ci/templates/.github/workflows/
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     1917 2023-05-23 12:14:06.000000 ignord-0.1.1/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.411304 ignord-0.1.1/docs/
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       28 2023-05-23 12:14:06.000000 ignord-0.1.1/docs/authors.rst
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       30 2023-05-23 12:14:06.000000 ignord-0.1.1/docs/changelog.rst
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     1132 2023-05-24 09:07:27.000000 ignord-0.1.1/docs/conf.py
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       33 2023-05-23 12:14:06.000000 ignord-0.1.1/docs/contributing.rst
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      244 2023-05-23 12:14:06.000000 ignord-0.1.1/docs/index.rst
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      142 2023-05-24 09:07:22.000000 ignord-0.1.1/docs/installation.rst
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       27 2023-05-23 12:14:06.000000 ignord-0.1.1/docs/readme.rst
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.412304 ignord-0.1.1/docs/reference/
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       92 2023-05-24 09:07:29.000000 ignord-0.1.1/docs/reference/ignord.rst
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       58 2023-05-24 09:07:28.000000 ignord-0.1.1/docs/reference/index.rst
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       29 2023-05-23 12:14:06.000000 ignord-0.1.1/docs/requirements.txt
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      109 2023-05-23 12:14:06.000000 ignord-0.1.1/docs/spelling_wordlist.txt
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      185 2023-05-24 09:10:32.000000 ignord-0.1.1/docs/usage.rst
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     1207 2023-05-23 12:14:06.000000 ignord-0.1.1/pyproject.toml
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      771 2023-05-24 09:12:08.000000 ignord-0.1.1/pytest.ini
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       38 2023-05-24 09:23:59.413304 ignord-0.1.1/setup.cfg
--rwxr-xr-x   0 grafuls   (1000) grafuls   (1000)     2888 2023-05-24 09:07:36.000000 ignord-0.1.1/setup.py
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.410304 ignord-0.1.1/src/
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.412304 ignord-0.1.1/src/ignor.egg-info/
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2335 2023-05-24 08:54:05.000000 ignord-0.1.1/src/ignor.egg-info/PKG-INFO
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      892 2023-05-24 08:54:05.000000 ignord-0.1.1/src/ignor.egg-info/SOURCES.txt
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)        1 2023-05-24 08:54:05.000000 ignord-0.1.1/src/ignor.egg-info/dependency_links.txt
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       41 2023-05-24 08:54:05.000000 ignord-0.1.1/src/ignor.egg-info/entry_points.txt
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)        1 2023-05-23 12:23:46.000000 ignord-0.1.1/src/ignor.egg-info/not-zip-safe
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       17 2023-05-24 08:54:05.000000 ignord-0.1.1/src/ignor.egg-info/requires.txt
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)        6 2023-05-24 08:54:05.000000 ignord-0.1.1/src/ignor.egg-info/top_level.txt
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.412304 ignord-0.1.1/src/ignord/
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)    32229 2023-05-23 21:26:52.000000 ignord-0.1.1/src/ignord/.ignors
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       22 2023-05-24 09:10:31.000000 ignord-0.1.1/src/ignord/__init__.py
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      353 2023-05-24 09:10:30.000000 ignord-0.1.1/src/ignord/__main__.py
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     3904 2023-05-24 09:10:30.000000 ignord-0.1.1/src/ignord/cli.py
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.413304 ignord-0.1.1/src/ignord.egg-info/
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2389 2023-05-24 09:23:59.000000 ignord-0.1.1/src/ignord.egg-info/PKG-INFO
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     1137 2023-05-24 09:23:59.000000 ignord-0.1.1/src/ignord.egg-info/SOURCES.txt
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)        1 2023-05-24 09:23:59.000000 ignord-0.1.1/src/ignord.egg-info/dependency_links.txt
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       41 2023-05-24 09:23:59.000000 ignord-0.1.1/src/ignord.egg-info/entry_points.txt
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)        1 2023-05-24 09:13:13.000000 ignord-0.1.1/src/ignord.egg-info/not-zip-safe
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)       17 2023-05-24 09:23:59.000000 ignord-0.1.1/src/ignord.egg-info/requires.txt
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)        7 2023-05-24 09:23:59.000000 ignord-0.1.1/src/ignord.egg-info/top_level.txt
-drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:23:59.413304 ignord-0.1.1/tests/
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)      164 2023-05-24 09:07:37.000000 ignord-0.1.1/tests/test_ignord.py
--rw-r--r--   0 grafuls   (1000) grafuls   (1000)     1368 2023-05-23 22:27:08.000000 ignord-0.1.1/tox.ini
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.083934 ignord-0.1.2/
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      731 2023-05-24 09:10:29.000000 ignord-0.1.2/.bumpversion.cfg
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      174 2023-05-24 09:10:29.000000 ignord-0.1.2/.coveragerc
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      353 2023-05-23 12:14:06.000000 ignord-0.1.2/.editorconfig
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.079934 ignord-0.1.2/.github/
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.081934 ignord-0.1.2/.github/workflows/
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2585 2023-05-23 12:14:15.000000 ignord-0.1.2/.github/workflows/github-actions.yml
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      684 2023-05-23 12:14:06.000000 ignord-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      231 2023-05-23 12:14:06.000000 ignord-0.1.2/.readthedocs.yml
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       55 2023-05-23 12:14:06.000000 ignord-0.1.2/AUTHORS.rst
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      147 2023-05-24 09:10:27.000000 ignord-0.1.2/CHANGELOG.rst
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2299 2023-05-24 09:29:16.000000 ignord-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)    43650 2023-05-24 09:29:15.000000 ignord-0.1.2/LICENSE
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      427 2023-05-23 12:14:06.000000 ignord-0.1.2/MANIFEST.in
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2366 2023-05-24 09:32:30.083934 ignord-0.1.2/PKG-INFO
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2207 2023-05-24 09:12:07.000000 ignord-0.1.2/README.rst
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.081934 ignord-0.1.2/ci/
+-rwxr-xr-x   0 grafuls   (1000) grafuls   (1000)     2867 2023-05-23 12:14:06.000000 ignord-0.1.2/ci/bootstrap.py
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       72 2023-05-23 12:14:06.000000 ignord-0.1.2/ci/requirements.txt
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.079934 ignord-0.1.2/ci/templates/
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.079934 ignord-0.1.2/ci/templates/.github/
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.081934 ignord-0.1.2/ci/templates/.github/workflows/
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     1917 2023-05-23 12:14:06.000000 ignord-0.1.2/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.081934 ignord-0.1.2/docs/
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       28 2023-05-23 12:14:06.000000 ignord-0.1.2/docs/authors.rst
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       30 2023-05-23 12:14:06.000000 ignord-0.1.2/docs/changelog.rst
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     1132 2023-05-24 09:07:27.000000 ignord-0.1.2/docs/conf.py
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       33 2023-05-23 12:14:06.000000 ignord-0.1.2/docs/contributing.rst
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      244 2023-05-23 12:14:06.000000 ignord-0.1.2/docs/index.rst
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      142 2023-05-24 09:07:22.000000 ignord-0.1.2/docs/installation.rst
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       27 2023-05-23 12:14:06.000000 ignord-0.1.2/docs/readme.rst
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.082934 ignord-0.1.2/docs/reference/
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       93 2023-05-24 09:27:01.000000 ignord-0.1.2/docs/reference/ignord.rst
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       58 2023-05-24 09:07:28.000000 ignord-0.1.2/docs/reference/index.rst
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       29 2023-05-23 12:14:06.000000 ignord-0.1.2/docs/requirements.txt
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      109 2023-05-23 12:14:06.000000 ignord-0.1.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      185 2023-05-24 09:10:32.000000 ignord-0.1.2/docs/usage.rst
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     1207 2023-05-23 12:14:06.000000 ignord-0.1.2/pyproject.toml
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      771 2023-05-24 09:12:08.000000 ignord-0.1.2/pytest.ini
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       38 2023-05-24 09:32:30.083934 ignord-0.1.2/setup.cfg
+-rwxr-xr-x   0 grafuls   (1000) grafuls   (1000)     2867 2023-05-24 09:31:51.000000 ignord-0.1.2/setup.py
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.079934 ignord-0.1.2/src/
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.082934 ignord-0.1.2/src/ignor.egg-info/
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2335 2023-05-24 08:54:05.000000 ignord-0.1.2/src/ignor.egg-info/PKG-INFO
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      892 2023-05-24 08:54:05.000000 ignord-0.1.2/src/ignor.egg-info/SOURCES.txt
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)        1 2023-05-24 08:54:05.000000 ignord-0.1.2/src/ignor.egg-info/dependency_links.txt
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       41 2023-05-24 08:54:05.000000 ignord-0.1.2/src/ignor.egg-info/entry_points.txt
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)        1 2023-05-23 12:23:46.000000 ignord-0.1.2/src/ignor.egg-info/not-zip-safe
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       17 2023-05-24 08:54:05.000000 ignord-0.1.2/src/ignor.egg-info/requires.txt
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)        6 2023-05-24 08:54:05.000000 ignord-0.1.2/src/ignor.egg-info/top_level.txt
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.082934 ignord-0.1.2/src/ignord/
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)    32229 2023-05-23 21:26:52.000000 ignord-0.1.2/src/ignord/.ignors
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:31:45.000000 ignord-0.1.2/src/ignord/__init__.py
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      353 2023-05-24 09:10:30.000000 ignord-0.1.2/src/ignord/__main__.py
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     3904 2023-05-24 09:10:30.000000 ignord-0.1.2/src/ignord/cli.py
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.083934 ignord-0.1.2/src/ignord.egg-info/
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     2366 2023-05-24 09:32:30.000000 ignord-0.1.2/src/ignord.egg-info/PKG-INFO
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     1137 2023-05-24 09:32:30.000000 ignord-0.1.2/src/ignord.egg-info/SOURCES.txt
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)        1 2023-05-24 09:32:30.000000 ignord-0.1.2/src/ignord.egg-info/dependency_links.txt
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       43 2023-05-24 09:32:30.000000 ignord-0.1.2/src/ignord.egg-info/entry_points.txt
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)        1 2023-05-24 09:13:13.000000 ignord-0.1.2/src/ignord.egg-info/not-zip-safe
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)       17 2023-05-24 09:32:30.000000 ignord-0.1.2/src/ignord.egg-info/requires.txt
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)        7 2023-05-24 09:32:30.000000 ignord-0.1.2/src/ignord.egg-info/top_level.txt
+drwxr-xr-x   0 grafuls   (1000) grafuls   (1000)        0 2023-05-24 09:32:30.083934 ignord-0.1.2/tests/
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)      164 2023-05-24 09:07:37.000000 ignord-0.1.2/tests/test_ignord.py
+-rw-r--r--   0 grafuls   (1000) grafuls   (1000)     1368 2023-05-23 22:27:08.000000 ignord-0.1.2/tox.ini
```

### Comparing `ignord-0.1.1/.bumpversion.cfg` & `ignord-0.1.2/.bumpversion.cfg`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/.github/workflows/github-actions.yml` & `ignord-0.1.2/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/.pre-commit-config.yaml` & `ignord-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/CONTRIBUTING.rst` & `ignord-0.1.2/CONTRIBUTING.rst`

 * *Files 7% similar despite different names*

```diff
@@ -4,48 +4,48 @@
 
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given.
 
 Bug reports
 ===========
 
-When `reporting a bug <https://github.com/grafuls/python-ignor/issues>`_ please include:
+When `reporting a bug <https://github.com/grafuls/ignord/issues>`_ please include:
 
     * Your operating system name and version.
     * Any details about your local setup that might be helpful in troubleshooting.
     * Detailed steps to reproduce the bug.
 
 Documentation improvements
 ==========================
 
-ignor could always use more documentation, whether as part of the
-official ignor docs, in docstrings, or even on the web in blog posts,
+ignord could always use more documentation, whether as part of the
+official ignord docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Feature requests and feedback
 =============================
 
-The best way to send feedback is to file an issue at https://github.com/grafuls/python-ignor/issues.
+The best way to send feedback is to file an issue at https://github.com/grafuls/ignord/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that code contributions are welcome :)
 
 Development
 ===========
 
-To set up `python-ignor` for local development:
+To set up `ignord` for local development:
 
-1. Fork `python-ignor <https://github.com/grafuls/python-ignor>`_
+1. Fork `ignord <https://github.com/grafuls/ignord>`_
    (look for the "Fork" button).
 2. Clone your fork locally::
 
-    git clone git@github.com:YOURGITHUBNAME/python-ignor.git
+    git clone git@github.com:YOURGITHUBNAME/ignord.git
 
 3. Create a branch for local development::
 
     git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
```

### Comparing `ignord-0.1.1/LICENSE` & `ignord-0.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-ignor - ignor is a Python CLI application that generates git ignore files for a specific language.
+ignord - ignord is a Python CLI application that generates git ignore files for a specific language.
 Copyright (c) 2023, Gonzalo Rafuls.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License (version 3)
 as published by the Free Software Foundation.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `ignord-0.1.1/PKG-INFO` & `ignord-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ignord
-Version: 0.1.1
-Summary: ignor is a Python CLI application that generates git ignore files for a specific language.
-Home-page: https://github.com/grafuls/python-ignor
+Version: 0.1.2
+Summary: ignord is a Python CLI application that generates git ignore files for a specific language.
+Home-page: https://github.com/grafuls/ignord
 Author: Gonzalo Rafuls
 Author-email: grafuls@gmail.com
 License: LGPL-3.0-only
-Project-URL: Documentation, https://python-ignor.readthedocs.io/
-Project-URL: Changelog, https://python-ignor.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/grafuls/python-ignor/issues
+Project-URL: Documentation, https://ignord.readthedocs.io/
+Project-URL: Changelog, https://ignord.readthedocs.io/en/latest/changelog.html
+Project-URL: Issue Tracker, https://github.com/grafuls/ignord/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
```

### Comparing `ignord-0.1.1/README.rst` & `ignord-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/ci/bootstrap.py` & `ignord-0.1.2/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/ci/templates/.github/workflows/github-actions.yml` & `ignord-0.1.2/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/docs/conf.py` & `ignord-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/pyproject.toml` & `ignord-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/pytest.ini` & `ignord-0.1.2/pytest.ini`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/setup.py` & `ignord-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="ignord",
-    version="0.1.1",
+    version="0.1.2",
     license="LGPL-3.0-only",
-    description="ignor is a Python CLI application that generates git ignore files for a specific language.",
+    description="ignord is a Python CLI application that generates git ignore files for a specific language.",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Gonzalo Rafuls",
     author_email="grafuls@gmail.com",
-    url="https://github.com/grafuls/python-ignor",
+    url="https://github.com/grafuls/ignord",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=[path.stem for path in Path("src").glob("*.py")],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
@@ -49,17 +49,17 @@
         # uncomment if you test on these interpreters:
         # "Programming Language :: Python :: Implementation :: IronPython",
         # "Programming Language :: Python :: Implementation :: Jython",
         # "Programming Language :: Python :: Implementation :: Stackless",
         "Topic :: Utilities",
     ],
     project_urls={
-        "Documentation": "https://python-ignor.readthedocs.io/",
-        "Changelog": "https://python-ignor.readthedocs.io/en/latest/changelog.html",
-        "Issue Tracker": "https://github.com/grafuls/python-ignor/issues",
+        "Documentation": "https://ignord.readthedocs.io/",
+        "Changelog": "https://ignord.readthedocs.io/en/latest/changelog.html",
+        "Issue Tracker": "https://github.com/grafuls/ignord/issues",
     },
     keywords=[
         # eg: "keyword1", "keyword2", "keyword3",
     ],
     python_requires=">=3.7",
     install_requires=[
         "requests==2.31.0",
@@ -67,11 +67,11 @@
     extras_require={
         # eg:
         #   "rst": ["docutils>=0.11"],
         #   ":python_version=="2.6"": ["argparse"],
     },
     entry_points={
         "console_scripts": [
-            "ignor = ignor.cli:main",
+            "ignord = ignord.cli:main",
         ]
     },
 )
```

### Comparing `ignord-0.1.1/src/ignor.egg-info/PKG-INFO` & `ignord-0.1.2/src/ignor.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/src/ignor.egg-info/SOURCES.txt` & `ignord-0.1.2/src/ignor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/src/ignord/.ignors` & `ignord-0.1.2/src/ignord/.ignors`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/src/ignord/cli.py` & `ignord-0.1.2/src/ignord/cli.py`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/src/ignord.egg-info/PKG-INFO` & `ignord-0.1.2/src/ignord.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ignord
-Version: 0.1.1
-Summary: ignor is a Python CLI application that generates git ignore files for a specific language.
-Home-page: https://github.com/grafuls/python-ignor
+Version: 0.1.2
+Summary: ignord is a Python CLI application that generates git ignore files for a specific language.
+Home-page: https://github.com/grafuls/ignord
 Author: Gonzalo Rafuls
 Author-email: grafuls@gmail.com
 License: LGPL-3.0-only
-Project-URL: Documentation, https://python-ignor.readthedocs.io/
-Project-URL: Changelog, https://python-ignor.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/grafuls/python-ignor/issues
+Project-URL: Documentation, https://ignord.readthedocs.io/
+Project-URL: Changelog, https://ignord.readthedocs.io/en/latest/changelog.html
+Project-URL: Issue Tracker, https://github.com/grafuls/ignord/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
```

### Comparing `ignord-0.1.1/src/ignord.egg-info/SOURCES.txt` & `ignord-0.1.2/src/ignord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ignord-0.1.1/tox.ini` & `ignord-0.1.2/tox.ini`

 * *Files identical despite different names*

