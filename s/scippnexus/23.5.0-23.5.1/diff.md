# Comparing `tmp/scippnexus-23.5.0.tar.gz` & `tmp/scippnexus-23.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scippnexus-23.5.0.tar", last modified: Tue May  9 04:46:44 2023, max compression
+gzip compressed data, was "scippnexus-23.5.1.tar", last modified: Wed May 24 07:01:07 2023, max compression
```

## Comparing `scippnexus-23.5.0.tar` & `scippnexus-23.5.1.tar`

### file list

```diff
@@ -1,124 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.790512 scippnexus-23.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.778512 scippnexus-23.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.778512 scippnexus-23.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-05-09 04:46:34.000000 scippnexus-23.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-09 04:46:34.000000 scippnexus-23.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-09 04:46:44.790512 scippnexus-23.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-05-09 04:46:34.000000 scippnexus-23.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.778512 scippnexus-23.5.0/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-05-09 04:46:34.000000 scippnexus-23.5.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    17823 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/_static/logo-2022.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/_templates/scipp-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/_templates/sections/header-article.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7029 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/about/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8453 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/getting-started/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10348 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/getting-started/quick-start-guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (122)     9320 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/user-guide/application-definitions.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/user-guide/classes.rst
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/user-guide/functions.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11308 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/user-guide/nexus-classes.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4037 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/version.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-05-09 04:46:34.000000 scippnexus-23.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      572 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-05-09 04:46:34.000000 scippnexus-23.5.0/resources/logo-2022.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-09 04:46:44.790512 scippnexus-23.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.778512 scippnexus-23.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.786512 scippnexus-23.5.0/src/scippnexus/
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/_hdf5_nexus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.786512 scippnexus-23.5.0/src/scippnexus/data/
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      876 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.786512 scippnexus-23.5.0/src/scippnexus/definitions/
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/definitions/nxcansas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.786512 scippnexus-23.5.0/src/scippnexus/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7424 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md
--rw-r--r--   0 runner    (1001) docker     (122)      941 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/file.py
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/leaf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nexus_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxcylindrical_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    11291 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     9912 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxdetector.py
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxdisk_chopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     5064 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxevent_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxfermi_chopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxlog.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxmonitor.py
--rw-r--r--   0 runner    (1001) docker     (122)    24870 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxoff_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxsample.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxsource.py
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxtransformations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.790512 scippnexus-23.5.0/src/scippnexus/v2/
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.778512 scippnexus-23.5.0/src/scippnexus/v2/application_definitions/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.790512 scippnexus-23.5.0/src/scippnexus/v2/application_definitions/nxcansas/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/application_definitions/nxcansas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4970 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/attrs.py
--rw-r--r--   0 runner    (1001) docker     (122)    18015 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8974 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/field.py
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/file.py
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nexus_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3137 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxcylindrical_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    26648 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     6001 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxevent_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxoff_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxsample.py
--rw-r--r--   0 runner    (1001) docker     (122)     8552 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxtransformations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.786512 scippnexus-23.5.0/src/scippnexus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-09 04:46:44.000000 scippnexus-23.5.0/src/scippnexus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-05-09 04:46:44.000000 scippnexus-23.5.0/src/scippnexus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 04:46:44.000000 scippnexus-23.5.0/src/scippnexus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-09 04:46:44.000000 scippnexus-23.5.0/src/scippnexus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-09 04:46:44.000000 scippnexus-23.5.0/src/scippnexus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.790512 scippnexus-23.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3863 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/application_definition_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/externalfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3317 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/load_files_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    19370 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nexus_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxcylindrical_geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    26815 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxdata_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    30034 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxdetector_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxevent_data_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     8869 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxlog_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxmonitor_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxoff_geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxsample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    18218 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxtransformations_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.320955 scippnexus-23.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-05-24 07:00:53.000000 scippnexus-23.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-24 07:00:53.000000 scippnexus-23.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-24 07:01:07.320955 scippnexus-23.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-05-24 07:00:53.000000 scippnexus-23.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-05-24 07:00:53.000000 scippnexus-23.5.1/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    17823 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/_static/logo-2022.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/_templates/scipp-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/_templates/sections/header-article.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/about/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8472 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/getting-started/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10348 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/getting-started/quick-start-guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (122)     9320 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/user-guide/application-definitions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/user-guide/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/user-guide/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11308 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/user-guide/nexus-classes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3865 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-24 07:00:53.000000 scippnexus-23.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-05-24 07:00:53.000000 scippnexus-23.5.1/resources/logo-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-24 07:01:07.320955 scippnexus-23.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.316955 scippnexus-23.5.1/src/scippnexus/
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4520 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2972 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/_hdf5_nexus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.316955 scippnexus-23.5.1/src/scippnexus/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.316955 scippnexus-23.5.1/src/scippnexus/definitions/
+-rw-r--r--   0 runner    (1001) docker     (122)     5027 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/definitions/nxcansas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.316955 scippnexus-23.5.1/src/scippnexus/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7424 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/leaf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nexus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxcylindrical_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11665 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9934 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxdetector.py
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxdisk_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxevent_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxfermi_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2420 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxlog.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxmonitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25066 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxoff_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxsample.py
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxsource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6885 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxtransformations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.320955 scippnexus-23.5.1/src/scippnexus/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/src/scippnexus/v2/application_definitions/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.320955 scippnexus-23.5.1/src/scippnexus/v2/application_definitions/nxcansas/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/application_definitions/nxcansas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4948 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18007 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/field.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nexus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxcylindrical_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26655 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5942 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxevent_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3549 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxoff_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxsample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8477 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxtransformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.316955 scippnexus-23.5.1/src/scippnexus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-24 07:01:07.000000 scippnexus-23.5.1/src/scippnexus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2848 2023-05-24 07:01:07.000000 scippnexus-23.5.1/src/scippnexus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 07:01:07.000000 scippnexus-23.5.1/src/scippnexus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-24 07:01:07.000000 scippnexus-23.5.1/src/scippnexus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-24 07:01:07.000000 scippnexus-23.5.1/src/scippnexus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.320955 scippnexus-23.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/application_definition_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/externalfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/load_files_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19069 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nexus_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxcylindrical_geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27977 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxdata_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28814 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxdetector_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5341 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxevent_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8468 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxlog_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxmonitor_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6059 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxoff_geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxsample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18094 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxtransformations_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tox.ini
```

### Comparing `scippnexus-23.5.0/.github/workflows/ci.yml` & `scippnexus-23.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/.github/workflows/docs.yml` & `scippnexus-23.5.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/.github/workflows/release.yml` & `scippnexus-23.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/.pre-commit-config.yaml` & `scippnexus-23.5.1/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,18 @@
         args: [ --markdown-linebreak-ext=md ]
         exclude: '\.svg'
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
         name: isort (python)
-  - repo: https://github.com/pre-commit/mirrors-yapf
-    rev: v0.32.0
+  - repo: https://github.com/psf/black
+    rev: 23.1.0
     hooks:
-      - id: yapf
-        args: [ "-i", "-r" ]
-        types: [ "python" ]
-        additional_dependencies: [ "toml" ]
+      - id: black
   - repo: https://github.com/kynan/nbstripout
     rev: 0.6.0
     hooks:
       - id: nbstripout
         types: [ "jupyter" ]
         args: [ "--drop-empty-cells",
                 "--extra-keys 'metadata.language_info.version cell.metadata.jp-MarkdownHeadingCollapsed cell.metadata.pycharm'" ]
```

### Comparing `scippnexus-23.5.0/LICENSE` & `scippnexus-23.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/PKG-INFO` & `scippnexus-23.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippnexus
-Version: 23.5.0
+Version: 23.5.1
 Summary: h5py-like utility for NeXus files based with seamless scipp integration
 Home-page: https://scipp.github.io/scippnexus
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/scippnexus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `scippnexus-23.5.0/README.md` & `scippnexus-23.5.1/README.md`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/conda/meta.yaml` & `scippnexus-23.5.1/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/_static/favicon.ico` & `scippnexus-23.5.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/_static/logo-2022.svg` & `scippnexus-23.5.1/docs/_static/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/_templates/scipp-class-template.rst` & `scippnexus-23.5.1/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/_templates/scipp-module-template.rst` & `scippnexus-23.5.1/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/_templates/sections/header-article.html` & `scippnexus-23.5.1/docs/_templates/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/about/about.rst` & `scippnexus-23.5.1/docs/about/about.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/about/release-notes.rst` & `scippnexus-23.5.1/docs/about/release-notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,23 @@
    Contributors
    ~~~~~~~~~~~~
 
    Simon Heybrock :sup:`a`\ ,
    Neil Vaytet :sup:`a`\ ,
    and Jan-Lukas Wynen :sup:`a`
 
+v23.05.1
+--------
+
+Bugfixes
+~~~~~~~~
+
+* Fix loading of data with legacy ``axes`` attribute on signal fields `#145 <https://github.com/scipp/scippnexus/pull/145>`_.
+* Fix loading of groups with single-valued and unit-less signal field `#145 <https://github.com/scipp/scippnexus/pull/145>`_.
+
 v23.05.0
 --------
 
 Features
 ~~~~~~~~
 
 * ``scippnexus.v2``: Support NXlog with "sublogs" such as connection_status and alarm `#138 <https://github.com/scipp/scippnexus/pull/138>`_.
```

### Comparing `scippnexus-23.5.0/docs/conf.py` & `scippnexus-23.5.1/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,42 +36,39 @@
     base = "https://scipp.github.io"
     l1 = []
     l1.append({"type": "link", "text": "scipp", "url": f"{base}"})
     l1.append({"type": "link", "text": "scippnexus", "url": f"{base}/scippnexus"})
     l1.append({"type": "link", "text": "scippneutron", "url": f"{base}/scippneutron"})
     l1.append({"type": "link", "text": "ess", "url": f"{base}/ess"})
     header_buttons = context["header_buttons"]
-    header_buttons.append({
-        "type": "group",
-        "buttons": l1,
-        "icon": "fa fa-caret-down",
-        "text": "Related projects"
-    })
+    header_buttons.append(
+        {
+            "type": "group",
+            "buttons": l1,
+            "icon": "fa fa-caret-down",
+            "text": "Related projects",
+        }
+    )
     releases = version_info.minor_releases(first='0.1')
     if outdated:
         current = f"{long_version} (outdated)"
         latest = "latest"
         entries = ['.'.join(long_version.split('.')[:2])]
     else:
         current = f"{long_version} (latest)"
         latest = f"{releases[0]} (latest)"
         entries = releases[1:]
     lines = [{"type": "link", "text": latest, "url": f"{base}/{project}"}]
     for r in entries:
-        lines.append({
-            "type": "link",
-            "text": f"{r}",
-            "url": f"{base}/{project}/release/{r}"
-        })
-    header_buttons.append({
-        "type": "group",
-        "buttons": lines,
-        "icon": "fa fa-caret-down",
-        "text": current
-    })
+        lines.append(
+            {"type": "link", "text": f"{r}", "url": f"{base}/{project}/release/{r}"}
+        )
+    header_buttons.append(
+        {"type": "group", "buttons": lines, "icon": "fa fa-caret-down", "text": current}
+    )
 
 
 sphinx_book_theme.add_launch_buttons = add_buttons
 
 html_show_sourcelink = True
 
 extensions = [
@@ -98,15 +95,15 @@
 """  # noqa: E501
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
     'scipp': ('https://scipp.github.io/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/', None),
-    'xarray': ('https://xarray.pydata.org/en/stable/', None)
+    'xarray': ('https://xarray.pydata.org/en/stable/', None),
 }
 
 # autodocs includes everything, even irrelevant API internals. autosummary
 # looks more suitable in the long run when the API grows.
 # For a nice example see how xarray handles its API documentation.
 autosummary_generate = True
 
@@ -192,15 +189,16 @@
 }
 
 if outdated:
     html_theme_options["announcement"] = (
         f"⚠️ You are viewing the documentation for an old version of {project}. "
         f"Switch to <a href='https://scipp.github.io/{project}' "
         "style='color:white;text-decoration:underline;'"
-        ">latest</a> version. ⚠️")
+        ">latest</a> version. ⚠️"
+    )
 
 html_logo = "_static/logo-2022.svg"
 html_favicon = "_static/favicon.ico"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
@@ -230,16 +228,23 @@
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'scipp', u'scipp Documentation', author, 'scipp',
-     'One line description of project.', 'Miscellaneous'),
+    (
+        master_doc,
+        'scipp',
+        u'scipp Documentation',
+        author,
+        'scipp',
+        'One line description of project.',
+        'Miscellaneous',
+    ),
 ]
 
 # -- Options for Matplotlib in notebooks ----------------------------------
 
 nbsphinx_execute_arguments = [
     "--Session.metadata=scipp_docs_build=True",
 ]
@@ -249,17 +254,20 @@
 doctest_global_setup = '''
 import numpy as np
 import scipp as sc
 '''
 
 # Using normalize whitespace because many __str__ functions in scipp produce
 # extraneous empty lines and it would look strange to include them in the docs.
-doctest_default_flags = doctest.ELLIPSIS | doctest.IGNORE_EXCEPTION_DETAIL | \
-                        doctest.DONT_ACCEPT_TRUE_FOR_1 | \
-                        doctest.NORMALIZE_WHITESPACE
+doctest_default_flags = (
+    doctest.ELLIPSIS
+    | doctest.IGNORE_EXCEPTION_DETAIL
+    | doctest.DONT_ACCEPT_TRUE_FOR_1
+    | doctest.NORMALIZE_WHITESPACE
+)
 
 # -- Options for linkcheck ------------------------------------------------
 
 linkcheck_ignore = [
     # Specific lines in Github blobs cannot be found by linkcheck.
     r'https?://github\.com/.*?/blob/[a-f0-9]+/.+?#',
 ]
```

### Comparing `scippnexus-23.5.0/docs/getting-started/installation.rst` & `scippnexus-23.5.1/docs/getting-started/installation.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/getting-started/quick-start-guide.ipynb` & `scippnexus-23.5.1/docs/getting-started/quick-start-guide.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/index.rst` & `scippnexus-23.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/user-guide/application-definitions.ipynb` & `scippnexus-23.5.1/docs/user-guide/application-definitions.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/user-guide/classes.rst` & `scippnexus-23.5.1/docs/user-guide/classes.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/user-guide/nexus-classes.ipynb` & `scippnexus-23.5.1/docs/user-guide/nexus-classes.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/docs/version.py` & `scippnexus-23.5.1/docs/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
             versions.append(parse(t.name))
         except InvalidVersion:
             pass
     return sorted(versions, reverse=True)
 
 
 class VersionInfo:
-
     def __init__(self):
         self._releases = _get_releases()
 
     def _to_version(self, version) -> Version:
         if isinstance(version, str):
             try:
                 return parse(version)
@@ -88,23 +87,24 @@
     elif action == 'get-target':
         print(info.target(version))
     return 0
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Process some integers.')
-    parser.add_argument('--action',
-                        choices=['is-latest', 'is-new', 'get-replaced', 'get-target'],
-                        required=True,
-                        help='Action to perform: Check whether this major or minor '
-                        'release exists or is new (is-latest), check whether this is a '
-                        'new major or minor release (is-new), get the version this is '
-                        'replacing (get-replaced), get the target folder for '
-                        'publishing the docs (get-target). In all cases the '
-                        'patch/micro version is ignored.')
-    parser.add_argument('--version',
-                        dest='version',
-                        required=True,
-                        help='Version the action refers to')
+    parser.add_argument(
+        '--action',
+        choices=['is-latest', 'is-new', 'get-replaced', 'get-target'],
+        required=True,
+        help='Action to perform: Check whether this major or minor '
+        'release exists or is new (is-latest), check whether this is a '
+        'new major or minor release (is-new), get the version this is '
+        'replacing (get-replaced), get the target folder for '
+        'publishing the docs (get-target). In all cases the '
+        'patch/micro version is ignored.',
+    )
+    parser.add_argument(
+        '--version', dest='version', required=True, help='Version the action refers to'
+    )
 
     args = parser.parse_args()
     sys.exit(main(**vars(args)))
```

### Comparing `scippnexus-23.5.0/requirements/ci.txt` & `scippnexus-23.5.1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/requirements/docs.txt` & `scippnexus-23.5.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/requirements/static.txt` & `scippnexus-23.5.1/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/resources/logo-2022.svg` & `scippnexus-23.5.1/resources/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/setup.cfg` & `scippnexus-23.5.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -36,15 +36,11 @@
 [options.package_data]
 scippnexus = py.typed
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203
 
-[yapf]
-based_on_style = pep8
-column_limit = 88
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `scippnexus-23.5.0/src/scippnexus/__init__.py` & `scippnexus-23.5.1/src/scippnexus/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/src/scippnexus/_common.py` & `scippnexus-23.5.1/src/scippnexus/_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 import numpy as np
 import scipp as sc
 
 from .typing import ScippIndex
 
 
 def convert_time_to_datetime64(
-        raw_times: sc.Variable,
-        start: str = None,
-        scaling_factor: Union[float, np.float_] = None) -> sc.Variable:
+    raw_times: sc.Variable,
+    start: str = None,
+    scaling_factor: Union[float, np.float_] = None,
+) -> sc.Variable:
     """
     The nexus standard allows an arbitrary scaling factor to be inserted
     between the numbers in the `time` series and the unit of time reported
     in the nexus attribute.
 
     The times are also relative to a given log start time, which might be
     different for each log. If this log start time is not available, the start of the
@@ -29,52 +30,60 @@
         start: Optional, the start time of the log in an ISO8601
             string. If not provided, defaults to the beginning of the
             unix epoch (1970-01-01T00:00:00).
         scaling_factor: Optional, the scaling factor between the provided
             time series data and the unit of the raw_times Variable. If
             not provided, defaults to 1 (a no-op scaling factor).
     """
-    if (raw_times.dtype
-            in (sc.DType.float64, sc.DType.float32)) or scaling_factor is not None:
+    if (
+        raw_times.dtype in (sc.DType.float64, sc.DType.float32)
+    ) or scaling_factor is not None:
         unit = sc.units.ns
     else:
         # determine more precise unit
         ratio = sc.scalar(1.0, unit=start.unit) / sc.scalar(
-            1.0, unit=raw_times.unit).to(unit=start.unit)
+            1.0, unit=raw_times.unit
+        ).to(unit=start.unit)
         unit = start.unit if ratio.value < 1.0 else raw_times.unit
 
     if scaling_factor is None:
         times = raw_times
     else:
         times = raw_times * sc.scalar(value=scaling_factor)
     return start.to(unit=unit, copy=False) + times.to(
-        dtype=sc.DType.int64, unit=unit, copy=False)
+        dtype=sc.DType.int64, unit=unit, copy=False
+    )
 
 
-def _to_canonical_select(dims: List[str],
-                         select: ScippIndex) -> Dict[str, Union[int, slice]]:
+def _to_canonical_select(
+    dims: List[str], select: ScippIndex
+) -> Dict[str, Union[int, slice]]:
     """Return selection as dict with explicit dim labels"""
 
     def check_1d():
         if len(dims) != 1:
-            raise sc.DimensionError(f"Dataset has multiple dimensions {dims}, "
-                                    "specify the dimension to index.")
+            raise sc.DimensionError(
+                f"Dataset has multiple dimensions {dims}, "
+                "specify the dimension to index."
+            )
 
     if select is Ellipsis:
         return {}
     if isinstance(select, tuple) and len(select) == 0:
         return {}
     if isinstance(select, tuple) and isinstance(select[0], str):
         key, sel = select
         return {key: sel}
     if isinstance(select, tuple):
         check_1d()
         if len(select) != 1:
-            raise sc.DimensionError(f"Dataset has single dimension {dims}, "
-                                    "but multiple indices {select} were specified.")
+            raise sc.DimensionError(
+                f"Dataset has single dimension {dims}, "
+                "but multiple indices {select} were specified."
+            )
         return {dims[0]: select[0]}
     elif isinstance(select, int) or isinstance(select, slice):
         check_1d()
         return {dims[0]: select}
     if not isinstance(select, dict):
         raise IndexError(f"Cannot process index {select}.")
     return select.copy()
@@ -85,25 +94,28 @@
     Given a valid "scipp" index 'select', return an equivalent plain numpy-style index.
     """
     select = _to_canonical_select(dims, select)
     index = [slice(None)] * len(dims)
     for key, sel in select.items():
         if key not in dims:
             raise sc.DimensionError(
-                f"'{key}' used for indexing not found in dataset dims {dims}.")
+                f"'{key}' used for indexing not found in dataset dims {dims}."
+            )
         index[dims.index(key)] = sel
     if len(index) == 1:
         return index[0]
     return tuple(index)
 
 
-def to_child_select(dims: List[str],
-                    child_dims: List[str],
-                    select: ScippIndex,
-                    bin_edge_dim: Optional[str] = None) -> ScippIndex:
+def to_child_select(
+    dims: List[str],
+    child_dims: List[str],
+    select: ScippIndex,
+    bin_edge_dim: Optional[str] = None,
+) -> ScippIndex:
     """
     Given a valid "scipp" index 'select' for a Nexus class, return a selection for a
     child field of the class, which may have fewer dimensions.
 
     This removes any selections that apply to the parent but not the child.
     """
     select = _to_canonical_select(dims, select)
```

### Comparing `scippnexus-23.5.0/src/scippnexus/_hdf5_nexus.py` & `scippnexus-23.5.1/src/scippnexus/_hdf5_nexus.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,30 @@
         Either "ascii" or "utf-8".
     """
     if cset == h5py.h5t.CSET_ASCII:
         return "ascii"
     elif cset == h5py.h5t.CSET_UTF8:
         return "utf-8"
     else:
-        raise ValueError(f"Unknown character set in HDF5 data file. Expected data "
-                         f"types are {h5py.h5t.CSET_ASCII=} or "
-                         f"{h5py.h5t.CSET_UTF8=} but got '{cset}'. ")
+        raise ValueError(
+            f"Unknown character set in HDF5 data file. Expected data "
+            f"types are {h5py.h5t.CSET_ASCII=} or "
+            f"{h5py.h5t.CSET_UTF8=} but got '{cset}'. "
+        )
 
 
 def _warn_latin1_decode(obj, decoded, error):
-    warnings.warn(f"Encoding for bytes '{obj}' declared as ascii, "
-                  f"but contains characters in extended ascii range. Assuming "
-                  f"extended ASCII (latin-1), but this behavior is not "
-                  f"specified by the HDF5 or nexus standards and may therefore "
-                  f"be incorrect. Decoded string using latin-1 is '{decoded}'. "
-                  f"Error was '{error}'.")
+    warnings.warn(
+        f"Encoding for bytes '{obj}' declared as ascii, "
+        f"but contains characters in extended ascii range. Assuming "
+        f"extended ASCII (latin-1), but this behavior is not "
+        f"specified by the HDF5 or nexus standards and may therefore "
+        f"be incorrect. Decoded string using latin-1 is '{decoded}'. "
+        f"Error was '{error}'."
+    )
 
 
 def _ensure_str(str_or_bytes: Union[str, bytes], encoding: str) -> str:
     """
     See https://docs.h5py.org/en/stable/strings.html for justification about some of
     the operations performed in this method. In particular, variable-length strings
     are returned as `str` from h5py, but need to be encoded using the surrogateescape
```

### Comparing `scippnexus-23.5.0/src/scippnexus/data/__init__.py` & `scippnexus-23.5.1/src/scippnexus/data/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 _version = '1'
 
 __all__ = ['get_path']
 
 
 def _make_pooch():
     import pooch
+
     return pooch.create(
         path=pooch.os_cache('scippnexus'),
         env='SCIPPNEXUS_DATA_DIR',
         retry_if_failed=3,
         base_url='https://public.esss.dk/groups/scipp/scippnexus/{version}/',
         version=_version,
         registry={
             'PG3_4844_event.nxs': 'md5:d5ae38871d0a09a28ae01f85d969de1e',
-        })
+        },
+    )
 
 
 _pooch = _make_pooch()
 
 
 def get_path(name: str) -> str:
     """
```

### Comparing `scippnexus-23.5.0/src/scippnexus/definition.py` & `scippnexus-23.5.1/src/scippnexus/definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,12 +18,11 @@
 
 def make_definition(mapping: Dict[NXobject, type]) -> ApplicationDefinition:
     """
     Create an application definition from a mapping of NeXus classes to strategies.
     """
 
     class Definition(ApplicationDefinition):
-
         def make_strategy(self, group: NXobject) -> type:
             return mapping.get(group.nx_class)
 
     return Definition()
```

### Comparing `scippnexus-23.5.0/src/scippnexus/definitions/nxcansas.py` & `scippnexus-23.5.1/src/scippnexus/definitions/nxcansas.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,49 +6,52 @@
 import scipp as sc
 
 from ..definition import ApplicationDefinition as BaseDef
 from ..nxobject import NXobject
 
 
 class ApplicationDefinition(BaseDef):
-
     def __init__(self, class_attribute: str, default: str = None):
         self._default_class = default
         self._class_attribute = class_attribute
         self._strategies = {}
 
     def make_strategy(self, group: NXobject):
         # This approach will likely need to be generalized as many application
         # definitions to not define a "class attribute" in the style of canSAS_class,
         # but seem to rely on basic structure and the NX_class attribute.
-        if (definition_class := group.attrs.get(self._class_attribute,
-                                                self._default_class)) is not None:
+        if (
+            definition_class := group.attrs.get(
+                self._class_attribute, self._default_class
+            )
+        ) is not None:
             return self._strategies.get(definition_class)
 
     def register(self, sas_class):
-
         def decorator(strategy):
             self._strategies[sas_class] = strategy
             return strategy
 
         return decorator
 
 
 NXcanSAS = ApplicationDefinition('canSAS_class', 'SASroot')
 
 
 class SASdata:
     nx_class = 'NXdata'
 
-    def __init__(self,
-                 data: sc.DataArray,
-                 Q_variances: Optional[Literal['uncertainties', 'resolutions']] = None):
+    def __init__(
+        self,
+        data: sc.DataArray,
+        Q_variances: Optional[Literal['uncertainties', 'resolutions']] = None,
+    ):
         self.data = data
         valid = ('uncertainties', 'resolutions')
-        if Q_variances not in (None, ) + valid:
+        if Q_variances not in (None,) + valid:
             raise ValueError(f"Q_variances must be in {valid}")
         self._variances = Q_variances
 
     def __write_to_nexus_group__(self, group: NXobject):
         da = self.data
         group.attrs['canSAS_class'] = 'SASdata'
         group.attrs['signal'] = 'I'
@@ -60,29 +63,30 @@
         # NXcanSAS.
         if da.variances is not None:
             signal.attrs['uncertainties'] = 'I_errors'
             group.create_field('I_errors', sc.stddevs(da.data))
         if da.coords.is_edges('Q'):
             raise ValueError(
                 "Q is given as bin-edges, but NXcanSAS requires Q points (such as "
-                "bin centers).")
+                "bin centers)."
+            )
         coord = group.create_field('Q', da.coords['Q'])
         if da.coords['Q'].variances is not None:
             if self._variances is None:
                 raise ValueError(
                     "Q has variances, must specify whether these represent "
-                    "'uncertainties' or 'resolutions' using the 'Q_variances' option'")
+                    "'uncertainties' or 'resolutions' using the 'Q_variances' option'"
+                )
 
             coord.attrs[self._variances] = 'Q_errors'
             group.create_field('Q_errors', sc.stddevs(da.coords['Q']))
 
 
 @NXcanSAS.register('SASdata')
 class SASdataStrategy:
-
     @staticmethod
     def axes(group: NXobject) -> Tuple[str]:
         return group.attrs.get('I_axes')
 
     @staticmethod
     def signal(group: NXobject) -> str:
         return group.attrs.get('signal', 'I')
@@ -105,21 +109,20 @@
         elif resolutions is None:
             return uncertainties
         raise RuntimeError("Cannot handle both uncertainties and resolutions for Q")
 
 
 @NXcanSAS.register('SAStransmission_spectrum')
 class SAStransmission_spectrumStrategy:
-
     @staticmethod
     def dims(group: NXobject) -> Tuple[str]:
         # TODO A valid file should have T_axes, do we need to fallback?
         if (axes := group.attrs.get('T_axes')) is not None:
-            return (axes, )
-        return ('lambda', )
+            return (axes,)
+        return ('lambda',)
 
 
 class SASentry:
     nx_class = 'NXentry'
 
     def __init__(self, *, title: str, run: Union[str, int]):
         self.title = title
```

### Comparing `scippnexus-23.5.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md` & `scippnexus-23.5.1/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/src/scippnexus/file.py` & `scippnexus-23.5.1/src/scippnexus/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import h5py
 from scipp import VisibleDeprecationWarning
 
 from .nexus_classes import NXroot
 
 
 class File(AbstractContextManager, NXroot):
-
     def __init__(self, *args, definition=None, **kwargs):
         warnings.warn(
             "This API is deprecated and will be removed and replaced in release 23.06. "
             "Switch to 'import scippnexus.v2 as snx' to prepare for this.",
-            VisibleDeprecationWarning)
+            VisibleDeprecationWarning,
+        )
         self._file = h5py.File(*args, **kwargs)
         NXroot.__init__(self, self._file, definition=definition)
 
     def __enter__(self):
         self._file.__enter__()
         return self
```

### Comparing `scippnexus-23.5.0/src/scippnexus/leaf.py` & `scippnexus-23.5.1/src/scippnexus/leaf.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 import scipp as sc
 
 from ._common import to_plain_index
 from .nxobject import NXobject, ScippIndex
 
 
 class Leaf(NXobject):
-    """Base class for "leaf" groups than can be loaded as a dict.
-    """
+    """Base class for "leaf" groups than can be loaded as a dict."""
 
-    def _getitem(self,
-                 select: ScippIndex) -> Dict[str, Union[sc.Variable, sc.DataArray]]:
+    def _getitem(
+        self, select: ScippIndex
+    ) -> Dict[str, Union[sc.Variable, sc.DataArray]]:
         from .nexus_classes import NXtransformations
+
         index = to_plain_index([], select)
         if index != tuple():
             raise ValueError(f"Cannot select slice when loading {type(self).__name__}")
         content = sc.DataGroup()
         for key, obj in self.items():
             if key == 'depends_on' or isinstance(obj, NXtransformations):
                 continue
```

### Comparing `scippnexus-23.5.0/src/scippnexus/nexus_classes.py` & `scippnexus-23.5.1/src/scippnexus/nexus_classes.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/src/scippnexus/nxcylindrical_geometry.py` & `scippnexus-23.5.1/src/scippnexus/nxcylindrical_geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,62 +4,66 @@
 from typing import Optional, Tuple, Union
 
 import scipp as sc
 
 from .nxobject import NexusStructureError, NXobject
 
 
-def _parse(*,
-           vertices: sc.Variable,
-           cylinders: sc.Variable,
-           detector_number: Optional[sc.Variable] = None,
-           parent_detector_number: Optional[sc.Variable] = None) -> sc.Variable:
+def _parse(
+    *,
+    vertices: sc.Variable,
+    cylinders: sc.Variable,
+    detector_number: Optional[sc.Variable] = None,
+    parent_detector_number: Optional[sc.Variable] = None
+) -> sc.Variable:
     face1_center = cylinders['vertex_index', 0]
     face1_edge = cylinders['vertex_index', 1]
     face2_center = cylinders['vertex_index', 2]
     ds = sc.Dataset()
     ds['face1_center'] = vertices[face1_center.values]
     ds['face1_edge'] = vertices[face1_edge.values]
     ds['face2_center'] = vertices[face2_center.values]
     ds = ds.rename(**{vertices.dim: 'cylinder'})
     if detector_number is None:
         # All cylinders belong to the same shape
         return sc.bins(begin=sc.index(0), dim='cylinder', data=ds)
     if parent_detector_number is None:
         raise NexusStructureError(
             "`detector_number` not given, but "
-            "NXcylindrical_geometry contains mapping to `detector_number`.")
+            "NXcylindrical_geometry contains mapping to `detector_number`."
+        )
     # detector_number gives indices into cylinders, the naming in the NeXus
     # standard appears to be misleading
     if parent_detector_number.values.size != detector_number.values.size:
         raise NexusStructureError(
             "Number of detector numbers in NXcylindrical_geometry "
-            "does not match the one given by the parent.")
+            "does not match the one given by the parent."
+        )
     detecting_cylinders = ds['cylinder', detector_number.values]
     # One cylinder per detector
-    begin = sc.arange('dummy',
-                      parent_detector_number.values.size,
-                      unit=None,
-                      dtype='int64')
+    begin = sc.arange(
+        'dummy', parent_detector_number.values.size, unit=None, dtype='int64'
+    )
     end = begin + sc.index(1)
     shape = sc.bins(begin=begin, end=end, dim='cylinder', data=detecting_cylinders)
     return shape.fold(dim='dummy', sizes=parent_detector_number.sizes)
 
 
 class NXcylindrical_geometry(NXobject):
     _dims = {
-        'vertices': ('vertex', ),
-        'detector_number': ('detector_number', ),
-        'cylinders': ('cylinder', 'vertex_index')
+        'vertices': ('vertex',),
+        'detector_number': ('detector_number',),
+        'cylinders': ('cylinder', 'vertex_index'),
     }
 
     def _get_field_dims(self, name: str) -> Union[None, Tuple[str]]:
         return self._dims.get(name)
 
     def _get_field_dtype(self, name: str) -> Union[None, sc.DType]:
         if name == 'vertices':
             return sc.DType.vector3
         return None
 
-    def load_as_array(self,
-                      detector_number: Optional[sc.Variable] = None) -> sc.Variable:
+    def load_as_array(
+        self, detector_number: Optional[sc.Variable] = None
+    ) -> sc.Variable:
         return _parse(**self[()], parent_detector_number=detector_number)
```

### Comparing `scippnexus-23.5.0/src/scippnexus/nxdata.py` & `scippnexus-23.5.1/src/scippnexus/nxdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 class NXdataStrategy:
     """
     Strategy used by :py:class:`scippnexus.NXdata`.
 
     May be subclassed to customize behavior.
     """
+
     _error_suffixes = ['_errors', '_error']  # _error is the deprecated suffix
 
     @staticmethod
     def axes(group):
         """Names of the axes (dimension labels)."""
         return group.attrs.get('axes')
 
@@ -58,29 +59,31 @@
     def coord_errors(group, name):
         """Name of the field to use for standard-deviations of a coordinate."""
         errors = [f'{name}{suffix}' for suffix in NXdataStrategy._error_suffixes]
         errors = [x for x in errors if x in group]
         if len(errors) == 0:
             return None
         if len(errors) == 2:
-            warn(f"Found {name}_errors as well as the deprecated "
-                 f"{name}_error. The latter will be ignored.")
+            warn(
+                f"Found {name}_errors as well as the deprecated "
+                f"{name}_error. The latter will be ignored."
+            )
         return errors[0]
 
 
 class NXdata(NXobject):
-
     def __init__(
-            self,
-            group: H5Group,
-            *,
-            definition=None,
-            strategy=None,
-            signal_override: Union[Field, '_EventField'] = None,  # noqa: F821
-            skip: List[str] = None):
+        self,
+        group: H5Group,
+        *,
+        definition=None,
+        strategy=None,
+        signal_override: Union[Field, '_EventField'] = None,  # noqa: F821
+        skip: List[str] = None,
+    ):
         """
         Parameters
         ----------
         signal_override:
             Field-like to use instead of trying to read signal from the file. This is
             used when there is no signal or to provide a signal computed from
             NXevent_data.
@@ -135,26 +138,32 @@
     @property
     def _signal(self) -> Union[Field, '_EventField', None]:  # noqa: F821
         if self._signal_override is not None:
             return self._signal_override
         if self._signal_name is not None:
             if self._signal_name not in self:
                 raise NexusStructureError(
-                    f"Signal field '{self._signal_name}' not found in group.")
+                    f"Signal field '{self._signal_name}' not found in group."
+                )
             return self[self._signal_name]
         return None
 
     def _get_axes(self):
         """Return labels of named axes. Does not include default 'dim_{i}' names."""
         if (axes := self._strategy.axes(self)) is not None:
             # Unlike self.dims we *drop* entries that are '.'
             return [a for a in axes if a != '.']
         elif (signal := self._signal) is not None:
             if (axes := signal.attrs.get('axes')) is not None:
-                return axes.split(',')
+                dims = axes.split(':')
+                # The standard says that the axes should be colon-separated, but some
+                # files use comma-separated.
+                if len(dims) == 1 and self._signal.ndim > 1:
+                    dims = tuple(axes.split(','))
+                return dims
         return []
 
     def _guess_dims(self, name: str):
         """Guess dims of non-signal dataset based on shape.
 
         Does not check for potential bin-edge coord.
         """
@@ -166,15 +175,16 @@
             for d, s in zip(self.dims, self.shape):
                 if self.shape.count(s) == 1:
                     lut[s] = d
         try:
             dims = [lut[s] for s in shape]
         except KeyError:
             raise NexusStructureError(
-                f"Could not determine axis indices for {self.name}/{name}")
+                f"Could not determine axis indices for {self.name}/{name}"
+            )
         return dims
 
     def _try_guess_dims(self, name):
         try:
             return self._guess_dims(name)
         except NexusStructureError:
             return None
@@ -182,26 +192,27 @@
     def _get_field_dims(self, name: str) -> Union[None, List[str]]:
         # Newly written files should always contain indices attributes, but the
         # standard recommends that readers should also make "best effort" guess
         # since legacy files do not set this attribute.
         if (indices := self.attrs.get(f'{name}_indices')) is not None:
             return list(np.array(self.dims)[np.array(indices).flatten()])
         if (axis := self._get_child(name).attrs.get('axis')) is not None:
-            return (self._get_group_dims()[axis - 1], )
+            return (self._get_group_dims()[axis - 1],)
         if name in [self._signal_name, self._errors_name]:
             return self._get_group_dims()  # if None, field determines dims itself
         if name in list(self.attrs.get('auxiliary_signals', [])):
             return self._try_guess_dims(name)
         if name in self._get_axes():
             # If there are named axes then items of same name are "dimension
             # coordinates", i.e., have a dim matching their name.
             # However, if the item is not 1-D we need more labels. Try to use labels of
             # signal if dimensionality matches.
             if self._signal_name in self and self._get_child(name).ndim == len(
-                    self.shape):
+                self.shape
+            ):
                 return self[self._signal_name].dims
             return [name]
         return self._try_guess_dims(name)
 
     def _bin_edge_dim(self, coord: Field) -> Union[None, str]:
         sizes = dict(zip(self.dims, self.shape))
         for dim, size in zip(coord.dims, coord.shape):
@@ -222,53 +233,64 @@
             return False
         if dim_of_coord not in da.dims:
             return True
         return False
 
     def _getitem(self, select: ScippIndex) -> sc.DataArray:
         from .nexus_classes import NXgeometry
+
         signal = self._signal
         if signal is None:
             raise NexusStructureError("No signal field found, cannot load group.")
         signal = signal[select]
         if self._errors_name is not None:
             stddevs = self[self._errors_name][select]
             # According to the standard, errors must have the same shape as the data.
             # This is not the case in all files we observed, is there any harm in
             # attempting a broadcast?
-            signal.variances = np.broadcast_to(sc.pow(stddevs, sc.scalar(2)).values,
-                                               shape=signal.shape)
-
-        da = sc.DataArray(data=signal) if isinstance(signal, sc.Variable) else signal
+            signal.variances = np.broadcast_to(
+                sc.pow(stddevs, sc.scalar(2)).values, shape=signal.shape
+            )
+
+        da = (
+            signal
+            if isinstance(signal, sc.DataArray)
+            else sc.DataArray(data=asarray(signal))
+        )
 
         skip = self._skip
         skip += [self._signal_name, self._errors_name]
         skip += list(self.attrs.get('auxiliary_signals', []))
         for name in self:
             if (errors := self._strategy.coord_errors(self, name)) is not None:
                 skip += [errors]
         for name in self:
             if name in skip:
                 continue
             # It is not entirely clear whether skipping NXtransformations is the right
             # solution. In principle NXobject will load them via the 'depends_on'
             # mechanism, so for valid files this should be sufficient.
-            allowed = (Field, NXtransformations, NXcylindrical_geometry, NXoff_geometry,
-                       NXgeometry)
+            allowed = (
+                Field,
+                NXtransformations,
+                NXcylindrical_geometry,
+                NXoff_geometry,
+                NXgeometry,
+            )
             if not isinstance(self._get_child(name), allowed):
                 raise NexusStructureError(
-                    "Invalid NXdata: may not contain nested groups")
+                    "Invalid NXdata: may not contain nested groups"
+                )
 
         for name, field in self[Field].items():
             if name in skip:
                 continue
-            sel = to_child_select(self.dims,
-                                  field.dims,
-                                  select,
-                                  bin_edge_dim=self._bin_edge_dim(field))
+            sel = to_child_select(
+                self.dims, field.dims, select, bin_edge_dim=self._bin_edge_dim(field)
+            )
             coord: sc.Variable = asarray(self[name][sel])
             if (error_name := self._strategy.coord_errors(self, name)) is not None:
                 stddevs = asarray(self[error_name][sel])
                 coord.variances = sc.pow(stddevs, sc.scalar(2)).values
             try:
                 if self._coord_to_attr(da, name, field):
                     # Like scipp, slicing turns coord into attr if slicing removes the
```

### Comparing `scippnexus-23.5.0/src/scippnexus/nxdetector.py` & `scippnexus-23.5.1/src/scippnexus/nxdetector.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     ScippIndex,
     asarray,
     is_dataset,
 )
 
 
 class NXdetectorStrategy(NXdataStrategy):
-
     @staticmethod
     def signal(group):
         # NXdata uses the 'signal' attribute to define the field name of the signal.
         # NXdetector uses a "hard-coded" signal name 'data', without specifying the
         # attribute in the file, so we pass this explicitly to NXdata.
         # Note the special case of an NXevent_data subgroup named 'data', which we
         # avoid by checking if 'data' is a dataset.
@@ -38,16 +37,15 @@
     if hasattr(da, 'group'):
         return da.group(groups)
     else:
         return sc.bin(da, groups=[groups])
 
 
 class EventSelector:
-    """A proxy object for creating an NXdetector based on a selection of events.
-    """
+    """A proxy object for creating an NXdetector based on a selection of events."""
 
     def __init__(self, detector):
         self._detector = detector
 
     def __getitem__(self, select: ScippIndex) -> NXdetector:
         """Return an NXdetector based on a selection (slice) of events."""
         det = copy(self._detector)
@@ -58,19 +56,21 @@
 class _EventField:
     """Field-like wrapper of NXevent_data binned into pixels.
 
     This has no equivalent in the NeXus format, but represents the conceptual
     event-data "signal" dataset of an NXdetector.
     """
 
-    def __init__(self,
-                 nxevent_data: NXevent_data,
-                 event_select: ScippIndex,
-                 grouping_key: Optional[str] = 'detector_number',
-                 grouping: Optional[Field] = None):
+    def __init__(
+        self,
+        nxevent_data: NXevent_data,
+        event_select: ScippIndex,
+        grouping_key: Optional[str] = 'detector_number',
+        grouping: Optional[Field] = None,
+    ):
         self._nxevent_data = nxevent_data
         self._event_select = event_select
         self._grouping_key = grouping_key
         self._grouping = grouping
 
     @property
     def name(self) -> str:
@@ -87,15 +87,16 @@
         return self._grouping.dims
 
     @property
     def shape(self):
         if self._grouping is None:
             raise NexusStructureError(
                 "Cannot get shape of NXdetector since no 'detector_number' "
-                "field found but detector contains event data.")
+                "field found but detector contains event data."
+            )
         return self._grouping.shape
 
     @property
     def unit(self) -> None:
         return self._nxevent_data.unit
 
     def __getitem__(self, select: ScippIndex) -> sc.DataArray:
@@ -103,35 +104,40 @@
         if isinstance(event_data, sc.DataGroup):
             raise NexusStructureError("Invalid NXevent_data in NXdetector.")
         if self._grouping is None:
             if select not in (Ellipsis, tuple(), slice(None)):
                 raise NexusStructureError(
                     "Cannot load slice of NXdetector since it contains event data "
                     "but no 'detector_number' field, i.e., the shape is unknown. "
-                    "Use ellipsis or an empty tuple to load the full detector.")
+                    "Use ellipsis or an empty tuple to load the full detector."
+                )
             # Ideally we would prefer to use np.unique, but a quick experiment shows
             # that this can easily be 100x slower, so it is not an option. In
             # practice most files have contiguous event_id values within a bank
             # (NXevent_data).
             id_min = event_data.bins.coords['event_id'].min()
             id_max = event_data.bins.coords['event_id'].max()
-            grouping = sc.arange(dim=self._grouping_key,
-                                 unit=None,
-                                 start=id_min.value,
-                                 stop=id_max.value + 1,
-                                 dtype=id_min.dtype)
+            grouping = sc.arange(
+                dim=self._grouping_key,
+                unit=None,
+                start=id_min.value,
+                stop=id_max.value + 1,
+                dtype=id_min.dtype,
+            )
         else:
             grouping = asarray(self._grouping[select])
             if (self._grouping_key in event_data.coords) and sc.identical(
-                    grouping, event_data.coords[self._grouping_key]):
+                grouping, event_data.coords[self._grouping_key]
+            ):
                 return event_data
         # copy since sc.bin cannot deal with a non-contiguous view
         event_id = grouping.flatten(to='event_id').copy()
         event_data.bins.coords['event_time_zero'] = sc.bins_like(
-            event_data, fill_value=event_data.coords['event_time_zero'])
+            event_data, fill_value=event_data.coords['event_time_zero']
+        )
         # After loading raw NXevent_data it is guaranteed that the event table
         # is contiguous and that there is no masking. We can therefore use the
         # more efficient approach of binning from scratch instead of erasing the
         # 'pulse' binning defined by NXevent_data.
         event_data = group(event_data.bins.constituents['data'], groups=event_id)
         if self._grouping is None:
             event_data.coords[self._grouping_key] = event_data.coords.pop('event_id')
@@ -148,16 +154,21 @@
     same format as NXevent_data.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._event_select = tuple()
         self._nxevent_data_fields = [
-            'event_time_zero', 'event_index', 'event_time_offset', 'event_id',
-            'cue_timestamp_zero', 'cue_index', 'pulse_height'
+            'event_time_zero',
+            'event_index',
+            'event_time_offset',
+            'event_id',
+            'cue_timestamp_zero',
+            'cue_index',
+            'pulse_height',
         ]
         self._detector_number_fields = ['detector_number', 'pixel_id', 'spectrum_index']
 
     @property
     def shape(self) -> List[int]:
         return self._signal.shape
 
@@ -195,29 +206,30 @@
             signal = None
         skip = None
         if events is not None:
             if events.name == self.name:
                 skip = self._nxevent_data_fields
             else:
                 skip = [events.name.split('/')[-1]]  # name of the subgroup
-        return NXdata(self._group,
-                      strategy=NXdetectorStrategy,
-                      signal_override=signal,
-                      skip=skip)
+        return NXdata(
+            self._group, strategy=NXdetectorStrategy, signal_override=signal, skip=skip
+        )
 
     @property
     def events(self) -> Union[None, NXevent_data]:
         """Return the underlying NXevent_data group, None if not event data."""
         # The standard is unclear on whether the 'data' field may be NXevent_data or
         # whether the fields of NXevent_data should be stored directly within this
         # NXdetector. Both cases are observed in the wild.
         event_entries = self[NXevent_data]
         if len(event_entries) > 1:
-            raise NexusStructureError("No unique NXevent_data entry in NXdetector. "
-                                      f"Found {len(event_entries)}.")
+            raise NexusStructureError(
+                "No unique NXevent_data entry in NXdetector. "
+                f"Found {len(event_entries)}."
+            )
         if len(event_entries) == 1:
             # If there is also a signal dataset (not events) it will be ignored
             # (except for possibly using it to deduce shape and dims).
             return next(iter(event_entries.values()))
         if 'event_time_offset' in self:
             return NXevent_data(self._group)
         return None
@@ -226,15 +238,16 @@
     def select_events(self) -> EventSelector:
         """
         Return a proxy object for selecting a slice of the underlying NXevent_data
         group, while keeping wrapping the NXdetector.
         """
         if self.events is None:
             raise NexusStructureError(
-                "Cannot select events in NXdetector not containing NXevent_data.")
+                "Cannot select events in NXdetector not containing NXevent_data."
+            )
         return EventSelector(self)
 
     def _get_field_dims(self, name: str) -> Union[None, List[str]]:
         if self.events is not None:
             if name in self._nxevent_data_fields:
                 # Event field is direct child of this class
                 return self.events._get_field_dims(name)
```

### Comparing `scippnexus-23.5.0/src/scippnexus/nxevent_data.py` & `scippnexus-23.5.1/src/scippnexus/nxevent_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from .nxobject import NexusStructureError, NXobject, ScippIndex
 
 _event_dimension = "event"
 _pulse_dimension = "pulse"
 
 
 class NXevent_data(NXobject):
-
     @property
     def shape(self) -> List[int]:
         return self['event_index'].shape
 
     @property
     def dims(self) -> List[str]:
         return [_pulse_dimension]
@@ -63,50 +62,54 @@
 
         num_event = self["event_time_offset"].shape[0]
         # Some files contain uint64 "max" indices, which turn into negatives during
         # conversion to int64. This is a hack to get around this.
         event_index[event_index < 0] = num_event
 
         if len(event_index) > 0:
-            event_select = slice(event_index[0],
-                                 event_index[-1] if last_loaded else num_event)
+            event_select = slice(
+                event_index[0], event_index[-1] if last_loaded else num_event
+            )
         else:
             event_select = slice(None)
 
         if (event_id := self.get('event_id')) is not None:
             event_id = event_id[event_select]
             if event_id.dtype not in [sc.DType.int32, sc.DType.int64]:
                 raise NexusStructureError(
-                    "NXevent_data contains event_id field with non-integer values")
+                    "NXevent_data contains event_id field with non-integer values"
+                )
 
         event_time_offset = self['event_time_offset'][event_select]
 
         # Weights are not stored in NeXus, so use 1s
-        weights = sc.ones(dims=[_event_dimension],
-                          shape=event_time_offset.shape,
-                          unit='counts',
-                          dtype=np.float32)
-
-        events = sc.DataArray(data=weights,
-                              coords={'event_time_offset': event_time_offset})
+        weights = sc.ones(
+            dims=[_event_dimension],
+            shape=event_time_offset.shape,
+            unit='counts',
+            dtype=np.float32,
+        )
+
+        events = sc.DataArray(
+            data=weights, coords={'event_time_offset': event_time_offset}
+        )
         if event_id is not None:
             events.coords['event_id'] = event_id
 
         if not last_loaded:
             event_index = np.append(event_index, num_event)
         else:
             # Not a bin-edge coord, all events in bin are associated with same
             # (previous) pulse time value
             # Copy to avoid confusing size display in _repr_html_
             event_time_zero = event_time_zero[:-1].copy()
 
-        event_index = sc.array(dims=[_pulse_dimension],
-                               values=event_index,
-                               dtype=sc.DType.int64,
-                               unit=None)
+        event_index = sc.array(
+            dims=[_pulse_dimension], values=event_index, dtype=sc.DType.int64, unit=None
+        )
 
         event_index -= event_index.min()
 
         # There is some variation in the last recorded event_index in files from
         # different institutions. We try to make sure here that it is what would be the
         # first index of the next pulse. In other words, ensure that event_index
         # includes the bin edge for the last pulse.
@@ -118,16 +121,18 @@
             begins = event_index[_pulse_dimension, :-1]
             ends = event_index[_pulse_dimension, 1:]
 
         try:
             binned = sc.bins(data=events, dim=_event_dimension, begin=begins, end=ends)
         except IndexError as e:
             raise NexusStructureError(
-                f"Invalid index in NXevent_data at {self.name}/event_index:\n{e}.")
+                f"Invalid index in NXevent_data at {self.name}/event_index:\n{e}."
+            )
 
         return sc.DataArray(data=binned, coords={'event_time_zero': event_time_zero})
 
     def _check_for_missing_fields(self):
         for field in ("event_time_zero", "event_index", "event_time_offset"):
             if field not in self:
                 raise NexusStructureError(
-                    f"Required field {field} not found in NXevent_data")
+                    f"Required field {field} not found in NXevent_data"
+                )
```

### Comparing `scippnexus-23.5.0/src/scippnexus/nxlog.py` & `scippnexus-23.5.1/src/scippnexus/nxlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import scipp as sc
 
 from .nxdata import NXdata, NXdataStrategy
 from .nxobject import NXobject, ScippIndex
 
 
 class NXlogStrategy(NXdataStrategy):
-
     @staticmethod
     def axes(group):
         if (ax := NXdataStrategy.axes(group)) is not None:
             return ax
         # We get the shape from the original dataset, to make sure we do not squeeze
         # dimensions too early
         child_dataset = group._get_child('value')._dataset
@@ -39,32 +38,33 @@
         # NXdata uses the 'signal' attribute to define the field name of the signal.
         # NXlog uses a "hard-coded" signal name 'value', without specifying the
         # attribute in the file, so we pass this explicitly to NXdata.
         return group.attrs.get('signal', 'value')
 
 
 class NXlog(NXobject):
-
     @property
     def shape(self):
         return self._nxbase.shape
 
     @property
     def dims(self):
         return self._nxbase.dims
 
     @property
     def unit(self):
         return self._nxbase.unit
 
     @property
     def _nxbase(self) -> NXdata:
-        return NXdata(self._group,
-                      strategy=NXlogStrategy,
-                      skip=['cue_timestamp_zero', 'cue_index'])
+        return NXdata(
+            self._group,
+            strategy=NXlogStrategy,
+            skip=['cue_timestamp_zero', 'cue_index'],
+        )
 
     def _getitem(self, select: ScippIndex) -> sc.DataArray:
         base = self._nxbase
         # Field loads datetime offset attributes automatically, but for NXlog this
         # may apparently be omitted and must then interpreted as relative to epoch.
         base.child_params['time'] = {'is_time': True}
         return base[select]
```

### Comparing `scippnexus-23.5.0/src/scippnexus/nxmonitor.py` & `scippnexus-23.5.1/src/scippnexus/nxmonitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 from typing import Dict, Union
 
 from .nxdetector import NXdetector
 from .nxobject import Field
 
 
 class NXmonitor(NXdetector):
-
     @property
     def _event_grouping(self) -> Dict[str, Union[str, Field]]:
         # Unlike NXdetector, NXmonitor does not group by 'detector_number'. We pass
         # grouping information that matches the underlying binning of NXevent_data
         # such that no addition binning will need to be performed. That is, the by-pulse
         # binning present in the file (in NXevent_data) is preserved.
         return {
             'grouping_key': 'event_time_zero',
-            'grouping': self.events.get('event_time_zero')
+            'grouping': self.events.get('event_time_zero'),
         }
```

### Comparing `scippnexus-23.5.0/src/scippnexus/nxobject.py` & `scippnexus-23.5.1/src/scippnexus/nxobject.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,28 +49,26 @@
 
     @property
     def dims(self) -> List[str]:
         """Dimension labels for the values"""
 
 
 class AttributeManager(Protocol):
-
     def __getitem__(self, name: str):
         """Get attribute"""
 
 
 class NexusStructureError(Exception):
-    """Invalid or unsupported class and field structure in Nexus.
-    """
+    """Invalid or unsupported class and field structure in Nexus."""
+
     pass
 
 
 class Attrs:
-    """HDF5 attributes.
-    """
+    """HDF5 attributes."""
 
     def __init__(self, attrs: AttributeManager):
         self._attrs = attrs
 
     def __contains__(self, name: str) -> bool:
         return name in self._attrs
 
@@ -148,21 +146,23 @@
 
 class Field:
     """NeXus field.
 
     In HDF5 fields are represented as dataset.
     """
 
-    def __init__(self,
-                 dataset: H5Dataset,
-                 *,
-                 ancestor,
-                 dims=None,
-                 dtype: Optional[sc.DType] = None,
-                 is_time=None):
+    def __init__(
+        self,
+        dataset: H5Dataset,
+        *,
+        ancestor,
+        dims=None,
+        dtype: Optional[sc.DType] = None,
+        is_time=None,
+    ):
         self._ancestor = ancestor  # Usually the parent, but may be grandparent, etc.
         self._dataset = dataset
         self._dtype = _dtype_from_dataset(dataset) if dtype is None else dtype
         self._shape = self._dataset.shape
         if self._dtype == sc.DType.vector3:
             self._shape = self._shape[:-1]
         self._is_time = is_time
@@ -172,31 +172,36 @@
         # the same as the shape of the underlying dataset.
         if dims is not None:
             self._dims = tuple(dims)
             if len(self._dims) < len(self._shape):
                 # The convention here is that the given dimensions apply to the shapes
                 # starting from the left. So we only squeeze dimensions that are after
                 # len(dims).
-                self._shape = self._shape[:len(self._dims)] + tuple(
-                    size for size in self._shape[len(self._dims):] if size != 1)
+                self._shape = self._shape[: len(self._dims)] + tuple(
+                    size for size in self._shape[len(self._dims) :] if size != 1
+                )
         elif (axes := self.attrs.get('axes')) is not None:
-            self._dims = tuple(axes.split(','))
+            self._dims = tuple(axes.split(':'))
+            # The standard says that the axes should be colon-separated, but some
+            # files use comma-separated.
+            if len(self._dims) == 1 and self._dataset.ndim > 1:
+                self._dims = tuple(axes.split(','))
         else:
             self._shape = tuple(size for size in self._shape if size != 1)
             self._dims = tuple(f'dim_{i}' for i in range(self.ndim))
 
     def __getitem__(self, select) -> Union[Any, sc.Variable]:
         """Load the field as a :py:class:`scipp.Variable` or Python object.
 
         If the shape is empty and no unit is given this returns a Python object, such
         as a string or integer. Otherwise a :py:class:`scipp.Variable` is returned.
         """
         index = to_plain_index(self.dims, select)
         if isinstance(index, (int, slice)):
-            index = (index, )
+            index = (index,)
 
         base_dims = self.dims
         base_shape = self.shape
         dims = []
         shape = []
         for i, ind in enumerate(index):
             if not isinstance(ind, int):
@@ -239,15 +244,16 @@
                     starts.append(dt)
             if self._is_time and len(starts) == 0:
                 starts.append(sc.epoch(unit=self.unit))
             if len(starts) == 1:
                 variable = convert_time_to_datetime64(
                     variable,
                     start=starts[0],
-                    scaling_factor=self.attrs.get('scaling_factor'))
+                    scaling_factor=self.attrs.get('scaling_factor'),
+                )
         if variable.ndim == 0 and variable.unit is None:
             # Work around scipp/scipp#2815, and avoid returning NumPy bool
             if isinstance(variable.values, np.ndarray) and variable.dtype != 'bool':
                 return variable.values[()]
             else:
                 return variable.value
         return variable
@@ -305,46 +311,48 @@
 
     @property
     def unit(self) -> Union[sc.Unit, None]:
         if (unit := self.attrs.get('units')) is not None:
             try:
                 return sc.Unit(unit)
             except sc.UnitError:
-                warnings.warn(f"Unrecognized unit '{unit}' for value dataset "
-                              f"in '{self.name}'; setting unit as 'dimensionless'")
+                warnings.warn(
+                    f"Unrecognized unit '{unit}' for value dataset "
+                    f"in '{self.name}'; setting unit as 'dimensionless'"
+                )
                 return sc.units.one
         return None
 
 
 def is_dataset(obj: Union[H5Group, H5Dataset]) -> bool:
     """Return true if the object is an h5py.Dataset or equivalent.
 
     Use this instead of isinstance(obj, h5py.Dataset) to ensure that code is compatible
     with other h5py-alike interfaces.
     """
     return hasattr(obj, 'shape')
 
 
 class NXobjectStrategy:
-
     @staticmethod
     def include_child(_) -> bool:
         """Return True if the child should be included when loading."""
         return True
 
 
 class NXobject:
-    """Base class for all NeXus groups.
-    """
+    """Base class for all NeXus groups."""
 
-    def __init__(self,
-                 group: H5Group,
-                 *,
-                 definition: Any = None,
-                 strategy: Optional[Callable] = None):
+    def __init__(
+        self,
+        group: H5Group,
+        *,
+        definition: Any = None,
+        strategy: Optional[Callable] = None,
+    ):
         self._group = group
         # TODO can strategies replace child-params?
         self.child_params = {}
         self._definition = definition
         self._strategy = strategy
         if strategy is None and self._definition is not None:
             self._strategy = self._definition.make_strategy(self)
@@ -356,70 +364,75 @@
         Default strategy to use when none given and when the application definition
         does not provide one. Override in child classes to set a default.
         """
         return NXobjectStrategy
 
     def _make(self, group) -> NXobject:
         if (nx_class := Attrs(group.attrs).get('NX_class')) is not None:
-            return _nx_class_registry().get(nx_class,
-                                            NXobject)(group,
-                                                      definition=self._definition)
+            return _nx_class_registry().get(nx_class, NXobject)(
+                group, definition=self._definition
+            )
         return group  # Return underlying (h5py) group
 
     def _get_child(
-            self,
-            name: NXobjectIndex,
-            use_field_dims: bool = False) -> Union['NXobject', Field, sc.DataArray]:
+        self, name: NXobjectIndex, use_field_dims: bool = False
+    ) -> Union['NXobject', Field, sc.DataArray]:
         """Get item, with flag to control whether fields dims should be inferred"""
         if name is None:
             raise KeyError("None is not a valid index")
         if isinstance(name, str):
             item = self._group[name]
             if is_dataset(item):
                 try:
                     dims = self._get_field_dims(name) if use_field_dims else None
                 except Exception as e:
-                    msg = (f"Failed to determine axis names of {item.name}: {e}. "
-                           "Falling back to default dimension labels.")
+                    msg = (
+                        f"Failed to determine axis names of {item.name}: {e}. "
+                        "Falling back to default dimension labels."
+                    )
                     warnings.warn(msg)
                     dims = None
                 dtype = self._get_field_dtype(name)
-                return Field(item,
-                             dims=dims,
-                             dtype=dtype,
-                             ancestor=self,
-                             **self.child_params.get(name, {}))
+                return Field(
+                    item,
+                    dims=dims,
+                    dtype=dtype,
+                    ancestor=self,
+                    **self.child_params.get(name, {}),
+                )
             else:
                 return self._make(item)
 
         try:
             da = self._getitem(name)
             self._insert_leaf_properties(da)
         except NexusStructureError as e:
             # If the child class cannot load this group, we fall back to returning the
             # underlying datasets in a DataGroup.
             if type(self)._getitem == NXobject._getitem:
                 raise
             else:
                 msg = (
                     f"Failed to load {self.name} as {type(self).__name__}: {e} "
-                    "Falling back to loading HDF5 group children as scipp.DataGroup.")
+                    "Falling back to loading HDF5 group children as scipp.DataGroup."
+                )
                 warnings.warn(msg)
             da = NXobject._getitem(self, name)
         return da
 
     def _insert_leaf_properties(self, container):
         from .nexus_classes import NXgeometry
         from .nxcylindrical_geometry import NXcylindrical_geometry
         from .nxoff_geometry import NXoff_geometry
 
         def insert(container, name, obj):
             if hasattr(container, 'coords'):
-                container.coords[name] = obj if isinstance(
-                    obj, sc.Variable) else sc.scalar(obj)
+                container.coords[name] = (
+                    obj if isinstance(obj, sc.Variable) else sc.scalar(obj)
+                )
             else:
                 container[name] = obj
 
         detector_number = getattr(self, 'detector_number', None)
         if detector_number is not None:
             detector_number = container.coords[detector_number]
         for key, child in self[[NXcylindrical_geometry, NXoff_geometry]].items():
@@ -430,20 +443,21 @@
             insert(container, 'depends_on', t)
             # If loading the transformation failed, 'depends_on' returns a string, the
             # path to the transformation. If this is a nested group, we load it here.
             # Note that this info is currently incomplete, since attributes are not
             # loaded.
             if isinstance(t, str):
                 from .nexus_classes import NXtransformations
+
                 for key, group in self[NXtransformations].items():
                     insert(container, key, group[()])
 
     def _get_children_by_nx_class(
-            self, select: Union[type,
-                                List[type]]) -> Dict[str, Union['NXobject', Field]]:
+        self, select: Union[type, List[type]]
+    ) -> Dict[str, Union['NXobject', Field]]:
         children = {}
         select = tuple(select) if isinstance(select, list) else select
         for key in self.keys():
             if issubclass(type(self._get_child(key)), select):
                 # Get child again via __getitem__ so correct field dims are used.
                 children[key] = self[key]
         return children
@@ -485,24 +499,25 @@
         :
             Field, group, dict of fields, or loaded data.
         """
 
         def isclass(x):
             return inspect.isclass(x) and issubclass(x, (Field, NXobject))
 
-        if isclass(name) or (isinstance(name, list) and len(name)
-                             and all(isclass(x) for x in name)):
+        if isclass(name) or (
+            isinstance(name, list) and len(name) and all(isclass(x) for x in name)
+        ):
             return self._get_children_by_nx_class(name)
         return self._get_child(name, use_field_dims=True)
 
     def _getitem(self, index: ScippIndex) -> Union[sc.DataArray, sc.DataGroup]:
         include = getattr(self._strategy, 'include_child', lambda x: True)
         return sc.DataGroup(
-            {name: child[index]
-             for name, child in self.items() if include(child)})
+            {name: child[index] for name, child in self.items() if include(child)}
+        )
 
     def _get_field_dims(self, name: str) -> Union[None, List[str]]:
         """Subclasses should reimplement this to provide dimension labels for fields."""
         return None
 
     def _get_field_dtype(self, name: str) -> Union[None, sc.DType]:
         """Subclasses should reimplement this to override the dtype for fields."""
@@ -557,20 +572,22 @@
             return _nx_class_registry().get(nxclass)
 
     @property
     def depends_on(self) -> Union[sc.Variable, sc.DataArray, None]:
         if (depends_on := self.get('depends_on')) is not None:
             # Imported late to avoid cyclic import
             from .nxtransformations import TransformationError, get_full_transformation
+
             try:
                 return get_full_transformation(depends_on)
             except (NexusStructureError, TransformationError) as e:
                 warnings.warn(
                     f"Failed to load transformation {self.name}/{depends_on}:\n{e}\n"
-                    "Falling back to returning the path to the transformation.")
+                    "Falling back to returning the path to the transformation."
+                )
                 return depends_on[()]
         return None
 
     def __repr__(self) -> str:
         return f'<{type(self).__name__} "{self._group.name}">'
 
     def create_field(self, name: str, data: DimensionedArray, **kwargs) -> Field:
@@ -622,16 +639,18 @@
         if nxclass is None:
             raise AttributeError(f"'NXobject' object has no attribute {attr}")
         matches = self[nxclass]
         if len(matches) == 0:
             raise NexusStructureError(f"No group with requested NX_class='{nxclass}'")
         if len(matches) == 1:
             return next(iter(matches.values()))
-        raise NexusStructureError(f"Multiple keys match {nxclass}, use obj[{nxclass}] "
-                                  f"to obtain all matches instead of obj.{attr}.")
+        raise NexusStructureError(
+            f"Multiple keys match {nxclass}, use obj[{nxclass}] "
+            f"to obtain all matches instead of obj.{attr}."
+        )
 
     def __dir__(self):
         keys = super().__dir__()
         nxclasses = []
         # Avoiding self.values() since it is more costly, but mainly since there may be
         # edge cases where creation of Field/NXobject may raise on unrelated children.
         for _, val in self._group.items():
@@ -658,8 +677,9 @@
         # that were inspired by the reference implementation. We thus hardcode NXroot:
         return NXroot
 
 
 @functools.lru_cache()
 def _nx_class_registry():
     from . import nexus_classes
+
     return dict(inspect.getmembers(nexus_classes, inspect.isclass))
```

### Comparing `scippnexus-23.5.0/src/scippnexus/nxoff_geometry.py` & `scippnexus-23.5.1/src/scippnexus/nxoff_geometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from typing import Optional, Tuple, Union
 
 import scipp as sc
 
 from .nxobject import NexusStructureError, NXobject
 
 
-def off_to_shape(*,
-                 vertices: sc.Variable,
-                 winding_order: sc.Variable,
-                 faces: sc.Variable,
-                 detector_faces: Optional[sc.Variable] = None,
-                 detector_number: Optional[sc.Variable] = None) -> sc.Variable:
+def off_to_shape(
+    *,
+    vertices: sc.Variable,
+    winding_order: sc.Variable,
+    faces: sc.Variable,
+    detector_faces: Optional[sc.Variable] = None,
+    detector_number: Optional[sc.Variable] = None
+) -> sc.Variable:
     """
     Convert OFF shape description to simpler shape representation.
     """
     # Vertices in winding order. This duplicates vertices if they are part of more than
     # one faces.
     vw = vertices[winding_order.values]
     # Same as above, grouped by face.
@@ -26,43 +28,48 @@
     high = fvw.bins.size().max().value
     if low == high:
         # Vertices in winding order, groupbed by face. Unlike `fvw` above we now know
         # that each face has the same number of vertices, so we can fold instead of
         # using binned data.
         shapes = vw.fold(dim=vertices.dim, sizes={faces.dim: -1, vertices.dim: low})
     else:
-        raise NotImplementedError("Conversion from OFF to shape not implemented for "
-                                  "inconsistent number of vertices in faces.")
+        raise NotImplementedError(
+            "Conversion from OFF to shape not implemented for "
+            "inconsistent number of vertices in faces."
+        )
     if detector_faces is None:  # if detector_number is not None, all have same shape
         return sc.bins(begin=sc.index(0), dim=faces.dim, data=shapes)
     if detector_number is None:
-        raise NexusStructureError("`detector_number` not given but NXoff_geometry "
-                                  "contains `detector_faces`.")
+        raise NexusStructureError(
+            "`detector_number` not given but NXoff_geometry "
+            "contains `detector_faces`."
+        )
     shape_index = detector_faces['column', 0].copy()
     detid = detector_faces['column', 1].copy()
-    da = sc.DataArray(shape_index, coords={
-        'detector_number': detid
-    }).group(detector_number.flatten(to='detector_number'))
+    da = sc.DataArray(shape_index, coords={'detector_number': detid}).group(
+        detector_number.flatten(to='detector_number')
+    )
     comps = da.bins.constituents
     comps['data'] = shapes[faces.dim, comps['data'].values]
     return sc.bins(**comps).fold(dim='detector_number', sizes=detector_number.sizes)
 
 
 class NXoff_geometry(NXobject):
     _dims = {
         'detector_faces': ('face', 'column'),
-        'vertices': ('vertex', ),
-        'winding_order': ('winding_order', ),
-        'faces': ('face', )
+        'vertices': ('vertex',),
+        'winding_order': ('winding_order',),
+        'faces': ('face',),
     }
 
     def _get_field_dims(self, name: str) -> Union[None, Tuple[str]]:
         return self._dims.get(name)
 
     def _get_field_dtype(self, name: str) -> Union[None, sc.DType]:
         if name == 'vertices':
             return sc.DType.vector3
         return None
 
-    def load_as_array(self,
-                      detector_number: Optional[sc.Variable] = None) -> sc.Variable:
+    def load_as_array(
+        self, detector_number: Optional[sc.Variable] = None
+    ) -> sc.Variable:
         return off_to_shape(**self[()], detector_number=detector_number)
```

### Comparing `scippnexus-23.5.0/src/scippnexus/nxsample.py` & `scippnexus-23.5.1/src/scippnexus/nxsample.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 from .leaf import Leaf
 from .nxobject import ScippIndex
 
 _matrix_units = dict(zip(['orientation_matrix', 'ub_matrix'], ['one', '1/Angstrom']))
 
 
 class NXsample(Leaf):
-    """Sample information, can be read as a dict.
-    """
+    """Sample information, can be read as a dict."""
 
-    def _getitem(self,
-                 select: ScippIndex) -> Dict[str, Union[sc.Variable, sc.DataArray]]:
+    def _getitem(
+        self, select: ScippIndex
+    ) -> Dict[str, Union[sc.Variable, sc.DataArray]]:
         content = super()._getitem(select)
         for key in _matrix_units:
             if (item := content.get(key)) is not None:
-                content[key] = linear_transform(value=item.values,
-                                                unit=_matrix_units[key])
+                content[key] = linear_transform(
+                    value=item.values, unit=_matrix_units[key]
+                )
         return content
```

### Comparing `scippnexus-23.5.0/src/scippnexus/nxtransformations.py` & `scippnexus-23.5.1/src/scippnexus/nxtransformations.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,23 +24,25 @@
     return None  # end of chain
 
 
 class NXtransformations(NXobject):
     """Group of transformations."""
 
     def _getitem(self, index: ScippIndex) -> sc.DataGroup:
-        return sc.DataGroup({
-            name: get_full_transformation_starting_at(Transformation(child),
-                                                      index=index)
-            for name, child in self.items()
-        })
+        return sc.DataGroup(
+            {
+                name: get_full_transformation_starting_at(
+                    Transformation(child), index=index
+                )
+                for name, child in self.items()
+            }
+        )
 
 
 class Transformation:
-
     def __init__(self, obj: Union[Field, NXobject]):  # could be an NXlog
         self._obj = obj
 
     @property
     def attrs(self):
         return self._obj.attrs
 
@@ -57,15 +59,16 @@
     @property
     def offset(self):
         if (offset := self.attrs.get('offset')) is None:
             return None
         if (offset_units := self.attrs.get('offset_units')) is None:
             raise TransformationError(
                 f"Found {offset=} but no corresponding 'offset_units' "
-                f"attribute at {self.name}")
+                f"attribute at {self.name}"
+            )
         return sc.spatial.translation(value=offset, unit=offset_units)
 
     @property
     def vector(self) -> sc.Variable:
         return sc.vector(value=self.attrs.get('vector'))
 
     def __getitem__(self, select: ScippIndex):
@@ -73,107 +76,116 @@
         # According to private communication with Tobias Richter, NeXus allows 0-D or
         # shape=[1] for single values. It is unclear how and if this could be
         # distinguished from a scan of length 1.
         value = self._obj[select]
         try:
             if isinstance(value, sc.DataGroup):
                 raise TransformationError(
-                    f"Failed to load transformation at {self.name}.")
+                    f"Failed to load transformation at {self.name}."
+                )
             t = value * self.vector
             v = t if isinstance(t, sc.Variable) else t.data
             if transformation_type == 'translation':
                 v = v.to(unit='m', copy=False)
                 v = sc.spatial.translations(dims=v.dims, values=v.values, unit=v.unit)
             elif transformation_type == 'rotation':
                 v = sc.spatial.rotations_from_rotvecs(v)
             else:
                 raise TransformationError(
                     f"{transformation_type=} attribute at {self.name},"
-                    " expected 'translation' or 'rotation'.")
+                    " expected 'translation' or 'rotation'."
+                )
             if isinstance(t, sc.Variable):
                 t = v
             else:
                 t.data = v
             if (offset := self.offset) is None:
                 return t
             offset = sc.vector(value=offset.values, unit=offset.unit).to(unit='m')
             offset = sc.spatial.translation(value=offset.value, unit=offset.unit)
             return t * offset
         except (sc.DimensionError, sc.UnitError) as e:
             raise NexusStructureError(
-                f"Invalid transformation in NXtransformations: {e}") from e
+                f"Invalid transformation in NXtransformations: {e}"
+            ) from e
 
 
 def _interpolate_transform(transform, xnew):
     # scipy can't interpolate with a single value
     if transform.sizes["time"] == 1:
         transform = sc.concat([transform, transform], dim="time")
-    return interpolate.interp1d(transform,
-                                "time",
-                                kind="previous",
-                                fill_value="extrapolate")(xnew=xnew)
+    return interpolate.interp1d(
+        transform, "time", kind="previous", fill_value="extrapolate"
+    )(xnew=xnew)
 
 
 def _smaller_unit(a, b):
     if a.unit == b.unit:
         return a.unit
     ratio = sc.scalar(1.0, unit=a.unit).to(unit=b.unit)
     if ratio.value < 1.0:
         return a.unit
     else:
         return b.unit
 
 
 def get_full_transformation(
-        depends_on: Field) -> Union[None, sc.DataArray, sc.Variable]:
+    depends_on: Field,
+) -> Union[None, sc.DataArray, sc.Variable]:
     """
     Get the 4x4 transformation matrix for a component, resulting
     from the full chain of transformations linked by "depends_on"
     attributes
     """
     if (t0 := make_transformation(depends_on, depends_on[()])) is None:
         return None
     return get_full_transformation_starting_at(t0)
 
 
 def get_full_transformation_starting_at(
-        t0: Transformation,
-        *,
-        index: ScippIndex = None) -> Union[None, sc.DataArray, sc.Variable]:
+    t0: Transformation, *, index: ScippIndex = None
+) -> Union[None, sc.DataArray, sc.Variable]:
     transformations = _get_transformations(t0, index=() if index is None else index)
 
     total_transform = None
     for transform in transformations:
         if total_transform is None:
             total_transform = transform
         elif isinstance(total_transform, sc.DataArray) and isinstance(
-                transform, sc.DataArray):
-            unit = _smaller_unit(transform.coords['time'],
-                                 total_transform.coords['time'])
+            transform, sc.DataArray
+        ):
+            unit = _smaller_unit(
+                transform.coords['time'], total_transform.coords['time']
+            )
             total_transform.coords['time'] = total_transform.coords['time'].to(
-                unit=unit, copy=False)
-            transform.coords['time'] = transform.coords['time'].to(unit=unit,
-                                                                   copy=False)
-            time = sc.concat([total_transform.coords["time"], transform.coords["time"]],
-                             dim="time")
+                unit=unit, copy=False
+            )
+            transform.coords['time'] = transform.coords['time'].to(
+                unit=unit, copy=False
+            )
+            time = sc.concat(
+                [total_transform.coords["time"], transform.coords["time"]], dim="time"
+            )
             time = sc.datetimes(values=np.unique(time.values), dims=["time"], unit=unit)
-            total_transform = _interpolate_transform(transform, time) \
-                * _interpolate_transform(total_transform, time)
+            total_transform = _interpolate_transform(
+                transform, time
+            ) * _interpolate_transform(total_transform, time)
         else:
             total_transform = transform * total_transform
     if isinstance(total_transform, sc.DataArray):
         time_dependent = [t for t in transformations if isinstance(t, sc.DataArray)]
         times = [da.coords['time'][0] for da in time_dependent]
         latest_log_start = sc.reduce(times).max()
         return total_transform['time', latest_log_start:].copy()
     return total_transform
 
 
-def _get_transformations(transform: Transformation, *,
-                         index: ScippIndex) -> List[Union[sc.DataArray, sc.Variable]]:
+def _get_transformations(
+    transform: Transformation, *, index: ScippIndex
+) -> List[Union[sc.DataArray, sc.Variable]]:
     """Get all transformations in the depends_on chain."""
     transformations = []
     t = transform
     while t is not None:
         transformations.append(t[index])
         t = t.depends_on
     # TODO: this list of transformation should probably be cached in the future
```

### Comparing `scippnexus-23.5.0/src/scippnexus/typing.py` & `scippnexus-23.5.1/src/scippnexus/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # @author Simon Heybrock
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Protocol, Tuple, Union
 
 
 class H5Base(Protocol):
-
     @property
     def attrs(self) -> List[int]:
         """Attributes of dataset or group"""
 
     @property
     def name(self) -> str:
         """Name of dataset or group"""
@@ -61,14 +60,21 @@
 
 
 if TYPE_CHECKING:
     from enum import Enum
 
     class ellipsis(Enum):
         Ellipsis = "..."
+
 else:
     ellipsis = type(Ellipsis)
 
 # Note that scipp does not support dicts yet, but this HDF5 code does, to
 # allow for loading blocks of 2d (or higher) data efficiently.
-ScippIndex = Union[ellipsis, int, tuple, slice, Tuple[str, Union[int, slice]],
-                   Dict[str, Union[int, slice]]]
+ScippIndex = Union[
+    ellipsis,
+    int,
+    tuple,
+    slice,
+    Tuple[str, Union[int, slice]],
+    Dict[str, Union[int, slice]],
+]
```

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/__init__.py` & `scippnexus-23.5.1/src/scippnexus/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py` & `scippnexus-23.5.1/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,20 +25,22 @@
         create_field(group, 'title', self.title)
         create_field(group, 'run', self.run)
 
 
 class SASdata:
     nx_class = 'NXdata'
 
-    def __init__(self,
-                 data: sc.DataArray,
-                 Q_variances: Optional[Literal['uncertainties', 'resolutions']] = None):
+    def __init__(
+        self,
+        data: sc.DataArray,
+        Q_variances: Optional[Literal['uncertainties', 'resolutions']] = None,
+    ):
         self.data = data
         valid = ('uncertainties', 'resolutions')
-        if Q_variances not in (None, ) + valid:
+        if Q_variances not in (None,) + valid:
             raise ValueError(f"Q_variances must be in {valid}")
         self._variances = Q_variances
 
     def __write_to_nexus_group__(self, group: H5Group):
         da = self.data
         group.attrs['canSAS_class'] = 'SASdata'
         group.attrs['signal'] = 'I'
@@ -51,36 +53,39 @@
         # NXcanSAS.
         if da.variances is not None:
             signal.attrs['uncertainties'] = 'I_errors'
             create_field(group, 'I_errors', sc.stddevs(da.data))
         if da.coords.is_edges('Q'):
             raise ValueError(
                 "Q is given as bin-edges, but NXcanSAS requires Q points (such as "
-                "bin centers).")
+                "bin centers)."
+            )
         coord = create_field(group, 'Q', da.coords['Q'])
         if da.coords['Q'].variances is not None:
             if self._variances is None:
                 raise ValueError(
                     "Q has variances, must specify whether these represent "
-                    "'uncertainties' or 'resolutions' using the 'Q_variances' option'")
+                    "'uncertainties' or 'resolutions' using the 'Q_variances' option'"
+                )
 
             coord.attrs[self._variances] = 'Q_errors'
             create_field(group, 'Q_errors', sc.stddevs(da.coords['Q']))
 
 
 class _SASdata(NXdata):
-
     def __init__(self, attrs: Dict[str, Any], children: Dict[str, Union[Field, Group]]):
         fallback_dims = attrs.get('I_axes')
         if fallback_dims is not None:
-            fallback_dims = (fallback_dims, )
-        super().__init__(attrs=attrs,
-                         children=children,
-                         fallback_dims=fallback_dims,
-                         fallback_signal_name='I')
+            fallback_dims = (fallback_dims,)
+        super().__init__(
+            attrs=attrs,
+            children=children,
+            fallback_dims=fallback_dims,
+            fallback_signal_name='I',
+        )
 
     # TODO Mechanism for custom error names
     @staticmethod
     def signal_errors(group: NXobject) -> Optional[str]:
         signal_name = group.attrs.get('signal', 'I')
         signal = group._group[signal_name]
         return signal.attrs.get('uncertainties')
@@ -96,29 +101,29 @@
             return resolutions
         elif resolutions is None:
             return uncertainties
         raise RuntimeError("Cannot handle both uncertainties and resolutions for Q")
 
 
 class _SAStransmission_spectrum(NXdata):
-
     def __init__(self, attrs: Dict[str, Any], children: Dict[str, Union[Field, Group]]):
         # TODO A valid file should have T_axes, do we need to fallback?
-        super().__init__(attrs=attrs,
-                         children=children,
-                         fallback_dims=(attrs.get('T_axes', 'lambda'), ),
-                         fallback_signal_name='T')
+        super().__init__(
+            attrs=attrs,
+            children=children,
+            fallback_dims=(attrs.get('T_axes', 'lambda'),),
+            fallback_signal_name='T',
+        )
 
 
 class NXcanSAS:
-
     def get(self, key: type, default: Callable) -> Callable:
-
-        def _definition_factory(attrs: Dict[str, Any],
-                                children: Dict[str, Union[Field, Group]]) -> NXobject:
+        def _definition_factory(
+            attrs: Dict[str, Any], children: Dict[str, Union[Field, Group]]
+        ) -> NXobject:
             if (cls := attrs.get('canSAS_class')) is not None:
                 if cls == 'SASdata':
                     return _SASdata(attrs, children)
                 if cls == 'SAStransmission_spectrum':
                     return _SAStransmission_spectrum(attrs, children)
             return base_definitions().get(key, default)(attrs, children)
```

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/attrs.py` & `scippnexus-23.5.1/src/scippnexus/v2/attrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from collections.abc import Mapping
 from typing import Any, Iterator
 
 from .._hdf5_nexus import _cset_to_encoding, _ensure_str
 
 
 class Attrs(Mapping):
-
     def __init__(self, attrs: Mapping):
         self._base_attrs = attrs
         self._attrs = dict(attrs) if attrs else dict()
 
     def __getitem__(self, name: str) -> Any:
         attr = self._attrs[name]
         # Is this check for string attributes sufficient? Is there a better way?
```

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/base.py` & `scippnexus-23.5.1/src/scippnexus/v2/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 
 def asvariable(obj: Union[Any, sc.Variable]) -> sc.Variable:
     return obj if isinstance(obj, sc.Variable) else sc.scalar(obj, unit=None)
 
 
 class NexusStructureError(Exception):
-    """Invalid or unsupported class and field structure in Nexus.
-    """
+    """Invalid or unsupported class and field structure in Nexus."""
+
     pass
 
 
 def is_dataset(obj: Union[H5Group, H5Dataset]) -> bool:
     """Return true if the object is an h5py.Dataset or equivalent.
 
     Use this instead of isinstance(obj, h5py.Dataset) to ensure that code is compatible
@@ -54,21 +54,20 @@
 
 
 def _dtype_fromdataset(dataset: H5Dataset) -> sc.DType:
     return _scipp_dtype.get(dataset.dtype, sc.DType.string)
 
 
 def _squeezed_field_sizes(dataset: H5Dataset) -> Dict[str, int]:
-    if (shape := dataset.shape) == (1, ):
+    if (shape := dataset.shape) == (1,):
         return {}
     return {f'dim_{i}': size for i, size in enumerate(shape)}
 
 
 class NXobject:
-
     def _init_field(self, field: Field):
         if field.sizes is None:
             field.sizes = _squeezed_field_sizes(field.dataset)
         field.dtype = _dtype_fromdataset(field.dataset)
 
     def __init__(self, attrs: Dict[str, Any], children: Dict[str, Union[Field, Group]]):
         """Subclasses should call this in their __init__ method, or ensure that they
@@ -78,22 +77,23 @@
         for field in children.values():
             if isinstance(field, Field):
                 self._init_field(field)
 
     @property
     def unit(self) -> Union[None, sc.Unit]:
         raise AttributeError(
-            f"Group-like {self._attrs.get('NX_class')} has no well-defined unit")
+            f"Group-like {self._attrs.get('NX_class')} has no well-defined unit"
+        )
 
     @cached_property
     def sizes(self) -> Dict[str, int]:
         return sc.DataGroup(self._children).sizes
 
     def index_child(
-            self, child: Union[Field, Group], sel: ScippIndex
+        self, child: Union[Field, Group], sel: ScippIndex
     ) -> Union[sc.Variable, sc.DataArray, sc.Dataset, sc.DataGroup]:
         """
         When a Group is indexed, this method is called to index each child.
 
         The main purpose of this is to translate the Group index to the child index.
         Since the group dimensions (usually given by the signal) may be a superset of
         the child dimensions, we need to translate the group index to a child index.
@@ -114,21 +114,24 @@
         The default implementation simply calls index_child on each child and returns
         the result as a DataGroup.
 
         Subclasses of NXobject, in particular NXevent_data, override this method to
         to implement special logic for reading children with interdependencies, i.e.,
         where reading each child in isolation is not possible.
         """
-        return sc.DataGroup({
-            name: self.index_child(child, sel)
-            for name, child in self._children.items()
-        })
-
-    def assemble(self,
-                 dg: sc.DataGroup) -> Union[sc.DataGroup, sc.DataArray, sc.Dataset]:
+        return sc.DataGroup(
+            {
+                name: self.index_child(child, sel)
+                for name, child in self._children.items()
+            }
+        )
+
+    def assemble(
+        self, dg: sc.DataGroup
+    ) -> Union[sc.DataGroup, sc.DataArray, sc.Dataset]:
         """
         When a Group is indexed, this method is called to assemble the read children
         into the result object.
 
         The default implementation simply returns the DataGroup.
 
         Subclasses of NXobject, in particular NXdata, override this method to return
@@ -212,15 +215,14 @@
     def _children(self) -> Dict[str, Union[Field, Group]]:
         """Lazily initialized children of the group."""
         if self._lazy_children is None:
             self._lazy_children = self._read_children()
         return self._lazy_children
 
     def _read_children(self) -> Dict[str, Union[Field, Group]]:
-
         def _make_child(obj: Union[H5Dataset, H5Group]) -> Union[Field, Group]:
             if is_dataset(obj):
                 return Field(obj, parent=self)
             else:
                 return Group(obj, definitions=self._definitions)
 
         items = {name: _make_child(obj) for name, obj in self._group.items()}
@@ -232,17 +234,20 @@
         # could be leveraged for label-based indexing in the future.
         items = {k: v for k, v in items.items() if not k.startswith('cue_')}
         for suffix in ('_errors', '_error'):
             field_with_errors = [name for name in items if f'{name}{suffix}' in items]
             for name in field_with_errors:
                 values = items[name]
                 errors = items[f'{name}{suffix}']
-                if (isinstance(values, Field) and isinstance(errors, Field)
-                        and values.unit == errors.unit
-                        and values.dataset.shape == errors.dataset.shape):
+                if (
+                    isinstance(values, Field)
+                    and isinstance(errors, Field)
+                    and values.unit == errors.unit
+                    and values.dataset.shape == errors.dataset.shape
+                ):
                     values.errors = errors.dataset
                     del items[f'{name}{suffix}']
         return items
 
     @property
     def _nexus(self) -> NXobject:
         """Instance of the NXobject subclass corresponding to the NX_class attribute.
@@ -264,41 +269,43 @@
         general parse all the field and group properties, since for classes such
         as NXdata the properties of any field may indirectly depend on the properties
         of any other field. For example, field attributes may define which fields are
         axes, and dim labels of other fields can be defined by the names of the axes.
         """
         if self._lazy_nexus is not None:
             return
-        self._lazy_nexus = self._definitions.get(self.attrs.get('NX_class'),
-                                                 NXobject)(attrs=self.attrs,
-                                                           children=self._children)
+        self._lazy_nexus = self._definitions.get(self.attrs.get('NX_class'), NXobject)(
+            attrs=self.attrs, children=self._children
+        )
 
     def __len__(self) -> int:
         return len(self._children)
 
     def __iter__(self) -> Iterator[str]:
         return self._children.__iter__()
 
     def _get_children_by_nx_class(
-            self, select: Union[type, List[type]]) -> Dict[str, Union[NXobject, Field]]:
+        self, select: Union[type, List[type]]
+    ) -> Dict[str, Union[NXobject, Field]]:
         children = {}
         select = tuple(select) if isinstance(select, list) else select
         for key, child in self._children.items():
             nx_class = Field if isinstance(child, Field) else child.nx_class
             if nx_class is not None and issubclass(nx_class, select):
                 children[key] = self[key]
         return children
 
     @overload
     def __getitem__(self, sel: str) -> Union[Group, Field]:
         ...
 
     @overload
-    def __getitem__(self,
-                    sel: ScippIndex) -> Union[sc.DataArray, sc.DataGroup, sc.Dataset]:
+    def __getitem__(
+        self, sel: ScippIndex
+    ) -> Union[sc.DataArray, sc.DataGroup, sc.Dataset]:
         ...
 
     @overload
     def __getitem__(self, sel: Union[type, List[type]]) -> Dict[str, NXobject]:
         ...
 
     def __getitem__(self, sel):
@@ -314,15 +321,15 @@
           classes. ``Field`` selects all child fields, i.e., all datasets but not
           groups.
         - Scipp-style index: Load the specified slice of the current group, returning
           a :class:`scipp.DataArray` or :class:`scipp.DataGroup`.
 
         Parameters
         ----------
-        name:
+        sel:
             Child name, class, or index.
 
         Returns
         -------
         :
             Field, group, dict of fields, or loaded data.
         """
@@ -340,32 +347,36 @@
             if isinstance(child, Field):
                 self._populate_fields()
             return child
 
         def isclass(x):
             return inspect.isclass(x) and issubclass(x, (Field, NXobject))
 
-        if isclass(sel) or (isinstance(sel, list) and len(sel)
-                            and all(isclass(x) for x in sel)):
+        if isclass(sel) or (
+            isinstance(sel, list) and len(sel) and all(isclass(x) for x in sel)
+        ):
             return self._get_children_by_nx_class(sel)
 
         dg = self._nexus.read_children(sel)
         try:
             dg = self._nexus.assemble(dg)
         except (sc.DimensionError, NexusStructureError) as e:
             self._warn_fallback(e)
         # For a time-dependent transformation in NXtransformations, an NXlog may
         # take the place of the `value` field. In this case, we need to read the
         # properties of the NXlog group to make the actual transformation.
         from .nxtransformations import maybe_transformation
+
         return maybe_transformation(self, value=dg, sel=sel)
 
     def _warn_fallback(self, e: Exception) -> None:
-        msg = (f"Failed to load {self.name} as {type(self._nexus).__name__}: {e} "
-               "Falling back to loading HDF5 group children as scipp.DataGroup.")
+        msg = (
+            f"Failed to load {self.name} as {type(self._nexus).__name__}: {e} "
+            "Falling back to loading HDF5 group children as scipp.DataGroup."
+        )
         warnings.warn(msg)
 
     def __setitem__(self, key, value):
         """Set a child group or child dataset.
 
         Note that due to the caching mechanisms in this class, reading the group
         or its children may not reflect the changes made by this method."""
@@ -392,32 +403,34 @@
         ----------
         name:
             Group name.
         nx_class:
             Nexus class, can be a valid string for the NX_class attribute, or a
             subclass of NXobject, such as NXdata or NXlog.
         """
-        return Group(create_class(self._group, name, class_name),
-                     definitions=self._definitions)
+        return Group(
+            create_class(self._group, name, class_name), definitions=self._definitions
+        )
 
     @cached_property
     def sizes(self) -> Dict[str, int]:
         return self._nexus.sizes
 
     @property
     def dims(self) -> Tuple[str, ...]:
         return tuple(self.sizes)
 
     @property
     def shape(self) -> Tuple[int, ...]:
         return tuple(self.sizes.values())
 
 
-def create_field(group: H5Group, name: str, data: Union[np.ndarray, sc.Variable],
-                 **kwargs) -> H5Dataset:
+def create_field(
+    group: H5Group, name: str, data: Union[np.ndarray, sc.Variable], **kwargs
+) -> H5Dataset:
     if not isinstance(data, sc.Variable):
         return group.create_dataset(name, data=data, **kwargs)
     values = data.values
     if data.dtype == sc.DType.string:
         values = np.array(data.values, dtype=object)
     elif data.dtype == sc.DType.datetime64:
         start = sc.epoch(unit=data.unit)
@@ -446,14 +459,15 @@
     group.attrs['NX_class'] = attr
     return group
 
 
 @lru_cache()
 def _nx_class_registry():
     from . import nexus_classes
+
     return dict(inspect.getmembers(nexus_classes, inspect.isclass))
 
 
 base_definitions_dict = {}
 
 
 def base_definitions() -> Dict[str, type]:
```

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/field.py` & `scippnexus-23.5.1/src/scippnexus/v2/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 
 
 @dataclass
 class Field:
     """NeXus field.
     In HDF5 fields are represented as dataset.
     """
+
     dataset: H5Dataset
     parent: 'Group'
     sizes: Optional[Dict[str, int]] = None
     dtype: Optional[sc.DType] = None
     errors: Optional[H5Dataset] = None
 
     @cached_property
@@ -99,68 +100,84 @@
         return tuple(self.sizes.values())
 
     @cached_property
     def file(self) -> 'Group':
         return self.parent.file
 
     def _load_variances(self, var, index):
-        stddevs = sc.empty(dims=var.dims,
-                           shape=var.shape,
-                           dtype=var.dtype,
-                           unit=var.unit)
+        stddevs = sc.empty(
+            dims=var.dims, shape=var.shape, dtype=var.dtype, unit=var.unit
+        )
         try:
             self.errors.read_direct(stddevs.values, source_sel=index)
         except TypeError:
             stddevs.values = self.errors[index].squeeze()
         # According to the standard, errors must have the same shape as the data.
         # This is not the case in all files we observed, is there any harm in
         # attempting a broadcast?
-        var.variances = np.broadcast_to(sc.pow(stddevs, sc.scalar(2)).values,
-                                        shape=var.shape)
+        var.variances = np.broadcast_to(
+            sc.pow(stddevs, sc.scalar(2)).values, shape=var.shape
+        )
 
     def __getitem__(self, select: ScippIndex) -> Union[Any, sc.Variable]:
-        """Load the field as a :py:class:`scipp.Variable` or Python object.
+        """
+        Load the field as a :py:class:`scipp.Variable` or Python object.
+
         If the shape is empty and no unit is given this returns a Python object, such
         as a string or integer. Otherwise a :py:class:`scipp.Variable` is returned.
+
+        Parameters
+        ----------
+        select:
+            Scipp-style index: Load the specified slice of the current group.
+
+        Returns
+        -------
+        :
+            Loaded data.
         """
         from .nxtransformations import maybe_transformation
+
         index = to_plain_index(self.dims, select)
         if isinstance(index, (int, slice)):
-            index = (index, )
+            index = (index,)
 
         base_dims = self.dims
         base_shape = self.shape
         dims = []
         shape = []
         for i, ind in enumerate(index):
             if not isinstance(ind, int):
                 dims.append(base_dims[i])
                 shape.append(len(range(*ind.indices(base_shape[i]))))
 
-        variable = sc.empty(dims=dims,
-                            shape=shape,
-                            dtype=self.dtype,
-                            unit=self.unit,
-                            with_variances=self.errors is not None)
+        variable = sc.empty(
+            dims=dims,
+            shape=shape,
+            dtype=self.dtype,
+            unit=self.unit,
+            with_variances=self.errors is not None,
+        )
 
         # If the variable is empty, return early
         if np.prod(shape) == 0:
             variable = self._maybe_datetime(variable)
             return maybe_transformation(self, value=variable, sel=select)
 
         if self.dtype == sc.DType.string:
             try:
                 strings = self.dataset.asstr()[index]
             except UnicodeDecodeError as e:
                 strings = self.dataset.asstr(encoding='latin-1')[index]
                 _warn_latin1_decode(self.dataset, strings, str(e))
             variable.values = np.asarray(strings).flatten()
             if self.dataset.name.endswith('depends_on') and variable.ndim == 0:
-                variable.value = depends_on_to_relative_path(variable.value,
-                                                             self.dataset.parent.name)
+                variable.value = depends_on_to_relative_path(
+                    variable.value, self.dataset.parent.name
+                )
         elif variable.values.flags["C_CONTIGUOUS"]:
             # On versions of h5py prior to 3.2, a TypeError occurs in some cases
             # where h5py cannot broadcast data with e.g. shape (20, 1) to a buffer
             # of shape (20,). Note that broadcasting (1, 20) -> (20,) does work
             # (see https://github.com/h5py/h5py/pull/1796).
             # Therefore, we manually squeeze here.
             # A pin of h5py<3.2 is currently required by Mantid and hence scippneutron
@@ -190,15 +207,16 @@
             for name in self.attrs:
                 if (dt := _as_datetime(self.attrs[name])) is not None:
                     starts.append(dt)
             if len(starts) == 1:
                 variable = convert_time_to_datetime64(
                     variable,
                     start=starts[0],
-                    scaling_factor=self.attrs.get('scaling_factor'))
+                    scaling_factor=self.attrs.get('scaling_factor'),
+                )
 
         return variable
 
     def __repr__(self) -> str:
         return f'<Nexus field "{self.dataset.name}">'
 
     @property
@@ -215,11 +233,13 @@
 
     @cached_property
     def unit(self) -> Union[sc.Unit, None]:
         if (unit := self.attrs.get('units')) is not None:
             try:
                 return sc.Unit(unit)
             except sc.UnitError:
-                warnings.warn(f"Unrecognized unit '{unit}' for value dataset "
-                              f"in '{self.name}'; setting unit as 'dimensionless'")
+                warnings.warn(
+                    f"Unrecognized unit '{unit}' for value dataset "
+                    f"in '{self.name}'; setting unit as 'dimensionless'"
+                )
                 return sc.units.one
         return None
```

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/file.py` & `scippnexus-23.5.1/src/scippnexus/v2/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from .base import Group, base_definitions
 
 _default_definitions = object()
 
 
 class File(AbstractContextManager, Group):
-
     def __init__(self, *args, definitions: Mapping = _default_definitions, **kwargs):
         """Context manager for NeXus files, similar to h5py.File.
 
         Arguments other than documented are as in :py:class:`h5py.File`.
 
         Parameters
         ----------
```

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/nexus_classes.py` & `scippnexus-23.5.1/src/scippnexus/v2/nexus_classes.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/nxcylindrical_geometry.py` & `scippnexus-23.5.1/src/scippnexus/v2/nxcylindrical_geometry.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,70 +5,75 @@
 
 import scipp as sc
 
 from .base import Group, NexusStructureError, NXobject, base_definitions_dict
 from .field import Field
 
 
-def _parse(*,
-           vertices: sc.Variable,
-           cylinders: sc.Variable,
-           detector_number: Optional[sc.Variable] = None,
-           parent_detector_number: Optional[sc.Variable] = None) -> sc.Variable:
+def _parse(
+    *,
+    vertices: sc.Variable,
+    cylinders: sc.Variable,
+    detector_number: Optional[sc.Variable] = None,
+    parent_detector_number: Optional[sc.Variable] = None
+) -> sc.Variable:
     face1_center = cylinders['vertex_index', 0]
     face1_edge = cylinders['vertex_index', 1]
     face2_center = cylinders['vertex_index', 2]
     ds = sc.Dataset()
     ds['face1_center'] = vertices[face1_center.values]
     ds['face1_edge'] = vertices[face1_edge.values]
     ds['face2_center'] = vertices[face2_center.values]
     ds = ds.rename(**{vertices.dim: 'cylinder'})
     if detector_number is None:
         # All cylinders belong to the same shape
         return sc.bins(begin=sc.index(0), dim='cylinder', data=ds)
     if parent_detector_number is None:
         raise NexusStructureError(
             "`detector_number` not given, but "
-            "NXcylindrical_geometry contains mapping to `detector_number`.")
+            "NXcylindrical_geometry contains mapping to `detector_number`."
+        )
     # detector_number gives indices into cylinders, the naming in the NeXus
     # standard appears to be misleading
     if parent_detector_number.values.size != detector_number.values.size:
         raise NexusStructureError(
             "Number of detector numbers in NXcylindrical_geometry "
-            "does not match the one given by the parent.")
+            "does not match the one given by the parent."
+        )
     detecting_cylinders = ds['cylinder', detector_number.values]
     # One cylinder per detector
-    begin = sc.arange('dummy',
-                      parent_detector_number.values.size,
-                      unit=None,
-                      dtype='int64')
+    begin = sc.arange(
+        'dummy', parent_detector_number.values.size, unit=None, dtype='int64'
+    )
     end = begin + sc.index(1)
     shape = sc.bins(begin=begin, end=end, dim='cylinder', data=detecting_cylinders)
     return shape.fold(dim='dummy', sizes=parent_detector_number.sizes)
 
 
 class NXcylindrical_geometry(NXobject):
     _dims = {
-        'vertices': ('vertex', ),
-        'detector_number': ('detector_number', ),
-        'cylinders': ('cylinder', 'vertex_index')
+        'vertices': ('vertex',),
+        'detector_number': ('detector_number',),
+        'cylinders': ('cylinder', 'vertex_index'),
     }
 
     def __init__(self, attrs: Dict[str, Any], children: Dict[str, Union[Field, Group]]):
         super().__init__(attrs=attrs, children=children)
         for name, field in children.items():
             if isinstance(field, Field):
                 field.sizes = dict(zip(self._dims.get(name), field.dataset.shape))
                 if name == 'vertices':
                     field.dtype = sc.DType.vector3
 
-    def load_as_array(self,
-                      detector_number: Optional[sc.Variable] = None) -> sc.Variable:
+    def load_as_array(
+        self, detector_number: Optional[sc.Variable] = None
+    ) -> sc.Variable:
         return _parse(**self[()], parent_detector_number=detector_number)
 
     @staticmethod
-    def assemble_as_child(children: sc.DataGroup,
-                          detector_number: Optional[sc.Variable] = None) -> sc.Variable:
+    def assemble_as_child(
+        children: sc.DataGroup, detector_number: Optional[sc.Variable] = None
+    ) -> sc.Variable:
         return _parse(**children, parent_detector_number=detector_number)
 
 
 base_definitions_dict['NXcylindrical_geometry'] = NXcylindrical_geometry
```

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/nxdata.py` & `scippnexus-23.5.1/src/scippnexus/v2/nxdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,33 +42,38 @@
             return [lut[s] for s in shape]
         except KeyError:
             pass
     return None
 
 
 class NXdata(NXobject):
-
-    def __init__(self,
-                 attrs: Dict[str, Any],
-                 children: Dict[str, Union[Field, Group]],
-                 fallback_dims: Optional[Tuple[str, ...]] = None,
-                 fallback_signal_name: Optional[str] = None):
+    def __init__(
+        self,
+        attrs: Dict[str, Any],
+        children: Dict[str, Union[Field, Group]],
+        fallback_dims: Optional[Tuple[str, ...]] = None,
+        fallback_signal_name: Optional[str] = None,
+    ):
         super().__init__(attrs=attrs, children=children)
         self._valid = True  # True if the children can be assembled
         self._signal_name = None
         self._signal = None
         self._aux_signals = attrs.get('auxiliary_signals', [])
 
-        self._init_signal(name=attrs.get('signal', fallback_signal_name),
-                          children=children)
+        self._init_signal(
+            name=attrs.get('signal', fallback_signal_name), children=children
+        )
         if (errors := children.get('errors')) is not None:
-            if (isinstance(self._signal, Field) and isinstance(errors, Field)
-                    and self._signal.errors is None
-                    and (errors.unit is None or self._signal.unit == errors.unit)
-                    and self._signal.dataset.shape == errors.dataset.shape):
+            if (
+                isinstance(self._signal, Field)
+                and isinstance(errors, Field)
+                and self._signal.errors is None
+                and (errors.unit is None or self._signal.unit == errors.unit)
+                and self._signal.dataset.shape == errors.dataset.shape
+            ):
                 self._signal.errors = errors.dataset
                 del children['errors']
         self._init_axes(attrs=attrs, children=children)
         self._init_group_dims(attrs=attrs, fallback_dims=fallback_dims)
 
         for name, field in children.items():
             self._init_field_dims(name, field)
@@ -77,18 +82,18 @@
         if not isinstance(field, Field):
             # If the NXdata contains subgroups we can generally not define valid
             # sizes... except for some non-signal "special fields" that return
             # a DataGroup that will be wrapped in a scalar Variable.
             if name == self._signal_name or name in self._aux_signals:
                 return
             if field.attrs.get('NX_class') not in [
-                    'NXoff_geometry',
-                    'NXcylindrical_geometry',
-                    'NXgeometry',
-                    'NXtransformations',
+                'NXoff_geometry',
+                'NXcylindrical_geometry',
+                'NXgeometry',
+                'NXtransformations',
             ]:
                 self._valid = False
         elif (dims := self._get_dims(name, field)) is not None:
             # The convention here is that the given dimensions apply to the shapes
             # starting from the left. So we only squeeze dimensions that are after
             # len(dims).
             shape = _squeeze_trailing(dims, field.dataset.shape)
@@ -122,32 +127,38 @@
                 self._signal = children[name]
                 break
         # NXlog or NXevent_data can take the role of the signal.
         for name, field in children.items():
             if name == self._signal_name:
                 # Avoid duplicate handling
                 continue
-            if isinstance(field,
-                          EventField) or (isinstance(field, Group)
-                                          and field.nx_class in [NXlog, NXevent_data]):
+            if isinstance(field, EventField) or (
+                isinstance(field, Group) and field.nx_class in [NXlog, NXevent_data]
+            ):
                 if self._signal is None:
                     self._signal_name = name
                     self._signal = field
                 else:
                     self._aux_signals.append(name)
 
-    def _init_axes(self, attrs: Dict[str, Any], children: Dict[str, Union[Field,
-                                                                          Group]]):
+    def _init_axes(
+        self, attrs: Dict[str, Any], children: Dict[str, Union[Field, Group]]
+    ):
         # Latest way of defining axes
         self._axes = attrs.get('axes')
         # Older way of defining axes
-        self._signal_axes = None if self._signal is None else self._signal.attrs.get(
-            'axes')
+        self._signal_axes = (
+            None if self._signal is None else self._signal.attrs.get('axes')
+        )
         if self._signal_axes is not None:
-            self._signal_axes = tuple(self._signal_axes.split(','))
+            self._signal_axes = tuple(self._signal_axes.split(':'))
+            # The standard says that the axes should be colon-separated, but some
+            # files use comma-separated.
+            if len(self._signal_axes) == 1 and self._signal.dataset.ndim > 1:
+                self._signal_axes = tuple(self._signal_axes[0].split(','))
         # Another old way of defining axes. Apparently there are two different ways in
         # which this is used: A value of '1' indicates "this is an axis". As this would
         # not allow for determining an order, we have to assume that the signal field
         # has an "axes" attribute that defines the order. We can then ignore the "axis"
         # attributes, since they hold no further information. If there is not "axes"
         # attribute on the signal field then we have to assume that "axis" gives the
         # 1-based index of the axis.
@@ -169,27 +180,28 @@
             return ()
 
     def _get_group_dims(self) -> Optional[Tuple[str, ...]]:
         """Try three ways of defining group dimensions."""
         # Apparently it is not possible to define dim labels unless there are
         # corresponding coords. Special case of '.' entries means "no coord".
         if self._axes is not None:
-            return tuple(f'dim_{i}' if a == '.' else a
-                         for i, a in enumerate(self._axes))
+            return tuple(
+                f'dim_{i}' if a == '.' else a for i, a in enumerate(self._axes)
+            )
         if self._signal_axes is not None:
             return self._signal_axes
         if self._axis_index:
             return tuple(
-                k
-                for k, _ in sorted(self._axis_index.items(), key=lambda item: item[1]))
+                k for k, _ in sorted(self._axis_index.items(), key=lambda item: item[1])
+            )
         return None
 
-    def _init_group_dims(self,
-                         attrs: Dict[str, Any],
-                         fallback_dims: Optional[Tuple[str, ...]] = None):
+    def _init_group_dims(
+        self, attrs: Dict[str, Any], fallback_dims: Optional[Tuple[str, ...]] = None
+    ):
         group_dims = self._get_group_dims()
 
         if self._signal is None:
             self._valid = False
         elif isinstance(self._signal, EventField):
             group_dims = self._signal.dims
         else:
@@ -209,16 +221,17 @@
                 self._signal.sizes = dict(zip(group_dims, shape))
 
         self._group_dims = group_dims
         self._named_axes = self._get_named_axes(fallback_dims)
 
         indices_suffix = '_indices'
         indices_attrs = {
-            key[:-len(indices_suffix)]: attr
-            for key, attr in attrs.items() if key.endswith(indices_suffix)
+            key[: -len(indices_suffix)]: attr
+            for key, attr in attrs.items()
+            if key.endswith(indices_suffix)
         }
 
         dims = np.array(self._axes)
         self._dims_from_indices = {
             key: tuple(dims[np.array(indices).flatten()])
             for key, indices in indices_attrs.items()
         }
@@ -229,36 +242,44 @@
         # since legacy files do not set this attribute.
         if name == self._signal_name:
             return self._group_dims
         # Latest way of defining dims
         if (dims := self._dims_from_indices.get(name)) is not None:
             if '.' in dims:
                 hdf5_dims = self._dims_from_hdf5(field)
-                return tuple(dim if dim != '.' else hdf5_dim
-                             for dim, hdf5_dim in zip(dims, hdf5_dims))
+                return tuple(
+                    dim if dim != '.' else hdf5_dim
+                    for dim, hdf5_dim in zip(dims, hdf5_dims)
+                )
             return dims
         # Older way of defining dims via axis attribute
         if (axis := self._axis_index.get(name)) is not None:
-            return (self._group_dims[axis - 1], )
+            return (self._group_dims[axis - 1],)
         if name in self._aux_signals:
-            return _guess_dims(self._group_dims, self._signal.dataset.shape,
-                               field.dataset)
+            return _guess_dims(
+                self._group_dims, self._signal.dataset.shape, field.dataset
+            )
         if name in self._named_axes:
             # If there are named axes then items of same name are "dimension
             # coordinates", i.e., have a dim matching their name.
             # However, if the item is not 1-D we need more labels. Try to use labels
             # of signal if dimensionality matches.
             if isinstance(self._signal, Field) and len(field.dataset.shape) == len(
-                    self._signal.dataset.shape):
+                self._signal.dataset.shape
+            ):
                 return self._group_dims
-            return (name, )
+            return (name,)
         if self._signal is not None and self._group_dims is not None:
-            signal_shape = self._signal.dataset.shape if isinstance(
-                self._signal, Field) else (self._signal.shape if isinstance(
-                    self._signal, EventField) else None)
+            signal_shape = (
+                self._signal.dataset.shape
+                if isinstance(self._signal, Field)
+                else (
+                    self._signal.shape if isinstance(self._signal, EventField) else None
+                )
+            )
             return _guess_dims(self._group_dims, signal_shape, field.dataset)
         # While not mandated or recommended by the standard, we can try to find HDF5
         # dim labels as a fallback option for defining dimension labels. Ideally we
         # would like to do so in NXobject._init_field, but this causes significant
         # overhead for small files with many datasets. Defined here, this will only
         # take effect for NXdata, NXdetector, NXlog, and NXmonitor.
         return self._dims_from_hdf5(field)
@@ -290,38 +311,42 @@
         for dim, size in zip(coord.dims, coord.shape):
             if (sz := sizes.get(dim)) is not None and sz + 1 == size:
                 return dim
         return None
 
     def index_child(self, child: Union[Field, Group], sel: ScippIndex) -> ScippIndex:
         """Same as NXobject.index_child but also handles bin edges."""
-        child_sel = to_child_select(tuple(self.sizes),
-                                    child.dims,
-                                    sel,
-                                    bin_edge_dim=self._bin_edge_dim(child))
+        child_sel = to_child_select(
+            tuple(self.sizes), child.dims, sel, bin_edge_dim=self._bin_edge_dim(child)
+        )
         return child[child_sel]
 
-    def assemble(self,
-                 dg: sc.DataGroup) -> Union[sc.DataGroup, sc.DataArray, sc.Dataset]:
+    def assemble(
+        self, dg: sc.DataGroup
+    ) -> Union[sc.DataGroup, sc.DataArray, sc.Dataset]:
         if not self._valid:
             raise NexusStructureError("Could not determine signal field or dimensions.")
         dg = dg.copy(deep=False)
         aux = {name: dg.pop(name) for name in self._aux_signals}
         signal = dg.pop(self._signal_name)
         coords = dg
         if isinstance(signal, sc.DataGroup):
             raise NexusStructureError("Signal is not an array-like.")
-        da = sc.DataArray(data=signal) if isinstance(signal, sc.Variable) else signal
+        da = (
+            signal
+            if isinstance(signal, sc.DataArray)
+            else sc.DataArray(data=asvariable(signal))
+        )
         da = self._add_coords(da, coords)
         if aux:
             signals = {self._signal_name: da}
             signals.update(aux)
             if all(
-                    isinstance(v, (sc.Variable, sc.DataArray))
-                    for v in signals.values()):
+                isinstance(v, (sc.Variable, sc.DataArray)) for v in signals.values()
+            ):
                 return sc.Dataset(signals)
             return sc.DataGroup(signals)
         return da
 
     def _dim_of_coord(self, name: str, coord: sc.Variable) -> Union[None, str]:
         if len(coord.dims) == 1:
             return coord.dims[0]
@@ -351,15 +376,15 @@
                 da.attrs[name] = coord
             else:
                 da.coords[name] = coord
         return da
 
 
 def _squeeze_trailing(dims: Tuple[str, ...], shape: Tuple[int, ...]) -> Tuple[int, ...]:
-    return shape[:len(dims)] + tuple(size for size in shape[len(dims):] if size != 1)
+    return shape[: len(dims)] + tuple(size for size in shape[len(dims) :] if size != 1)
 
 
 class NXlog(NXdata):
     """
     NXlog, a time-series that can be loaded as a DataArray.
 
     In some cases the NXlog may contain additional time series, such as a connection
@@ -387,79 +412,81 @@
                     self._init_field(field)
                     field.sizes = {
                         'time' if i == 0 else f'dim_{i}': size
                         for i, size in enumerate(field.dataset.shape)
                     }
                     self._sublog_children[k] = field
 
-        super().__init__(attrs=attrs,
-                         children=children,
-                         fallback_dims=('time', ),
-                         fallback_signal_name='value')
+        super().__init__(
+            attrs=attrs,
+            children=children,
+            fallback_dims=('time',),
+            fallback_signal_name='value',
+        )
 
     def read_children(self, sel: ScippIndex) -> sc.DataGroup:
         # Sublogs have distinct time axes (with a different length). Must disable
         # positional indexing.
         if self._sublogs and ('time' in _to_canonical_select(list(self.sizes), sel)):
             raise sc.DimensionError(
                 "Cannot positionally select time since there are multiple "
-                "time fields. Label-based selection is not supported yet.")
+                "time fields. Label-based selection is not supported yet."
+            )
         dg = super().read_children(sel)
         for name, field in self._sublog_children.items():
             dg[name] = field[sel]
         return dg
 
     def _time_to_datetime(self, mapping):
         if (time := mapping.get('time')) is not None:
             if time.dtype != sc.DType.datetime64 and _is_time(time):
                 mapping['time'] = convert_time_to_datetime64(
-                    time, start=sc.epoch(unit=time.unit))
+                    time, start=sc.epoch(unit=time.unit)
+                )
 
-    def _assemble_sublog(self,
-                         dg: sc.DataGroup,
-                         name: str,
-                         value_name: Optional[str] = None) -> sc.DataArray:
+    def _assemble_sublog(
+        self, dg: sc.DataGroup, name: str, value_name: Optional[str] = None
+    ) -> sc.DataArray:
         value_name = name if value_name is None else f'{name}_{value_name}'
         da = sc.DataArray(dg.pop(value_name), coords={'time': dg.pop(f'{name}_time')})
         for k in list(dg):
             if k.startswith(name):
-                da.coords[k[len(name) + 1:]] = dg.pop(k)
+                da.coords[k[len(name) + 1 :]] = dg.pop(k)
         self._time_to_datetime(da.coords)
         return da
 
-    def assemble(self,
-                 dg: sc.DataGroup) -> Union[sc.DataGroup, sc.DataArray, sc.Dataset]:
+    def assemble(
+        self, dg: sc.DataGroup
+    ) -> Union[sc.DataGroup, sc.DataArray, sc.Dataset]:
         self._time_to_datetime(dg)
         dg = sc.DataGroup(dg)
         sublogs = sc.DataGroup()
         for name in self._sublogs:
             # Somewhat arbitrary definition of which fields is the "value"
             value_name = 'severity' if name == 'alarm' else None
             sublogs[name] = self._assemble_sublog(dg, name, value_name=value_name)
         out = super().assemble(dg)
         return out if not sublogs else sc.DataGroup(value=out, **sublogs)
 
 
 def _find_embedded_nxevent_data(
-        children: Dict[str, Union[Field, Group]]) -> Optional[Group]:
+    children: Dict[str, Union[Field, Group]]
+) -> Optional[Group]:
     if all(name in children for name in NXevent_data.mandatory_fields):
         parent = children['event_index'].parent._group
-        event_group = Group(parent,
-                            definitions={
-                                'NXmonitor': NXevent_data,
-                                'NXdetector': NXevent_data
-                            })
+        event_group = Group(
+            parent, definitions={'NXmonitor': NXevent_data, 'NXdetector': NXevent_data}
+        )
         for name in list(children):
             if name in NXevent_data.handled_fields:
                 del children[name]
         return event_group
 
 
 class EventField:
-
     def __init__(self, event_data: Group, grouping_name: str, grouping: Field) -> None:
         """Create a field that represents an event data group.
 
         Parameters
         ----------
         event_data:
             The event data group holding the NXevent_data fields.
@@ -510,104 +537,112 @@
             if name in children:
                 return name
 
     def __init__(self, attrs: Dict[str, Any], children: Dict[str, Union[Field, Group]]):
         fallback_dims = None
         if (det_num_name := NXdetector._detector_number(children)) is not None:
             if (detector_number := children[det_num_name]).dataset.ndim == 1:
-                fallback_dims = (det_num_name, )
+                fallback_dims = (det_num_name,)
                 detector_number.sizes = {det_num_name: detector_number.dataset.shape[0]}
 
         if (event_group := _find_embedded_nxevent_data(children)) is not None:
             embedded_events = uuid.uuid4().hex if 'events' in children else 'events'
             children[embedded_events] = event_group
         else:
             embedded_events = None
 
         def _maybe_event_field(name: str, child: Union[Field, Group]):
-            if ((name == embedded_events or
-                 (isinstance(child, Group) and child.nx_class == NXevent_data))
-                    and det_num_name is not None):
-                event_field = EventField(event_data=child,
-                                         grouping_name=det_num_name,
-                                         grouping=children.get(det_num_name))
+            if (
+                name == embedded_events
+                or (isinstance(child, Group) and child.nx_class == NXevent_data)
+            ) and det_num_name is not None:
+                event_field = EventField(
+                    event_data=child,
+                    grouping_name=det_num_name,
+                    grouping=children.get(det_num_name),
+                )
                 return event_field
             return child
 
         children = {
-            name: _maybe_event_field(name, child)
-            for name, child in children.items()
+            name: _maybe_event_field(name, child) for name, child in children.items()
         }
 
-        super().__init__(attrs=attrs,
-                         children=children,
-                         fallback_dims=fallback_dims,
-                         fallback_signal_name='data')
+        super().__init__(
+            attrs=attrs,
+            children=children,
+            fallback_dims=fallback_dims,
+            fallback_signal_name='data',
+        )
 
     @property
     def detector_number(self) -> Optional[str]:
         return self._detector_number(self._children)
 
 
 class NXmonitor(NXdata):
-
     def __init__(self, attrs: Dict[str, Any], children: Dict[str, Union[Field, Group]]):
         if (event_group := _find_embedded_nxevent_data(children)) is not None:
             signal = uuid.uuid4().hex if 'events' in children else 'events'
             children[signal] = event_group
         else:
             signal = 'data'
         super().__init__(attrs=attrs, children=children, fallback_signal_name=signal)
 
 
-def _group_events(*,
-                  event_data: sc.DataArray,
-                  grouping: Optional[sc.Variable] = None) -> sc.DataArray:
+def _group_events(
+    *, event_data: sc.DataArray, grouping: Optional[sc.Variable] = None
+) -> sc.DataArray:
     if grouping is None:
         event_id = 'event_id'
     else:
         # copy since sc.bin cannot deal with a non-contiguous view
         grouping = asvariable(grouping)
         event_id = grouping.flatten(to='event_id').copy()
     event_data.bins.coords['event_time_zero'] = sc.bins_like(
-        event_data, fill_value=event_data.coords['event_time_zero'])
+        event_data, fill_value=event_data.coords['event_time_zero']
+    )
     # After loading raw NXevent_data it is guaranteed that the event table
     # is contiguous and that there is no masking. We can therefore use the
     # more efficient approach of binning from scratch instead of erasing the
     # 'event_time_zero' binning defined by NXevent_data.
     event_data = event_data.bins.constituents['data'].group(event_id)
     if grouping is None:
         return event_data
     return event_data.fold(dim='event_id', sizes=grouping.sizes)
 
 
 def _find_event_entries(dg: sc.DataGroup) -> List[str]:
     event_entries = []
     for name, value in dg.items():
-        if isinstance(
-                value, sc.DataArray
-        ) and 'event_time_zero' in value.coords and value.bins is not None:
+        if (
+            isinstance(value, sc.DataArray)
+            and 'event_time_zero' in value.coords
+            and value.bins is not None
+        ):
             event_entries.append(name)
     return event_entries
 
 
 def group_events_by_detector_number(
-        dg: sc.DataGroup) -> Union[sc.DataArray, sc.Dataset]:
+    dg: sc.DataGroup,
+) -> Union[sc.DataArray, sc.Dataset]:
     dg = dg.copy(deep=False)
     grouping_key = None
     for key in NXdetector._detector_number_fields:
         if (grouping := dg.get(key)) is not None:
             grouping_key = key
             break
     grouping = None if grouping_key is None else asvariable(dg.pop(grouping_key))
     grouped_events = sc.DataGroup()
     for event_entry in _find_event_entries(dg):
         events = dg.pop(event_entry)
-        grouped_events[event_entry] = _group_events(event_data=events,
-                                                    grouping=grouping)
+        grouped_events[event_entry] = _group_events(
+            event_data=events, grouping=grouping
+        )
     if len(grouped_events) == 1:
         out = next(iter(grouped_events.values()))
     else:
         out = sc.Dataset(grouped_events)
     out.coords.update(dg)
     return out
```

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/nxevent_data.py` & `scippnexus-23.5.1/src/scippnexus/v2/nxevent_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,21 @@
 _pulse_dimension = "event_time_zero"
 
 
 def _check_for_missing_fields(fields):
     for field in NXevent_data.mandatory_fields:
         if field not in fields:
             raise NexusStructureError(
-                f"Required field {field} not found in NXevent_data")
+                f"Required field {field} not found in NXevent_data"
+            )
 
 
 class NXevent_data(NXobject):
     mandatory_fields = ("event_time_zero", "event_index", "event_time_offset")
-    handled_fields = mandatory_fields + ("event_id", )
+    handled_fields = mandatory_fields + ("event_id",)
 
     def __init__(self, attrs: Dict[str, Any], children: Dict[str, Union[Field, Group]]):
         super().__init__(attrs=attrs, children=children)
         for name, field in children.items():
             if name in ['event_time_zero', 'event_index']:
                 field.sizes = {_pulse_dimension: field.dataset.shape[0]}
             elif name in ['event_time_offset', 'event_id']:
@@ -43,25 +44,25 @@
     def shape(self) -> Tuple[int]:
         if (event_index := self._children.get('event_index')) is not None:
             return event_index.shape
         return ()
 
     @property
     def dims(self) -> List[str]:
-        return (_pulse_dimension, )[:len(self.shape)]
+        return (_pulse_dimension,)[: len(self.shape)]
 
     @property
     def sizes(self) -> Dict[str, int]:
         return dict(zip(self.dims, self.shape))
 
     def field_dims(self, name: str, field: Field) -> Tuple[str, ...]:
         if name in ['event_time_zero', 'event_index']:
-            return (_pulse_dimension, )
+            return (_pulse_dimension,)
         if name in ['event_time_offset', 'event_id']:
-            return (_event_dimension, )
+            return (_event_dimension,)
         return None
 
     def read_children(self, select: ScippIndex) -> sc.DataGroup:
         children = self._children
         if not children:  # TODO Check that select is trivial?
             return sc.DataGroup()
 
@@ -71,31 +72,36 @@
 
         num_event = children["event_time_offset"].shape[0]
         # Some files contain uint64 "max" indices, which turn into negatives during
         # conversion to int64. This is a hack to get around this.
         event_index[event_index < 0] = num_event
 
         if len(event_index) > 0:
-            event_select = slice(event_index[0],
-                                 event_index[-1] if last_loaded else num_event)
+            event_select = slice(
+                event_index[0], event_index[-1] if last_loaded else num_event
+            )
         else:
             event_select = slice(0, 0)
 
         event_time_offset = children['event_time_offset'][event_select]
 
-        event_index = sc.array(dims=[_pulse_dimension],
-                               values=event_index[:-1] if last_loaded else event_index,
-                               dtype=sc.DType.int64,
-                               unit=None)
+        event_index = sc.array(
+            dims=[_pulse_dimension],
+            values=event_index[:-1] if last_loaded else event_index,
+            dtype=sc.DType.int64,
+            unit=None,
+        )
 
         event_index -= event_index.min()
 
-        dg = sc.DataGroup(event_time_zero=event_time_zero,
-                          event_index=event_index,
-                          event_time_offset=event_time_offset)
+        dg = sc.DataGroup(
+            event_time_zero=event_time_zero,
+            event_index=event_index,
+            event_time_offset=event_time_offset,
+        )
         if (event_id := children.get('event_id')) is not None:
             dg['event_id'] = event_id[event_select]
         return dg
 
     def _get_event_index(self, children: sc.DataGroup, index):
         max_index = self.shape[0]
         if index is Ellipsis or index == tuple():
@@ -122,21 +128,24 @@
     def assemble(self, children: sc.DataGroup) -> sc.DataArray:
         _check_for_missing_fields(children)
         event_time_offset = children['event_time_offset']
         event_time_zero = children['event_time_zero']
         event_index = children['event_index']
 
         # Weights are not stored in NeXus, so use 1s
-        weights = sc.ones(dims=[_event_dimension],
-                          shape=event_time_offset.shape,
-                          unit='counts',
-                          dtype=np.float32)
-
-        events = sc.DataArray(data=weights,
-                              coords={'event_time_offset': event_time_offset})
+        weights = sc.ones(
+            dims=[_event_dimension],
+            shape=event_time_offset.shape,
+            unit='counts',
+            dtype=np.float32,
+        )
+
+        events = sc.DataArray(
+            data=weights, coords={'event_time_offset': event_time_offset}
+        )
         if (event_id := children.get('event_id')) is not None:
             events.coords['event_id'] = event_id
 
         # There is some variation in the last recorded event_index in files from
         # different institutions. We try to make sure here that it is what would be the
         # first index of the next pulse. In other words, ensure that event_index
         # includes the bin edge for the last pulse.
```

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/nxoff_geometry.py` & `scippnexus-23.5.1/src/scippnexus/v2/nxoff_geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,79 +5,89 @@
 
 import scipp as sc
 
 from .base import Group, NexusStructureError, NXobject, base_definitions_dict
 from .field import Field
 
 
-def off_to_shape(*,
-                 vertices: sc.Variable,
-                 winding_order: sc.Variable,
-                 faces: sc.Variable,
-                 detector_faces: Optional[sc.Variable] = None,
-                 detector_number: Optional[sc.Variable] = None) -> sc.Variable:
+def off_to_shape(
+    *,
+    vertices: sc.Variable,
+    winding_order: sc.Variable,
+    faces: sc.Variable,
+    detector_faces: Optional[sc.Variable] = None,
+    detector_number: Optional[sc.Variable] = None
+) -> sc.Variable:
     """
     Convert OFF shape description to simpler shape representation.
     """
     # Vertices in winding order. This duplicates vertices if they are part of more than
     # one faces.
     # TODO Should use this:
     #     vw = vertices[winding_order.values]
     # but NumPy is currently much faster.
     # See https://github.com/scipp/scipp/issues/3044
-    vw = sc.vectors(dims=vertices.dims,
-                    values=vertices.values[winding_order.values],
-                    unit=vertices.unit)
+    vw = sc.vectors(
+        dims=vertices.dims,
+        values=vertices.values[winding_order.values],
+        unit=vertices.unit,
+    )
     # Same as above, grouped by face.
     fvw = sc.bins(begin=faces, data=vw, dim=vw.dim)
     low = fvw.bins.size().min().value
     high = fvw.bins.size().max().value
     if low == high:
         # Vertices in winding order, grouped by face. Unlike `fvw` above we now know
         # that each face has the same number of vertices, so we can fold instead of
         # using binned data.
         shapes = vw.fold(dim=vertices.dim, sizes={faces.dim: -1, vertices.dim: low})
     else:
-        raise NotImplementedError("Conversion from OFF to shape not implemented for "
-                                  "inconsistent number of vertices in faces.")
+        raise NotImplementedError(
+            "Conversion from OFF to shape not implemented for "
+            "inconsistent number of vertices in faces."
+        )
     if detector_faces is None:  # if detector_number is not None, all have same shape
         return sc.bins(begin=sc.index(0), dim=faces.dim, data=shapes)
     if detector_number is None:
-        raise NexusStructureError("`detector_number` not given but NXoff_geometry "
-                                  "contains `detector_faces`.")
+        raise NexusStructureError(
+            "`detector_number` not given but NXoff_geometry "
+            "contains `detector_faces`."
+        )
     shape_index = detector_faces['face_index|detector_number', 0].copy()
     detid = detector_faces['face_index|detector_number', 1].copy()
-    da = sc.DataArray(shape_index, coords={
-        'detector_number': detid
-    }).group(detector_number.flatten(to='detector_number'))
+    da = sc.DataArray(shape_index, coords={'detector_number': detid}).group(
+        detector_number.flatten(to='detector_number')
+    )
     comps = da.bins.constituents
     comps['data'] = shapes[faces.dim, comps['data'].values]
     return sc.bins(**comps).fold(dim='detector_number', sizes=detector_number.sizes)
 
 
 class NXoff_geometry(NXobject):
     _dims = {
         'detector_faces': ('face', 'face_index|detector_number'),
-        'vertices': ('vertex', ),
-        'winding_order': ('winding_order', ),
-        'faces': ('face', )
+        'vertices': ('vertex',),
+        'winding_order': ('winding_order',),
+        'faces': ('face',),
     }
 
     def __init__(self, attrs: Dict[str, Any], children: Dict[str, Union[Field, Group]]):
         super().__init__(attrs=attrs, children=children)
         for name, field in children.items():
             if isinstance(field, Field):
                 field.sizes = dict(zip(self._dims.get(name), field.dataset.shape))
                 if name == 'vertices':
                     field.dtype = sc.DType.vector3
 
-    def load_as_array(self,
-                      detector_number: Optional[sc.Variable] = None) -> sc.Variable:
+    def load_as_array(
+        self, detector_number: Optional[sc.Variable] = None
+    ) -> sc.Variable:
         return off_to_shape(**self[()], detector_number=detector_number)
 
     @staticmethod
-    def assemble_as_child(children: sc.DataGroup,
-                          detector_number: Optional[sc.Variable] = None) -> sc.Variable:
+    def assemble_as_child(
+        children: sc.DataGroup, detector_number: Optional[sc.Variable] = None
+    ) -> sc.Variable:
         return off_to_shape(**children, detector_number=detector_number)
 
 
 base_definitions_dict['NXoff_geometry'] = NXoff_geometry
```

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/nxsample.py` & `scippnexus-23.5.1/src/scippnexus/v2/nxsample.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
         super().__init__(attrs=attrs, children=children)
         for key in _matrix_units:
             if (field := children.get(key)) is not None:
                 field.sizes = {k: field.sizes[k] for k in field.dims[:-2]}
                 field.dtype = sc.DType.linear_transform3
 
     def read_children(self, sel: ScippIndex) -> sc.DataGroup:
-        return sc.DataGroup({
-            name: _fix_unit(name, self.index_child(child, sel))
-            for name, child in self._children.items()
-        })
+        return sc.DataGroup(
+            {
+                name: _fix_unit(name, self.index_child(child, sel))
+                for name, child in self._children.items()
+            }
+        )
 
 
 base_definitions_dict['NXsample'] = NXsample
```

### Comparing `scippnexus-23.5.0/src/scippnexus/v2/nxtransformations.py` & `scippnexus-23.5.1/src/scippnexus/v2/nxtransformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 
 class NXtransformations(NXobject):
     """Group of transformations."""
 
 
 class Transformation:
-
     def __init__(self, obj: Union[Field, NXobject]):  # could be an NXlog
         self._obj = obj
 
     @property
     def sizes(self) -> dict:
         return self._obj.sizes
 
@@ -63,44 +62,50 @@
     @property
     def offset(self):
         if (offset := self.attrs.get('offset')) is None:
             return None
         if (offset_units := self.attrs.get('offset_units')) is None:
             raise TransformationError(
                 f"Found {offset=} but no corresponding 'offset_units' "
-                f"attribute at {self.name}")
+                f"attribute at {self.name}"
+            )
         return sc.spatial.translation(value=offset, unit=offset_units)
 
     @property
     def vector(self) -> sc.Variable:
         return sc.vector(value=self.attrs.get('vector'))
 
     def __getitem__(self, select: ScippIndex):
         transformation_type = self.attrs.get('transformation_type')
         # According to private communication with Tobias Richter, NeXus allows 0-D or
         # shape=[1] for single values. It is unclear how and if this could be
         # distinguished from a scan of length 1.
         value = self._obj[select]
         return self.make_transformation(value, transformation_type, select)
 
-    def make_transformation(self, value: Union[sc.Variable, sc.DataArray],
-                            transformation_type: str, select: ScippIndex):
+    def make_transformation(
+        self,
+        value: Union[sc.Variable, sc.DataArray],
+        transformation_type: str,
+        select: ScippIndex,
+    ):
         try:
             if isinstance(value, sc.DataGroup):
                 return value
             t = value * self.vector
             v = t if isinstance(t, sc.Variable) else t.data
             if transformation_type == 'translation':
                 v = sc.spatial.translations(dims=v.dims, values=v.values, unit=v.unit)
             elif transformation_type == 'rotation':
                 v = sc.spatial.rotations_from_rotvecs(v)
             else:
                 raise TransformationError(
                     f"{transformation_type=} attribute at {self.name},"
-                    " expected 'translation' or 'rotation'.")
+                    " expected 'translation' or 'rotation'."
+                )
             if isinstance(t, sc.Variable):
                 t = v
             else:
                 t.data = v
             if (offset := self.offset) is None:
                 transform = t
             else:
@@ -109,111 +114,121 @@
                 if transformation_type == 'translation':
                     offset = offset.to(unit=t.unit, copy=False)
                 transform = t * offset
             if (depends_on := self.attrs.get('depends_on')) is not None:
                 if not isinstance(transform, sc.DataArray):
                     transform = sc.DataArray(transform)
                 transform.attrs['depends_on'] = sc.scalar(
-                    depends_on_to_relative_path(depends_on, self._obj.parent.name))
+                    depends_on_to_relative_path(depends_on, self._obj.parent.name)
+                )
             return transform
         except (sc.DimensionError, sc.UnitError, TransformationError):
             # TODO We should probably try to return some other data structure and
             # also insert offset and other attributes.
             return value
 
 
 def _interpolate_transform(transform, xnew):
     # scipy can't interpolate with a single value
     if transform.sizes["time"] == 1:
         transform = sc.concat([transform, transform], dim="time")
-    return interpolate.interp1d(transform,
-                                "time",
-                                kind="previous",
-                                fill_value="extrapolate")(xnew=xnew)
+    return interpolate.interp1d(
+        transform, "time", kind="previous", fill_value="extrapolate"
+    )(xnew=xnew)
 
 
 def _smaller_unit(a, b):
     if a.unit == b.unit:
         return a.unit
     ratio = sc.scalar(1.0, unit=a.unit).to(unit=b.unit)
     if ratio.value < 1.0:
         return a.unit
     else:
         return b.unit
 
 
 def get_full_transformation(
-        depends_on: Field) -> Union[None, sc.DataArray, sc.Variable]:
+    depends_on: Field,
+) -> Union[None, sc.DataArray, sc.Variable]:
     """
     Get the 4x4 transformation matrix for a component, resulting
     from the full chain of transformations linked by "depends_on"
     attributes
     """
     if (t0 := make_transformation(depends_on, depends_on[()])) is None:
         return None
     return get_full_transformation_starting_at(t0)
 
 
 def get_full_transformation_starting_at(
-        t0: Transformation,
-        *,
-        index: ScippIndex = None) -> Union[None, sc.DataArray, sc.Variable]:
+    t0: Transformation, *, index: ScippIndex = None
+) -> Union[None, sc.DataArray, sc.Variable]:
     transformations = _get_transformations(t0, index=() if index is None else index)
 
     total_transform = None
     for transform in transformations:
         if total_transform is None:
             total_transform = transform
         elif isinstance(total_transform, sc.DataArray) and isinstance(
-                transform, sc.DataArray):
-            unit = _smaller_unit(transform.coords['time'],
-                                 total_transform.coords['time'])
+            transform, sc.DataArray
+        ):
+            unit = _smaller_unit(
+                transform.coords['time'], total_transform.coords['time']
+            )
             total_transform.coords['time'] = total_transform.coords['time'].to(
-                unit=unit, copy=False)
-            transform.coords['time'] = transform.coords['time'].to(unit=unit,
-                                                                   copy=False)
-            time = sc.concat([total_transform.coords["time"], transform.coords["time"]],
-                             dim="time")
+                unit=unit, copy=False
+            )
+            transform.coords['time'] = transform.coords['time'].to(
+                unit=unit, copy=False
+            )
+            time = sc.concat(
+                [total_transform.coords["time"], transform.coords["time"]], dim="time"
+            )
             time = sc.datetimes(values=np.unique(time.values), dims=["time"], unit=unit)
-            total_transform = _interpolate_transform(transform, time) \
-                * _interpolate_transform(total_transform, time)
+            total_transform = _interpolate_transform(
+                transform, time
+            ) * _interpolate_transform(total_transform, time)
         else:
             total_transform = transform * total_transform
     if isinstance(total_transform, sc.DataArray):
         time_dependent = [t for t in transformations if isinstance(t, sc.DataArray)]
         times = [da.coords['time'][0] for da in time_dependent]
         latest_log_start = sc.reduce(times).max()
         return total_transform['time', latest_log_start:].copy()
     return total_transform
 
 
-def _get_transformations(transform: Transformation, *,
-                         index: ScippIndex) -> List[Union[sc.DataArray, sc.Variable]]:
+def _get_transformations(
+    transform: Transformation, *, index: ScippIndex
+) -> List[Union[sc.DataArray, sc.Variable]]:
     """Get all transformations in the depends_on chain."""
     transformations = []
     t = transform
     while t is not None:
         transformations.append(t[index])
         t = t.depends_on
     # TODO: this list of transformation should probably be cached in the future
     # to deal with changing beamline components (e.g. pixel positions) during a
     # live data stream (see https://github.com/scipp/scippneutron/issues/76).
     return transformations
 
 
 def maybe_transformation(
-        obj: Union[Field, Group], value: Union[sc.Variable, sc.DataArray, sc.DataGroup],
-        sel: ScippIndex) -> Union[sc.Variable, sc.DataArray, sc.DataGroup]:
+    obj: Union[Field, Group],
+    value: Union[sc.Variable, sc.DataArray, sc.DataGroup],
+    sel: ScippIndex,
+) -> Union[sc.Variable, sc.DataArray, sc.DataGroup]:
     """
     Return a loaded field, possibly modified if it is a transformation.
 
     Transformations are usually stored in NXtransformations groups. However, identifying
     transformation fields in this way requires inspecting the parent group, which
     is cumbersome to implement. Furthermore, according to the NXdetector documentation
     transformations are not necessarily placed inside NXtransformations.
     Instead we use the presence of the attribute 'transformation_type' to identify
     transformation fields.
     """
     if (transformation_type := obj.attrs.get('transformation_type')) is not None:
         from .nxtransformations import Transformation
+
         return Transformation(obj).make_transformation(value, transformation_type, sel)
     return value
```

### Comparing `scippnexus-23.5.0/src/scippnexus.egg-info/PKG-INFO` & `scippnexus-23.5.1/src/scippnexus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippnexus
-Version: 23.5.0
+Version: 23.5.1
 Summary: h5py-like utility for NeXus files based with seamless scipp integration
 Home-page: https://scipp.github.io/scippnexus
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/scippnexus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `scippnexus-23.5.0/src/scippnexus.egg-info/SOURCES.txt` & `scippnexus-23.5.1/src/scippnexus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.git-blame-ignore-revs
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
```

### Comparing `scippnexus-23.5.0/tests/application_definition_test.py` & `scippnexus-23.5.1/tests/application_definition_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
 @pytest.fixture()
 def I_of_Q():
     data = sc.array(
         dims=['Q'],
         values=[0.1, 0.2, 0.1, 0.4],
         variances=[1.0, 4.0, 9.0, 4.0],  # values chosen for exact sqrt
-        unit='1/counts')
+        unit='1/counts',
+    )
     da = sc.DataArray(data=data)
     da.coords['Q'] = sc.linspace('Q', 0, 1, num=5, unit='1/angstrom')
     da.coords['Q'].variances = sc.array(dims=['Q'], values=[1, 1, 4, 4, 1]).values
     return da
 
 
 def test_setitem_SASdata_raises_ValueError_when_given_bin_edges(nxroot, I_of_Q):
@@ -51,49 +52,50 @@
 
 
 def test_setitem_SASdata_raises_if_interpretation_of_variances_not_specified(nxroot):
     data = sc.array(
         dims=['Q'],
         values=[0.1, 0.2, 0.1, 0.4],
         variances=[1.0, 4.0, 9.0, 4.0],  # values chosen for exact sqrt
-        unit='1/counts')
+        unit='1/counts',
+    )
     da = sc.DataArray(data=data)
     da.coords['Q'] = sc.linspace('Q', 0, 1, num=5, unit='1/angstrom')
     da.coords['Q'].variances = sc.array(dims=['Q'], values=[1, 1, 4, 4, 1]).values
     with pytest.raises(ValueError):
         nxroot['sasdata'] = nxcansas.SASdata(da)
 
 
 def test_load_SASdata(nxroot):
     nxroot['sasentry'] = nxcansas.SASentry(title='A test', run=12345)
     entry = nxroot['sasentry']
     da = sc.DataArray(
         sc.array(dims=['Q'], values=[1, 2, 3], unit=''),
-        coords={'Q': sc.array(dims=['Q'], values=[1, 2, 3, 4], unit='1/angstrom')})
+        coords={'Q': sc.array(dims=['Q'], values=[1, 2, 3, 4], unit='1/angstrom')},
+    )
     group = entry.create_class('sasdata', snx.NXdata)
     group._group.attrs['canSAS_class'] = 'SASdata'
     group._group.attrs['signal'] = 'I'
     group._group.attrs['I_axes'] = 'Q'
     group['I'] = da.data
     group['Q'] = da.coords['Q']
     sasroot = snx.Group(nxroot._group, definitions=nxcansas.definitions)
     loaded = sasroot['sasentry/sasdata'][()]
     assert_identical(loaded, da)
 
 
 def test_load_SAStransmission_spectrum(nxroot):
     nxroot['sasentry'] = nxcansas.SASentry(title='A test', run=12345)
     entry = nxroot['sasentry']
-    spectrum = sc.DataArray(sc.array(dims=['lambda'], values=[1, 2, 3], unit='counts'),
-                            coords={
-                                'lambda':
-                                sc.array(dims=['lambda'],
-                                         values=[1, 2, 3, 4],
-                                         unit='angstrom')
-                            })
+    spectrum = sc.DataArray(
+        sc.array(dims=['lambda'], values=[1, 2, 3], unit='counts'),
+        coords={
+            'lambda': sc.array(dims=['lambda'], values=[1, 2, 3, 4], unit='angstrom')
+        },
+    )
     group = entry.create_class('sastransmission_spectrum', snx.NXdata)
     group._group.attrs['canSAS_class'] = 'SAStransmission_spectrum'
     group._group.attrs['signal'] = 'T'
     group._group.attrs['T_axes'] = 'lambda'
     group['T'] = spectrum.data
     group['lambda'] = spectrum.coords['lambda']
     sasroot = snx.Group(nxroot._group, definitions=nxcansas.definitions)
```

### Comparing `scippnexus-23.5.0/tests/conftest.py` & `scippnexus-23.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.0/tests/load_files_test.py` & `scippnexus-23.5.1/tests/load_files_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,30 +29,30 @@
 
 
 def assert_schema(dg: sc.DataGroup, schema: Dict[str, Any]) -> None:
     for name, validate in schema.items():
         validate(get_item_at_path(dg, name))
 
 
-def validator(item_type: type,
-              sizes: Optional[Dict[str, int]] = None,
-              dtype: Optional[Union[str, sc.DType]] = None) -> None:
-
+def validator(
+    item_type: type,
+    sizes: Optional[Dict[str, int]] = None,
+    dtype: Optional[Union[str, sc.DType]] = None,
+) -> None:
     def _validator(item):
         assert isinstance(item, item_type)
         if sizes is not None:
             assert item.sizes == sizes
         if dtype is not None:
             assert item.dtype == dtype
 
     return _validator
 
 
 def bins_validator(item_type: type, sizes: Optional[Dict[str, int]] = None):
-
     def _validator(item):
         assert isinstance(item, item_type)
         assert item.bins is not None
         if sizes is not None:
             assert item.sizes == sizes
 
     return _validator
@@ -76,29 +76,35 @@
 
 @pytest.mark.externalfile
 def test_amor2020n000346_tweaked():
     with snx.File(externalfile.get_path('2023/amor2020n000346_tweaked.nxs')) as f:
         dg = f[()]
     schema = {}
     schema['entry/instrument/multiblade_detector'] = bins_validator(
-        sc.DataArray, {'detector_number': 9216})
+        sc.DataArray, {'detector_number': 9216}
+    )
     schema['entry/stages/com'] = validator(sc.DataArray, {'time': 1, 'dim_1': 1})
     schema['entry/facility'] = validator(str)
     assert_schema(dg, schema)
 
 
 @pytest.mark.externalfile
 def test_LOKI_60322_2022_03_02_2205_fixed():
     with snx.File(
-            externalfile.get_path('2023/LOKI_60322-2022-03-02_2205_fixed.nxs')) as f:
+        externalfile.get_path('2023/LOKI_60322-2022-03-02_2205_fixed.nxs')
+    ) as f:
         dg = f[()]
     schema = {}
     schema['entry/instrument/larmor_detector'] = bins_validator(
-        sc.DataArray, {'detector_number': 458752})
-    schema['entry/instrument/monitor_1'] = bins_validator(sc.DataArray,
-                                                          {'event_time_zero': 1987})
-    schema['entry/instrument/monitor_2'] = bins_validator(sc.DataArray,
-                                                          {'event_time_zero': 1987})
+        sc.DataArray, {'detector_number': 458752}
+    )
+    schema['entry/instrument/monitor_1'] = bins_validator(
+        sc.DataArray, {'event_time_zero': 1987}
+    )
+    schema['entry/instrument/monitor_2'] = bins_validator(
+        sc.DataArray, {'event_time_zero': 1987}
+    )
     schema['entry/instrument/source/transformations/trans_2'] = validator(
-        sc.DataArray, {}, sc.DType.translation3)
+        sc.DataArray, {}, sc.DType.translation3
+    )
 
     assert_schema(dg, schema)
```

### Comparing `scippnexus-23.5.0/tests/nexus_test.py` & `scippnexus-23.5.1/tests/nexus_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,19 +61,18 @@
 def test_nxobject_items(nxroot):
     items = nxroot.items()
     assert len(items) == 1
     name, entry = next(iter(items))
     assert name == 'entry'
     entry.create_class('monitor', NXmonitor)
     entry.create_class('log', NXlog)
-    assert {k: v.nx_class
-            for k, v in entry.items()} == {
-                'log': NXlog,
-                'monitor': NXmonitor
-            }
+    assert {k: v.nx_class for k, v in entry.items()} == {
+        'log': NXlog,
+        'monitor': NXmonitor,
+    }
 
 
 def test_nxobject_iter(nxroot):
     nxroot.create_class('entry2', NXentry)
     # With missing __iter__ this used to raise since Python just calls __getitem__
     # with an int range.
     list(nxroot)
@@ -149,16 +148,19 @@
 
 
 def test_nxobject_getitem_by_class_list(nxroot):
     nxroot['entry'].create_class('log', NXlog)
     nxroot['entry'].create_class('events_0', NXevent_data)
     nxroot['entry'].create_class('events_1', NXevent_data)
     nxroot['entry']['field1'] = sc.arange('event', 4.0, unit='ns')
-    assert set(nxroot['entry'][[NXlog,
-                                NXevent_data]]) == {'log', 'events_0', 'events_1'}
+    assert set(nxroot['entry'][[NXlog, NXevent_data]]) == {
+        'log',
+        'events_0',
+        'events_1',
+    }
     assert set(nxroot['entry'][[NXlog, snx.Field]]) == {'log', 'field1'}
 
 
 def test_nxobject_dataset_items_are_returned_as_Field(nxroot):
     events = nxroot['entry'].create_class('events_0', NXevent_data)
     events['event_time_offset'] = sc.arange('event', 5)
     field = nxroot['entry/events_0/event_time_offset']
@@ -167,34 +169,34 @@
 
 def test_field_properties(nxroot):
     events = nxroot['entry'].create_class('events_0', NXevent_data)
     events['event_time_offset'] = sc.arange('event', 6, dtype='int64', unit='ns')
     field = nxroot['entry/events_0/event_time_offset']
     assert field.dtype == 'int64'
     assert field.name == '/entry/events_0/event_time_offset'
-    assert field.shape == (6, )
+    assert field.shape == (6,)
     assert field.unit == sc.Unit('ns')
 
 
 def test_field_dim_labels(nxroot):
     events = nxroot['entry'].create_class('events_0', NXevent_data)
     events['event_time_offset'] = sc.arange('ignored', 2)
     events['event_time_zero'] = sc.arange('ignored', 2)
     events['event_index'] = sc.arange('ignored', 2)
     events['event_id'] = sc.arange('ignored', 2)
     event_data = nxroot['entry/events_0']
-    assert event_data['event_time_offset'].dims == ('event', )
-    assert event_data['event_time_zero'].dims == ('event_time_zero', )
-    assert event_data['event_index'].dims == ('event_time_zero', )
-    assert event_data['event_id'].dims == ('event', )
+    assert event_data['event_time_offset'].dims == ('event',)
+    assert event_data['event_time_zero'].dims == ('event_time_zero',)
+    assert event_data['event_index'].dims == ('event_time_zero',)
+    assert event_data['event_id'].dims == ('event',)
     log = nxroot['entry'].create_class('log', NXlog)
     log['value'] = sc.arange('ignored', 2)
     log['time'] = sc.arange('ignored', 2)
-    assert log['time'].dims == ('time', )
-    assert log['value'].dims == ('time', )
+    assert log['time'].dims == ('time',)
+    assert log['value'].dims == ('time',)
 
 
 def test_field_unit_is_none_if_no_units_attribute(nxroot):
     log = nxroot.create_class('log', NXlog)
     log['value'] = sc.arange('ignored', 2, unit=None)
     log['time'] = sc.arange('ignored', 2)
     assert log.unit is None
@@ -217,18 +219,20 @@
     value = nxroot['group']['value'][()]
     assert_identical(value, sc.scalar(value=10.0, unit='m'))
     assert 'value_errors' in nxroot['group']
     errors = nxroot['group']['value_errors'][()]
     assert_identical(errors, sc.scalar(value=200.0, unit='cm'))
 
 
-@pytest.mark.parametrize('value,type_', [(1.2, np.float32), (123, np.int32),
-                                         ('abc', str), (True, bool)])
+@pytest.mark.parametrize(
+    'value,type_', [(1.2, np.float32), (123, np.int32), ('abc', str), (True, bool)]
+)
 def test_field_is_returned_as_python_object_if_shape_empty_and_no_unit(
-        nxroot, value, type_):
+    nxroot, value, type_
+):
     nxroot['field1'] = sc.scalar(value, unit=None, dtype=type_)
     field = nxroot['field1'][()]
     assert isinstance(field, type_)
     assert field == type_(value)
 
 
 @pytest.mark.parametrize('value', [1.2, 123, True, 'abc'])
@@ -239,106 +243,133 @@
 
 
 def test_field_getitem_returns_variable_with_correct_size_and_values(nxroot):
     nxroot['field'] = sc.arange('ignored', 6, dtype='int64', unit='ns')
     field = nxroot['field']
     assert sc.identical(
         field[...],
-        sc.array(dims=['dim_0'], unit='ns', values=[0, 1, 2, 3, 4, 5], dtype='int64'))
+        sc.array(dims=['dim_0'], unit='ns', values=[0, 1, 2, 3, 4, 5], dtype='int64'),
+    )
     assert sc.identical(
         field[1:],
-        sc.array(dims=['dim_0'], unit='ns', values=[1, 2, 3, 4, 5], dtype='int64'))
+        sc.array(dims=['dim_0'], unit='ns', values=[1, 2, 3, 4, 5], dtype='int64'),
+    )
     assert sc.identical(
         field[:-1],
-        sc.array(dims=['dim_0'], unit='ns', values=[0, 1, 2, 3, 4], dtype='int64'))
+        sc.array(dims=['dim_0'], unit='ns', values=[0, 1, 2, 3, 4], dtype='int64'),
+    )
 
 
 @pytest.mark.parametrize("string", UTF8_TEST_STRINGS)
 def test_field_of_utf8_encoded_dataset_is_loaded_correctly(nxroot, string):
-    nxroot['entry']['title'] = sc.array(dims=['ignored'],
-                                        values=[string, string + string])
+    nxroot['entry']['title'] = sc.array(
+        dims=['ignored'], values=[string, string + string]
+    )
     title = nxroot['entry/title']
-    assert sc.identical(title[...],
-                        sc.array(dims=['dim_0'], values=[string, string + string]))
+    assert sc.identical(
+        title[...], sc.array(dims=['dim_0'], values=[string, string + string])
+    )
 
 
 def test_field_of_extended_ascii_in_ascii_encoded_dataset_is_loaded_correctly():
     # When writing, if we use bytes h5py will write as ascii encoding
     # 0xb0 = degrees symbol in latin-1 encoding.
-    string = b"run at rot=90" + bytes([0xb0])
+    string = b"run at rot=90" + bytes([0xB0])
     with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
         f['title'] = np.array([string, string + b'x'])
         title = snx.Group(f)['title']
         assert sc.identical(
             title[...],
-            sc.array(dims=['dim_0'], values=["run at rot=90°", "run at rot=90°x"]))
+            sc.array(dims=['dim_0'], values=["run at rot=90°", "run at rot=90°x"]),
+        )
 
 
 def test_ms_field_with_second_datetime_attribute_loaded_as_ms_datetime(nxroot):
     nxroot['mytime'] = sc.arange('ignored', 2, unit='ms')
     nxroot['mytime'].dataset.attrs['start_time'] = '2022-12-12T12:13:14'
     assert sc.identical(
         nxroot['mytime'][...],
-        sc.datetimes(dims=['dim_0'],
-                     unit='ms',
-                     values=['2022-12-12T12:13:14.000', '2022-12-12T12:13:14.001']))
+        sc.datetimes(
+            dims=['dim_0'],
+            unit='ms',
+            values=['2022-12-12T12:13:14.000', '2022-12-12T12:13:14.001'],
+        ),
+    )
 
 
 def test_ns_field_with_second_datetime_attribute_loaded_as_ns_datetime(nxroot):
     nxroot['mytime'] = sc.arange('ignored', 2, unit='ns')
     nxroot['mytime'].dataset.attrs['start_time'] = '1970-01-01T00:00:00'
     assert sc.identical(
         nxroot['mytime'][...],
         sc.datetimes(
             dims=['dim_0'],
             unit='ns',
-            values=['1970-01-01T00:00:00.000000000', '1970-01-01T00:00:00.000000001']))
+            values=['1970-01-01T00:00:00.000000000', '1970-01-01T00:00:00.000000001'],
+        ),
+    )
 
 
 def test_second_field_with_ns_datetime_attribute_loaded_as_ns_datetime(nxroot):
     nxroot['mytime'] = sc.arange('ignored', 2, unit='s')
     nxroot['mytime'].dataset.attrs['start_time'] = '1984-01-01T00:00:00.000000000'
     assert sc.identical(
         nxroot['mytime'][...],
-        sc.datetimes(dims=['dim_0'],
-                     unit='ns',
-                     values=['1984-01-01T00:00:00', '1984-01-01T00:00:01']))
-
-
-@pytest.mark.parametrize('timezone,hhmm', [('Z', '12:00'), ('+04', '08:00'),
-                                           ('+00', '12:00'), ('-02', '14:00'),
-                                           ('+1130', '00:30'), ('-0930', '21:30'),
-                                           ('+11:30', '00:30'), ('-09:30', '21:30')])
+        sc.datetimes(
+            dims=['dim_0'],
+            unit='ns',
+            values=['1984-01-01T00:00:00', '1984-01-01T00:00:01'],
+        ),
+    )
+
+
+@pytest.mark.parametrize(
+    'timezone,hhmm',
+    [
+        ('Z', '12:00'),
+        ('+04', '08:00'),
+        ('+00', '12:00'),
+        ('-02', '14:00'),
+        ('+1130', '00:30'),
+        ('-0930', '21:30'),
+        ('+11:30', '00:30'),
+        ('-09:30', '21:30'),
+    ],
+)
 def test_timezone_information_in_datetime_attribute_is_applied(nxroot, timezone, hhmm):
     nxroot['mytime'] = sc.scalar(value=3, unit='s')
     nxroot['mytime'].dataset.attrs['start_time'] = f'1984-01-01T12:00:00{timezone}'
-    assert sc.identical(nxroot['mytime'][...],
-                        sc.datetime(unit='s', value=f'1984-01-01T{hhmm}:03'))
+    assert sc.identical(
+        nxroot['mytime'][...], sc.datetime(unit='s', value=f'1984-01-01T{hhmm}:03')
+    )
 
 
 def test_timezone_information_in_datetime_attribute_preserves_ns_precision(nxroot):
     nxroot['mytime'] = sc.scalar(value=3, unit='s')
     nxroot['mytime'].dataset.attrs['start_time'] = '1984-01-01T12:00:00.123456789+0200'
-    assert sc.identical(nxroot['mytime'][...],
-                        sc.datetime(unit='ns', value='1984-01-01T10:00:03.123456789'))
+    assert sc.identical(
+        nxroot['mytime'][...],
+        sc.datetime(unit='ns', value='1984-01-01T10:00:03.123456789'),
+    )
 
 
 def test_loads_bare_timestamps_if_multiple_candidate_datetime_offsets_found(nxroot):
     offsets = sc.arange('ignored', 2, unit='ms')
     nxroot['mytime'] = offsets
     nxroot['mytime'].dataset.attrs['offset'] = '2022-12-12T12:13:14'
     nxroot['mytime'].dataset.attrs['start_time'] = '2022-12-12T12:13:15'
     assert sc.identical(nxroot['mytime'][...], offsets.rename(ignored='dim_0'))
 
 
 def test_length_0_field_with_datetime_attribute_loaded_as_datetime(nxroot):
     nxroot['mytime'] = sc.arange('ignored', 0, unit='ms')
     nxroot['mytime'].dataset.attrs['start_time'] = '2022-12-12T12:13:14'
-    assert_identical(nxroot['mytime'][...],
-                     sc.datetimes(dims=['dim_0'], unit='ms', values=[]))
+    assert_identical(
+        nxroot['mytime'][...], sc.datetimes(dims=['dim_0'], unit='ms', values=[])
+    )
 
 
 @pytest.mark.skip(reason='Special attributes disabled for now. Do we keep them?')
 def test___getattr__for_unique_child_groups(nxroot):
     entry = nxroot['entry']
     with pytest.raises(NexusStructureError):
         entry.log
@@ -395,16 +426,16 @@
     data['time_errors'] = np.arange(5.0)
     data['time_errors'].attrs['units'] = 's'
     obj = snx.Group(data)
     assert set(obj._children.keys()) == {'signal', 'time'}
     dg = obj[()]
     assert dg['signal'].variances is not None
     assert dg['time'].variances is not None
-    assert np.array_equal(dg['signal'].variances, np.arange(4.0)**2)
-    assert np.array_equal(dg['time'].variances, np.arange(5.0)**2)
+    assert np.array_equal(dg['signal'].variances, np.arange(4.0) ** 2)
+    assert np.array_equal(dg['time'].variances, np.arange(5.0) ** 2)
 
 
 def test_read_field(h5root):
     entry = h5root.create_group('entry')
     data = entry.create_group('data')
     data['signal'] = np.arange(4)
     data['signal'].attrs['units'] = 'm'
@@ -418,19 +449,20 @@
     data = entry.create_group('data')
     data.attrs['NX_class'] = 'NXdata'
     data.attrs['signal'] = 'signal'
     data.attrs['axes'] = ['time', 'temperature']
     data.attrs['time_indices'] = [0]
     data.attrs['temperature_indices'] = [1]
     ref = sc.DataArray(
-        data=sc.ones(dims=['time', 'temperature'], shape=[3, 4], unit='m'))
+        data=sc.ones(dims=['time', 'temperature'], shape=[3, 4], unit='m')
+    )
     ref.coords['time'] = sc.array(dims=['time'], values=np.arange(3), unit='s')
-    ref.coords['temperature'] = sc.array(dims=['temperature'],
-                                         values=np.arange(4),
-                                         unit='K')
+    ref.coords['temperature'] = sc.array(
+        dims=['temperature'], values=np.arange(4), unit='K'
+    )
     data['signal'] = ref.values
     data['signal'].attrs['units'] = str(ref.unit)
     data['time'] = ref.coords['time'].values
     data['time'].attrs['units'] = str(ref.coords['time'].unit)
     data['temperature'] = ref.coords['temperature'].values
     data['temperature'].attrs['units'] = str(ref.coords['temperature'].unit)
     obj = snx.Group(data, definitions=snx.base_definitions())
@@ -443,19 +475,20 @@
     data = entry.create_group('data')
     data.attrs['NX_class'] = 'NXdata'
     data.attrs['signal'] = 'signal'
     data.attrs['axes'] = ['time', 'temperature']
     data.attrs['time_indices'] = [0]
     data.attrs['temperature_indices'] = [1]
     ref = sc.DataArray(
-        data=sc.ones(dims=['time', 'temperature'], shape=[3, 4], unit='m'))
+        data=sc.ones(dims=['time', 'temperature'], shape=[3, 4], unit='m')
+    )
     ref.coords['time'] = sc.array(dims=['time'], values=np.arange(3), unit='s')
-    ref.coords['temperature'] = sc.array(dims=['temperature'],
-                                         values=np.arange(4),
-                                         unit='K')
+    ref.coords['temperature'] = sc.array(
+        dims=['temperature'], values=np.arange(4), unit='K'
+    )
     data['signal'] = ref.values
     data['signal'].attrs['units'] = str(ref.unit)
     data['time'] = ref.coords['time'].values
     data['time'].attrs['units'] = str(ref.coords['time'].unit)
     data['temperature'] = ref.coords['temperature'].values
     data['temperature'].attrs['units'] = str(ref.coords['temperature'].unit)
     obj = snx.Group(data, definitions=snx.base_definitions())
@@ -468,19 +501,20 @@
     data = entry.create_group('data')
     data.attrs['NX_class'] = 'NXdata'
     data.attrs['signal'] = 'signal'
     data.attrs['axes'] = ['time', 'temperature']
     data.attrs['time_indices'] = [0]
     data.attrs['temperature_indices'] = [1]
     ref = sc.DataArray(
-        data=sc.ones(dims=['time', 'temperature'], shape=[3, 4], unit='m'))
+        data=sc.ones(dims=['time', 'temperature'], shape=[3, 4], unit='m')
+    )
     ref.coords['time'] = sc.array(dims=['time'], values=np.arange(3), unit='s')
-    ref.coords['temperature'] = sc.array(dims=['temperature'],
-                                         values=np.arange(5),
-                                         unit='K')
+    ref.coords['temperature'] = sc.array(
+        dims=['temperature'], values=np.arange(5), unit='K'
+    )
     data['signal'] = ref.values
     data['signal'].attrs['units'] = str(ref.unit)
     data['time'] = ref.coords['time'].values
     data['time'].attrs['units'] = str(ref.coords['time'].unit)
     data['temperature'] = ref.coords['temperature'].values
     data['temperature'].attrs['units'] = str(ref.coords['temperature'].unit)
     obj = snx.Group(data, definitions=snx.base_definitions())
```

### Comparing `scippnexus-23.5.0/tests/nxcylindrical_geometry_test.py` & `scippnexus-23.5.1/tests/nxcylindrical_geometry_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,25 +15,26 @@
 
 
 def test_vertices_loaded_as_vector3(nxroot):
     shape = nxroot['entry'].create_class('shape', snx.NXcylindrical_geometry)
     values = [[1, 2, 3], [4, 5, 6]]
     shape['vertices'] = sc.array(dims=['ignored', 'comp'], values=values, unit='mm')
     loaded = shape[()]
-    assert sc.identical(loaded['vertices'],
-                        sc.vectors(dims=['vertex'], values=values, unit='mm'))
+    assert sc.identical(
+        loaded['vertices'], sc.vectors(dims=['vertex'], values=values, unit='mm')
+    )
 
 
 def test_field_properties(nxroot):
     shape = nxroot['entry'].create_class('shape', snx.NXcylindrical_geometry)
     values = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
     shape['vertices'] = sc.array(dims=['ignored', 'comp'], values=values, unit='m')
-    shape['cylinders'] = sc.array(dims=['ignored', 'index'],
-                                  values=[[0, 1, 2]],
-                                  unit=None)
+    shape['cylinders'] = sc.array(
+        dims=['ignored', 'index'], values=[[0, 1, 2]], unit=None
+    )
     shape['detector_number'] = sc.array(dims=['ignored'], values=[], unit=None)
     loaded = shape[()]
-    assert loaded['vertices'].dims == ('vertex', )
+    assert loaded['vertices'].dims == ('vertex',)
     assert loaded['cylinders'].dims == ('cylinder', 'vertex_index')
     assert loaded['cylinders'].unit is None
-    assert loaded['detector_number'].dims == ('detector_number', )
+    assert loaded['detector_number'].dims == ('detector_number',)
     assert loaded['detector_number'].unit is None
```

### Comparing `scippnexus-23.5.0/tests/nxdata_test.py` & `scippnexus-23.5.1/tests/nxdata_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,41 +32,44 @@
     data.attrs['signal'] = 'signal'
     obj = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(obj[...], sc.DataArray(signal))
 
 
 def test_with_coords_matching_axis_names(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
     da.coords['xx'] = da.data['yy', 0]
     data = snx.create_class(h5root, 'data1', snx.NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     snx.create_field(data, 'signal', da.data)
     snx.create_field(data, 'xx', da.coords['xx'])
     group = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(group[...], da)
 
 
 def test_guessed_dim_for_coord_not_matching_axis_name(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
     da.coords['xx2'] = da.data['yy', 1]
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     snx.create_field(data, 'signal', da.data)
     snx.create_field(data, 'xx2', da.coords['xx2'])
     data = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(data[...], da)
 
 
 def test_multiple_coords(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
     da.coords['xx'] = da.data['yy', 0]
     da.coords['xx2'] = da.data['yy', 1]
     da.coords['yy'] = da.data['xx', 0]
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     snx.create_field(data, 'signal', da.data)
@@ -92,15 +95,16 @@
     data = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(data['xx', :2], da['xx', :2])
     assert sc.identical(data[:2], da['xx', :2])
 
 
 def test_slice_of_multiple_coords(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
     da.coords['xx'] = da.data['yy', 0]
     da.coords['xx2'] = da.data['yy', 1]
     da.coords['yy'] = da.data['xx', 0]
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     snx.create_field(data, 'signal', da.data)
@@ -109,28 +113,30 @@
     snx.create_field(data, 'yy', da.coords['yy'])
     data = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(data['xx', :2], da['xx', :2])
 
 
 def test_guessed_dim_for_2d_coord_not_matching_axis_name(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
     da.coords['xx2'] = da.data
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     snx.create_field(data, 'signal', da.data)
     snx.create_field(data, 'xx2', da.coords['xx2'])
     data = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(data[...], da)
 
 
 def test_skips_axis_if_dim_guessing_finds_ambiguous_shape(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6], [7, 8, 9]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6], [7, 8, 9]])
+    )
     da.coords['yy2'] = da.data['xx', 0]
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     snx.create_field(data, 'signal', da.data)
     snx.create_field(data, 'yy2', da.coords['yy2'])
     data = snx.Group(data, definitions=snx.base_definitions())
@@ -139,15 +145,16 @@
     assert isinstance(dg, sc.DataGroup)
     assert 'yy2' in dg
     assert set(dg.dims) == {'dim_0', 'xx', 'yy'}
 
 
 def test_guesses_transposed_dims_for_2d_coord(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
     da.coords['xx2'] = sc.transpose(da.data)
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     snx.create_field(data, 'signal', da.data)
     snx.create_field(data, 'xx2', da.coords['xx2'])
     data = snx.Group(data, definitions=snx.base_definitions())
@@ -193,62 +200,66 @@
     snx.create_field(data, 'xx2', da.coords['xx2'])
     data = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(data[...], da)
 
 
 def test_auxiliary_signal_causes_load_as_dataset(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
     da.coords['xx'] = da.data['xx', 0]
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     # We flag 'xx' as auxiliary_signal. It should thus not be loaded as a coord,
     # even though we create the field.
     data.attrs['auxiliary_signals'] = ['xx']
     snx.create_field(data, 'signal', da.data)
     snx.create_field(data, 'xx', da.coords['xx'])
     data = snx.Group(data, definitions=snx.base_definitions())
     assert_identical(data[...], sc.Dataset({'signal': da.data, 'xx': da.coords['xx']}))
 
 
 def test_NXlog_data_is_loaded_as_time_dependent_data_array(nxroot):
-    da = sc.DataArray(data=sc.array(dims=['time'], unit='K', values=[1, 2, 3]),
-                      coords={
-                          'time':
-                          sc.epoch(unit='s') +
-                          sc.array(dims=['time'], unit='s', values=[1, 2, 3])
-                      })
+    da = sc.DataArray(
+        data=sc.array(dims=['time'], unit='K', values=[1, 2, 3]),
+        coords={
+            'time': sc.epoch(unit='s')
+            + sc.array(dims=['time'], unit='s', values=[1, 2, 3])
+        },
+    )
     data = nxroot.create_class('data1', NXdata)
     log = data.create_class('data', NXlog)
     log['time'] = da.coords['time']
     log['value'] = da.data
     data._group.attrs['signal'] = 'data'
 
     loaded = data[()]
     assert_identical(loaded, da)
 
 
 @pytest.mark.parametrize("time_unit", ['m', None])
 def test_NXlog_with_nontime_time_axis_can_be_loaded(nxroot, time_unit):
     da = sc.DataArray(
         data=sc.array(dims=['time'], unit='K', values=[1, 2, 3]),
-        coords={'time': sc.array(dims=['time'], unit=time_unit, values=[1, 2, 3])})
+        coords={'time': sc.array(dims=['time'], unit=time_unit, values=[1, 2, 3])},
+    )
     data = nxroot.create_class('data1', NXdata)
     log = data.create_class('data', NXlog)
     log['time'] = da.coords['time']
     log['value'] = da.data
     loaded = data[()]
     assert_identical(loaded, da)
     assert loaded.coords['time'].dtype != sc.DType.datetime64
 
 
 def test_field_dims_match_NXdata_dims(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
     da.coords['xx'] = da.data['yy', 0]
     da.coords['xx2'] = da.data['yy', 1]
     da.coords['yy'] = da.data['xx', 0]
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal1'
     snx.create_field(data, 'signal1', da.data)
@@ -260,36 +271,38 @@
     assert sc.identical(data['xx', :2].coords['xx'], data['xx']['xx', :2])
     assert sc.identical(data['xx', :2].coords['xx2'], data['xx2']['xx', :2])
     assert sc.identical(data['xx', :2].coords['yy'], data['yy'][:])
 
 
 def test_field_dims_match_NXdata_dims_when_selected_via_class_name(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
     da.coords['xx'] = da.data['yy', 0]
     da.coords['xx2'] = da.data['yy', 1]
     da.coords['yy'] = da.data['xx', 0]
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal1'
     snx.create_field(data, 'signal1', da.data)
     snx.create_field(data, 'xx', da.coords['xx'])
     snx.create_field(data, 'xx2', da.coords['xx2'])
     snx.create_field(data, 'yy', da.coords['yy'])
     data = snx.Group(data, definitions=snx.base_definitions())
     fields = data[snx.Field]
     assert fields['signal1'].dims == ('xx', 'yy')
-    assert fields['xx'].dims == ('xx', )
-    assert fields['xx2'].dims == ('xx', )
-    assert fields['yy'].dims == ('yy', )
+    assert fields['xx'].dims == ('xx',)
+    assert fields['xx2'].dims == ('xx',)
+    assert fields['yy'].dims == ('yy',)
 
 
 def test_uses_default_field_dims_if_inference_fails(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
     yy2 = sc.arange('yy', 5)
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     snx.create_field(data, 'signal', da.data)
     snx.create_field(data, 'yy2', yy2)
     data = snx.Group(data, definitions=snx.base_definitions())
@@ -306,15 +319,16 @@
     loaded = group['field'][...]
     # Nexus does not support storing dim labels
     assert sc.identical(loaded, var.rename(xx=loaded.dim))
 
 
 def test_create_datetime_field_from_variable(h5root):
     var = sc.datetime(np.datetime64('now'), unit='ns') + sc.arange(
-        'time', 1, 4, dtype='int64', unit='ns')
+        'time', 1, 4, dtype='int64', unit='ns'
+    )
     snx.create_field(h5root, 'field', var)
     group = snx.Group(h5root, definitions=snx.base_definitions())
     loaded = group['field'][...]
     # Nexus does not support storing dim labels
     assert sc.identical(loaded, var.rename(time=loaded.dim))
 
 
@@ -322,55 +336,54 @@
 def test_create_class(nxroot, nx_class):
     group = nxroot.create_class('group', nx_class)
     assert group.nx_class == nx_class
 
 
 def test_deprecated_errors_field_is_used_for_signal_errors(h5root):
     data = snx.create_class(h5root, 'data1', NXdata)
-    values = sc.array(dims=['xx', 'yy'], unit='m', values=[[1., 2, 3], [4, 5, 6]])
-    errors = sc.array(dims=['xx', 'yy'], unit='m', values=[[0., 2, 3], [0, 5, 6]])
+    values = sc.array(dims=['xx', 'yy'], unit='m', values=[[1.0, 2, 3], [4, 5, 6]])
+    errors = sc.array(dims=['xx', 'yy'], unit='m', values=[[0.0, 2, 3], [0, 5, 6]])
     data.attrs['axes'] = values.dims
     data.attrs['signal'] = 'data'
     snx.create_field(data, 'data', values)
     snx.create_field(data, 'errors', errors)
     data = snx.Group(data, definitions=snx.base_definitions())
     loaded = data[()]
     assert_identical(sc.values(loaded), sc.DataArray(values))
     assert_identical(sc.stddevs(loaded), sc.DataArray(errors))
 
 
 @pytest.mark.parametrize("errors_suffix", ['_error', '_errors'])
 def test_field_matching_errors_regex_is_loaded_if_no_corresponding_value_field(
-        h5root, errors_suffix):
+    h5root, errors_suffix
+):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
     da.coords[f'xx{errors_suffix}'] = da.data['yy', 0]
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     snx.create_field(data, 'signal', da.data)
     snx.create_field(data, f'xx{errors_suffix}', da.coords[f'xx{errors_suffix}'])
     data = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(data[...], da)
 
 
 @pytest.mark.parametrize("errors_suffix", ['_error', '_errors'])
 def test_uncertainties_of_coords_are_loaded(h5root, errors_suffix):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]]))
-    da.coords['xx'] = sc.array(dims=['xx'],
-                               unit='m',
-                               values=[1, 2, 3],
-                               variances=[1, 4, 9],
-                               dtype='float64')
-    da.coords['xx2'] = sc.array(dims=['xx'],
-                                unit='m',
-                                values=[2, 3],
-                                variances=[4, 9],
-                                dtype='float64')
+        sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2, 3], [4, 5, 6]])
+    )
+    da.coords['xx'] = sc.array(
+        dims=['xx'], unit='m', values=[1, 2, 3], variances=[1, 4, 9], dtype='float64'
+    )
+    da.coords['xx2'] = sc.array(
+        dims=['xx'], unit='m', values=[2, 3], variances=[4, 9], dtype='float64'
+    )
     da.coords['scalar'] = sc.scalar(value=1.2, variance=4.0, unit='K')
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     data.attrs['xx2_indices'] = 0
     snx.create_field(data, 'signal', da.data)
     snx.create_field(data, 'xx', sc.values(da.coords['xx']))
@@ -408,15 +421,15 @@
     # shape=[2,1]
     xx = sc.array(dims=['xx', 'ignored'], values=[[1.1], [2.2]])
     snx.create_field(data, 'xx', xx)
     data = snx.Group(data, definitions=snx.base_definitions())
     loaded = data[...]
     assert sc.identical(loaded.coords['xx'], xx['ignored', 0])
     assert data['xx'].ndim == 1
-    assert data['xx'].shape == (2, )
+    assert data['xx'].shape == (2,)
     assert sc.identical(data['xx'][...], xx['ignored', 0])
 
 
 def test_dims_of_length_1_are_kept_when_axes_specified(h5root):
     signal = sc.array(dims=['xx', 'yy'], unit='m', values=[[1.1]])
     data = snx.create_class(h5root, 'data1', NXdata)
     snx.create_field(data, 'signal', signal)
@@ -444,30 +457,32 @@
 def test_multi_dims_of_length_1_are_kept_when_no_axes_specified(h5root):
     signal = sc.array(dims=['xx', 'yy'], unit='m', values=[[1.1]])
     data = snx.create_class(h5root, 'data1', NXdata)
     snx.create_field(data, 'signal', signal)
     data.attrs['signal'] = 'signal'
     data = snx.Group(data, definitions=snx.base_definitions())
     loaded = data[...]
-    assert sc.identical(loaded.data,
-                        sc.array(dims=['dim_0', 'dim_1'], unit='m', values=[[1.1]]))
+    assert sc.identical(
+        loaded.data, sc.array(dims=['dim_0', 'dim_1'], unit='m', values=[[1.1]])
+    )
     assert data['signal'].ndim == 2
     assert data['signal'].shape == (1, 1)
 
 
 def test_one_dim_of_length_1_is_kept_when_no_axes_specified(h5root):
     signal = sc.array(dims=['xx', 'yy'], unit='m', values=[[1.1, 2.2]])
     data = snx.create_class(h5root, 'data1', NXdata)
     snx.create_field(data, 'signal', signal)
     data.attrs['signal'] = 'signal'
     data = snx.Group(data, definitions=snx.base_definitions())
     loaded = data[...]
     # Note that dimension gets renamed to `dim_0` since no axes are specified
     assert sc.identical(
-        loaded.data, sc.array(dims=['dim_0', 'dim_1'], unit='m', values=[[1.1, 2.2]]))
+        loaded.data, sc.array(dims=['dim_0', 'dim_1'], unit='m', values=[[1.1, 2.2]])
+    )
     assert data['signal'].ndim == 2
     assert data['signal'].shape == (1, 2)
     assert data['signal'].dims == ('dim_0', 'dim_1')
 
 
 def test_only_one_axis_specified_for_2d_field(h5root):
     signal = sc.array(dims=['xx', 'yy'], unit='m', values=[[1.1]])
@@ -478,16 +493,17 @@
     data = snx.Group(data, definitions=snx.base_definitions())
     loaded = data[...]
     assert sc.identical(loaded.data, sc.array(dims=['zz'], unit='m', values=[1.1]))
 
 
 def test_fields_with_datetime_attribute_are_loaded_as_datetime(h5root):
     da = sc.DataArray(
-        sc.epoch(unit='s') +
-        sc.array(dims=['xx', 'yy'], unit='s', values=[[1, 2, 3], [4, 5, 6]]))
+        sc.epoch(unit='s')
+        + sc.array(dims=['xx', 'yy'], unit='s', values=[[1, 2, 3], [4, 5, 6]])
+    )
     da.coords['xx'] = da.data['yy', 0]
     da.coords['xx2'] = da.data['yy', 1]
     da.coords['yy'] = da.data['xx', 0]
     data = snx.create_class(h5root, 'data1', NXdata)
     data.attrs['axes'] = da.dims
     data.attrs['signal'] = 'signal'
     snx.create_field(data, 'signal', da.data)
@@ -551,57 +567,76 @@
     signal.attrs['signal'] = 1
     xx.attrs['axis'] = 1
     yy.attrs['axis'] = 2
     data = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(data[...], da)
 
 
-def test_alternative_legacy_axis_attrs_with_signal_axes(h5root):
+@pytest.mark.parametrize('axis_sep', [':', ','])
+def test_alternative_legacy_axis_attrs_with_signal_axes(h5root, axis_sep):
     da = sc.DataArray(sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2], [4, 5]]))
     da.coords['xx'] = da.data['yy', 0]
     da.coords['yy'] = da.data['xx', 0]
     data = snx.create_class(h5root, 'data1', NXdata)
     signal = snx.create_field(data, 'signal', da.data)
     xx = snx.create_field(data, 'xx', da.coords['xx'])
     yy = snx.create_field(data, 'yy', da.coords['yy'])
     signal.attrs['signal'] = 1
     # According to personal communication with Tobias Richter, the legacy 'axis'
     # attributes may have been used with two different meanings:
     # 1. As a 1-based integer (see other tests)
     # 2. As a boolean, where "1" means that the field is an axis.
     # In the latter case it appears to be useless since axis order cannot be inferred,
     # and we ignore the value if the signal has an `axes` attribute.
-    signal.attrs['axes'] = 'xx,yy'
+    signal.attrs['axes'] = axis_sep.join(['xx', 'yy'])
+    xx.attrs['axis'] = 1
+    yy.attrs['axis'] = 1
+    data = snx.Group(data, definitions=snx.base_definitions())
+    assert sc.identical(data[...], da)
+
+
+def test_legacy_axis_favors_colon_sep(h5root):
+    da = sc.DataArray(sc.array(dims=['xx,zz', 'yy'], unit='m', values=[[1, 2], [4, 5]]))
+    da.coords['xx,zz'] = da.data['yy', 0]
+    da.coords['yy'] = da.data['xx,zz', 0]
+    data = snx.create_class(h5root, 'data1', NXdata)
+    signal = snx.create_field(data, 'signal', da.data)
+    xx = snx.create_field(data, 'xx,zz', da.coords['xx,zz'])
+    yy = snx.create_field(data, 'yy', da.coords['yy'])
+    signal.attrs['signal'] = 1
+    signal.attrs['axes'] = 'xx,zz:yy'
     xx.attrs['axis'] = 1
     yy.attrs['axis'] = 1
     data = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(data[...], da)
 
 
-def test_guesses_dims_of_bin_edge_fields(h5root):
+@pytest.mark.parametrize('axis_sep', [':', ','])
+def test_guesses_dims_of_bin_edge_fields(h5root, axis_sep):
     da = sc.DataArray(sc.ones(dims=['xx', 'yy'], unit='m', shape=(2, 4)))
     da.coords['xx2'] = sc.array(dims=['xx'], unit='m', values=[1, 2, 3])
     da.coords['yy2'] = sc.array(dims=['yy'], unit='m', values=[1, 2, 3, 4, 5])
     data = snx.create_class(h5root, 'data1', NXdata)
     signal = snx.create_field(data, 'signal', da.data)
     signal.attrs['signal'] = 1
-    signal.attrs['axes'] = 'xx,yy'
+    signal.attrs['axes'] = axis_sep.join(['xx', 'yy'])
     snx.create_field(data, 'xx2', da.coords['xx2'])
     snx.create_field(data, 'yy2', da.coords['yy2'])
     data = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(data[...], da)
 
 
-def test_guesses_dims_of_2d_bin_edge_fields(h5root):
+@pytest.mark.parametrize('axis_sep', [':', ','])
+def test_guesses_dims_of_2d_bin_edge_fields(h5root, axis_sep):
     da = sc.DataArray(sc.ones(dims=['xx', 'yy'], unit='m', shape=(2, 4)))
     da.coords['xx2'] = sc.ones(dims=['xx', 'yy'], unit='m', shape=(2, 5))
     data = snx.create_class(h5root, 'data1', NXdata)
     signal = snx.create_field(data, 'signal', da.data)
     signal.attrs['signal'] = 1
-    signal.attrs['axes'] = 'xx,yy'
+    signal.attrs['axes'] = axis_sep.join(['xx', 'yy'])
     snx.create_field(data, 'xx2', da.coords['xx2'])
     data = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(data[...], da)
 
 
 def test_nested_groups_trigger_fallback_to_load_as_data_group(h5root):
     da = sc.DataArray(sc.array(dims=['xx', 'yy'], unit='m', values=[[1, 2], [4, 5]]))
@@ -622,7 +657,20 @@
     data.attrs['signal'] = 'signal'
     data = snx.Group(data, definitions=snx.base_definitions())
     assert sc.identical(data[...], sc.DataArray(signal))
     with pytest.raises(IndexError):
         data['xx', 2]
     with pytest.raises(sc.DimensionError):
         data['zz', 0]
+
+
+def test_scalar_signal_without_unit_works(h5root):
+    da = sc.DataArray(
+        sc.scalar(1.1, unit=None), coords={'xx': sc.scalar(2.0, unit='m')}
+    )
+    data = snx.create_class(h5root, 'data1', snx.NXdata)
+    data.attrs['axes'] = []
+    data.attrs['signal'] = 'signal'
+    snx.create_field(data, 'signal', da.data)
+    snx.create_field(data, 'xx', da.coords['xx'])
+    group = snx.Group(data, definitions=snx.base_definitions())
+    assert sc.identical(group[...], da)
```

### Comparing `scippnexus-23.5.0/tests/nxdetector_test.py` & `scippnexus-23.5.1/tests/nxdetector_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,16 @@
     detector = snx.create_class(h5root, 'detector0', NXdetector)
     snx.create_field(detector, 'detector_numbers', detector_numbers)
     detector['detector_numbers'][...]
 
 
 def test_finds_data_from_group_attr(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]]))
+        sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
+    )
     da.coords['detector_numbers'] = detector_numbers_xx_yy_1234()
     detector = snx.create_class(h5root, 'detector0', NXdetector)
     snx.create_field(detector, 'detector_numbers', da.coords['detector_numbers'])
     snx.create_field(detector, 'custom', da.data)
     detector.attrs['signal'] = 'custom'
     detector = make_group(detector)
     assert sc.identical(detector[...], da.rename_dims({'xx': 'dim_0', 'yy': 'dim_1'}))
@@ -74,27 +75,29 @@
 
 
 def test_loads_as_data_array_with_embedded_events(nxroot):
     detector_number = sc.array(dims=[''], unit=None, values=np.array([1, 2, 3]))
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_number)
     detector.create_field('event_id', sc.array(dims=[''], unit=None, values=[1]))
-    detector.create_field('event_time_offset', sc.array(dims=[''], unit='s',
-                                                        values=[1]))
+    detector.create_field(
+        'event_time_offset', sc.array(dims=[''], unit='s', values=[1])
+    )
     detector.create_field('event_time_zero', sc.array(dims=[''], unit='s', values=[1]))
     detector.create_field('event_index', sc.array(dims=[''], unit='None', values=[0]))
     assert detector.dims == ('detector_number', 'event_time_zero')
     da = detector[...]
     assert da.bins is not None
     assert_identical(
         da.bins.size(),
         sc.DataArray(
             data=sc.array(dims=['detector_number'], unit=None, values=[1, 0, 0]),
-            coords={'detector_number': detector_number.rename({'':
-                                                               'detector_number'})}))
+            coords={'detector_number': detector_number.rename({'': 'detector_number'})},
+        ),
+    )
 
 
 def detector_numbers_xx_yy_1234():
     return sc.array(dims=['xx', 'yy'], unit=None, values=np.array([[1, 2], [3, 4]]))
 
 
 def test_loads_data_without_coords(h5root):
@@ -103,53 +106,55 @@
     detector = snx.create_class(h5root, 'detector0', NXdetector)
     snx.create_field(detector, 'detector_numbers', da.coords['detector_numbers'])
     snx.create_field(detector, 'data', da.data)
     detector = make_group(detector)
     assert sc.identical(detector[...], da.rename_dims({'xx': 'dim_0', 'yy': 'dim_1'}))
 
 
-@pytest.mark.parametrize('detector_number_key',
-                         ['detector_number', 'pixel_id', 'spectrum_index'])
+@pytest.mark.parametrize(
+    'detector_number_key', ['detector_number', 'pixel_id', 'spectrum_index']
+)
 def test_detector_number_key_alias(h5root, detector_number_key):
     da = sc.DataArray(sc.array(dims=['xx', 'yy'], values=[[1.1, 2.2], [3.3, 4.4]]))
     da.coords[detector_number_key] = detector_numbers_xx_yy_1234()
     detector = snx.create_class(h5root, 'detector0', NXdetector)
     snx.create_field(detector, detector_number_key, da.coords[detector_number_key])
     snx.create_field(detector, 'data', da.data)
     detector = make_group(detector)
     assert sc.identical(detector[...], da.rename_dims({'xx': 'dim_0', 'yy': 'dim_1'}))
 
 
 def test_loads_data_with_coords(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]]))
+        sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
+    )
     da.coords['detector_numbers'] = detector_numbers_xx_yy_1234()
     da.coords['xx'] = sc.array(dims=['xx'], unit='m', values=[0.1, 0.2])
     detector = snx.create_class(h5root, 'detector0', NXdetector)
     snx.create_field(detector, 'detector_numbers', da.coords['detector_numbers'])
     snx.create_field(detector, 'xx', da.coords['xx'])
     snx.create_field(detector, 'data', da.data)
     detector.attrs['axes'] = ['xx', '.']
     detector = make_group(detector)
     assert sc.identical(detector[...], da.rename_dims({'yy': 'dim_1'}))
 
 
 def test_slicing_works_as_in_scipp(h5root):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2, 3.3], [3.3, 4.4,
-                                                                        5.5]]))
-    da.coords['detector_numbers'] = sc.array(dims=['xx', 'yy'],
-                                             unit=None,
-                                             values=np.array([[1, 2, 3], [4, 5, 6]]))
+        sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2, 3.3], [3.3, 4.4, 5.5]])
+    )
+    da.coords['detector_numbers'] = sc.array(
+        dims=['xx', 'yy'], unit=None, values=np.array([[1, 2, 3], [4, 5, 6]])
+    )
     da.coords['xx'] = sc.array(dims=['xx'], unit='m', values=[0.1, 0.2])
     da.coords['xx2'] = sc.array(dims=['xx'], unit='m', values=[0.3, 0.4])
     da.coords['yy'] = sc.array(dims=['yy'], unit='m', values=[0.1, 0.2, 0.3])
-    da.coords['2d_edges'] = sc.array(dims=['yy', 'xx'],
-                                     unit='m',
-                                     values=[[1, 2, 3], [4, 5, 6], [7, 8, 9]])
+    da.coords['2d_edges'] = sc.array(
+        dims=['yy', 'xx'], unit='m', values=[[1, 2, 3], [4, 5, 6], [7, 8, 9]]
+    )
     detector = snx.create_class(h5root, 'detector0', NXdetector)
     snx.create_field(detector, 'detector_numbers', da.coords['detector_numbers'])
     snx.create_field(detector, 'xx', da.coords['xx'])
     snx.create_field(detector, 'xx2', da.coords['xx2'])
     snx.create_field(detector, 'yy', da.coords['yy'])
     snx.create_field(detector, '2d_edges', da.coords['2d_edges'])
     snx.create_field(detector, 'data', da.data)
@@ -163,183 +168,198 @@
     assert_identical(detector['yy', 0], da['yy', 0])
     assert_identical(detector['yy', 1], da['yy', 1])
     assert_identical(detector['yy', 0:1], da['yy', 0:1])
     assert_identical(detector['yy', 1:1], da['yy', 1:1])  # empty slice
 
 
 def create_event_data_ids_1234(group):
-    group.create_field('event_id',
-                       sc.array(dims=[''], unit=None, values=[1, 2, 4, 1, 2, 2]))
-    group.create_field('event_time_offset',
-                       sc.array(dims=[''], unit='s', values=[456, 7, 3, 345, 632, 23]))
-    group.create_field('event_time_zero',
-                       sc.array(dims=[''], unit='s', values=[1, 2, 3, 4]))
-    group.create_field('event_index',
-                       sc.array(dims=[''], unit='None', values=[0, 3, 3, 5]))
+    group.create_field(
+        'event_id', sc.array(dims=[''], unit=None, values=[1, 2, 4, 1, 2, 2])
+    )
+    group.create_field(
+        'event_time_offset',
+        sc.array(dims=[''], unit='s', values=[456, 7, 3, 345, 632, 23]),
+    )
+    group.create_field(
+        'event_time_zero', sc.array(dims=[''], unit='s', values=[1, 2, 3, 4])
+    )
+    group.create_field(
+        'event_index', sc.array(dims=[''], unit='None', values=[0, 3, 3, 5])
+    )
 
 
 def test_loads_event_data_mapped_to_detector_numbers_based_on_their_event_id(nxroot):
-    detector_numbers = sc.array(dims=[''],
-                                unit=None,
-                                values=np.array([1, 2, 3, 4, 5, 6]))
+    detector_numbers = sc.array(
+        dims=[''], unit=None, values=np.array([1, 2, 3, 4, 5, 6])
+    )
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers)
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
     assert detector.sizes == {'detector_number': 6, 'event_time_zero': 4}
     da = detector[...]
     assert sc.identical(
         da.bins.size().data,
-        sc.array(dims=['detector_number'],
-                 unit=None,
-                 dtype='int64',
-                 values=[2, 3, 0, 1, 0, 0]))
+        sc.array(
+            dims=['detector_number'],
+            unit=None,
+            dtype='int64',
+            values=[2, 3, 0, 1, 0, 0],
+        ),
+    )
     assert 'event_time_offset' in da.bins.coords
     assert 'event_time_zero' in da.bins.coords
 
 
 def test_detector_number_fallback_dims_determines_dims_with_event_data(nxroot):
-    detector_numbers = sc.array(dims=['detector_number'],
-                                unit=None,
-                                values=np.array([1, 2, 3, 4, 5, 6]))
+    detector_numbers = sc.array(
+        dims=['detector_number'], unit=None, values=np.array([1, 2, 3, 4, 5, 6])
+    )
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers)
     detector.create_field('pixel_offset', detector_numbers)
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
     da = detector[()]
     assert da.sizes == {'detector_number': 6}
     assert_identical(da.coords['pixel_offset'], detector_numbers)
 
 
 def test_loads_event_data_with_0d_detector_numbers(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', sc.index(1, dtype='int64'))
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
-    assert detector.dims == ('event_time_zero', )
-    assert detector.shape == (4, )
+    assert detector.dims == ('event_time_zero',)
+    assert detector.shape == (4,)
     da = detector[...]
     assert sc.identical(da.bins.size().data, sc.index(2, dtype='int64'))
 
 
 def test_loads_event_data_with_2d_detector_numbers(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers_xx_yy_1234())
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
     assert detector.sizes == {'dim_0': 2, 'dim_1': 2, 'event_time_zero': 4}
     da = detector[...]
     assert sc.identical(
         da.bins.size().data,
-        sc.array(dims=['dim_0', 'dim_1'],
-                 unit=None,
-                 dtype='int64',
-                 values=[[2, 3], [0, 1]]))
+        sc.array(
+            dims=['dim_0', 'dim_1'], unit=None, dtype='int64', values=[[2, 3], [0, 1]]
+        ),
+    )
 
 
 def test_selecting_pixels_works_with_event_signal(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers_xx_yy_1234())
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
     assert detector.sizes == {'dim_0': 2, 'dim_1': 2, 'event_time_zero': 4}
     da = detector['dim_0', 0]
-    assert_identical(da.bins.size().data,
-                     sc.array(dims=['dim_1'], unit=None, dtype='int64', values=[2, 3]))
+    assert_identical(
+        da.bins.size().data,
+        sc.array(dims=['dim_1'], unit=None, dtype='int64', values=[2, 3]),
+    )
 
 
 def test_selecting_pixels_works_with_embedded_event_signal(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers_xx_yy_1234())
     create_event_data_ids_1234(detector)
     assert detector.sizes == {'dim_0': 2, 'dim_1': 2, 'event_time_zero': 4}
     da = detector['dim_0', 0]
-    assert_identical(da.bins.size().data,
-                     sc.array(dims=['dim_1'], unit=None, dtype='int64', values=[2, 3]))
+    assert_identical(
+        da.bins.size().data,
+        sc.array(dims=['dim_1'], unit=None, dtype='int64', values=[2, 3]),
+    )
 
 
 def test_select_events_slices_underlying_event_data(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers_xx_yy_1234())
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
     da = detector['event_time_zero', :2]
     assert sc.identical(
         da.bins.size().data,
-        sc.array(dims=['dim_0', 'dim_1'],
-                 unit=None,
-                 dtype='int64',
-                 values=[[1, 1], [0, 1]]))
+        sc.array(
+            dims=['dim_0', 'dim_1'], unit=None, dtype='int64', values=[[1, 1], [0, 1]]
+        ),
+    )
     da = detector['event_time_zero', :3]
     assert sc.identical(
         da.bins.size().data,
-        sc.array(dims=['dim_0', 'dim_1'],
-                 unit=None,
-                 dtype='int64',
-                 values=[[2, 2], [0, 1]]))
+        sc.array(
+            dims=['dim_0', 'dim_1'], unit=None, dtype='int64', values=[[2, 2], [0, 1]]
+        ),
+    )
     da = detector['event_time_zero', 3]
     assert sc.identical(
         da.bins.size().data,
-        sc.array(dims=['dim_0', 'dim_1'],
-                 unit=None,
-                 dtype='int64',
-                 values=[[0, 1], [0, 0]]))
+        sc.array(
+            dims=['dim_0', 'dim_1'], unit=None, dtype='int64', values=[[0, 1], [0, 0]]
+        ),
+    )
     da = detector[()]
     assert sc.identical(
         da.bins.size().data,
-        sc.array(dims=['dim_0', 'dim_1'],
-                 unit=None,
-                 dtype='int64',
-                 values=[[2, 3], [0, 1]]))
+        sc.array(
+            dims=['dim_0', 'dim_1'], unit=None, dtype='int64', values=[[2, 3], [0, 1]]
+        ),
+    )
 
 
 def test_loading_event_data_without_detector_numbers_does_not_group_events(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
-    assert detector.dims == ('event_time_zero', )
+    assert detector.dims == ('event_time_zero',)
     da = detector[...]
     assert_identical(
         da.bins.size().data,
-        sc.array(dims=['event_time_zero'],
-                 unit=None,
-                 dtype='int64',
-                 values=[3, 0, 2, 1]))
+        sc.array(
+            dims=['event_time_zero'], unit=None, dtype='int64', values=[3, 0, 2, 1]
+        ),
+    )
 
 
 def test_loading_event_data_with_det_selection_and_automatic_detector_numbers_raises(
-        nxroot):
+    nxroot,
+):
     detector = nxroot.create_class('detector0', NXdetector)
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
-    assert detector.dims == ('event_time_zero', )
+    assert detector.dims == ('event_time_zero',)
     with pytest.raises(sc.DimensionError):
         detector['detector_number', 0]
 
 
 def test_loading_event_data_with_full_selection_and_automatic_detector_numbers_works(
-        nxroot):
+    nxroot,
+):
     detector = nxroot.create_class('detector0', NXdetector)
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
-    assert detector.dims == ('event_time_zero', )
-    assert tuple(detector[...].shape) == (4, )
-    assert tuple(detector[()].shape) == (4, )
+    assert detector.dims == ('event_time_zero',)
+    assert tuple(detector[...].shape) == (4,)
+    assert tuple(detector[()].shape) == (4,)
 
 
 def test_event_data_field_dims_labels(nxroot):
     detector_numbers = sc.array(dims=[''], unit=None, values=np.array([1, 2, 3, 4]))
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers)
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
-    assert detector['detector_number'].dims == ('detector_number', )
+    assert detector['detector_number'].dims == ('detector_number',)
 
 
 def test_nxevent_data_without_detector_number_selection_yields_correct_pulses(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
 
     class Load:
-
         def __getitem__(self, select=...):
             da = detector[select]
-            assert da.bins.size().sum(
-            ).value == da.bins.constituents['data'].sizes['event']
+            assert (
+                da.bins.size().sum().value
+                == da.bins.constituents['data'].sizes['event']
+            )
             return da.bins.size().values
 
     assert np.array_equal(Load()[...], [3, 0, 2, 1])
     assert np.array_equal(Load()['event_time_zero', 0], 3)
     assert np.array_equal(Load()['event_time_zero', 1], 0)
     assert np.array_equal(Load()['event_time_zero', 3], 1)
     assert np.array_equal(Load()['event_time_zero', -1], 1)
@@ -360,15 +380,14 @@
 def test_nxevent_data_selection_yields_correct_pulses(nxroot):
     detector_numbers = sc.array(dims=[''], unit=None, values=np.array([1, 2, 3, 4]))
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers)
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
 
     class Load:
-
         def __getitem__(self, select=...):
             da = detector[select]
             return da.bins.size().values
 
     assert np.array_equal(Load()[...], [2, 3, 0, 1])
     assert np.array_equal(Load()['event_time_zero', 0], [1, 1, 0, 1])
     assert np.array_equal(Load()['event_time_zero', 1], [0, 0, 0, 0])
@@ -385,194 +404,219 @@
     assert np.array_equal(Load()['event_time_zero', 0:-3], [1, 1, 0, 1])
     assert np.array_equal(Load()['event_time_zero', -1:], [0, 1, 0, 0])
     assert np.array_equal(Load()['event_time_zero', -2:-1], [1, 1, 0, 0])
     assert np.array_equal(Load()['event_time_zero', -2:], [1, 2, 0, 0])
     assert np.array_equal(Load()['event_time_zero', :-2], [1, 1, 0, 1])
 
 
-def create_off_geometry_detector_numbers_1234(group: snx.Group,
-                                              name: str,
-                                              detector_faces: bool = True
-                                              ) -> sc.DataGroup:
+def create_off_geometry_detector_numbers_1234(
+    group: snx.Group, name: str, detector_faces: bool = True
+) -> sc.DataGroup:
     dg = sc.DataGroup()
     off = group.create_class(name, NXoff_geometry)
     # square with point in center
     values = np.array([[0, 0, 0], [0, 1, 0], [1, 0, 0], [1, 1, 0], [0.5, 0.5, 0]])
     dg['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
     # triangles
-    dg['winding_order'] = sc.array(dims=['winding_order'],
-                                   values=[0, 1, 4, 1, 2, 4, 2, 3, 4, 3, 0, 4],
-                                   unit=None)
+    dg['winding_order'] = sc.array(
+        dims=['winding_order'], values=[0, 1, 4, 1, 2, 4, 2, 3, 4, 3, 0, 4], unit=None
+    )
     dg['faces'] = sc.array(dims=['face'], values=[0, 3, 6, 9], unit=None)
     if detector_faces:
-        dg['detector_faces'] = sc.array(dims=['face', 'face_index|detector_number'],
-                                        values=[[0, 1], [1, 2], [2, 3], [3, 4]],
-                                        unit=None)
+        dg['detector_faces'] = sc.array(
+            dims=['face', 'face_index|detector_number'],
+            values=[[0, 1], [1, 2], [2, 3], [3, 4]],
+            unit=None,
+        )
     for name, var in dg.items():
         off[name] = var
     dg['vertices'] = sc.vectors(dims=['vertex'], values=values, unit='m')
     return dg
 
 
-@pytest.mark.parametrize('detid_name',
-                         ['detector_number', 'pixel_id', 'spectrum_index'])
+@pytest.mark.parametrize(
+    'detid_name', ['detector_number', 'pixel_id', 'spectrum_index']
+)
 def test_loads_data_with_coords_and_off_geometry(nxroot, detid_name):
     da = sc.DataArray(
-        sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]]))
+        sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
+    )
     da.coords['detector_number'] = detector_numbers_xx_yy_1234()
     da.coords['xx'] = sc.array(dims=['xx'], unit='m', values=[0.1, 0.2])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field(detid_name, da.coords['detector_number'])
     detector.create_field('xx', da.coords['xx'])
     detector.create_field('data', da.data)
     detector._group.attrs['axes'] = ['xx', 'yy']
     expected = create_off_geometry_detector_numbers_1234(detector, name='shape')
     loaded = detector[...]
     assert_identical(loaded.coords['shape'].value, expected)
 
 
 def test_missing_detector_numbers_given_off_geometry_with_det_faces_loads_as_usual(
-        nxroot):
+    nxroot,
+):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
     detector._group.attrs['axes'] = ['xx', 'yy']
     expected = create_off_geometry_detector_numbers_1234(detector, name='shape')
     loaded = detector[...]
     assert_identical(loaded.coords['shape'].value, expected)
 
 
 def test_off_geometry_without_detector_faces_loaded_as_0d_with_multiple_faces(nxroot):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
     detector._group.attrs['axes'] = ['xx', 'yy']
-    expected = create_off_geometry_detector_numbers_1234(detector,
-                                                         name='shape',
-                                                         detector_faces=False)
+    expected = create_off_geometry_detector_numbers_1234(
+        detector, name='shape', detector_faces=False
+    )
     loaded = detector[...]
     assert_identical(loaded.coords['shape'].value, expected)
     shape = snx.NXoff_geometry.assemble_as_child(loaded.coords['shape'].value)
     assert sc.identical(shape.bins.size(), sc.index(4))
 
 
-def create_cylindrical_geometry_detector_numbers_1234(group: snx.Group,
-                                                      name: str,
-                                                      detector_numbers: bool = True
-                                                      ) -> sc.DataGroup:
+def create_cylindrical_geometry_detector_numbers_1234(
+    group: snx.Group, name: str, detector_numbers: bool = True
+) -> sc.DataGroup:
     shape = group.create_class(name, snx.NXcylindrical_geometry)
     values = np.array([[0, 0, 0], [0, 1, 0], [3, 0, 0]])
     dg = sc.DataGroup()
     dg['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
-    dg['cylinders'] = sc.array(dims=['cylinder', 'vertex_index'],
-                               values=[[0, 1, 2], [2, 1, 0]],
-                               unit=None)
+    dg['cylinders'] = sc.array(
+        dims=['cylinder', 'vertex_index'], values=[[0, 1, 2], [2, 1, 0]], unit=None
+    )
     if detector_numbers:
-        dg['detector_number'] = sc.array(dims=['detector_number'],
-                                         values=[0, 1, 1, 0],
-                                         unit=None)
+        dg['detector_number'] = sc.array(
+            dims=['detector_number'], values=[0, 1, 1, 0], unit=None
+        )
     for name, var in dg.items():
         shape[name] = var
     dg['vertices'] = sc.vectors(dims=['vertex'], values=values, unit='m')
     return dg
 
 
 def test_cylindrical_geometry_without_detector_numbers_loaded_as_0d(nxroot):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
     detector._group.attrs['axes'] = ['xx', 'yy']
-    expected = create_cylindrical_geometry_detector_numbers_1234(detector,
-                                                                 name='shape',
-                                                                 detector_numbers=False)
+    expected = create_cylindrical_geometry_detector_numbers_1234(
+        detector, name='shape', detector_numbers=False
+    )
     loaded = detector[...]
     assert_identical(loaded.coords['shape'].value, expected)
     shape = snx.NXcylindrical_geometry.assemble_as_child(loaded.coords['shape'].value)
     assert shape.dims == ()
     assert sc.identical(shape.bins.size(), sc.index(2))
     assert sc.identical(
         shape.value,
-        sc.Dataset({
-            'face1_center':
-            sc.vectors(dims=['cylinder'], values=[[0, 0, 0], [3, 0, 0]], unit='m'),
-            'face1_edge':
-            sc.vectors(dims=['cylinder'], values=[[0, 1, 0], [0, 1, 0]], unit='m'),
-            'face2_center':
-            sc.vectors(dims=['cylinder'], values=[[3, 0, 0], [0, 0, 0]], unit='m'),
-        }))
+        sc.Dataset(
+            {
+                'face1_center': sc.vectors(
+                    dims=['cylinder'], values=[[0, 0, 0], [3, 0, 0]], unit='m'
+                ),
+                'face1_edge': sc.vectors(
+                    dims=['cylinder'], values=[[0, 1, 0], [0, 1, 0]], unit='m'
+                ),
+                'face2_center': sc.vectors(
+                    dims=['cylinder'], values=[[3, 0, 0], [0, 0, 0]], unit='m'
+                ),
+            }
+        ),
+    )
 
 
 def test_cylindrical_geometry_with_missing_parent_detector_numbers_loads_as_usual(
-        nxroot):
+    nxroot,
+):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
     detector._group.attrs['axes'] = ['xx', 'yy']
-    expected = create_cylindrical_geometry_detector_numbers_1234(detector,
-                                                                 name='shape',
-                                                                 detector_numbers=True)
+    expected = create_cylindrical_geometry_detector_numbers_1234(
+        detector, name='shape', detector_numbers=True
+    )
     loaded = detector[...]
     assert_identical(loaded.coords['shape'].value, expected)
 
 
 def test_cylindrical_geometry_with_inconsistent_detector_numbers_loads_as_usual(nxroot):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1], [3.3]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
     detector._group.attrs['axes'] = ['xx', 'yy']
-    detector.create_field('detector_number',
-                          sc.array(dims=var.dims, values=[[1], [2]], unit=None))
-    expected = create_cylindrical_geometry_detector_numbers_1234(detector,
-                                                                 name='shape',
-                                                                 detector_numbers=True)
+    detector.create_field(
+        'detector_number', sc.array(dims=var.dims, values=[[1], [2]], unit=None)
+    )
+    expected = create_cylindrical_geometry_detector_numbers_1234(
+        detector, name='shape', detector_numbers=True
+    )
     loaded = detector[...]
     assert_identical(loaded.coords['shape'].value, expected)
     detector_number = loaded.coords['detector_number']
     with pytest.raises(snx.NexusStructureError):
-        snx.NXcylindrical_geometry.assemble_as_child(loaded.coords['shape'].value,
-                                                     detector_number=detector_number)
+        snx.NXcylindrical_geometry.assemble_as_child(
+            loaded.coords['shape'].value, detector_number=detector_number
+        )
 
 
 def test_cylindrical_geometry_with_detector_numbers(nxroot):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
     detector._group.attrs['axes'] = ['xx', 'yy']
     detector_number = sc.array(dims=var.dims, values=[[1, 2], [3, 4]], unit=None)
     detector.create_field('detector_number', detector_number)
-    expected = create_cylindrical_geometry_detector_numbers_1234(detector,
-                                                                 name='shape',
-                                                                 detector_numbers=True)
+    expected = create_cylindrical_geometry_detector_numbers_1234(
+        detector, name='shape', detector_numbers=True
+    )
     loaded = detector[...]
     assert_identical(loaded.coords['shape'].value, expected)
     shape = snx.NXcylindrical_geometry.assemble_as_child(
-        loaded.coords['shape'].value, detector_number=loaded.coords['detector_number'])
+        loaded.coords['shape'].value, detector_number=loaded.coords['detector_number']
+    )
     assert shape.dims == detector_number.dims
     for i in [0, 3]:
         assert sc.identical(
             shape.values[i],
-            sc.Dataset({
-                'face1_center':
-                sc.vectors(dims=['cylinder'], values=[[0, 0, 0]], unit='m'),
-                'face1_edge':
-                sc.vectors(dims=['cylinder'], values=[[0, 1, 0]], unit='m'),
-                'face2_center':
-                sc.vectors(dims=['cylinder'], values=[[3, 0, 0]], unit='m'),
-            }))
+            sc.Dataset(
+                {
+                    'face1_center': sc.vectors(
+                        dims=['cylinder'], values=[[0, 0, 0]], unit='m'
+                    ),
+                    'face1_edge': sc.vectors(
+                        dims=['cylinder'], values=[[0, 1, 0]], unit='m'
+                    ),
+                    'face2_center': sc.vectors(
+                        dims=['cylinder'], values=[[3, 0, 0]], unit='m'
+                    ),
+                }
+            ),
+        )
     for i in [1, 2]:
         assert sc.identical(
             shape.values[i],
-            sc.Dataset({
-                'face1_center':
-                sc.vectors(dims=['cylinder'], values=[[3, 0, 0]], unit='m'),
-                'face1_edge':
-                sc.vectors(dims=['cylinder'], values=[[0, 1, 0]], unit='m'),
-                'face2_center':
-                sc.vectors(dims=['cylinder'], values=[[0, 0, 0]], unit='m'),
-            }))
+            sc.Dataset(
+                {
+                    'face1_center': sc.vectors(
+                        dims=['cylinder'], values=[[3, 0, 0]], unit='m'
+                    ),
+                    'face1_edge': sc.vectors(
+                        dims=['cylinder'], values=[[0, 1, 0]], unit='m'
+                    ),
+                    'face2_center': sc.vectors(
+                        dims=['cylinder'], values=[[0, 0, 0]], unit='m'
+                    ),
+                }
+            ),
+        )
 
 
 def test_falls_back_to_hdf5_dim_labels(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     xy = sc.array(dims=['x', 'y'], values=[[1, 2], [3, 4]])
     z = sc.array(dims=['z'], values=[1, 2, 3])
     dataset = detector.create_field('xy', xy)
```

### Comparing `scippnexus-23.5.0/tests/nxevent_data_test.py` & `scippnexus-23.5.1/tests/nxevent_data_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         root = snx.Group(f, definitions=snx.base_definitions())
         root.create_class('entry', snx.NXentry)
         yield root
 
 
 def create_event_data_ids_1234(group):
     group['event_id'] = sc.array(dims=[''], unit=None, values=[1, 2, 4, 1, 2, 2])
-    group['event_time_offset'] = sc.array(dims=[''],
-                                          unit='s',
-                                          values=[456, 7, 3, 345, 632, 23])
+    group['event_time_offset'] = sc.array(
+        dims=[''], unit='s', values=[456, 7, 3, 345, 632, 23]
+    )
     group['event_time_zero'] = sc.array(dims=[''], unit='s', values=[1, 2, 3, 4])
     group['event_index'] = sc.array(dims=[''], unit=None, values=[0, 3, 3, -1000])
 
 
 def test_negative_event_index_converted_to_num_event(nxroot):
     event_data = nxroot['entry'].create_class('events_0', snx.NXevent_data)
     create_event_data_ids_1234(event_data)
@@ -49,17 +49,17 @@
     event_data['event_time_zero'] = sc.array(dims=[''], unit='s', values=[1, 2, 3, 4])
     event_data['event_index'] = sc.array(dims=[''], unit=None, values=[0, 3, 3, 666])
     dg = nxroot['entry/events_0'][...]
     assert isinstance(dg, sc.DataGroup)
 
 
 def create_event_data_without_event_id(group):
-    group['event_time_offset'] = sc.array(dims=[''],
-                                          unit='s',
-                                          values=[456, 7, 3, 345, 632, 23])
+    group['event_time_offset'] = sc.array(
+        dims=[''], unit='s', values=[456, 7, 3, 345, 632, 23]
+    )
     group['event_time_zero'] = sc.array(dims=[''], unit='s', values=[1, 2, 3, 4])
     group['event_index'] = sc.array(dims=[''], unit=None, values=[0, 3, 3, 5])
 
 
 def test_event_data_without_event_id_can_be_loaded(nxroot):
     event_data = nxroot['entry'].create_class('events_0', snx.NXevent_data)
     create_event_data_without_event_id(event_data)
@@ -100,41 +100,53 @@
 
 
 def test_nxevent_data_keys(h5root):
     entry = make_event_data(h5root)
     root = snx.Group(entry)
     event_data = root['events']
     assert set(event_data.keys()) == {
-        'event_id', 'event_time_offset', 'event_time_zero', 'event_index'
+        'event_id',
+        'event_time_offset',
+        'event_time_zero',
+        'event_index',
     }
 
 
 def test_nxevent_data_children_read_as_variables_with_correct_dims(h5root):
     entry = make_event_data(h5root)
     root = snx.Group(entry, definitions=snx.base_definitions())
     event_data = root['events']
-    assert sc.identical(event_data['event_id'][()],
-                        sc.array(dims=['event'], values=[1, 1, 1, 0], unit=None))
-    assert sc.identical(event_data['event_time_offset'][()],
-                        sc.array(dims=['event'], values=[0, 1, 2, 3], unit='ns'))
+    assert sc.identical(
+        event_data['event_id'][()],
+        sc.array(dims=['event'], values=[1, 1, 1, 0], unit=None),
+    )
+    assert sc.identical(
+        event_data['event_time_offset'][()],
+        sc.array(dims=['event'], values=[0, 1, 2, 3], unit='ns'),
+    )
     assert sc.identical(
         event_data['event_time_zero'][()],
-        sc.array(dims=['event_time_zero'], values=[100, 200], unit='ms'))
-    assert sc.identical(event_data['event_index'][()],
-                        sc.array(dims=['event_time_zero'], values=[0, 3], unit=None))
+        sc.array(dims=['event_time_zero'], values=[100, 200], unit='ms'),
+    )
+    assert sc.identical(
+        event_data['event_index'][()],
+        sc.array(dims=['event_time_zero'], values=[0, 3], unit=None),
+    )
 
 
 def test_nxevent_data_dims_and_sizes_ignore_pulse_contents(h5root):
     entry = make_event_data(h5root)
     root = snx.Group(entry, definitions=snx.base_definitions())
     event_data = root['events']
-    assert event_data.dims == ('event_time_zero', )
+    assert event_data.dims == ('event_time_zero',)
     assert event_data.sizes == {'event_time_zero': 2}
 
 
 def test_read_nxevent_data(h5root):
     entry = make_event_data(h5root)
     root = snx.Group(entry, definitions=snx.base_definitions())
     event_data = root['events']
     da = event_data[()]
-    assert sc.identical(da.data.bins.size(),
-                        sc.array(dims=['event_time_zero'], values=[3, 1], unit=None))
+    assert sc.identical(
+        da.data.bins.size(),
+        sc.array(dims=['event_time_zero'], values=[3, 1], unit=None),
+    )
```

### Comparing `scippnexus-23.5.0/tests/nxlog_test.py` & `scippnexus-23.5.1/tests/nxlog_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,47 +32,52 @@
     with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
         root = snx.Group(f, definitions=snx.base_definitions())
         root.create_class('entry', NXentry)
         yield root
 
 
 def test_nxobject_log(h5root):
-    da = sc.DataArray(sc.array(dims=['time'], values=[1.1, 2.2, 3.3]),
-                      coords={
-                          'time':
-                          sc.epoch(unit='ns') +
-                          sc.array(dims=['time'], unit='s', values=[4.4, 5.5, 6.6]).to(
-                              unit='ns', dtype='int64')
-                      })
+    da = sc.DataArray(
+        sc.array(dims=['time'], values=[1.1, 2.2, 3.3]),
+        coords={
+            'time': sc.epoch(unit='ns')
+            + sc.array(dims=['time'], unit='s', values=[4.4, 5.5, 6.6]).to(
+                unit='ns', dtype='int64'
+            )
+        },
+    )
     log = snx.create_class(h5root, 'log', NXlog)
     snx.create_field(log, 'value', da.data)
     snx.create_field(log, 'time', da.coords['time'] - sc.epoch(unit='ns'))
     log = snx.Group(log, definitions=snx.base_definitions())
     assert sc.identical(log[...], da)
 
 
 def test_nxlog_with_missing_value_triggers_fallback(nxroot):
     time = sc.epoch(unit='ns') + sc.array(
-        dims=['time'], unit='s', values=[4.4, 5.5, 6.6]).to(unit='ns', dtype='int64')
+        dims=['time'], unit='s', values=[4.4, 5.5, 6.6]
+    ).to(unit='ns', dtype='int64')
     log = nxroot['entry'].create_class('log', NXlog)
     log['time'] = time - sc.epoch(unit='ns')
     loaded = log[()]
     # Fallback to DataGroup, but we still have partial info from NXlog: dim is time
     assert_identical(loaded, sc.DataGroup(time=time))
 
 
 def test_nxlog_length_1(h5root):
     nxroot = snx.Group(h5root, definitions=snx.base_definitions())
     da = sc.DataArray(
         sc.array(dims=['time'], values=[1.1]),
         coords={
-            'time':
-            sc.epoch(unit='ns') +
-            sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
-        })
+            'time': sc.epoch(unit='ns')
+            + sc.array(dims=['time'], unit='s', values=[4.4]).to(
+                unit='ns', dtype='int64'
+            )
+        },
+    )
     log = nxroot.create_class('log', NXlog)
     log['value'] = da.data
     log['time'] = da.coords['time'] - sc.epoch(unit='ns')
     assert sc.identical(log[...], da)
 
 
 def test_nxlog_length_1_two_dims_no_time_defaults_inner_dim_name(nxroot):
@@ -82,78 +87,90 @@
     assert_identical(log[...], sc.DataArray(var.rename(ignored='dim_1')))
 
 
 def test_nxlog_length_1_two_dims_with_time_defaults_inner_dim_name(nxroot):
     da = sc.DataArray(
         sc.array(dims=['time', 'ignored'], values=[[1.1]]),
         coords={
-            'time':
-            sc.epoch(unit='ns') +
-            sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
-        })
+            'time': sc.epoch(unit='ns')
+            + sc.array(dims=['time'], unit='s', values=[4.4]).to(
+                unit='ns', dtype='int64'
+            )
+        },
+    )
     log = nxroot['entry'].create_class('log', NXlog)
     log['value'] = da.data
     log['time'] = da.coords['time'] - sc.epoch(unit='ns')
     assert sc.identical(log[...], da.rename(ignored='dim_1'))
 
 
 def test_nxlog_axes_replaces_time_dim(nxroot):
     da = sc.DataArray(
         sc.array(dims=['time', 'ignored'], values=[[1.1]]),
         coords={
-            'time':
-            sc.epoch(unit='ns') +
-            sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
-        })
+            'time': sc.epoch(unit='ns')
+            + sc.array(dims=['time'], unit='s', values=[4.4]).to(
+                unit='ns', dtype='int64'
+            )
+        },
+    )
     log = nxroot['entry'].create_class('log', NXlog)
     log._group.attrs['axes'] = ['yy', 'xx']
     log['value'] = da.data
     log['time'] = da.coords['time'] - sc.epoch(unit='ns')
-    expected = sc.DataArray(sc.array(dims=['yy', 'xx'], values=[[1.1]]),
-                            coords={'time': da.coords['time'].squeeze()})
+    expected = sc.DataArray(
+        sc.array(dims=['yy', 'xx'], values=[[1.1]]),
+        coords={'time': da.coords['time'].squeeze()},
+    )
     assert sc.identical(log[...], expected)
 
 
 def test_nxlog_three_dims_with_time_of_length_1(nxroot):
     da = sc.DataArray(
-        sc.array(dims=['time', 'a', 'b'], values=np.arange(9.).reshape(1, 3, 3)),
+        sc.array(dims=['time', 'a', 'b'], values=np.arange(9.0).reshape(1, 3, 3)),
         coords={
-            'time':
-            sc.epoch(unit='ns') +
-            sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
-        })
+            'time': sc.epoch(unit='ns')
+            + sc.array(dims=['time'], unit='s', values=[4.4]).to(
+                unit='ns', dtype='int64'
+            )
+        },
+    )
     log = nxroot['entry'].create_class('log', NXlog)
     log['value'] = da.data
     log['time'] = da.coords['time'] - sc.epoch(unit='ns')
     loaded = log[...]
     assert_identical(
         loaded.data,
-        sc.array(dims=['time', 'dim_1', 'dim_2'], values=np.arange(9.).reshape(1, 3,
-                                                                               3)))
+        sc.array(
+            dims=['time', 'dim_1', 'dim_2'], values=np.arange(9.0).reshape(1, 3, 3)
+        ),
+    )
 
 
 def test_nxlog_with_shape_0(nxroot):
-    da = sc.DataArray(sc.ones(dims=['time', 'ignored'], shape=(0, 1)),
-                      coords={'time': sc.ones(dims=['time'], shape=(0, ), unit='s')})
+    da = sc.DataArray(
+        sc.ones(dims=['time', 'ignored'], shape=(0, 1)),
+        coords={'time': sc.ones(dims=['time'], shape=(0,), unit='s')},
+    )
     log = nxroot['entry'].create_class('log', NXlog)
     log['value'] = da.data
     log['time'] = da.coords['time']
     da.coords['time'] = sc.datetimes(dims=['time'], values=[], unit='ns')
     assert_identical(log[...], da.rename(ignored='dim_1'))
 
 
 def test_log_with_connection_status_raises_with_positional_indexing(h5root):
-    da = sc.DataArray(sc.array(dims=['time'], values=[1.1, 2.2, 3.3]),
-                      coords={
-                          'time':
-                          sc.array(dims=['time'],
-                                   unit='s',
-                                   values=[44, 55, 66],
-                                   dtype='int64')
-                      })
+    da = sc.DataArray(
+        sc.array(dims=['time'], values=[1.1, 2.2, 3.3]),
+        coords={
+            'time': sc.array(
+                dims=['time'], unit='s', values=[44, 55, 66], dtype='int64'
+            )
+        },
+    )
     log = snx.create_class(h5root, 'log', NXlog)
     snx.create_field(log, 'value', da.data)
     snx.create_field(log, 'time', da.coords['time'])
     connection_status = da['time', :2].copy()
     snx.create_field(log, 'connection_status', connection_status.data)
     snx.create_field(log, 'connection_status_time', connection_status.coords['time'])
     log = snx.Group(log, definitions=snx.base_definitions())
@@ -163,47 +180,49 @@
         log[:2]
     with pytest.raises(sc.DimensionError):
         log[:]
 
 
 @pytest.mark.parametrize('sublog_length', [0, 1, 2])
 def test_log_with_connection_status_loaded_as_datagroup_containing_data_arrays(
-        h5root, sublog_length):
-    da = sc.DataArray(sc.array(dims=['time'], values=[1.1, 2.2, 3.3]),
-                      coords={
-                          'time':
-                          sc.array(dims=['time'],
-                                   unit='s',
-                                   values=[44, 55, 66],
-                                   dtype='int64')
-                      })
+    h5root, sublog_length
+):
+    da = sc.DataArray(
+        sc.array(dims=['time'], values=[1.1, 2.2, 3.3]),
+        coords={
+            'time': sc.array(
+                dims=['time'], unit='s', values=[44, 55, 66], dtype='int64'
+            )
+        },
+    )
     log = snx.create_class(h5root, 'log', NXlog)
     snx.create_field(log, 'value', da.data)
     snx.create_field(log, 'time', da.coords['time'])
     connection_status = da['time', :sublog_length].copy()
     snx.create_field(log, 'connection_status', connection_status.data)
     snx.create_field(log, 'connection_status_time', connection_status.coords['time'])
     log = snx.Group(log, definitions=snx.base_definitions())
     loaded = log[()]
     da.coords['time'] = sc.epoch(unit='s') + da.coords['time']
-    connection_status.coords['time'] = sc.epoch(
-        unit='s') + connection_status.coords['time']
+    connection_status.coords['time'] = (
+        sc.epoch(unit='s') + connection_status.coords['time']
+    )
     assert_identical(loaded['value'], da)
     assert_identical(loaded['connection_status'], connection_status)
 
 
 def test_log_with_alarm_loaded_as_datagroup_containing_data_arrays(h5root):
-    da = sc.DataArray(sc.array(dims=['time'], values=[1.1, 2.2, 3.3]),
-                      coords={
-                          'time':
-                          sc.array(dims=['time'],
-                                   unit='s',
-                                   values=[44, 55, 66],
-                                   dtype='int64')
-                      })
+    da = sc.DataArray(
+        sc.array(dims=['time'], values=[1.1, 2.2, 3.3]),
+        coords={
+            'time': sc.array(
+                dims=['time'], unit='s', values=[44, 55, 66], dtype='int64'
+            )
+        },
+    )
     log = snx.create_class(h5root, 'log', NXlog)
     snx.create_field(log, 'value', da.data)
     snx.create_field(log, 'time', da.coords['time'])
     alarm = da['time', :2].copy()
     alarm.coords['message'] = sc.array(dims=['time'], values=['alarm 1', 'alarm 2'])
     snx.create_field(log, 'alarm_severity', alarm.data)
     snx.create_field(log, 'alarm_message', alarm.coords['message'])
```

### Comparing `scippnexus-23.5.0/tests/nxmonitor_test.py` & `scippnexus-23.5.1/tests/nxmonitor_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,52 +24,56 @@
         yield snx.Group(f, definitions=snx.base_definitions())
 
 
 def test_dense_monitor(h5root):
     monitor = snx.create_class(h5root, 'monitor', snx.NXmonitor)
     da = sc.DataArray(
         sc.array(dims=['time_of_flight'], values=[1.0]),
-        coords={'time_of_flight': sc.array(dims=['time_of_flight'], values=[1.0])})
+        coords={'time_of_flight': sc.array(dims=['time_of_flight'], values=[1.0])},
+    )
     data = snx.create_field(monitor, 'data', da.data)
     data.attrs['axes'] = 'time_of_flight'
     snx.create_field(monitor, 'time_of_flight', da.coords['time_of_flight'])
     monitor = make_group(monitor)
     assert sc.identical(monitor[...], da)
 
 
 def create_event_data_no_ids(group):
-    group.create_field('event_time_offset',
-                       sc.array(dims=[''], unit='s', values=[456, 7, 3, 345, 632, 23]))
-    group.create_field('event_time_zero',
-                       sc.array(dims=[''], unit='s', values=[1, 2, 3, 4]))
-    group.create_field('event_index', sc.array(dims=[''],
-                                               unit=None,
-                                               values=[0, 3, 3, 5]))
+    group.create_field(
+        'event_time_offset',
+        sc.array(dims=[''], unit='s', values=[456, 7, 3, 345, 632, 23]),
+    )
+    group.create_field(
+        'event_time_zero', sc.array(dims=[''], unit='s', values=[1, 2, 3, 4])
+    )
+    group.create_field(
+        'event_index', sc.array(dims=[''], unit=None, values=[0, 3, 3, 5])
+    )
 
 
 def test_loads_event_data_in_current_group_as_data_array(group):
     monitor = group.create_class('monitor1', snx.NXmonitor)
     create_event_data_no_ids(monitor)
-    assert monitor.dims == ('event_time_zero', )
-    assert monitor.shape == (4, )
+    assert monitor.dims == ('event_time_zero',)
+    assert monitor.shape == (4,)
     loaded = monitor[...]
     assert_identical(
         loaded.bins.size().data,
-        sc.array(dims=['event_time_zero'],
-                 unit=None,
-                 dtype='int64',
-                 values=[3, 0, 2, 1]))
+        sc.array(
+            dims=['event_time_zero'], unit=None, dtype='int64', values=[3, 0, 2, 1]
+        ),
+    )
 
 
 def test_loads_event_data_in_child_group_as_data_array(group):
     monitor = group.create_class('monitor1', snx.NXmonitor)
     create_event_data_no_ids(monitor.create_class('events', snx.NXevent_data))
-    assert monitor.dims == ('event_time_zero', )
-    assert monitor.shape == (4, )
+    assert monitor.dims == ('event_time_zero',)
+    assert monitor.shape == (4,)
     loaded = monitor[...]
     assert isinstance(loaded, sc.DataArray)
     assert sc.identical(
         loaded.bins.size().data,
-        sc.array(dims=['event_time_zero'],
-                 unit=None,
-                 dtype='int64',
-                 values=[3, 0, 2, 1]))
+        sc.array(
+            dims=['event_time_zero'], unit=None, dtype='int64', values=[3, 0, 2, 1]
+        ),
+    )
```

### Comparing `scippnexus-23.5.0/tests/nxoff_geometry_test.py` & `scippnexus-23.5.1/tests/nxoff_geometry_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 
 
 def test_vertices_loaded_as_vector3(group):
     shape = group.create_class('shape', NXoff_geometry)
     values = [[1, 2, 3], [4, 5, 6]]
     shape['vertices'] = sc.array(dims=['ignored', 'comp'], values=values, unit='mm')
     loaded = shape[()]
-    assert sc.identical(loaded['vertices'],
-                        sc.vectors(dims=['vertex'], values=values, unit='mm'))
+    assert sc.identical(
+        loaded['vertices'], sc.vectors(dims=['vertex'], values=values, unit='mm')
+    )
 
 
 def test_field_properties(group):
     shape = group.create_class('shape', NXoff_geometry)
     values = [[1, 2, 3], [4, 5, 6]]
     shape['vertices'] = sc.array(dims=['ignored', 'comp'], values=values, unit='m')
     shape['winding_order'] = sc.array(dims=['ignored'], values=[], unit=None)
     shape['faces'] = sc.array(dims=['ignored'], values=[], unit=None)
     loaded = shape[()]
-    assert loaded['vertices'].dims == ('vertex', )
-    assert loaded['winding_order'].dims == ('winding_order', )
+    assert loaded['vertices'].dims == ('vertex',)
+    assert loaded['winding_order'].dims == ('winding_order',)
     assert loaded['winding_order'].unit is None
-    assert loaded['faces'].dims == ('face', )
+    assert loaded['faces'].dims == ('face',)
     assert loaded['faces'].unit is None
 
 
 def test_off_to_shape_without_detector_faces_yields_scalar_shape_with_all_faces(group):
     off = group.create_class('off', NXoff_geometry)
     values = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
     off['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
@@ -53,86 +54,92 @@
     off = group.create_class('off', NXoff_geometry)
     values = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
     off['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
     off['winding_order'] = sc.array(dims=['_'], values=[0, 1, 2, 0, 2, 1], unit=None)
     off['faces'] = sc.array(dims=['_'], values=[0, 3], unit=None)
     det_num1 = 1
     det_num2 = 3
-    off['detector_faces'] = sc.array(dims=['_', 'dummy'],
-                                     values=[[0, det_num2], [1, det_num1]],
-                                     unit=None)
+    off['detector_faces'] = sc.array(
+        dims=['_', 'dummy'], values=[[0, det_num2], [1, det_num1]], unit=None
+    )
     loaded = off[()]
     with pytest.raises(snx.NexusStructureError):
         off_to_shape(**loaded)
 
 
 def test_off_to_shape_with_single_detector_yields_1d_shape(group):
     off = group.create_class('off', NXoff_geometry)
     values = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
     off['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
     off['winding_order'] = sc.array(dims=['_'], values=[0, 1, 2, 0, 2, 1], unit=None)
     off['faces'] = sc.array(dims=['_'], values=[0, 3], unit=None)
     det_num1 = 7
-    off['detector_faces'] = sc.array(dims=['_', 'dummy'],
-                                     values=[[0, det_num1], [1, det_num1]],
-                                     unit=None)
+    off['detector_faces'] = sc.array(
+        dims=['_', 'dummy'], values=[[0, det_num1], [1, det_num1]], unit=None
+    )
     loaded = off[()]
 
     detector_number = sc.index(1)  # not in detector_faces => no faces
     shape = off_to_shape(**loaded, detector_number=detector_number)
     assert sc.identical(shape.bins.size(), sc.array(dims=[], values=0, unit=None))
 
     detector_number = sc.index(det_num1)
     shape = off_to_shape(**loaded, detector_number=detector_number)
     assert sc.identical(shape.bins.size(), sc.array(dims=[], values=2, unit=None))
 
     detector_number = sc.array(dims=['detector_number'], values=[det_num1], unit=None)
     shape = off_to_shape(**loaded, detector_number=detector_number)
-    assert sc.identical(shape.bins.size(),
-                        sc.array(dims=['detector_number'], values=[2], unit=None))
+    assert sc.identical(
+        shape.bins.size(), sc.array(dims=['detector_number'], values=[2], unit=None)
+    )
 
 
 def test_off_to_shape_with_two_detectors_yields_1d_shape(group):
     off = group.create_class('off', NXoff_geometry)
     values = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
     off['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
     off['winding_order'] = sc.array(dims=['_'], values=[0, 1, 2, 0, 2, 1], unit=None)
     off['faces'] = sc.array(dims=['_'], values=[0, 3], unit=None)
     det_num1 = 1
     det_num2 = 3
-    off['detector_faces'] = sc.array(dims=['_', 'dummy'],
-                                     values=[[0, det_num2], [1, det_num1]],
-                                     unit=None)
+    off['detector_faces'] = sc.array(
+        dims=['_', 'dummy'], values=[[0, det_num2], [1, det_num1]], unit=None
+    )
     loaded = off[()]
-    detector_number = sc.array(dims=['detector_number'],
-                               values=[det_num1, det_num2],
-                               unit=None)
+    detector_number = sc.array(
+        dims=['detector_number'], values=[det_num1, det_num2], unit=None
+    )
     shape = off_to_shape(**loaded, detector_number=detector_number)
     assert shape.sizes == {'detector_number': 2}
-    assert sc.identical(shape.bins.size(),
-                        sc.array(dims=['detector_number'], values=[1, 1], unit=None))
+    assert sc.identical(
+        shape.bins.size(), sc.array(dims=['detector_number'], values=[1, 1], unit=None)
+    )
     assert sc.identical(
         shape[0].value,
-        sc.vectors(dims=['face', 'vertex'], values=[values[[0, 2, 1]]], unit='m'))
-    assert sc.identical(shape[1].value,
-                        sc.vectors(dims=['face', 'vertex'], values=[values], unit='m'))
+        sc.vectors(dims=['face', 'vertex'], values=[values[[0, 2, 1]]], unit='m'),
+    )
+    assert sc.identical(
+        shape[1].value, sc.vectors(dims=['face', 'vertex'], values=[values], unit='m')
+    )
 
 
 def test_off_to_shape_uses_order_of_provided_detector_number_param(group):
     off = group.create_class('off', NXoff_geometry)
     values = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
     off['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
     off['winding_order'] = sc.array(dims=['_'], values=[0, 1, 2, 0, 2, 1], unit=None)
     off['faces'] = sc.array(dims=['_'], values=[0, 3], unit=None)
     det_num1 = 1
     det_num2 = 3
-    off['detector_faces'] = sc.array(dims=['_', 'dummy'],
-                                     values=[[0, det_num2], [1, det_num1]],
-                                     unit=None)
+    off['detector_faces'] = sc.array(
+        dims=['_', 'dummy'], values=[[0, det_num2], [1, det_num1]], unit=None
+    )
     loaded = off[()]
     detector_number = sc.array(dims=['detector_number'], values=[3, 1], unit=None)
     shape = off_to_shape(**loaded, detector_number=detector_number)
-    assert sc.identical(shape[0].value,
-                        sc.vectors(dims=['face', 'vertex'], values=[values], unit='m'))
+    assert sc.identical(
+        shape[0].value, sc.vectors(dims=['face', 'vertex'], values=[values], unit='m')
+    )
     assert sc.identical(
         shape[1].value,
-        sc.vectors(dims=['face', 'vertex'], values=[values[[0, 2, 1]]], unit='m'))
+        sc.vectors(dims=['face', 'vertex'], values=[values[[0, 2, 1]]], unit='m'),
+    )
```

### Comparing `scippnexus-23.5.0/tests/nxsample_test.py` & `scippnexus-23.5.1/tests/nxsample_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,31 +21,40 @@
     sample = nxroot.create_class('data1', snx.NXsample)
     matrix = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
     sample['ub_matrix'] = matrix
     loaded = sample[()]
     assert_identical(
         loaded,
         sc.DataGroup(
-            ub_matrix=spatial.linear_transform(value=matrix, unit='1/angstrom')))
+            ub_matrix=spatial.linear_transform(value=matrix, unit='1/angstrom')
+        ),
+    )
 
 
 def test_ub_matrix_array_can_be_loaded(nxroot):
     sample = nxroot.create_class('data1', snx.NXsample)
-    matrices = np.array([[[1, 2, 3], [4, 5, 6], [7, 8, 9]],
-                         [[2, 3, 4], [5, 6, 7], [8, 9, 10]]])
+    matrices = np.array(
+        [[[1, 2, 3], [4, 5, 6], [7, 8, 9]], [[2, 3, 4], [5, 6, 7], [8, 9, 10]]]
+    )
     sample['ub_matrix'] = matrices
     loaded = sample[()]
     assert_identical(
         loaded,
-        sc.DataGroup(ub_matrix=spatial.linear_transforms(
-            dims=('dim_0', ), values=matrices, unit='1/angstrom')))
+        sc.DataGroup(
+            ub_matrix=spatial.linear_transforms(
+                dims=('dim_0',), values=matrices, unit='1/angstrom'
+            )
+        ),
+    )
 
 
 def test_orientation_matrix_loaded_as_linear_transform_with_dimensionless_unit(nxroot):
     sample = nxroot.create_class('data1', snx.NXsample)
     matrix = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
     sample['orientation_matrix'] = matrix
     loaded = sample[()]
     assert_identical(
         loaded,
         sc.DataGroup(
-            orientation_matrix=spatial.linear_transform(value=matrix, unit='')))
+            orientation_matrix=spatial.linear_transform(value=matrix, unit='')
+        ),
+    )
```

### Comparing `scippnexus-23.5.0/tests/nxtransformations_test.py` & `scippnexus-23.5.1/tests/nxtransformations_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,28 @@
     """Yield h5py root group (file)"""
     with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
         yield f
 
 
 def create_detector(group):
     data = sc.array(dims=['xx', 'yy'], values=[[1.1, 2.2], [3.3, 4.4]])
-    detector_numbers = sc.array(dims=['xx', 'yy'],
-                                unit=None,
-                                values=np.array([[1, 2], [3, 4]]))
+    detector_numbers = sc.array(
+        dims=['xx', 'yy'], unit=None, values=np.array([[1, 2], [3, 4]])
+    )
     detector = snx.create_class(group, 'detector_0', snx.NXdetector)
     snx.create_field(detector, 'detector_number', detector_numbers)
     snx.create_field(detector, 'data', data)
     return detector
 
 
 def test_Transformation_with_single_value(h5root):
     detector = create_detector(h5root)
-    snx.create_field(detector, 'depends_on',
-                     sc.scalar('/detector_0/transformations/t1'))
+    snx.create_field(
+        detector, 'depends_on', sc.scalar('/detector_0/transformations/t1')
+    )
     transformations = snx.create_class(detector, 'transformations', NXtransformations)
     value = sc.scalar(6.5, unit='mm')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='mm')
     vector = sc.vector(value=[0, 0, 1])
     t = value * vector
     expected = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
     expected = expected * offset
@@ -54,16 +55,17 @@
     assert depends_on == 'transformations/t1'
     t = detector[depends_on][()]
     assert_identical(t, expected)
 
 
 def test_time_independent_Transformation_with_length_0(h5root):
     detector = create_detector(h5root)
-    snx.create_field(detector, 'depends_on',
-                     sc.scalar('/detector_0/transformations/t1'))
+    snx.create_field(
+        detector, 'depends_on', sc.scalar('/detector_0/transformations/t1')
+    )
     transformations = snx.create_class(detector, 'transformations', NXtransformations)
     value = sc.array(dims=['dim_0'], values=[], unit='mm')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='mm')
     vector = sc.vector(value=[0, 0, 1])
     t = value * vector
     expected = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
     expected = expected * offset
@@ -95,15 +97,16 @@
     snx.create_field(det1, 'depends_on', sc.scalar('transformations/t1'))
 
     depends_on = make_group(det1)['depends_on'][()]
     assert depends_on == 'transformations/t1'
 
 
 def test_depends_on_attr_absolute_path_to_sibling_group_resolved_to_relative_path(
-        h5root):
+    h5root,
+):
     det1 = snx.create_class(h5root, 'det1', NXtransformations)
     transformations = snx.create_class(det1, 'transformations', NXtransformations)
     t1 = snx.create_field(transformations, 't1', sc.scalar(0.1, unit='cm'))
     t1.attrs['depends_on'] = '/det2/transformations/t2'
     t1.attrs['transformation_type'] = 'translation'
     t1.attrs['vector'] = [0, 0, 1]
 
@@ -124,16 +127,17 @@
     t1.attrs['depends_on'] = 't2'
     loaded = make_group(det)['transformations/t1'][()]
     assert loaded.attrs['depends_on'].value == 't2'
 
 
 def test_chain_with_single_values_and_different_unit(h5root):
     detector = create_detector(h5root)
-    snx.create_field(detector, 'depends_on',
-                     sc.scalar('/detector_0/transformations/t1'))
+    snx.create_field(
+        detector, 'depends_on', sc.scalar('/detector_0/transformations/t1')
+    )
     transformations = snx.create_class(detector, 'transformations', NXtransformations)
     value = sc.scalar(6.5, unit='mm')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='mm')
     vector = sc.vector(value=[0, 0, 1])
     t = value * vector
     value1 = snx.create_field(transformations, 't1', value)
     value1.attrs['depends_on'] = 't2'
@@ -143,35 +147,38 @@
     value1.attrs['vector'] = vector.value
     value2 = snx.create_field(transformations, 't2', value.to(unit='cm'))
     value2.attrs['depends_on'] = '.'
     value2.attrs['transformation_type'] = 'translation'
     value2.attrs['vector'] = vector.value
 
     t1 = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) * offset
-    t2 = sc.spatial.translations(dims=t.dims, values=t.values,
-                                 unit=t.unit).to(unit='cm')
+    t2 = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit).to(
+        unit='cm'
+    )
     detector = make_group(h5root['detector_0'])
     loaded = detector[()]
     depends_on = loaded.coords['depends_on']
     assert depends_on.value == 'transformations/t1'
     transforms = loaded.coords['transformations'].value
     assert_identical(transforms['t1'].data, t1)
     assert transforms['t1'].attrs['depends_on'].value == 't2'
     assert_identical(transforms['t2'].data, t2)
     assert transforms['t2'].attrs['depends_on'].value == '.'
 
 
 def test_Transformation_with_multiple_values(h5root):
     detector = create_detector(h5root)
-    snx.create_field(detector, 'depends_on',
-                     sc.scalar('/detector_0/transformations/t1'))
+    snx.create_field(
+        detector, 'depends_on', sc.scalar('/detector_0/transformations/t1')
+    )
     transformations = snx.create_class(detector, 'transformations', NXtransformations)
     log = sc.DataArray(
         sc.array(dims=['time'], values=[1.1, 2.2], unit='m'),
-        coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')})
+        coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')},
+    )
     log.coords['time'] = sc.epoch(unit='ns') + log.coords['time'].to(unit='ns')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='m')
     vector = sc.vector(value=[0, 0, 1])
     t = log * vector
     t.data = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
     value = snx.create_class(transformations, 't1', snx.NXlog)
     snx.create_field(value, 'time', log.coords['time'] - sc.epoch(unit='ns'))
@@ -188,20 +195,22 @@
     depends_on = detector['depends_on'][()]
     assert depends_on == 'transformations/t1'
     assert_identical(detector[depends_on][()], expected)
 
 
 def test_chain_with_multiple_values(h5root):
     detector = create_detector(h5root)
-    snx.create_field(detector, 'depends_on',
-                     sc.scalar('/detector_0/transformations/t1'))
+    snx.create_field(
+        detector, 'depends_on', sc.scalar('/detector_0/transformations/t1')
+    )
     transformations = snx.create_class(detector, 'transformations', NXtransformations)
     log = sc.DataArray(
         sc.array(dims=['time'], values=[1.1, 2.2], unit='m'),
-        coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')})
+        coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')},
+    )
     log.coords['time'] = sc.epoch(unit='ns') + log.coords['time'].to(unit='ns')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='m')
     vector = sc.vector(value=[0, 0, 1])
     t = log * vector
     t.data = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
     value1 = snx.create_class(transformations, 't1', snx.NXlog)
     snx.create_field(value1, 'time', log.coords['time'] - sc.epoch(unit='ns'))
@@ -227,38 +236,41 @@
     assert depends_on.value == 'transformations/t1'
     assert_identical(detector.coords['transformations'].value['t1'], expected1)
     assert_identical(detector.coords['transformations'].value['t2'], expected2)
 
 
 def test_chain_with_multiple_values_and_different_time_unit(h5root):
     detector = create_detector(h5root)
-    snx.create_field(detector, 'depends_on',
-                     sc.scalar('/detector_0/transformations/t1'))
+    snx.create_field(
+        detector, 'depends_on', sc.scalar('/detector_0/transformations/t1')
+    )
     transformations = snx.create_class(detector, 'transformations', NXtransformations)
     # Making sure to not use nanoseconds since that is used internally and may thus
     # mask bugs.
     log = sc.DataArray(
         sc.array(dims=['time'], values=[1.1, 2.2], unit='m'),
-        coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')})
+        coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')},
+    )
     log.coords['time'] = sc.epoch(unit='us') + log.coords['time'].to(unit='us')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='m')
     vector = sc.vector(value=[0, 0, 1])
     t = log * vector
     t.data = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
     value1 = snx.create_class(transformations, 't1', snx.NXlog)
     snx.create_field(value1, 'time', log.coords['time'] - sc.epoch(unit='us'))
     snx.create_field(value1, 'value', log.data)
     value1.attrs['depends_on'] = 't2'
     value1.attrs['transformation_type'] = 'translation'
     value1.attrs['offset'] = offset.values
     value1.attrs['offset_units'] = str(offset.unit)
     value1.attrs['vector'] = vector.value
     value2 = snx.create_class(transformations, 't2', snx.NXlog)
-    snx.create_field(value2, 'time',
-                     log.coords['time'].to(unit='ms') - sc.epoch(unit='ms'))
+    snx.create_field(
+        value2, 'time', log.coords['time'].to(unit='ms') - sc.epoch(unit='ms')
+    )
     snx.create_field(value2, 'value', log.data)
     value2.attrs['depends_on'] = '.'
     value2.attrs['transformation_type'] = 'translation'
     value2.attrs['vector'] = vector.value
 
     expected1 = t * offset
     expected1.attrs['depends_on'] = sc.scalar('t2')
@@ -273,22 +285,25 @@
     depends_on = loaded.coords['depends_on']
     assert depends_on.value == 'transformations/t1'
     assert_identical(loaded.coords['transformations'].value['t1'], expected1)
     assert_identical(loaded.coords['transformations'].value['t2'], expected2)
 
 
 def test_broken_time_dependent_transformation_returns_datagroup_but_sets_up_depends_on(
-        h5root):
+    h5root,
+):
     detector = create_detector(h5root)
-    snx.create_field(detector, 'depends_on',
-                     sc.scalar('/detector_0/transformations/t1'))
+    snx.create_field(
+        detector, 'depends_on', sc.scalar('/detector_0/transformations/t1')
+    )
     transformations = snx.create_class(detector, 'transformations', NXtransformations)
     log = sc.DataArray(
         sc.array(dims=['time'], values=[1.1, 2.2], unit='m'),
-        coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')})
+        coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')},
+    )
     log.coords['time'] = sc.epoch(unit='ns') + log.coords['time'].to(unit='ns')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='m')
     vector = sc.vector(value=[0, 0, 1])
     t = log * vector
     t.data = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
     value = snx.create_class(transformations, 't1', snx.NXlog)
     snx.create_field(value, 'time', log.coords['time'] - sc.epoch(unit='ns'))
@@ -310,30 +325,32 @@
     t1 = t['t1']
     assert isinstance(t1, sc.DataGroup)
     assert t1.keys() == {'time', 'value'}
     assert loaded.coords['depends_on'].value == 'transformations/t1'
     assert_identical(loaded.coords['transformations'].value['t1'], t1)
 
 
-def write_translation(group, name: str, value: sc.Variable, offset: sc.Variable,
-                      vector: sc.Variable) -> None:
+def write_translation(
+    group, name: str, value: sc.Variable, offset: sc.Variable, vector: sc.Variable
+) -> None:
     dset = snx.create_field(group, name, value)
     dset.attrs['transformation_type'] = 'translation'
     dset.attrs['offset'] = offset.values
     dset.attrs['offset_units'] = str(offset.unit)
     dset.attrs['vector'] = vector.value
 
 
 def test_nxtransformations_group_single_item(h5root):
     value = sc.scalar(2.4, unit='mm')
     offset = sc.spatial.translation(value=[6, 2, 6], unit='mm')
     vector = sc.vector(value=[0, 1, 1])
     t = value * vector
-    expected = (sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) *
-                offset)
+    expected = (
+        sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) * offset
+    )
 
     transformations = snx.create_class(h5root, 'transformations', NXtransformations)
     write_translation(transformations, 't1', value, offset, vector)
 
     loaded = make_group(h5root)['transformations'][()]
     assert set(loaded.keys()) == {'t1'}
     assert sc.identical(loaded['t1'], expected)
@@ -343,22 +360,24 @@
     transformations = snx.create_class(h5root, 'transformations', NXtransformations)
 
     value = sc.scalar(2.4, unit='mm')
     offset = sc.spatial.translation(value=[6, 2, 6], unit='mm')
     vector = sc.vector(value=[0, 1, 1])
     t = value * vector
     write_translation(transformations, 't1', value, offset, vector)
-    expected1 = (sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) *
-                 offset)
+    expected1 = (
+        sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) * offset
+    )
 
     value = value * 0.1
     t = value * vector
     write_translation(transformations, 't2', value, offset, vector)
-    expected2 = (sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) *
-                 offset)
+    expected2 = (
+        sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) * offset
+    )
 
     loaded = make_group(h5root)['transformations'][()]
     assert set(loaded.keys()) == {'t1', 't2'}
     assert sc.identical(loaded['t1'], expected1)
     assert sc.identical(loaded['t2'], expected2)
 
 
@@ -366,36 +385,39 @@
     transformations = snx.create_class(h5root, 'transformations', NXtransformations)
 
     value = sc.scalar(2.4, unit='mm')
     offset = sc.spatial.translation(value=[6, 2, 6], unit='mm')
     vector = sc.vector(value=[0, 1, 1])
     t = value * vector
     write_translation(transformations, 't1', value, offset, vector)
-    expected1 = (sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) *
-                 offset)
+    expected1 = (
+        sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) * offset
+    )
 
     value = value * 0.1
     t = value * vector
     write_translation(transformations, 't2', value, offset, vector)
     transformations['t2'].attrs['depends_on'] = 't1'
-    expected2 = (sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) *
-                 offset)
+    expected2 = (
+        sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) * offset
+    )
 
     loaded = make_group(h5root)['transformations'][()]
     assert set(loaded.keys()) == {'t1', 't2'}
     assert_identical(loaded['t1'], expected1)
     assert_identical(loaded['t2'].data, expected2)
     assert loaded['t2'].attrs['depends_on'].value == 't1'
 
 
 def test_slice_transformations(h5root):
     transformations = snx.create_class(h5root, 'transformations', NXtransformations)
     log = sc.DataArray(
         sc.array(dims=['time'], values=[1.1, 2.2, 3.3], unit='m'),
-        coords={'time': sc.array(dims=['time'], values=[11, 22, 33], unit='s')})
+        coords={'time': sc.array(dims=['time'], values=[11, 22, 33], unit='s')},
+    )
     log.coords['time'] = sc.epoch(unit='ns') + log.coords['time'].to(unit='ns')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='m')
     vector = sc.vector(value=[0, 0, 1])
     t = log * vector
     t.data = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
     value1 = snx.create_class(transformations, 't1', snx.NXlog)
     snx.create_field(value1, 'time', log.coords['time'] - sc.epoch(unit='ns'))
@@ -404,8 +426,9 @@
     value1.attrs['offset'] = offset.values
     value1.attrs['offset_units'] = str(offset.unit)
     value1.attrs['vector'] = vector.value
 
     expected = t * offset
 
     assert sc.identical(
-        make_group(h5root)['transformations']['time', 1:3]['t1'], expected['time', 1:3])
+        make_group(h5root)['transformations']['time', 1:3]['t1'], expected['time', 1:3]
+    )
```

### Comparing `scippnexus-23.5.0/tox.ini` & `scippnexus-23.5.1/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 setenv =
   JUPYTER_PLATFORM_DIRS = 1
 commands = pytest
 
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
 basepython = python3.8
-deps = {posargs:}
-       -r requirements/docs.txt
+deps =
+  {posargs:}
+  -r requirements/docs.txt
 allowlist_externals=find
 setenv =
   {[testenv]setenv}
   # Search directory for confuse for custom config enabling plopp plotting
   SCIPPDIR={toxinidir}{/}docs{/}buildconfig
 commands = python -m sphinx -j2 -v -b html -d {toxworkdir}/docs_doctrees docs html
            python -m sphinx -j2 -v -b doctest -d {toxworkdir}/docs_doctrees docs html
```

