# Comparing `tmp/nbsphinx-0.9.1.tar.gz` & `tmp/nbsphinx-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbsphinx-0.9.1.tar", last modified: Tue Mar 14 18:10:23 2023, max compression
+gzip compressed data, was "nbsphinx-0.9.2.tar", last modified: Wed May 24 20:53:04 2023, max compression
```

## Comparing `nbsphinx-0.9.1.tar` & `nbsphinx-0.9.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-03-14 18:10:23.366583 nbsphinx-0.9.1/
--rw-r--r--   0 mg        (1000) mg        (1000)     3700 2022-09-18 14:14:25.000000 nbsphinx-0.9.1/CONTRIBUTING.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     1063 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)      229 2022-08-28 14:43:55.000000 nbsphinx-0.9.1/MANIFEST.in
--rw-r--r--   0 mg        (1000) mg        (1000)    13268 2023-03-14 18:09:26.000000 nbsphinx-0.9.1/NEWS.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     1929 2023-03-14 18:10:23.366583 nbsphinx-0.9.1/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)      980 2022-09-18 14:14:25.000000 nbsphinx-0.9.1/README.rst
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-03-14 18:10:23.358583 nbsphinx-0.9.1/doc/
--rw-r--r--   0 mg        (1000) mg        (1000)     9223 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/a-normal-rst-file.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     2297 2022-08-28 14:43:55.000000 nbsphinx-0.9.1/doc/allow-errors-per-cell.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2578 2022-09-18 14:14:25.000000 nbsphinx-0.9.1/doc/allow-errors.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    24079 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/code-cells.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     6817 2023-03-14 10:38:30.000000 nbsphinx-0.9.1/doc/conf.py
--rw-r--r--   0 mg        (1000) mg        (1000)    13609 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/configuration.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     3318 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/configuring-kernels.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)       33 2022-08-28 14:43:55.000000 nbsphinx-0.9.1/doc/contributing.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     3642 2022-08-28 14:43:55.000000 nbsphinx-0.9.1/doc/custom-css.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1556 2022-09-18 16:09:51.000000 nbsphinx-0.9.1/doc/executing-notebooks.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2113 2022-08-21 14:47:54.000000 nbsphinx-0.9.1/doc/hidden-cells.ipynb
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-03-14 18:10:23.362583 nbsphinx-0.9.1/doc/images/
--rw-r--r--   0 mg        (1000) mg        (1000)     8031 2017-11-28 19:42:46.000000 nbsphinx-0.9.1/doc/images/notebook_icon.png
--rw-r--r--   0 mg        (1000) mg        (1000)    15301 2022-08-28 14:43:55.000000 nbsphinx-0.9.1/doc/images/python_logo.svg
--rw-r--r--   0 mg        (1000) mg        (1000)    39583 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/images/raw_cells_jupyter_notebook.png
--rw-r--r--   0 mg        (1000) mg        (1000)    37656 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/images/raw_cells_jupyterlab.png
--rw-r--r--   0 mg        (1000) mg        (1000)     2405 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/index.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     7002 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/installation.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     7864 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/links.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    29113 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/markdown-cells.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1913 2022-08-21 14:47:54.000000 nbsphinx-0.9.1/doc/never-execute.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2035 2022-08-21 14:47:54.000000 nbsphinx-0.9.1/doc/orphan.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     7234 2022-09-18 14:14:25.000000 nbsphinx-0.9.1/doc/pre-executed.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     5441 2022-09-18 14:14:25.000000 nbsphinx-0.9.1/doc/prolog-and-epilog.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     6746 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/raw-cells.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)      977 2022-08-21 14:47:54.000000 nbsphinx-0.9.1/doc/references.bib
--rw-r--r--   0 mg        (1000) mg        (1000)      806 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/references.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      347 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/requirements.txt
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-03-14 18:10:23.362583 nbsphinx-0.9.1/doc/subdir/
--rw-r--r--   0 mg        (1000) mg        (1000)     2394 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/subdir/a-notebook-in-a-subdir.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2294 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/subdir/gallery.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     5033 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/subdir/toctree.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1729 2022-08-28 14:43:55.000000 nbsphinx-0.9.1/doc/timeout.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    22745 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/doc/usage.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)       58 2022-08-28 14:43:55.000000 nbsphinx-0.9.1/doc/version-history.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      908 2023-03-02 19:46:03.000000 nbsphinx-0.9.1/doc/yet-another.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)       91 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/pyproject.toml
--rw-r--r--   0 mg        (1000) mg        (1000)       38 2023-03-14 18:10:23.366583 nbsphinx-0.9.1/setup.cfg
--rw-r--r--   0 mg        (1000) mg        (1000)     1807 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/setup.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-03-14 18:10:23.338583 nbsphinx-0.9.1/src/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-03-14 18:10:23.362583 nbsphinx-0.9.1/src/nbsphinx/
--rw-r--r--   0 mg        (1000) mg        (1000)    73231 2023-03-14 18:08:59.000000 nbsphinx-0.9.1/src/nbsphinx/__init__.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-03-14 18:10:23.366583 nbsphinx-0.9.1/src/nbsphinx/_static/
--rw-r--r--   0 mg        (1000) mg        (1000)     4467 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/src/nbsphinx/_static/nbsphinx-broken-thumbnail.svg
--rw-r--r--   0 mg        (1000) mg        (1000)     7108 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/src/nbsphinx/_static/nbsphinx-code-cells.css_t
--rw-r--r--   0 mg        (1000) mg        (1000)      584 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/src/nbsphinx/_static/nbsphinx-gallery.css
--rw-r--r--   0 mg        (1000) mg        (1000)     2871 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/src/nbsphinx/_static/nbsphinx-no-thumbnail.svg
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-03-14 18:10:23.366583 nbsphinx-0.9.1/src/nbsphinx/_texinputs/
--rw-r--r--   0 mg        (1000) mg        (1000)     8202 2023-03-14 09:55:02.000000 nbsphinx-0.9.1/src/nbsphinx/_texinputs/nbsphinx.sty
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-03-14 18:10:23.362583 nbsphinx-0.9.1/src/nbsphinx.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)     1929 2023-03-14 18:10:23.000000 nbsphinx-0.9.1/src/nbsphinx.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)     1324 2023-03-14 18:10:23.000000 nbsphinx-0.9.1/src/nbsphinx.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-03-14 18:10:23.000000 nbsphinx-0.9.1/src/nbsphinx.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       65 2023-03-14 18:10:23.000000 nbsphinx-0.9.1/src/nbsphinx.egg-info/requires.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        9 2023-03-14 18:10:23.000000 nbsphinx-0.9.1/src/nbsphinx.egg-info/top_level.txt
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 20:53:04.985066 nbsphinx-0.9.2/
+-rw-r--r--   0 mg        (1000) mg        (1000)     3700 2022-09-18 14:14:25.000000 nbsphinx-0.9.2/CONTRIBUTING.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     1063 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/LICENSE
+-rw-r--r--   0 mg        (1000) mg        (1000)      229 2022-08-28 14:43:55.000000 nbsphinx-0.9.2/MANIFEST.in
+-rw-r--r--   0 mg        (1000) mg        (1000)    13609 2023-05-24 20:51:58.000000 nbsphinx-0.9.2/NEWS.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     1929 2023-05-24 20:53:04.985066 nbsphinx-0.9.2/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)      980 2022-09-18 14:14:25.000000 nbsphinx-0.9.2/README.rst
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 20:53:04.973066 nbsphinx-0.9.2/doc/
+-rw-r--r--   0 mg        (1000) mg        (1000)     9607 2023-05-21 10:29:22.000000 nbsphinx-0.9.2/doc/a-normal-rst-file.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     2297 2022-08-28 14:43:55.000000 nbsphinx-0.9.2/doc/allow-errors-per-cell.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     2578 2022-09-18 14:14:25.000000 nbsphinx-0.9.2/doc/allow-errors.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    21584 2023-05-21 15:37:19.000000 nbsphinx-0.9.2/doc/code-cells.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     7143 2023-05-24 19:44:25.000000 nbsphinx-0.9.2/doc/conf.py
+-rw-r--r--   0 mg        (1000) mg        (1000)    13609 2023-05-06 17:18:22.000000 nbsphinx-0.9.2/doc/configuration.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     3318 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/doc/configuring-kernels.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)       33 2022-08-28 14:43:55.000000 nbsphinx-0.9.2/doc/contributing.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     3642 2022-08-28 14:43:55.000000 nbsphinx-0.9.2/doc/custom-css.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     1556 2022-09-18 16:09:51.000000 nbsphinx-0.9.2/doc/executing-notebooks.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     2113 2022-08-21 14:47:54.000000 nbsphinx-0.9.2/doc/hidden-cells.ipynb
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 20:53:04.977066 nbsphinx-0.9.2/doc/images/
+-rw-r--r--   0 mg        (1000) mg        (1000)     8031 2017-11-28 19:42:46.000000 nbsphinx-0.9.2/doc/images/notebook_icon.png
+-rw-r--r--   0 mg        (1000) mg        (1000)    15301 2022-08-28 14:43:55.000000 nbsphinx-0.9.2/doc/images/python_logo.svg
+-rw-r--r--   0 mg        (1000) mg        (1000)    39583 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/doc/images/raw_cells_jupyter_notebook.png
+-rw-r--r--   0 mg        (1000) mg        (1000)    37656 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/doc/images/raw_cells_jupyterlab.png
+-rw-r--r--   0 mg        (1000) mg        (1000)     2405 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/doc/index.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     6987 2023-05-21 10:29:22.000000 nbsphinx-0.9.2/doc/installation.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     7864 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/doc/links.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    29649 2023-05-21 10:29:22.000000 nbsphinx-0.9.2/doc/markdown-cells.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     1913 2022-08-21 14:47:54.000000 nbsphinx-0.9.2/doc/never-execute.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     2035 2022-08-21 14:47:54.000000 nbsphinx-0.9.2/doc/orphan.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     7234 2022-09-18 14:14:25.000000 nbsphinx-0.9.2/doc/pre-executed.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     5441 2022-09-18 14:14:25.000000 nbsphinx-0.9.2/doc/prolog-and-epilog.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     6746 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/doc/raw-cells.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)      977 2022-08-21 14:47:54.000000 nbsphinx-0.9.2/doc/references.bib
+-rw-r--r--   0 mg        (1000) mg        (1000)      775 2023-05-21 15:37:19.000000 nbsphinx-0.9.2/doc/references.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      158 2023-05-21 15:37:19.000000 nbsphinx-0.9.2/doc/requirements.txt
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 20:53:04.981066 nbsphinx-0.9.2/doc/subdir/
+-rw-r--r--   0 mg        (1000) mg        (1000)     2394 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/doc/subdir/a-notebook-in-a-subdir.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     2294 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/doc/subdir/gallery.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     5033 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/doc/subdir/toctree.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     1729 2022-08-28 14:43:55.000000 nbsphinx-0.9.2/doc/timeout.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    23012 2023-05-24 20:47:39.000000 nbsphinx-0.9.2/doc/usage.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)       58 2022-08-28 14:43:55.000000 nbsphinx-0.9.2/doc/version-history.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      908 2023-03-02 19:46:03.000000 nbsphinx-0.9.2/doc/yet-another.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)       91 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/pyproject.toml
+-rw-r--r--   0 mg        (1000) mg        (1000)       38 2023-05-24 20:53:04.985066 nbsphinx-0.9.2/setup.cfg
+-rw-r--r--   0 mg        (1000) mg        (1000)     1807 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/setup.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 20:53:04.945066 nbsphinx-0.9.2/src/
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 20:53:04.981066 nbsphinx-0.9.2/src/nbsphinx/
+-rw-r--r--   0 mg        (1000) mg        (1000)    74234 2023-05-24 20:49:14.000000 nbsphinx-0.9.2/src/nbsphinx/__init__.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 20:53:04.985066 nbsphinx-0.9.2/src/nbsphinx/_static/
+-rw-r--r--   0 mg        (1000) mg        (1000)     4467 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/src/nbsphinx/_static/nbsphinx-broken-thumbnail.svg
+-rw-r--r--   0 mg        (1000) mg        (1000)     7344 2023-05-24 20:43:35.000000 nbsphinx-0.9.2/src/nbsphinx/_static/nbsphinx-code-cells.css_t
+-rw-r--r--   0 mg        (1000) mg        (1000)      584 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/src/nbsphinx/_static/nbsphinx-gallery.css
+-rw-r--r--   0 mg        (1000) mg        (1000)     2871 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/src/nbsphinx/_static/nbsphinx-no-thumbnail.svg
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 20:53:04.985066 nbsphinx-0.9.2/src/nbsphinx/_texinputs/
+-rw-r--r--   0 mg        (1000) mg        (1000)     8202 2023-03-14 09:55:02.000000 nbsphinx-0.9.2/src/nbsphinx/_texinputs/nbsphinx.sty
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 20:53:04.981066 nbsphinx-0.9.2/src/nbsphinx.egg-info/
+-rw-r--r--   0 mg        (1000) mg        (1000)     1929 2023-05-24 20:53:04.000000 nbsphinx-0.9.2/src/nbsphinx.egg-info/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)     1324 2023-05-24 20:53:04.000000 nbsphinx-0.9.2/src/nbsphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-05-24 20:53:04.000000 nbsphinx-0.9.2/src/nbsphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       65 2023-05-24 20:53:04.000000 nbsphinx-0.9.2/src/nbsphinx.egg-info/requires.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        9 2023-05-24 20:53:04.000000 nbsphinx-0.9.2/src/nbsphinx.egg-info/top_level.txt
```

### Comparing `nbsphinx-0.9.1/CONTRIBUTING.rst` & `nbsphinx-0.9.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/LICENSE` & `nbsphinx-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/NEWS.rst` & `nbsphinx-0.9.2/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Version 0.9.2 -- 2023-05-24 -- PyPI__ -- diff__
+ * Improve support for ``sphinx_immaterial`` theme
+ * Improve support for links starting with ``#``
+ * Add support for in-text citations
+ * LaTeX: Add support for admonition titles
+
+__ https://pypi.org/project/nbsphinx/0.9.2/
+__ https://github.com/spatialaudio/nbsphinx/compare/0.9.1...0.9.2
+
 Version 0.9.1 -- 2023-03-14 -- PyPI__ -- diff__
  * pandoc: disable "smart" option only for version 2.0+
 
 __ https://pypi.org/project/nbsphinx/0.9.1/
 __ https://github.com/spatialaudio/nbsphinx/compare/0.9.0...0.9.1
 
 Version 0.9.0 -- 2023-03-12 -- PyPI__ -- diff__
```

### Comparing `nbsphinx-0.9.1/PKG-INFO` & `nbsphinx-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsphinx
-Version: 0.9.1
+Version: 0.9.2
 Summary: Jupyter Notebook Tools for Sphinx
 Home-page: https://nbsphinx.readthedocs.io/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: MIT
 Project-URL: Documentation, https://nbsphinx.readthedocs.io/
 Project-URL: Source Code, https://github.com/spatialaudio/nbsphinx/
```

### Comparing `nbsphinx-0.9.1/README.rst` & `nbsphinx-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/a-normal-rst-file.rst` & `nbsphinx-0.9.2/doc/a-normal-rst-file.rst`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,15 @@
     extensions = [
         'nbsphinx',
         'sphinxcontrib.bibtex',
         # Probably more extensions here ...
     ]
 
     bibtex_bibfiles = ['my-references.bib']
+    bibtex_reference_style = 'author_year'
 
 Afterwards all the references defined in the bibliography file(s) can be used
 throughout the Jupyter notebooks and other source files as detailed in the following.
 
 .. _standard Sphinx Citations: https://www.sphinx-doc.org/en/master/usage/
     restructuredtext/basics.html#citations
 .. _sphinxcontrib.bibtex: https://sphinxcontrib-bibtex.readthedocs.io/
@@ -200,14 +201,22 @@
 
 You can create citations like :cite:`perez2011python`:
 
 .. code-block:: rst
 
     :cite:`perez2011python`
 
+You can also create so-called in-text citations,
+where the names of the authors, for example :cite:t:`perez2011python`,
+are part of the sentence:
+
+.. code-block:: rst
+
+    :cite:t:`perez2011python`
+
 You can create similar citations in Jupyter notebooks with a special HTML
 syntax, see the section about
 `citations in Markdown cells <markdown-cells.ipynb#Citations>`__.
 
 You can create a list of references in any reStructuredText file
 (or `reST cell <raw-cells.ipynb#reST>`_ in a notebook) like this:
 
@@ -225,14 +234,20 @@
 possible to create footnote bibliographies with footnote
 citations like :footcite:`perez2011python`.
 
 .. code-block:: rst
 
     :footcite:`perez2011python`
 
+In-text citations like :footcite:t:`kluyver2016jupyter` can be created like this:
+
+.. code-block:: rst
+
+    :footcite:t:`kluyver2016jupyter`
+
 Also footnote citations can be used within Jupyter notebooks with a special HTML syntax,
 see the section about
 `footnote citations in Markdown cells <markdown-cells.ipynb#Footnote-citations>`__.
 Footnote citations are restricted to their own source file and the assembly of the
 bibliography is (analogously to normal citations) invoked with the
 
 .. code-block:: rst
```

### Comparing `nbsphinx-0.9.1/doc/allow-errors-per-cell.ipynb` & `nbsphinx-0.9.2/doc/allow-errors-per-cell.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/allow-errors.ipynb` & `nbsphinx-0.9.2/doc/allow-errors.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/code-cells.ipynb` & `nbsphinx-0.9.2/doc/code-cells.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9849397590361446%*

 * *Differences: {"'cells'": '{delete: [54, 53, 52, 51, 50, 49, 48, 47, 17, 16]}'}*

```diff
@@ -146,36 +146,14 @@
                 "</div>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Cell Magics\n",
-                "\n",
-                "IPython can handle code in other languages by means of [cell magics](https://ipython.readthedocs.io/en/stable/interactive/magics.html#cell-magics):"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "%%bash\n",
-                "for i in 1 2 3\n",
-                "do\n",
-                "    echo $i\n",
-                "done"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 "## Special Display Formats\n",
                 "\n",
                 "See [IPython example notebook](https://nbviewer.jupyter.org/github/ipython/ipython/blob/main/examples/IPython Kernel/Rich Output.ipynb)."
             ]
         },
         {
             "cell_type": "markdown",
@@ -462,92 +440,14 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": [
-                "df = pd.DataFrame(np.random.randint(0, 100, size=[5, 4]),\n",
-                "                  columns=['a', 'b', 'c', 'd'])\n",
-                "df"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "For LaTeX output, however, the plain text output is used by default.\n",
-                "\n",
-                "To get nice LaTeX tables, a few settings have to be changed:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "pd.set_option('display.latex.repr', True)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "This is not enabled by default because of\n",
-                "[Pandas issue #12182](https://github.com/pandas-dev/pandas/issues/12182).\n",
-                "\n",
-                "The generated LaTeX tables utilize the `booktabs` package, so you have to make sure that package is [loaded in the preamble](https://www.sphinx-doc.org/en/master/latex.html) with:\n",
-                "\n",
-                "    \\usepackage{booktabs}\n",
-                "\n",
-                "In order to allow page breaks within tables, you should use:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "pd.set_option('display.latex.longtable', True)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "The `longtable` package is already used by Sphinx,\n",
-                "so you don't have to manually load it in the preamble.\n",
-                "\n",
-                "Finally, if you want to use LaTeX math expressions in your dataframe, you'll have to disable escaping:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "pd.set_option('display.latex.escape', False)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "The above settings should have no influence on the HTML output, but the LaTeX output should now look nicer:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
             "source": [
                 "df = pd.DataFrame(np.random.randint(0, 100, size=[10, 4]),\n",
                 "                  columns=[r'$\\alpha$', r'$\\beta$', r'$\\gamma$', r'$\\delta$'])\n",
                 "df"
             ]
         },
         {
```

### Comparing `nbsphinx-0.9.1/doc/conf.py` & `nbsphinx-0.9.2/doc/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,15 +84,17 @@
     {{ docname | escape_latex }}}} ends here.}}
 """
 
 mathjax3_config = {
     'tex': {'tags': 'ams', 'useLabelIds': True},
 }
 
+# https://sphinxcontrib-bibtex.readthedocs.io/en/latest/usage.html
 bibtex_bibfiles = ['references.bib']
+bibtex_reference_style = 'author_year'
 
 # Support for notebook formats other than .ipynb
 nbsphinx_custom_formats = {
     '.pct.py': ['jupytext.reads', {'fmt': 'py:percent'}],
     '.md': ['jupytext.reads', {'fmt': 'Rmd'}],
 }
 
@@ -108,14 +110,16 @@
 author = 'Matthias Geier'
 copyright = '2020, ' + author
 html_show_copyright = False
 
 linkcheck_ignore = [
     r'http://localhost:\d+/',
     'https://github.com/spatialaudio/nbsphinx/compare/',
+    # 418 Client Error: Unknown for url: https://ieeexplore.ieee.org/document/5582063/
+    'https://doi.org/10.1109/MCSE.2010.119',
 ]
 
 nitpicky = True
 
 # -- Get version information and date from Git ----------------------------
 
 try:
@@ -137,33 +141,34 @@
 
 # See https://www.sphinx-doc.org/en/master/latex.html
 latex_elements = {
     'papersize': 'a4paper',
     'printindex': '',
     'sphinxsetup': r"""
 HeaderFamily=\rmfamily\bfseries,
-%verbatimwithframe=false,
-%verbatimwrapslines=false,
-%verbatimhintsturnover=false,
-noteBorderColor={HTML}{E0E0E0},
-noteborder=0.5pt,
-warningBorderColor={HTML}{E0E0E0},
-warningborder=1.5pt,
-warningBgColor={HTML}{FBFBFB},
+div.note_border-TeXcolor={HTML}{E0E0E0},
+div.note_border-width=0.5pt,
+div.note_box-decoration-break=slice,
+div.warning_border-TeXcolor={HTML}{E0E0E0},
+div.warning_border-width=1.5pt,
+div.warning_background-TeXcolor={HTML}{FBFBFB},
+div.warning_box-decoration-break=slice,
+div.topic_box-shadow=none,
+div.topic_border-TeXcolor={HTML}{E0E0E0},
+div.topic_border-width=0.5pt,
+div.topic_box-decoration-break=slice,
 """,
     'fontpkg': r"""
 \usepackage{mathpazo}
 \linespread{1.05}  % see http://www.tug.dk/FontCatalogue/urwpalladio/
 \setmainfont{TeX Gyre Pagella}[Numbers=OldStyle]
 \setmonofont{Latin Modern Mono Light}[Numbers=Lining]
 """,
     'preamble': r"""
 \urlstyle{tt}
-\renewenvironment{sphinxnote}[1]
-  {\begin{sphinxheavybox}\sphinxstrong{#1} }{\end{sphinxheavybox}}
 """,
 }
 
 latex_engine = 'lualatex'
 latex_use_xindy = False
 
 latex_table_style = ['booktabs']
```

### Comparing `nbsphinx-0.9.1/doc/configuration.ipynb` & `nbsphinx-0.9.2/doc/configuration.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/configuring-kernels.ipynb` & `nbsphinx-0.9.2/doc/configuring-kernels.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/custom-css.ipynb` & `nbsphinx-0.9.2/doc/custom-css.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/executing-notebooks.ipynb` & `nbsphinx-0.9.2/doc/executing-notebooks.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/hidden-cells.ipynb` & `nbsphinx-0.9.2/doc/hidden-cells.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/images/notebook_icon.png` & `nbsphinx-0.9.2/doc/images/notebook_icon.png`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/images/python_logo.svg` & `nbsphinx-0.9.2/doc/images/python_logo.svg`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/images/raw_cells_jupyter_notebook.png` & `nbsphinx-0.9.2/doc/images/raw_cells_jupyter_notebook.png`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/images/raw_cells_jupyterlab.png` & `nbsphinx-0.9.2/doc/images/raw_cells_jupyterlab.png`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/index.rst` & `nbsphinx-0.9.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/installation.ipynb` & `nbsphinx-0.9.2/doc/installation.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994453044375645%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(14, "*

 * *            "'[Anaconda](https://www.anaconda.com/download#downloads)),\\n')], delete: [14]}}, 2: "*

 * *            '{\'source\': {insert: [(8, "If you don\'t know which one is best for you, you can try '*

 * *            '[Miniforge/Mambaforge](https://github.com/conda-forge/miniforge).\\n")], delete: '*

 * *            '[8]}}}'}*

```diff
@@ -23,15 +23,15 @@
                 "\n",
                 "[![Anaconda Badge](https://anaconda.org/conda-forge/nbsphinx/badges/version.svg)](https://anaconda.org/conda-forge/nbsphinx)\n",
                 "\n",
                 "If you are using the `conda` package manager\n",
                 "(e.g. with\n",
                 "[Miniforge](https://github.com/conda-forge/miniforge),\n",
                 "[Miniconda](https://docs.conda.io/en/latest/miniconda.html) or\n",
-                "[Anaconda](https://www.anaconda.com/products/distribution#Downloads)),\n",
+                "[Anaconda](https://www.anaconda.com/download#downloads)),\n",
                 "you can install `nbsphinx` from the [conda-forge](https://conda-forge.org/) channel:\n",
                 "\n",
                 "    conda install -c conda-forge nbsphinx\n",
                 "\n",
                 "[![PyPI version](https://badge.fury.io/py/nbsphinx.png)](https://pypi.org/project/nbsphinx)\n",
                 "\n",
                 "You can of course also install `nbsphinx` with `pip`, Python's own package manager:\n",
@@ -56,15 +56,15 @@
                 "\n",
                 "Some of the aforementioned packages will install some of these prerequisites automatically, some of the things may be already installed on your computer anyway.\n",
                 "\n",
                 "### Python\n",
                 "\n",
                 "Of course you'll need Python, because both Sphinx and `nbsphinx` are implemented in Python.\n",
                 "There are many ways to get Python.\n",
-                "If you don't know which one is best for you, you can try [Anaconda](https://www.anaconda.com/products/individual#Downloads).\n",
+                "If you don't know which one is best for you, you can try [Miniforge/Mambaforge](https://github.com/conda-forge/miniforge).\n",
                 "\n",
                 "### Sphinx\n",
                 "\n",
                 "You'll need [Sphinx](https://www.sphinx-doc.org/) as well, because `nbsphinx` is just a Sphinx extension and doesn't do anything on its own.\n",
                 "\n",
                 "If you use `conda`, you can get [Sphinx from the conda-forge channel](https://anaconda.org/conda-forge/sphinx):\n",
                 "\n",
```

### Comparing `nbsphinx-0.9.1/doc/links.ipynb` & `nbsphinx-0.9.2/doc/links.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/markdown-cells.ipynb` & `nbsphinx-0.9.2/doc/markdown-cells.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996603260869565%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(6, 'Example: <cite "*

 * *            'data-cite="kluyver2016jupyter">(Kluyver et al. 2016)</cite>.\\n\'), (9, \'<cite '*

 * *            'data-cite="kluyver2016jupyter">(Kluyver et al. 2016)</cite>\\n\'), (18, \'```\\n\'), '*

 * *            "(19, '\\n'), (20, 'In-text citations like\\n'), (21, '<cite "*

 * *            'data-cite-t="kluyver2016jupyter">Kluyver et al. (2016)</cite>\\n\'), (22, \'can be '*

 * *            "created like this:\\n'), (23, '\\n'), (24, '```html\\n'), (25, '<cite " […]*

```diff
@@ -195,45 +195,61 @@
             "source": [
                 "## Citations\n",
                 "\n",
                 "According to https://nbconvert.readthedocs.io/en/latest/latex_citations.html,\n",
                 "`nbconvert` supports citations using a special HTML-based syntax.\n",
                 "`nbsphinx` supports the same syntax.\n",
                 "\n",
-                "Example: <cite data-cite=\"kluyver2016jupyter\">Kluyver et al. (2016)</cite>.\n",
+                "Example: <cite data-cite=\"kluyver2016jupyter\">(Kluyver et al. 2016)</cite>.\n",
                 "\n",
                 "```html\n",
-                "<cite data-cite=\"kluyver2016jupyter\">Kluyver et al. (2016)</cite>\n",
+                "<cite data-cite=\"kluyver2016jupyter\">(Kluyver et al. 2016)</cite>\n",
                 "```\n",
                 "\n",
                 "You don't actually have to use `<cite>`,\n",
                 "any inline HTML tag can be used, e.g. `<strong>`:\n",
                 "<strong data-cite=\"perez2011python\">Python: An Ecosystem for Scientific Computing</strong>.\n",
                 "\n",
                 "```html\n",
                 "<strong data-cite=\"perez2011python\">Python: An Ecosystem for Scientific Computing</strong>\n",
                 "```\n",
                 "\n",
+                "In-text citations like\n",
+                "<cite data-cite-t=\"kluyver2016jupyter\">Kluyver et al. (2016)</cite>\n",
+                "can be created like this:\n",
+                "\n",
+                "```html\n",
+                "<cite data-cite-t=\"kluyver2016jupyter\">Kluyver et al. (2016)</cite>\n",
+                "```\n",
+                "\n",
                 "You'll also have to define a list of references,\n",
                 "see [the section about references](a-normal-rst-file.rst#references).\n",
                 "\n",
                 "There is also a Notebook extension which may or may not be useful: https://github.com/takluyver/cite2c.\n",
                 "\n",
                 "### Footnote citations\n",
                 "\n",
                 "Since version `2.0.0` of sphinxcontrib-bibtex, [footnote citations](https://sphinxcontrib-bibtex.readthedocs.io/en/latest/usage.html#role-footcite) are possible. This generates footnotes for all foot-citations up to the point of the [bibliography directive](a-normal-rst-file.rst#footnote-citations), which is typically placed at the end of the source file.\n",
                 "\n",
                 "Depending on whether the documentation is rendered into HTML or into LaTeX/PDF, the citations are either placed into a bibliography as ordinary citations (HTML output) or placed into the footnotes of the citation's respective page (PDF).\n",
                 "\n",
-                "Example: <cite data-footcite=\"perez2011python\">P\u00e9rez et al. (2011)</cite>.\n",
+                "Example: <cite data-footcite=\"perez2011python\">(P\u00e9rez et al. 2011)</cite>.\n",
                 "\n",
                 "```html\n",
-                "<cite data-footcite=\"perez2011python\">P\u00e9rez et al. (2011)</cite>\n",
+                "<cite data-footcite=\"perez2011python\">(P\u00e9rez et al. 2011)</cite>\n",
                 "```\n",
                 "\n",
+                "Example for an in-text citation:\n",
+                "<cite data-footcite-t=\"perez2011python\">P\u00e9rez et al. (2011)</cite>.\n",
+                "\n",
+                "```html\n",
+                "<cite data-footcite-t=\"perez2011python\">P\u00e9rez et al. (2011)</cite>\n",
+                "```\n",
+                "\n",
+                "\n",
                 "As footnote references are restricted to their own Jupyter notebook or other source file, a raw nbconvert cell of reST format (see [the section about raw cells](raw-cells.ipynb)) can be added to the notebook, containing the\n",
                 "\n",
                 "```rst\n",
                 ".. footbibliography::\n",
                 "```\n",
                 "\n",
                 "directive."
```

### Comparing `nbsphinx-0.9.1/doc/never-execute.ipynb` & `nbsphinx-0.9.2/doc/never-execute.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/orphan.ipynb` & `nbsphinx-0.9.2/doc/orphan.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/pre-executed.ipynb` & `nbsphinx-0.9.2/doc/pre-executed.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/prolog-and-epilog.ipynb` & `nbsphinx-0.9.2/doc/prolog-and-epilog.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/raw-cells.ipynb` & `nbsphinx-0.9.2/doc/raw-cells.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/references.bib` & `nbsphinx-0.9.2/doc/references.bib`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/references.rst` & `nbsphinx-0.9.2/doc/references.rst`

 * *Files 22% similar despite different names*

```diff
@@ -24,9 +24,8 @@
     \endgroup
 
 .. warning::
 
     With ``docutils`` versions 0.18 and 0.19,
     the HTML output after the bibliography is broken,
     see https://github.com/mcmtroffaes/sphinxcontrib-bibtex/issues/309.
-    This problem will be fixed in the next ``docutils`` version
-    (either 0.19.1 or 0.20).
+    This problem has been fixed in ``docutils`` version 0.20.
```

### Comparing `nbsphinx-0.9.1/doc/subdir/a-notebook-in-a-subdir.ipynb` & `nbsphinx-0.9.2/doc/subdir/a-notebook-in-a-subdir.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/subdir/gallery.ipynb` & `nbsphinx-0.9.2/doc/subdir/gallery.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/subdir/toctree.ipynb` & `nbsphinx-0.9.2/doc/subdir/toctree.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/timeout.ipynb` & `nbsphinx-0.9.2/doc/timeout.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/doc/usage.ipynb` & `nbsphinx-0.9.2/doc/usage.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999473905723906%*

 * *Differences: {"'cells'": "{9: {'source': {insert: [(121, '\\n'), (122, '* "*

 * *            "[sphinx_immaterial](https://github.com/jbms/sphinx-immaterial):\\n'), (123, '  "*

 * *            "[example](https://nbsphinx.readthedocs.io/en/immaterial-theme/),\\n'), (124, '  "*

 * *            "[usage](https://github.com/spatialaudio/nbsphinx/compare/immaterial-theme^...immaterial-theme)\\n')]}}}"}*

```diff
@@ -432,14 +432,18 @@
                 "  [example](https://nbsphinx.readthedocs.io/en/sphinx-book-theme/),\n",
                 "  [usage](https://github.com/spatialaudio/nbsphinx/compare/sphinx-book-theme^...sphinx-book-theme)\n",
                 "\n",
                 "* [sphinx_holoviz_theme](https://github.com/pyviz-dev/sphinx_holoviz_theme):\n",
                 "  [example](https://nbsphinx.readthedocs.io/en/holoviz-theme/),\n",
                 "  [usage](https://github.com/spatialaudio/nbsphinx/compare/holoviz-theme^...holoviz-theme)\n",
                 "\n",
+                "* [sphinx_immaterial](https://github.com/jbms/sphinx-immaterial):\n",
+                "  [example](https://nbsphinx.readthedocs.io/en/immaterial-theme/),\n",
+                "  [usage](https://github.com/spatialaudio/nbsphinx/compare/immaterial-theme^...immaterial-theme)\n",
+                "\n",
                 "* [sphinx_material](https://github.com/bashtage/sphinx-material):\n",
                 "  [example](https://nbsphinx.readthedocs.io/en/material-theme/),\n",
                 "  [usage](https://github.com/spatialaudio/nbsphinx/compare/material-theme^...material-theme)\n",
                 "\n",
                 "* [sphinx_py3doc_enhanced_theme](https://github.com/ionelmc/sphinx-py3doc-enhanced-theme):\n",
                 "  [example](https://nbsphinx.readthedocs.io/en/py3doc-enhanced-theme/),\n",
                 "  [usage](https://github.com/spatialaudio/nbsphinx/compare/py3doc-enhanced-theme^...py3doc-enhanced-theme)\n",
```

### Comparing `nbsphinx-0.9.1/doc/yet-another.ipynb` & `nbsphinx-0.9.2/doc/yet-another.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/setup.py` & `nbsphinx-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/src/nbsphinx/__init__.py` & `nbsphinx-0.9.2/src/nbsphinx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Jupyter Notebook Tools for Sphinx.
 
 https://nbsphinx.readthedocs.io/
 
 """
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 
 import collections.abc
 import copy
 import html
 from itertools import chain
 import json
 import os
@@ -25,14 +25,19 @@
 import sphinx
 import sphinx.directives
 import sphinx.directives.other
 import sphinx.environment
 import sphinx.errors
 import sphinx.transforms.post_transforms.images
 from sphinx.util.matching import patmatch
+try:
+    from sphinx.util.display import status_iterator
+except ImportError:
+    # This will be removed in Sphinx 8:
+    from sphinx.util import status_iterator
 import traitlets
 
 
 if sys.version_info >= (3, 8) and sys.platform == 'win32':
     # See: https://github.com/jupyter/jupyter_client/issues/583
     import asyncio
 
@@ -861,34 +866,44 @@
 
     """
     if from_format != 'markdown' and to_format != 'rst':
         raise ValueError('Unsupported conversion')
     return markdown2rst(text)
 
 
+_CITE_ROLES = {
+    'data-cite': 'cite',
+    'data-footcite': 'footcite',
+}
+_CITE_ROLES.update({
+    f'{k}-{suffix}': f'{v}:{suffix}'
+    for k, v in _CITE_ROLES.items()
+    for suffix in ('p', 'ps', 't', 'ts', 'ct', 'cts')
+})
+
+
 class CitationParser(html.parser.HTMLParser):
 
     def handle_starttag(self, tag, attrs):
         if self._check_cite(attrs):
             self.starttag = tag
 
     def handle_endtag(self, tag):
         self.endtag = tag
 
     def handle_startendtag(self, tag, attrs):
         self._check_cite(attrs)
 
     def _check_cite(self, attrs):
         for name, value in attrs:
-            if name == 'data-cite':
-                self.cite = ':cite:`' + value + '`'
-                return True
-            elif name == 'data-footcite':
-                self.cite = ':footcite:`' + value + '`'
-                return True
+            try:
+                self.cite = f':{_CITE_ROLES[name]}:`{value}`'
+            except KeyError:
+                continue
+            return True
         return False
 
     def reset(self):
         super().reset()
         self.starttag = ''
         self.endtag = ''
         self.cite = ''
@@ -1164,20 +1179,20 @@
         if not target:
             # No corresponding target, Sphinx may warn later
             return '', ''
         refuri = target.get('refuri')
         if not refuri:
             # Target doesn't have URI
             return '', ''
-    if '://' in refuri:
-        # Not a local link
-        return '', ''
-    elif refuri.startswith('#') or refuri.startswith('mailto:'):
+    if '://' in refuri or refuri.startswith('mailto:'):
         # Not a local link
         return '', ''
+    elif refuri.startswith('#'):
+        # Kinda not a local link
+        return '', refuri
 
     # NB: We look for "fragment identifier" before unquoting
     match = re.match(r'^([^#]*)(#.*)$', refuri)
     if match:
         filename = unquote(match.group(1))
         # NB: The "fragment identifier" is not unquoted
         fragment = match.group(2)
@@ -1210,15 +1225,23 @@
 
     def apply(self):
         env = self.document.settings.env
         for node in self.document.traverse(docutils.nodes.reference):
             filename, fragment = _local_file_from_reference(
                 node, self.document)
             if not filename:
-                continue
+                if fragment:
+                    # This should not be needed if it weren't for
+                    # https://github.com/sphinx-doc/sphinx/issues/11336 and
+                    # https://github.com/sphinx-doc/sphinx/issues/11335
+                    filename = os.path.basename(env.doc2path(env.docname))
+                    if fragment == '#':
+                        fragment = ''
+                else:
+                    continue
 
             for s in env.config.source_suffix:
                 if filename.lower().endswith(s.lower()):
                     assert len(s) > 0
                     target = filename[:-len(s)]
                     suffix = filename[-len(s):]
                     if fragment:
@@ -1627,15 +1650,14 @@
 
 
 def html_collect_pages(app):
     """This event handler is abused to copy local files around."""
     files = set()
     for file_list in app.env.nbsphinx_files.values():
         files.update(file_list)
-    status_iterator = sphinx.util.status_iterator
     for file in status_iterator(files, 'copying linked files... ',
                                 sphinx.util.console.brown, len(files)):
         target = os.path.join(app.builder.outdir, file)
         sphinx.util.ensuredir(os.path.dirname(target))
         try:
             sphinx.util.copyfile(os.path.join(app.env.srcdir, file), target)
         except OSError as err:
@@ -1905,17 +1927,25 @@
 
 
 def depart_admonition_html(self, node):
     self.body.append('</div>\n')
 
 
 def visit_admonition_latex(self, node):
-    # See http://tex.stackexchange.com/q/305898/:
-    self.body.append(
-        '\n\\begin{sphinxadmonition}{' + node['classes'][1] + '}{}\\unskip')
+    kind = node['classes'][1]
+    if len(node.children) >= 2 and isinstance(
+            node.children[0], docutils.nodes.paragraph):
+        title = node.children[0].astext()
+        del node.children[0]
+        self.body.append(
+            '\n\\begin{sphinxadmonition}{' + kind + '}{' + title + '}\\par')
+    else:
+        # See http://tex.stackexchange.com/q/305898/:
+        self.body.append(
+            '\n\\begin{sphinxadmonition}{' + kind + '}{}\\unskip')
 
 
 def depart_admonition_latex(self, node):
     self.body.append('\\end{sphinxadmonition}\n')
 
 
 def visit_admonition_text(self, node):
```

### Comparing `nbsphinx-0.9.1/src/nbsphinx/_static/nbsphinx-broken-thumbnail.svg` & `nbsphinx-0.9.2/src/nbsphinx/_static/nbsphinx-broken-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/src/nbsphinx/_static/nbsphinx-code-cells.css_t` & `nbsphinx-0.9.2/src/nbsphinx/_static/nbsphinx-code-cells.css_t`

 * *Files 7% similar despite different names*

```diff
@@ -58,20 +58,24 @@
 
 /* last container */
 div.nblast.container {
     padding-bottom: 5px;
 }
 
 /* input prompt */
-div.nbinput.container div.prompt pre {
+div.nbinput.container div.prompt pre,
+/* for sphinx_immaterial theme: */
+div.nbinput.container div.prompt pre > code {
     color: #307FC1;
 }
 
 /* output prompt */
-div.nboutput.container div.prompt pre {
+div.nboutput.container div.prompt pre,
+/* for sphinx_immaterial theme: */
+div.nboutput.container div.prompt pre > code {
     color: #BF5B3D;
 }
 
 /* all prompts */
 div.nbinput.container div.prompt,
 div.nboutput.container div.prompt {
     width: {{ nbsphinx_prompt_width }};
@@ -200,16 +204,18 @@
 
 /* fix copybtn overflow problem in chromium (needed for 'sphinx_copybutton') */
 div.nbinput.container div.input_area > div[class^='highlight'],
 div.nboutput.container div.output_area > div[class^='highlight']{
     overflow-y: hidden;
 }
 
-/* hide copybtn icon on prompts (needed for 'sphinx_copybutton') */
-.prompt .copybtn {
+/* hide copy button on prompts for 'sphinx_copybutton' extension ... */
+.prompt .copybtn,
+/* ... and 'sphinx_immaterial' theme */
+.prompt .md-clipboard.md-icon {
     display: none;
 }
 
 /* Some additional styling taken form the Jupyter notebook CSS */
 .jp-RenderedHTMLCommon table,
 div.rendered_html table {
   border: none;
```

### Comparing `nbsphinx-0.9.1/src/nbsphinx/_static/nbsphinx-gallery.css` & `nbsphinx-0.9.2/src/nbsphinx/_static/nbsphinx-gallery.css`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/src/nbsphinx/_static/nbsphinx-no-thumbnail.svg` & `nbsphinx-0.9.2/src/nbsphinx/_static/nbsphinx-no-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/src/nbsphinx/_texinputs/nbsphinx.sty` & `nbsphinx-0.9.2/src/nbsphinx/_texinputs/nbsphinx.sty`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.1/src/nbsphinx.egg-info/PKG-INFO` & `nbsphinx-0.9.2/src/nbsphinx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsphinx
-Version: 0.9.1
+Version: 0.9.2
 Summary: Jupyter Notebook Tools for Sphinx
 Home-page: https://nbsphinx.readthedocs.io/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: MIT
 Project-URL: Documentation, https://nbsphinx.readthedocs.io/
 Project-URL: Source Code, https://github.com/spatialaudio/nbsphinx/
```

### Comparing `nbsphinx-0.9.1/src/nbsphinx.egg-info/SOURCES.txt` & `nbsphinx-0.9.2/src/nbsphinx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

