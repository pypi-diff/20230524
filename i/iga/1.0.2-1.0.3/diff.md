# Comparing `tmp/iga-1.0.2.tar.gz` & `tmp/iga-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iga-1.0.2.tar", last modified: Tue May 23 15:25:38 2023, max compression
+gzip compressed data, was "iga-1.0.3.tar", last modified: Wed May 24 21:09:36 2023, max compression
```

## Comparing `iga-1.0.2.tar` & `iga-1.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-23 15:25:38.557029 iga-1.0.2/
--rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-05-22 20:41:59.000000 iga-1.0.2/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)    37612 2023-05-23 15:25:38.557165 iga-1.0.2/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)    36706 2023-05-22 20:41:59.000000 iga-1.0.2/README.md
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-23 15:25:38.553055 iga-1.0.2/iga/
--rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-05-23 15:20:22.000000 iga-1.0.2/iga/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-05-22 20:41:59.000000 iga-1.0.2/iga/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    34712 2023-05-22 20:41:59.000000 iga-1.0.2/iga/cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-05-22 20:41:59.000000 iga-1.0.2/iga/data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-05-22 20:41:59.000000 iga-1.0.2/iga/doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1252 2023-05-22 20:41:59.000000 iga-1.0.2/iga/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1514 2023-05-22 20:41:59.000000 iga-1.0.2/iga/exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)    15499 2023-05-22 20:41:59.000000 iga-1.0.2/iga/github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-05-22 20:41:59.000000 iga-1.0.2/iga/id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)    18504 2023-05-22 20:41:59.000000 iga-1.0.2/iga/invenio.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-05-22 20:41:59.000000 iga-1.0.2/iga/json_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-05-22 20:41:59.000000 iga-1.0.2/iga/licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    70404 2023-05-23 15:20:22.000000 iga-1.0.2/iga/metadata.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14563 2023-05-22 20:41:59.000000 iga-1.0.2/iga/name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-05-22 20:41:59.000000 iga-1.0.2/iga/orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-05-22 20:41:59.000000 iga-1.0.2/iga/reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-05-22 20:41:59.000000 iga-1.0.2/iga/ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-05-22 20:41:59.000000 iga-1.0.2/iga/text_utils.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-23 15:25:38.553923 iga-1.0.2/iga.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)    37612 2023-05-23 15:25:38.000000 iga-1.0.2/iga.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-05-23 15:25:38.000000 iga-1.0.2/iga.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-23 15:25:38.000000 iga-1.0.2/iga.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-05-23 15:25:38.000000 iga-1.0.2/iga.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-23 15:25:38.000000 iga-1.0.2/iga.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-05-23 15:25:38.000000 iga-1.0.2/iga.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-05-23 15:25:38.000000 iga-1.0.2/iga.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-05-23 15:25:38.557502 iga-1.0.2/setup.cfg
--rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-05-22 20:41:59.000000 iga-1.0.2/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-23 15:25:38.556913 iga-1.0.2/tests/
--rw-r--r--   0 mhucka     (503) staff       (20)     6117 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_github_mocks.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)      641 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_init.py
--rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_is_person.py
--rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_name_splitting.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5997 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_record_from_codemeta.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-05-22 20:41:59.000000 iga-1.0.2/tests/test_text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 21:09:36.324432 iga-1.0.3/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-05-23 15:45:07.000000 iga-1.0.3/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    38059 2023-05-24 21:09:36.324552 iga-1.0.3/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    37153 2023-05-24 21:02:11.000000 iga-1.0.3/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 21:09:36.321238 iga-1.0.3/iga/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-05-24 21:02:11.000000 iga-1.0.3/iga/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-05-23 15:45:07.000000 iga-1.0.3/iga/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    34712 2023-05-23 15:45:07.000000 iga-1.0.3/iga/cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-05-23 15:45:07.000000 iga-1.0.3/iga/data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-05-23 15:45:07.000000 iga-1.0.3/iga/doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1252 2023-05-23 15:45:07.000000 iga-1.0.3/iga/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1514 2023-05-23 15:45:07.000000 iga-1.0.3/iga/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15499 2023-05-23 15:45:07.000000 iga-1.0.3/iga/github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-05-23 15:45:07.000000 iga-1.0.3/iga/id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    18504 2023-05-23 15:45:07.000000 iga-1.0.3/iga/invenio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2064 2023-05-24 21:02:11.000000 iga-1.0.3/iga/json_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-05-23 15:45:07.000000 iga-1.0.3/iga/licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    70404 2023-05-23 15:45:07.000000 iga-1.0.3/iga/metadata.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14593 2023-05-24 19:21:29.000000 iga-1.0.3/iga/name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-05-23 15:45:07.000000 iga-1.0.3/iga/orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-05-23 15:45:07.000000 iga-1.0.3/iga/reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-05-23 15:45:07.000000 iga-1.0.3/iga/ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-05-23 15:45:07.000000 iga-1.0.3/iga/text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 21:09:36.322023 iga-1.0.3/iga.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    38059 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-05-24 21:09:36.324861 iga-1.0.3/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-05-23 15:45:07.000000 iga-1.0.3/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 21:09:36.324320 iga-1.0.3/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     6117 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_github_mocks.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      641 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_init.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_is_person.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_name_splitting.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5997 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_record_from_codemeta.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_text_utils.py
```

### Comparing `iga-1.0.2/LICENSE` & `iga-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/PKG-INFO` & `iga-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,10 @@
-Metadata-Version: 2.1
-Name: iga
-Version: 1.0.2
-Summary: InvenioRDM GitHub Archiver
-Home-page: https://github.com/caltechlibrary/iga
-Author: Michael Hucka
-Author-email: helpdesk@library.caltech.edu
-License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
-Project-URL: Source Code, https://github.com/caltechlibrary/iga
-Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
-Keywords: Python,applications
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
-IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Action](https://github.com/marketplace/actions/iga) that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
+IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/iga) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
@@ -45,15 +21,15 @@
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
 
 [InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and data sets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the [_InvenioRDM GitHub Archiver_](https://github.com/caltechlibrary/iga) (IGA) comes in.
 
-IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to archive GitHub releases automatically for a repository each time they are made.
+IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Actions](https://docs.github.com/en/actions) workflow to archive GitHub releases automatically for a repository each time they are made.
 
 <p align=center>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
 <span style="font-size: 150%">➜</span>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
 </p>
 
@@ -120,39 +96,37 @@
 
 After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
 ```shell
 iga --help
 ```
 
 
-### IGA as a GitHub Action
+### IGA as a GitHub Actions workflow
 
-A [GitHub Action](https://docs.github.com/en/actions) is a workflow that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
+A [GitHub Actions](https://docs.github.com/en/actions) workflow is an automated process that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
 
 1. In the main branch of your GitHub repository, create a `.github/workflows` directory
-2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/develop/sample-workflow.yml) into it:
+2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/main/sample-workflow.yml) into it:
     ```yaml
     name: InvenioRDM GitHub Archiver
-
     env:
       # 👋🏻 Set the next variable to your InvenioRDM server address 👋🏻
       INVENIO_SERVER: https://your-invenio-server.org
 
-      # Set to an InvenioRDM record ID to mark releases as new versions.
+      # Set to an InvenioRDM record ID to mark release as a new version.
       parent_record: none
 
-      # The remaining variables are other IGA options. Please see the docs.
+      # The variables below are other IGA options. Please see the docs.
       community:     none
       draft:         false
       all_assets:    false
       all_metadata:  false
       debug:         false
 
-    # ~~~~~~~~~~~~~~~~ The rest of this file should be left as-is. ~~~~~~~~~~~~~~~~
-
+    # ~~~~~~~~~~~~ The rest of this file should be left as-is ~~~~~~~~~~~~
     on:
       release:
         types: [published]
       workflow_dispatch:
         inputs:
           release_tag:
             description: "The release tag (empty = latest):"
@@ -169,37 +143,47 @@
           all_metadata:
             default: false
             description: "Include additional GitHub metadata:"
           debug:
             default: false
             description: "Print debug info in the GitHub log:"
     jobs:
-      Send_to_InvenioRDM:
+      run_iga:
+        name: "Send to ${{needs.get_repository.outputs.server}}"
         runs-on: ubuntu-latest
+        needs: get_repository
         steps:
           - uses: caltechlibrary/iga@main
             with:
               INVENIO_SERVER: ${{env.INVENIO_SERVER}}
               INVENIO_TOKEN:  ${{secrets.INVENIO_TOKEN}}
               all_assets:     ${{github.event.inputs.all_assets || env.all_assets}}
               all_metadata:   ${{github.event.inputs.all_metadata || env.all_metadata}}
               debug:          ${{github.event.inputs.debug || env.debug}}
               draft:          ${{github.event.inputs.draft || env.draft}}
               community:      ${{github.event.inputs.community || env.community}}
               parent_record:  ${{github.event.inputs.parent_record || env.parent_record}}
               release_tag:    ${{github.event.inputs.release_tag || 'latest'}}
+      get_repository:
+        name: "Get repository name"
+        runs-on: ubuntu-latest
+        outputs:
+          server: ${{steps.parse.outputs.host}}
+        steps:
+          - id: parse
+            run: echo "host=$(cut -d'/' -f3 <<< ${{env.INVENIO_SERVER}} | cut -d':' -f1)" >> $GITHUB_OUTPUT
     ```
-3. **Edit the value of the `INVENIO_SERVER` variable (line 5 above)** ↑
+3. **Edit the value of the `INVENIO_SERVER` variable (line 4 above)** ↑
 4. Optionally, change the values of other options (`parent_record`, `community`, etc.)
 5. Save the file, commit the changes to git, and push your changes to GitHub
 
 
 ## Quick start
 
-No matter whether IGA is run locally on your computer or as a GitHub Action, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
+No matter whether IGA is run locally on your computer or as a GitHub Actions workflow, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
 is the first step.
 
 ### Getting an InvenioRDM token
 
 <img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" width="60%" align="right">
 
 1. Log in to your InvenioRDM account
@@ -227,17 +211,17 @@
 ```shell
 iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 More options are described in the section on [detailed usage information](#usage) below.
 
 
-### Configuring and running IGA as a GitHub Action
+### Configuring and running IGA as a GitHub Actions workflow
 
-After doing the [GitHub Action installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
+After doing the [GitHub Actions installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
 
 1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" width="85%"></p>
 2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" width="40%"></p>
 3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" width="60%"></p>
 4. Name the variable `INVENIO_TOKEN` and paste in your InvenioRDM token
 5. Finish by clicking the green <kbd>Add secret</kbd> button
 
@@ -272,15 +256,15 @@
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
 It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some repositories IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
 
-Note that when you run IGA as a GitHub Action, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Action workflow.
+Note that when you run IGA as a GitHub Actions workflow, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Actions workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
```

### Comparing `iga-1.0.2/README.md` & `iga-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,34 @@
+Metadata-Version: 2.1
+Name: iga
+Version: 1.0.3
+Summary: InvenioRDM GitHub Archiver
+Home-page: https://github.com/caltechlibrary/iga
+Author: Michael Hucka
+Author-email: helpdesk@library.caltech.edu
+License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
+Project-URL: Source Code, https://github.com/caltechlibrary/iga
+Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
+Keywords: Python,applications
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
-IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Action](https://github.com/marketplace/actions/iga) that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
+IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/iga) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
@@ -21,15 +45,15 @@
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
 
 [InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and data sets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the [_InvenioRDM GitHub Archiver_](https://github.com/caltechlibrary/iga) (IGA) comes in.
 
-IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to archive GitHub releases automatically for a repository each time they are made.
+IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Actions](https://docs.github.com/en/actions) workflow to archive GitHub releases automatically for a repository each time they are made.
 
 <p align=center>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
 <span style="font-size: 150%">➜</span>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
 </p>
 
@@ -96,39 +120,37 @@
 
 After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
 ```shell
 iga --help
 ```
 
 
-### IGA as a GitHub Action
+### IGA as a GitHub Actions workflow
 
-A [GitHub Action](https://docs.github.com/en/actions) is a workflow that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
+A [GitHub Actions](https://docs.github.com/en/actions) workflow is an automated process that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
 
 1. In the main branch of your GitHub repository, create a `.github/workflows` directory
-2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/develop/sample-workflow.yml) into it:
+2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/main/sample-workflow.yml) into it:
     ```yaml
     name: InvenioRDM GitHub Archiver
-
     env:
       # 👋🏻 Set the next variable to your InvenioRDM server address 👋🏻
       INVENIO_SERVER: https://your-invenio-server.org
 
-      # Set to an InvenioRDM record ID to mark releases as new versions.
+      # Set to an InvenioRDM record ID to mark release as a new version.
       parent_record: none
 
-      # The remaining variables are other IGA options. Please see the docs.
+      # The variables below are other IGA options. Please see the docs.
       community:     none
       draft:         false
       all_assets:    false
       all_metadata:  false
       debug:         false
 
-    # ~~~~~~~~~~~~~~~~ The rest of this file should be left as-is. ~~~~~~~~~~~~~~~~
-
+    # ~~~~~~~~~~~~ The rest of this file should be left as-is ~~~~~~~~~~~~
     on:
       release:
         types: [published]
       workflow_dispatch:
         inputs:
           release_tag:
             description: "The release tag (empty = latest):"
@@ -145,37 +167,47 @@
           all_metadata:
             default: false
             description: "Include additional GitHub metadata:"
           debug:
             default: false
             description: "Print debug info in the GitHub log:"
     jobs:
-      Send_to_InvenioRDM:
+      run_iga:
+        name: "Send to ${{needs.get_repository.outputs.server}}"
         runs-on: ubuntu-latest
+        needs: get_repository
         steps:
           - uses: caltechlibrary/iga@main
             with:
               INVENIO_SERVER: ${{env.INVENIO_SERVER}}
               INVENIO_TOKEN:  ${{secrets.INVENIO_TOKEN}}
               all_assets:     ${{github.event.inputs.all_assets || env.all_assets}}
               all_metadata:   ${{github.event.inputs.all_metadata || env.all_metadata}}
               debug:          ${{github.event.inputs.debug || env.debug}}
               draft:          ${{github.event.inputs.draft || env.draft}}
               community:      ${{github.event.inputs.community || env.community}}
               parent_record:  ${{github.event.inputs.parent_record || env.parent_record}}
               release_tag:    ${{github.event.inputs.release_tag || 'latest'}}
+      get_repository:
+        name: "Get repository name"
+        runs-on: ubuntu-latest
+        outputs:
+          server: ${{steps.parse.outputs.host}}
+        steps:
+          - id: parse
+            run: echo "host=$(cut -d'/' -f3 <<< ${{env.INVENIO_SERVER}} | cut -d':' -f1)" >> $GITHUB_OUTPUT
     ```
-3. **Edit the value of the `INVENIO_SERVER` variable (line 5 above)** ↑
+3. **Edit the value of the `INVENIO_SERVER` variable (line 4 above)** ↑
 4. Optionally, change the values of other options (`parent_record`, `community`, etc.)
 5. Save the file, commit the changes to git, and push your changes to GitHub
 
 
 ## Quick start
 
-No matter whether IGA is run locally on your computer or as a GitHub Action, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
+No matter whether IGA is run locally on your computer or as a GitHub Actions workflow, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
 is the first step.
 
 ### Getting an InvenioRDM token
 
 <img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" width="60%" align="right">
 
 1. Log in to your InvenioRDM account
@@ -203,17 +235,17 @@
 ```shell
 iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 More options are described in the section on [detailed usage information](#usage) below.
 
 
-### Configuring and running IGA as a GitHub Action
+### Configuring and running IGA as a GitHub Actions workflow
 
-After doing the [GitHub Action installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
+After doing the [GitHub Actions installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
 
 1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" width="85%"></p>
 2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" width="40%"></p>
 3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" width="60%"></p>
 4. Name the variable `INVENIO_TOKEN` and paste in your InvenioRDM token
 5. Finish by clicking the green <kbd>Add secret</kbd> button
 
@@ -248,15 +280,15 @@
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
 It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some repositories IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
 
-Note that when you run IGA as a GitHub Action, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Action workflow.
+Note that when you run IGA as a GitHub Actions workflow, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Actions workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
```

### Comparing `iga-1.0.2/iga/__init__.py` & `iga-1.0.3/iga/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '1.0.2'
+__version__     = '1.0.3'
 __description__ = 'InvenioRDM GitHub Archiver'
 __url__         = 'https://github.com/caltechlibrary/iga'
 __author__      = 'Michael Hucka'
 __email__       = 'helpdesk@library.caltech.edu'
 __license__     = 'https://github.com/caltechlibrary/iga/blob/main/LICENSE'
```

### Comparing `iga-1.0.2/iga/__main__.py` & `iga-1.0.3/iga/__main__.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/cli.py` & `iga-1.0.3/iga/cli.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/data_utils.py` & `iga-1.0.3/iga/data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/doi.py` & `iga-1.0.3/iga/doi.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/exceptions.py` & `iga-1.0.3/iga/exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/exit_codes.py` & `iga-1.0.3/iga/exit_codes.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/github.py` & `iga-1.0.3/iga/github.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/id_utils.py` & `iga-1.0.3/iga/id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/invenio.py` & `iga-1.0.3/iga/invenio.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/json_utils.py` & `iga-1.0.3/iga/json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,14 @@
     try:
         return dict(dirtyjson.loads(content))
     except KeyboardInterrupt:
         raise
     except dirtyjson.error.Error as ex:
         # Do we have a line number?
         log('error parsing JSON: ' + str(ex))
-        if line := getattr(ex, 'lineno'):
+        if line := getattr(ex, 'lineno', None):
             if recursion <= _MAX_RECURSION_DEPTH:
                 return partial_json(content, line, recursion + 1)
             else:
                 log('exceeded recursion depth and admitting failure')
                 return {}
     return {}
```

### Comparing `iga-1.0.2/iga/licenses.py` & `iga-1.0.3/iga/licenses.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/metadata.py` & `iga-1.0.3/iga/metadata.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/name_utils.py` & `iga-1.0.3/iga/name_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,21 +99,21 @@
     In the most general case, it is impossible to reliably determine whether a
     given string of characters represents the name of a person and not, say,
     the name of a company or product. This function makes a best-effort guess
     using heuristics in combination with methods from natural language
     processing (NLP), but it will sometimes make mistakes.
 
     This function is designed with the assumption that its input is already
-    expected to be a name, and it only needs to make the determination of
-    whether it is the name of a person or not.
+    expected to be the name of a person or organization, and it only needs to
+    make the determination of whether it is the name of a person.
     '''
     if not name:
         return False
 
-    # A string like "Joe's Foobar" is not a name.
+    # A string like "Joe's Foobar" is not a person name.
     if any(item in name for item in _NON_PERSON_ELEMENTS):
         log(f'{name} contains non-person elements => not a person')
         return False
 
     # If the input contains a mix of Latin and CJK characters, it's likely to
     # contain both an English and CJK version of the same thing. (E.g.,
     # someone might write their name in Chinese in parentheses after an English
```

### Comparing `iga-1.0.2/iga/orcid.py` & `iga-1.0.3/iga/orcid.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/reference.py` & `iga-1.0.3/iga/reference.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/ror.py` & `iga-1.0.3/iga/ror.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga/text_utils.py` & `iga-1.0.3/iga/text_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga.egg-info/PKG-INFO` & `iga-1.0.3/iga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 1.0.2
+Version: 1.0.3
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
-IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Action](https://github.com/marketplace/actions/iga) that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
+IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/iga) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
@@ -45,15 +45,15 @@
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
 
 [InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and data sets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the [_InvenioRDM GitHub Archiver_](https://github.com/caltechlibrary/iga) (IGA) comes in.
 
-IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to archive GitHub releases automatically for a repository each time they are made.
+IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Actions](https://docs.github.com/en/actions) workflow to archive GitHub releases automatically for a repository each time they are made.
 
 <p align=center>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
 <span style="font-size: 150%">➜</span>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
 </p>
 
@@ -120,39 +120,37 @@
 
 After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
 ```shell
 iga --help
 ```
 
 
-### IGA as a GitHub Action
+### IGA as a GitHub Actions workflow
 
-A [GitHub Action](https://docs.github.com/en/actions) is a workflow that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
+A [GitHub Actions](https://docs.github.com/en/actions) workflow is an automated process that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
 
 1. In the main branch of your GitHub repository, create a `.github/workflows` directory
-2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/develop/sample-workflow.yml) into it:
+2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/main/sample-workflow.yml) into it:
     ```yaml
     name: InvenioRDM GitHub Archiver
-
     env:
       # 👋🏻 Set the next variable to your InvenioRDM server address 👋🏻
       INVENIO_SERVER: https://your-invenio-server.org
 
-      # Set to an InvenioRDM record ID to mark releases as new versions.
+      # Set to an InvenioRDM record ID to mark release as a new version.
       parent_record: none
 
-      # The remaining variables are other IGA options. Please see the docs.
+      # The variables below are other IGA options. Please see the docs.
       community:     none
       draft:         false
       all_assets:    false
       all_metadata:  false
       debug:         false
 
-    # ~~~~~~~~~~~~~~~~ The rest of this file should be left as-is. ~~~~~~~~~~~~~~~~
-
+    # ~~~~~~~~~~~~ The rest of this file should be left as-is ~~~~~~~~~~~~
     on:
       release:
         types: [published]
       workflow_dispatch:
         inputs:
           release_tag:
             description: "The release tag (empty = latest):"
@@ -169,37 +167,47 @@
           all_metadata:
             default: false
             description: "Include additional GitHub metadata:"
           debug:
             default: false
             description: "Print debug info in the GitHub log:"
     jobs:
-      Send_to_InvenioRDM:
+      run_iga:
+        name: "Send to ${{needs.get_repository.outputs.server}}"
         runs-on: ubuntu-latest
+        needs: get_repository
         steps:
           - uses: caltechlibrary/iga@main
             with:
               INVENIO_SERVER: ${{env.INVENIO_SERVER}}
               INVENIO_TOKEN:  ${{secrets.INVENIO_TOKEN}}
               all_assets:     ${{github.event.inputs.all_assets || env.all_assets}}
               all_metadata:   ${{github.event.inputs.all_metadata || env.all_metadata}}
               debug:          ${{github.event.inputs.debug || env.debug}}
               draft:          ${{github.event.inputs.draft || env.draft}}
               community:      ${{github.event.inputs.community || env.community}}
               parent_record:  ${{github.event.inputs.parent_record || env.parent_record}}
               release_tag:    ${{github.event.inputs.release_tag || 'latest'}}
+      get_repository:
+        name: "Get repository name"
+        runs-on: ubuntu-latest
+        outputs:
+          server: ${{steps.parse.outputs.host}}
+        steps:
+          - id: parse
+            run: echo "host=$(cut -d'/' -f3 <<< ${{env.INVENIO_SERVER}} | cut -d':' -f1)" >> $GITHUB_OUTPUT
     ```
-3. **Edit the value of the `INVENIO_SERVER` variable (line 5 above)** ↑
+3. **Edit the value of the `INVENIO_SERVER` variable (line 4 above)** ↑
 4. Optionally, change the values of other options (`parent_record`, `community`, etc.)
 5. Save the file, commit the changes to git, and push your changes to GitHub
 
 
 ## Quick start
 
-No matter whether IGA is run locally on your computer or as a GitHub Action, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
+No matter whether IGA is run locally on your computer or as a GitHub Actions workflow, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
 is the first step.
 
 ### Getting an InvenioRDM token
 
 <img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" width="60%" align="right">
 
 1. Log in to your InvenioRDM account
@@ -227,17 +235,17 @@
 ```shell
 iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 More options are described in the section on [detailed usage information](#usage) below.
 
 
-### Configuring and running IGA as a GitHub Action
+### Configuring and running IGA as a GitHub Actions workflow
 
-After doing the [GitHub Action installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
+After doing the [GitHub Actions installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
 
 1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" width="85%"></p>
 2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" width="40%"></p>
 3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" width="60%"></p>
 4. Name the variable `INVENIO_TOKEN` and paste in your InvenioRDM token
 5. Finish by clicking the green <kbd>Add secret</kbd> button
 
@@ -272,15 +280,15 @@
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
 It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some repositories IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
 
-Note that when you run IGA as a GitHub Action, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Action workflow.
+Note that when you run IGA as a GitHub Actions workflow, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Actions workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
```

### Comparing `iga-1.0.2/iga.egg-info/SOURCES.txt` & `iga-1.0.3/iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/iga.egg-info/requires.txt` & `iga-1.0.3/iga.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/setup.cfg` & `iga-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iga
-version = 1.0.2
+version = 1.0.3
 description = InvenioRDM GitHub Archiver
 author = Michael Hucka
 author_email = helpdesk@library.caltech.edu
 license = https://github.com/caltechlibrary/iga/blob/main/LICENSE
 license_files = LICENSE
 url = https://github.com/caltechlibrary/iga
 project_urls =
```

### Comparing `iga-1.0.2/setup.py` & `iga-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_cli.py` & `iga-1.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_data_utils.py` & `iga-1.0.3/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_doi.py` & `iga-1.0.3/tests/test_doi.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_exceptions.py` & `iga-1.0.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_github.py` & `iga-1.0.3/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_github_mocks.py` & `iga-1.0.3/tests/test_github_mocks.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_id_utils.py` & `iga-1.0.3/tests/test_id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_init.py` & `iga-1.0.3/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_is_person.py` & `iga-1.0.3/tests/test_is_person.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_licenses.py` & `iga-1.0.3/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_name_splitting.py` & `iga-1.0.3/tests/test_name_splitting.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_name_utils.py` & `iga-1.0.3/tests/test_name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_orcid.py` & `iga-1.0.3/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_record_from_codemeta.py` & `iga-1.0.3/tests/test_record_from_codemeta.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_reference.py` & `iga-1.0.3/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_ror.py` & `iga-1.0.3/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.2/tests/test_text_utils.py` & `iga-1.0.3/tests/test_text_utils.py`

 * *Files identical despite different names*

