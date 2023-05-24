# Comparing `tmp/bsplines2d-0.0.3.tar.gz` & `tmp/bsplines2d-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsplines2d-0.0.3.tar", last modified: Tue Apr 11 08:09:55 2023, max compression
+gzip compressed data, was "bsplines2d-0.0.4.tar", last modified: Wed May 24 16:39:12 2023, max compression
```

## Comparing `bsplines2d-0.0.3.tar` & `bsplines2d-0.0.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:55.593397 bsplines2d-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-11 08:09:55.593397 bsplines2d-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/_updateversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:55.589397 bsplines2d-0.0.3/bsplines2d/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_Mesh2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_checks_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_polar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_tri.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_outline.py
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_rect_cropping.py
--rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    22224 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    31494 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_BSplines2D.py
--rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_operators_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_operators_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_polar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_tri.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    27590 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_contours.py
--rw-r--r--   0 runner    (1001) docker     (123)    54051 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_interpolate_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    28950 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_plot_as_profile2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_plot_as_profile2d_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class03_Bins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class03_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class03_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    21736 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class11_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_generic_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_generic_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_utils_bsplines.py
--rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_utils_bsplines_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:55.589397 bsplines2d-0.0.3/bsplines2d/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_01_Mesh2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_02_BSplines2D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:55.593397 bsplines2d-0.0.3/bsplines2d/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_data/WEST_Poly.npz
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_data/WEST_trimesh.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_data/trimesh_quad.npz
--rw-r--r--   0 runner    (1001) docker     (123)    26411 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:55.589397 bsplines2d-0.0.3/bsplines2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:09:55.593397 bsplines2d-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:12.575929 bsplines2d-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-24 16:39:12.575929 bsplines2d-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/_updateversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:12.571929 bsplines2d-0.0.4/bsplines2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_Mesh2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_checks_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_polar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_tri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_outline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_rect_cropping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22224 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31494 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_BSplines2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_operators_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_operators_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_polar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_tri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27590 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_contours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54051 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_interpolate_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28950 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_plot_as_profile2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_plot_as_profile2d_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class03_Bins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class03_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class03_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21736 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class11_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_generic_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_generic_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_utils_bsplines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_utils_bsplines_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:12.575929 bsplines2d-0.0.4/bsplines2d/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_01_Mesh2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_02_BSplines2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:12.575929 bsplines2d-0.0.4/bsplines2d/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_data/WEST_Poly.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_data/WEST_trimesh.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_data/trimesh_quad.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    26411 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:12.571929 bsplines2d-0.0.4/bsplines2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:39:12.575929 bsplines2d-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/setup.py
```

### Comparing `bsplines2d-0.0.3/LICENSE` & `bsplines2d-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/PKG-INFO` & `bsplines2d-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsplines2d
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library for generic multidimensional bsplines on various meshes, using datastock
 Home-page: https://github.com/ToFuProject/bsplines2d
 Author: Didier VEZINET
 Author-email: didier.vezinet@gmail.com
 License: MIT
 Keywords: bsplines data analysis modelling mesh plot
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bsplines2d-0.0.3/_updateversion.py` & `bsplines2d-0.0.4/_updateversion.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class01_Mesh2D.py` & `bsplines2d-0.0.4/bsplines2d/_class01_Mesh2D.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class01_checks_1d.py` & `bsplines2d-0.0.4/bsplines2d/_class01_checks_1d.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_polar.py` & `bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_polar.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_rect.py` & `bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_rect.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_tri.py` & `bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_tri.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class01_outline.py` & `bsplines2d-0.0.4/bsplines2d/_class01_outline.py`

 * *Files 26% similar despite different names*

```diff
@@ -111,94 +111,186 @@
         x0min, x0max = knots0.min(), knots0.max()
         x1min, x1max = knots1.min(), knots1.max()
         x0 = np.r_[x0min, x0max, x0max, x0min]
         x1 = np.r_[x1min, x1min, x1max, x1max]
 
     else:
         crop = coll.ddata[crop]['data']
-        crop0, crop1 = (~crop).nonzero()
-        crop = np.array([crop0, crop1]).T.tolist()
 
         # indices of knots
         (i0, i1), (ic0, ic1) = coll.select_mesh_elements(
             key=key,
             crop=True,
             elements='knots',
             returnas='ind',
             return_neighbours=True,
         )
 
         # only keep edge knots
         i0min, i1min = i0.min(), i1.min()
         i0max, i1max = i0.max(), i1.max()
 
+        # get indices of edge knots
+        iok = (ic0 >= 0) & (ic1 >= 0)
         ind0 = np.array([
-            np.any([[ic0[ii, jj], ic1[ii, jj]] in crop for jj in [0, 1, 2, 3]])
+            np.any(~crop[ic0[ii, iok[ii, :]], ic1[ii, iok[ii, :]]])
             for ii in range(i0.size)
         ])
+
+        # get subest of extreme coordinates
         ind = (
             ind0
             | (i0 == i0min) | (i0 == i0max)
             | (i1 == i1min) | (i1 == i1max)
         )
         if not np.any(ind):
             import pdb; pdb.set_trace()     # DB
             pass
 
-        i00 = np.min(i0[ind])
-        p0 = [i00, np.min(i1[ind][i0[ind] == i00])]
-        pall = np.array([i0[ind], i1[ind]]).T.tolist()
+        # keep only limits
+        i0 = i0[ind]
+        i1 = i1[ind]
+        ic0 = ic0[ind, :]
+        ic1 = ic1[ind, :]
+
+        # get starting point
+        i0_min = np.min(i0)
+        i1_min = np.min(i1[i0 == i0_min])
+        ii0 = ((i0 == i0_min) & (i1 == i1_min)).nonzero()[0][0]
+
+        # pall = list(range(0, i0.size))
+
+        p0 = [i0[ii0], i1[ii0]]
+        pall = np.array([i0, i1]).T.tolist()
+
         lp = [p0]
+        pall.remove(p0)
 
         old = None
-        while len(lp) == 1 or lp[-1] != p0:
-            pp, old = _next_pp(
+        # while len(lp) == 1 or lp[-1] != p0:
+        while len(pall) > 0:
+            pp, old, ii0 = _next_pp(
                 p0=lp[-1],
+                ii0=ii0,
                 pall=pall,
+                i0=i0,
+                i1=i1,
+                ic0=ic0,
+                ic1=ic1,
+                crop=crop,
                 old=old,
             )
+
+            # ------ DEBUG --------
+            if pp is None:
+                import matplotlib.pyplot as plt
+                dax = coll.plot_mesh(key)
+                plt.gca().plot(
+                    knots0[np.array(lp)[:, 0]],
+                    knots1[np.array(lp)[:, 1]],
+                    ls='-',
+                    marker='o',
+                    lw=2,
+                )
+                plt.gca().plot(
+                    knots0[i0],
+                    knots1[i1],
+                    ls='None',
+                    marker='x',
+                )
+                import pdb; pdb.set_trace()     # DB
+            # -----------------------
+
             lp.append(pp)
 
         i0, i1 = np.array(lp).T
         x0 = knots0[i0]
         x1 = knots1[i1]
 
     return x0, x1
 
 
-def _next_pp(p0=None, pall=None, old=None):
+def _next_pp(
+    p0=None,
+    ii0=None,
+    pall=None,
+    i0=None,
+    i1=None,
+    ic0=None,
+    ic1=None,
+    crop=None,
+    old=None,
+):
 
     # inc0, inc1
-
     p1 = np.copy(p0)
     found = False
     ldir = [(1, 0), (0, 1), (-1, 0), (0, -1)]
     if old is not None:
         ldir = [pp for pp in ldir if pp != old]
 
-    for (ic0, ic1) in ldir:
+    for (ip0, ip1) in ldir:
 
         stop = False
         while stop is False:
 
-            p2 = [p1[0] + ic0, p1[1] + ic1]
+            p2 = [p1[0] + ip0, p1[1] + ip1]
+
             if p2 in pall:
-                p1 = p2
-                found = True
+
+                ii2 = ((i0 == p2[0]) & (i1 == p2[1])).nonzero()[0][0]
+                icc0 = np.intersect1d(
+                    ic0[ii0, :],
+                    ic0[ii2, :],
+                    assume_unique=False,
+                    return_indices=False,
+                )
+                icc1 = np.intersect1d(
+                    ic1[ii0, :],
+                    ic1[ii2, :],
+                    assume_unique=False,
+                    return_indices=False,
+                )
+
+                i00 = np.array([
+                    (ic0[ii0, :] == cc0).nonzero()[0] for cc0 in icc0
+                ]).ravel()
+                i11 = np.array([
+                    (ic1[ii0, :] == cc1).nonzero()[0] for cc1 in icc1
+                ]).ravel()
+
+                ic = np.intersect1d(
+                    i00,
+                    i11,
+                    assume_unique=False,
+                    return_indices=False,
+                )
+
+                c0 = np.any(crop[ic0[ii0, ic], ic1[ii0, ic]])
+
+                if c0:
+                    p1 = p2
+                    ii0 = ii2
+                    found = True
+                    pall.remove(p2)
+
+                else:
+                    stop = True
+
             else:
                 stop = True
 
         if found is True:
-            new = (-ic0, -ic1)
+            new = (-ip0, -ip1)
             break
 
     if found is False:
-        raise Exception("Next point not found!")
+        return None, None, None
 
-    return p1, new
+    return p1, new, ii0
 
 
 # ###############################################################
 # ###############################################################
 #               triangular
 # ###############################################################
```

### Comparing `bsplines2d-0.0.3/bsplines2d/_class01_plot.py` & `bsplines2d-0.0.4/bsplines2d/_class01_plot.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class01_rect_cropping.py` & `bsplines2d-0.0.4/bsplines2d/_class01_rect_cropping.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class01_sample.py` & `bsplines2d-0.0.4/bsplines2d/_class01_sample.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class01_select.py` & `bsplines2d-0.0.4/bsplines2d/_class01_select.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_BSplines2D.py` & `bsplines2d-0.0.4/bsplines2d/_class02_BSplines2D.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_1d.py` & `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_1d.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_operators_1d.py` & `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_operators_1d.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_operators_rect.py` & `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_operators_rect.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_polar.py` & `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_polar.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_rect.py` & `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_rect.py`

 * *Files 5% similar despite different names*

```diff
@@ -248,14 +248,19 @@
                 continue
             indok0 = np.copy(indok1)
 
             ind0 = indbs_tf[1] == iz
             i0 = indbs_tf[0][ind0]
             for ii, ii0 in enumerate(i0):
 
+                msg = (
+                    f'\t bspline {indtot[ind0][ii]} / {nbs}   ({x0.size} pts)'
+                )
+                print(msg, end='\r', flush=True)
+
                 if ii > 0:
                     indok0[...] = indok1
 
                 out0 = np.full((indok1.sum(), 1), np.nan)
 
                 scpinterp._bspl.evaluate_spline(
                     self.knots_per_bs_x0_pad[:, ii0],
```

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_tri.py` & `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_tri.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_checks.py` & `bsplines2d-0.0.4/bsplines2d/_class02_checks.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_compute.py` & `bsplines2d-0.0.4/bsplines2d/_class02_compute.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_contours.py` & `bsplines2d-0.0.4/bsplines2d/_class02_contours.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_interpolate.py` & `bsplines2d-0.0.4/bsplines2d/_class02_interpolate.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_interpolate_all.py` & `bsplines2d-0.0.4/bsplines2d/_class02_interpolate_all.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_operators.py` & `bsplines2d-0.0.4/bsplines2d/_class02_operators.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_plot.py` & `bsplines2d-0.0.4/bsplines2d/_class02_plot.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_plot_as_profile2d.py` & `bsplines2d-0.0.4/bsplines2d/_class02_plot_as_profile2d.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class02_plot_as_profile2d_compare.py` & `bsplines2d-0.0.4/bsplines2d/_class02_plot_as_profile2d_compare.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class03_Bins.py` & `bsplines2d-0.0.4/bsplines2d/_class03_Bins.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class03_binning.py` & `bsplines2d-0.0.4/bsplines2d/_class03_binning.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class03_checks.py` & `bsplines2d-0.0.4/bsplines2d/_class03_checks.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_class11_plot.py` & `bsplines2d-0.0.4/bsplines2d/_class11_plot.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_generic_check.py` & `bsplines2d-0.0.4/bsplines2d/_generic_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,22 +49,24 @@
             and (
                 (
                     issubclass(v0.__class__, plt.Axes)
                 )
                 or (
                     isinstance(v0, dict)
                     and issubclass(v0.get('handle').__class__, plt.Axes)
-                    and v0.get('type') in _LALLOWED_AXESTYPES
+                    # and v0.get('type') in _LALLOWED_AXESTYPES
                 )
             )
             for k0, v0 in dax.items()
         ])
     )
     if not c0:
         msg = (
+            "Arg dax is not conform:\n"
+            + str(dax)
         )
         import pdb; pdb.set_trace()     # DB
         raise Exception(msg)
 
     for k0, v0 in dax.items():
         if issubclass(v0.__class__, plt.Axes):
             dax[k0] = {'handle': v0, 'type': k0}
```

### Comparing `bsplines2d-0.0.3/bsplines2d/_generic_mesh.py` & `bsplines2d-0.0.4/bsplines2d/_generic_mesh.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_utils_bsplines.py` & `bsplines2d-0.0.4/bsplines2d/_utils_bsplines.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/_utils_bsplines_operators.py` & `bsplines2d-0.0.4/bsplines2d/_utils_bsplines_operators.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/tests/test_01_Mesh2D.py` & `bsplines2d-0.0.4/bsplines2d/tests/test_01_Mesh2D.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/tests/test_02_BSplines2D.py` & `bsplines2d-0.0.4/bsplines2d/tests/test_02_BSplines2D.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/tests/test_data/WEST_Poly.npz` & `bsplines2d-0.0.4/bsplines2d/tests/test_data/WEST_Poly.npz`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/tests/test_data/WEST_trimesh.npz` & `bsplines2d-0.0.4/bsplines2d/tests/test_data/WEST_trimesh.npz`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/tests/test_data/trimesh_quad.npz` & `bsplines2d-0.0.4/bsplines2d/tests/test_data/trimesh_quad.npz`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d/tests/test_input.py` & `bsplines2d-0.0.4/bsplines2d/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/bsplines2d.egg-info/PKG-INFO` & `bsplines2d-0.0.4/bsplines2d.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsplines2d
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library for generic multidimensional bsplines on various meshes, using datastock
 Home-page: https://github.com/ToFuProject/bsplines2d
 Author: Didier VEZINET
 Author-email: didier.vezinet@gmail.com
 License: MIT
 Keywords: bsplines data analysis modelling mesh plot
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bsplines2d-0.0.3/bsplines2d.egg-info/SOURCES.txt` & `bsplines2d-0.0.4/bsplines2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.3/setup.py` & `bsplines2d-0.0.4/setup.py`

 * *Files identical despite different names*

