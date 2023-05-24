# Comparing `tmp/pyhalo-0.2.0.tar.gz` & `tmp/pyhalo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhalo-0.2.0.tar", last modified: Wed May 10 03:55:10 2023, max compression
+gzip compressed data, was "pyhalo-0.2.1.tar", last modified: Wed May 24 16:06:12 2023, max compression
```

## Comparing `pyhalo-0.2.0.tar` & `pyhalo-0.2.1.tar`

### file list

```diff
@@ -1,85 +1,128 @@
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.822519 pyhalo-0.2.0/
--rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.0/AUTHORS.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.0/HISTORY.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.0/LICENSE
--rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.0/MANIFEST.in
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-10 03:55:10.822922 pyhalo-0.2.0/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     2052 2023-05-10 03:31:30.000000 pyhalo-0.2.0/README.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.419995 pyhalo-0.2.0/docs/
--rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/Makefile
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/authors.rst
--rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.0/docs/conf.py
--rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/contributing.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/history.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/index.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/installation.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/make.bat
--rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/readme.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/usage.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.454563 pyhalo-0.2.0/pyHalo/
--rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.0/pyHalo/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2570 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/concentration_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/defaults.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2447 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    36931 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/pyhalo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/realization_extensions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    36187 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1176 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/truncation_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    13604 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/utilities.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.476848 pyhalo-0.2.0/pyHalo.egg-info/
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     2539 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/SOURCES.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/dependency_links.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/entry_points.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.0/pyHalo.egg-info/not-zip-safe
--rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/requires.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        7 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/top_level.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-05-10 03:37:12.000000 pyhalo-0.2.0/pyproject.toml
--rw-r--r--   0 danielgilman   (501) staff       (20)      389 2023-05-10 03:55:10.824897 pyhalo-0.2.0/setup.cfg
--rw-r--r--   0 danielgilman   (501) staff       (20)     1594 2023-05-10 03:31:45.000000 pyhalo-0.2.0/setup.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.665311 pyhalo-0.2.0/tests/
--rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.0/tests/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1688 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_concentration_models.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.671231 pyhalo-0.2.0/tests/test_cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.0/tests/test_cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_cosmology/test_cone_geometry.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_cosmology/test_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_cosmology/test_cylinder_geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.800078 pyhalo-0.2.0/tests/test_halos/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.0/tests/test_halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2981 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_adiabatic_tides.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_concentrations.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4656 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_general_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_lenscosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_nfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_pjaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_point_mass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2719 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_tnfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2446 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_uldm.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_util.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3224 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_pyhalo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_realization_extensions.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.811419 pyhalo-0.2.0/tests/test_rendering/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.0/tests/test_rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_2halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_los.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.816602 pyhalo-0.2.0/tests/test_rendering/test_mass_functions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_mass_functions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-10 03:38:38.000000 pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_base_functions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    11175 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_population.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.821311 pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2191 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3373 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.597891 pyhalo-0.2.1/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.1/AUTHORS.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.1/HISTORY.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.1/LICENSE
+-rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.1/MANIFEST.in
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-24 16:06:12.596954 pyhalo-0.2.1/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1998 2023-05-18 15:44:57.000000 pyhalo-0.2.1/README.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.485276 pyhalo-0.2.1/docs/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/Makefile
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/authors.rst
+-rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.1/docs/conf.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/contributing.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/history.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/index.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/installation.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/make.bat
+-rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/readme.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/usage.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.495010 pyhalo-0.2.1/pyHalo/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.501973 pyhalo-0.2.1/pyHalo/Cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.1/pyHalo/Cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Cosmology/cosmology.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Cosmology/geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.506981 pyhalo-0.2.1/pyHalo/Halos/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.516430 pyhalo-0.2.1/pyHalo/Halos/HaloModels/
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/NFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/PTMass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/PsuedoJaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3967 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/TNFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/TNFWemulator.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/ULDM.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/generalized_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/powerlaw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.1/pyHalo/Halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8643 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/concentration.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5373 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/halo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/lens_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10172 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/tidal_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.525528 pyhalo-0.2.1/pyHalo/Rendering/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.531565 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/density_peaks.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/mass_function_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.537964 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3156 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4384 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.1/pyHalo/Rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/correlated_structure.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/halo_population.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4621 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/line_of_sight.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/rendering_class_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5972 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/two_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.1/pyHalo/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2570 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/concentration_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/defaults.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2447 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    46842 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/pyhalo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/realization_extensions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    36187 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1176 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/truncation_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    13604 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.499773 pyhalo-0.2.1/pyHalo.egg-info/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3893 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/entry_points.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.1/pyHalo.egg-info/not-zip-safe
+-rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/requires.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/top_level.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-05-24 16:05:34.000000 pyhalo-0.2.1/pyproject.toml
+-rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-05-24 16:06:12.598186 pyhalo-0.2.1/setup.cfg
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.1/setup.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.557114 pyhalo-0.2.1/tests/
+-rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.1/tests/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1688 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_concentration_models.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.560510 pyhalo-0.2.1/tests/test_cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.1/tests/test_cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_cosmology/test_cone_geometry.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_cosmology/test_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_cosmology/test_cylinder_geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.587367 pyhalo-0.2.1/tests/test_halos/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.1/tests/test_halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3025 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_adiabatic_tides.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_concentrations.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.1/tests/test_halos/test_general_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_lenscosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_nfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_pjaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_point_mass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.1/tests/test_halos/test_powerlaw_profile.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2719 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_tnfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2401 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_uldm.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_util.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3224 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_pyhalo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_realization_extensions.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.590775 pyhalo-0.2.1/tests/test_rendering/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.1/tests/test_rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_2halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_los.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.593581 pyhalo-0.2.1/tests/test_rendering/test_mass_functions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_mass_functions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_base_functions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    11175 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_population.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.596062 pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2191 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3373 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_utilities.py
```

### Comparing `pyhalo-0.2.0/CONTRIBUTING.rst` & `pyhalo-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/LICENSE` & `pyhalo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/PKG-INFO` & `pyhalo-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.0/README.rst` & `pyhalo-0.2.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 .. image:: https://travis-ci.com/dangilman/pyHalo.svg?branch=master
         :target: https://travis-ci.com/dangilman/pyHalo
 
 .. image:: https://coveralls.io/repos/github/dangilman/pyHalo/badge.svg?branch=master
         :target: https://coveralls.io/github/dangilman/pyHalo?branch=master
         
 .. image:: https://badge.fury.io/py/pyhalo.svg
-        :target: https://badge.fury.io/py/pyhalo.svg
+    :target: https://badge.fury.io/py/pyhalo
         
 .. image:: https://github.com/dangilman/pyHalo/blob/master/readme_fig.jpg
         :target: https://github.com/dangilman/pyHalo/blob/master/readme_fig
 
 pyHalo renders full mass distributions for substructure lensing simulations with the open source gravitational lensing software package lenstronomy (https://github.com/sibirrer/lenstronomy). The example notebooks illustrate the core functionality of this package. 
 
 If you would like to use this package and have questions, please get in touch with me at daniel.gilman@utoronto.ca - I am happy to help! 
 
 Installation
 ------------
-Download from pypi: pip install pyhalo
+Clone the repository, navigate into the directory that contains the setup.py file and run "python setup.py install"
 
-For earlier releases: clone the repository, select the version you want to download from the commit history (first code release is 8302393), clone it, run python3 setup.py develop --user. 
+The first code release, before majoring refactoring, is 8302393. 
 
 In order to use this package when not installing via pip, you'll need to install colossus http://www.benediktdiemer.com/code/colossus/ 
 
 Features
 --------
 
 - Quickly render full populations of dark matter subhalos and line of sight halos for gravitational lensing simulations. Implemented models currently include cold and warm dark matter, custom mass-concentration relations, self-interacting dark matter, and more.
```

### Comparing `pyhalo-0.2.0/docs/Makefile` & `pyhalo-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/docs/conf.py` & `pyhalo-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/docs/installation.rst` & `pyhalo-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/docs/make.bat` & `pyhalo-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/pyHalo/concentration_models.py` & `pyhalo-0.2.1/pyHalo/concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/pyHalo/defaults.py` & `pyhalo-0.2.1/pyHalo/defaults.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/pyHalo/mass_function_models.py` & `pyhalo-0.2.1/pyHalo/mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/pyHalo/preset_models.py` & `pyhalo-0.2.1/pyHalo/preset_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,38 +49,47 @@
         concentration_model_fieldhalos='DIEMERJOYCE19', kwargs_concentration_model_fieldhalos={},
         truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_trunction_model_subhalos={},
         truncation_model_fieldhalos='TRUNCATION_RN', kwargs_truncation_model_fieldhalos={},
         shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3,  r_tidal=0.25,
         LOS_normalization=1.0, two_halo_contribution=True, delta_power_law_index=0.0,
         geometry_type='DOUBLE_CONE', kwargs_cosmo=None):
     """
+    This class generates realizations of dark matter structure in Cold Dark Matter
 
-    :param z_lens:
-    :param z_source:
-    :param sigma_sub:
-    :param log_mlow:
-    :param log_mhigh:
-    :param concentration_model_subhalos:
-    :param kwargs_concentration_model_subhalos:
-    :param concentration_model_fieldhalos:
-    :param kwargs_concentration_model_fieldhalos:
-    :param truncation_model_subhalos:
-    :param kwargs_trunction_model_subhalos:
-    :param truncation_model_fieldhalos:
-    :param kwargs_truncation_model_fieldhalos:
-    :param shmf_log_slope:
-    :param cone_opening_angle_arcsec:
-    :param log_m_host:
-    :param r_tidal:
-    :param LOS_normalization:
-    :param two_halo_contribution:
-    :param delta_power_law_index:
-    :param geometry_type:
-    :param kwargs_cosmo:
-    :return:
+    :param z_lens: main deflector redshift
+    :param z_source: source redshift
+    :param sigma_sub: amplitude of the subhalo mass function at 10^8 solar masses in units [# of halos / kpc^2]
+    :param log_mlow: log base 10 of the minimum halo mass to render
+    :param log_mhigh: log base 10 of the maximum halo mass to render
+    :param concentration_model_subhalos: the concentration-mass relation applied to subhalos,
+    see concentration_models.py for a complete list of available models
+    :param kwargs_concentration_model_subhalos: keyword arguments for the subhalo MC relation
+    NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
+    :param concentration_model_subhalos: the concentration-mass relation applied to field halos,
+    see concentration_models.py for a complete list of available models
+    :param kwargs_concentration_model_fieldhalos: keyword arguments for the field halo MC relation
+    NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
+    :param truncation_model_subhalos: the truncation model applied to subhalos, see truncation_models for a complete list
+    :param kwargs_trunction_model_subhalos: keyword arguments for the truncation model applied to subhalos
+    :param truncation_model_fieldhalos: the truncation model applied to field halos, see truncation_models for a
+    complete list
+    :param kwargs_truncation_model_fieldhalos: keyword arguments for the truncation model applied to field halos
+    :param shmf_log_slope: the logarithmic slope of the subhalo mass function pivoting around 10^8 M_sun
+    :param cone_opening_angle_arcsec: the opening angle of the rendering volume in arcsec
+    :param log_m_host: log base 10 of the host halo mass [M_sun]
+    :param r_tidal: the core radius of the host halo in units of the host halo scale radius. Subhalos are distributed
+    in 3D with a cored NFW profile with this core radius
+    :param LOS_normalization: rescales the amplitude of the line-of-sight halo mass function
+    :param two_halo_contribution: bool; turns on and off the two-halo term
+    :param delta_power_law_index: tilts the logarithmic slope of the subhalo and field halo mass functions around pivot
+    at 10^8 M_sun
+    :param geometry_type: string that specifies the geometry of the rendering volume; options include
+    DOUBLE_CONE, CONE, CYLINDER
+    :param kwargs_cosmo: keyword arguments that specify the cosmology (see pyHalo.Cosmology.cosmology)
+    :return: a realization of dark matter halos
     """
 
     # FIRST WE CREATE AN INSTANCE OF PYHALO, WHICH SETS THE COSMOLOGY
     pyhalo = pyHalo(z_lens, z_source, kwargs_cosmo)
     # WE ALSO SPECIFY THE GEOMETRY OF THE RENDERING VOLUME
     geometry = Geometry(pyhalo.cosmology, z_lens, z_source,
                         cone_opening_angle_arcsec, geometry_type)
@@ -163,55 +172,62 @@
     realization_list = pyhalo.render(population_model_list, mass_function_class_list, kwargs_mass_function_list,
                                           spatial_distribution_class_list, kwargs_spatial_distribution_list,
                                           geometry, mdef_subhalos, mdef_field_halos, kwargs_halo_model, nrealizations=1)
     return realization_list[0]
 
 
 def WDM(z_lens, z_source, log_mc, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
-        mass_function_model_subhalos='SHMF_LOVELL2020', kwargs_mass_function_subhalos={},
+        mass_function_model_subhalos='LOVELL2020', kwargs_mass_function_subhalos={},
         mass_function_model_fieldhalos='LOVELL2020', kwargs_mass_function_fieldhalos={},
         concentration_model_subhalos='BOSE2016', kwargs_concentration_model_subhalos={},
         concentration_model_fieldhalos='BOSE2016', kwargs_concentration_model_fieldhalos={},
         truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_trunction_model_subhalos={},
         truncation_model_fieldhalos='TRUNCATION_RN', kwargs_truncation_model_fieldhalos={},
         shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3, r_tidal=0.25,
         LOS_normalization=1.0, geometry_type='DOUBLE_CONE', kwargs_cosmo=None,
         mdef_subhalos='TNFW', mdef_field_halos='TNFW', kwargs_density_profile={}):
 
     """
+    This class generates realizations of dark matter structure in Warm Dark Matter
 
-    :param z_lens:
-    :param z_source:
-    :param log_mc:
-    :param sigma_sub:
-    :param log_mlow:
-    :param log_mhigh:
-    :param mass_function_model_subhalos:
-    :param kwargs_mass_function_subhalos:
-    :param mass_function_model_fieldhalos:
-    :param kwargs_mass_function_fieldhalos:
-    :param concentration_model_subhalos:
-    :param kwargs_concentration_model_subhalos:
-    :param concentration_model_fieldhalos:
-    :param kwargs_concentration_model_fieldhalos:
-    :param truncation_model_subhalos:
-    :param kwargs_trunction_model_subhalos:
-    :param truncation_model_fieldhalos:
-    :param kwargs_truncation_model_fieldhalos:
-    :param shmf_log_slope:
-    :param cone_opening_angle_arcsec:
-    :param log_m_host:
-    :param r_tidal:
-    :param LOS_normalization:
-    :param geometry_type:
-    :param kwargs_cosmo:
-    :param mdef_subhalos:
-    :param mdef_field_halos:
-    :param kwargs_density_profile:
-    :return:
+    :param z_lens: main deflector redshift
+    :param z_source: source redshift
+    :param log_mc: the log base 10 of the half-mode mass
+    :param sigma_sub: amplitude of the subhalo mass function at 10^8 solar masses in units [# of halos / kpc^2]
+    :param log_mlow: log base 10 of the minimum halo mass to render
+    :param log_mhigh: log base 10 of the maximum halo mass to render
+    :param mass_function_model_subhalos: mass function model for subhalos, see mass_function_models.py for a list
+    :param kwargs_mass_function_subhalos: keyword arguments for the mass function model
+    :param mass_function_model_fieldhalos: mass function model for field halos, see mass_function_models.py for a list
+    :param kwargs_mass_function_fieldhalos: keyword arguments for the mass function model
+    :param concentration_model_subhalos: the concentration-mass relation applied to subhalos,
+    see concentration_models.py for a complete list of available models
+    :param kwargs_concentration_model_subhalos: keyword arguments for the subhalo MC relation
+    NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
+    :param concentration_model_subhalos: the concentration-mass relation applied to field halos,
+    see concentration_models.py for a complete list of available models
+    :param kwargs_concentration_model_fieldhalos: keyword arguments for the field halo MC relation
+    NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
+    :param truncation_model_subhalos: the truncation model applied to subhalos, see truncation_models for a complete list
+    :param kwargs_trunction_model_subhalos: keyword arguments for the truncation model applied to subhalos
+    :param truncation_model_fieldhalos: the truncation model applied to field halos, see truncation_models for a
+    complete list
+    :param kwargs_truncation_model_fieldhalos: keyword arguments for the truncation model applied to field halos
+    :param shmf_log_slope: the logarithmic slope of the subhalo mass function pivoting around 10^8 M_sun
+    :param cone_opening_angle_arcsec: the opening angle of the rendering volume in arcsec
+    :param log_m_host: log base 10 of the host halo mass [M_sun]
+    :param r_tidal: the core radius of the host halo in units of the host halo scale radius. Subhalos are distributed
+    in 3D with a cored NFW profile with this core radius
+    :param geometry_type: string that specifies the geometry of the rendering volume; options include
+    DOUBLE_CONE, CONE, CYLINDER
+    :param kwargs_cosmo: keyword arguments that specify the cosmology (see pyHalo.Cosmology.cosmology)
+    :param mdef_subhalos: mass definition for subhalos
+    :param mdef_field_halos: mass definition for field halos
+    :param kwargs_density_profile: keyword arguments for the specified mass profile
+    :return: a realization of dark matter halos
     """
     # FIRST WE CREATE AN INSTANCE OF PYHALO, WHICH SETS THE COSMOLOGY
     pyhalo = pyHalo(z_lens, z_source, kwargs_cosmo)
     # WE ALSO SPECIFY THE GEOMETRY OF THE RENDERING VOLUME
     geometry = Geometry(pyhalo.cosmology, z_lens, z_source,
                         cone_opening_angle_arcsec, geometry_type)
 
@@ -306,17 +322,16 @@
         mass_function_model_subhalos='SHMF_SCHIVE2016', kwargs_mass_function_subhalos={},
         mass_function_model_fieldhalos='SCHIVE2016', kwargs_mass_function_fieldhalos={},
         concentration_model_subhalos='LAROCHE2022', kwargs_concentration_model_subhalos={},
         concentration_model_fieldhalos='LAROCHE2022', kwargs_concentration_model_fieldhalos={},
         truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_trunction_model_subhalos={},
         truncation_model_fieldhalos='TRUNCATION_RN', kwargs_truncation_model_fieldhalos={},
         shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3, r_tidal=0.25,
-        LOS_normalization=1.0, geometry_type='DOUBLE_CONE', kwargs_cosmo=None, kwargs_density_profile={},
-         uldm_plaw=1 / 3, scale_nfw=False, flucs=True, flucs_shape='aperture', flucs_args={}, n_cut=50000,
-         rescale_fluc_amp=True, r_ein=1.0):
+        LOS_normalization=1.0, geometry_type='DOUBLE_CONE', kwargs_cosmo=None,
+         uldm_plaw=1 / 3, flucs=True, flucs_shape='aperture', flucs_args={}, n_cut=50000, r_ein=1.0):
 
     """
     This generates realizations of ultra-light dark matter (ULDM), including the ULDM halo mass function and halo density profiles,
     as well as density fluctuations in the main deflector halo.
 
     Similarly to WDMGeneral, the functional form of the subhalo mass function is the same as the field halo mass function.
     However, this model differs from WDMGeneral by creating halos which are composite ULDM + NFW density profiles.
@@ -370,59 +385,73 @@
 
     and
 
         Zeta(z) = (18*pi^2 + 82(Om(z) - 1) - 39(Om(z) - 1)^2) / Om(z),
 
     where Om(z) is the matter density parameter.
 
-    :param z_lens:
-    :param z_source:
-    :param log10_m_uldm:
-    :param log10_fluc_amplitude:
-    :param fluctuation_size_scale:
-    :param fluctuation_size_dispersion:
-    :param n_fluc_scale:
-    :param velocity_scale:
-    :param sigma_sub:
-    :param log_mlow:
-    :param log_mhigh:
-    :param mass_function_model_subhalos:
-    :param kwargs_mass_function_subhalos:
-    :param mass_function_model_fieldhalos:
-    :param kwargs_mass_function_fieldhalos:
-    :param concentration_model_subhalos:
-    :param kwargs_concentration_model_subhalos:
-    :param concentration_model_fieldhalos:
-    :param kwargs_concentration_model_fieldhalos:
-    :param truncation_model_subhalos:
-    :param kwargs_trunction_model_subhalos:
-    :param truncation_model_fieldhalos:
-    :param kwargs_truncation_model_fieldhalos:
-    :param shmf_log_slope:
-    :param cone_opening_angle_arcsec:
-    :param log_m_host:
-    :param r_tidal:
-    :param LOS_normalization:
-    :param geometry_type:
-    :param kwargs_cosmo:
-    :param kwargs_density_profile:
-    :return:
+    :param z_lens: main deflector redshift
+    :param z_source: source redshift
+    :param log10_m_uldm: log base 10 of the ULDM particle mass
+    :param log10_fluc_amplitude: log base 10 of the fluctuation amplitude in the host halo density profile
+    :param fluctuation_size_scale: sets the size of the fluctuations in host halo in units of de-Broglie wavelength
+    :param fluctuation_size_dispersion: sets the variance of the size of the fluctuations
+    :param n_fluc_scale: rescales the number of fluctuations
+    :param velocity_scale: the velocity scale of the host halo used to convert particle mass to de-Broglie wavelength
+    :param sigma_sub: amplitude of the subhalo mass function at 10^8 solar masses in units [# of halos / kpc^2]
+    :param log_mlow: log base 10 of the minimum halo mass to render
+    :param log_mhigh: log base 10 of the maximum halo mass to render
+    :param mass_function_model_subhalos: mass function model for subhalos, see mass_function_models.py for a list
+    :param kwargs_mass_function_subhalos: keyword arguments for the mass function model
+    :param mass_function_model_fieldhalos: mass function model for field halos, see mass_function_models.py for a list
+    :param kwargs_mass_function_fieldhalos: keyword arguments for the mass function model
+    :param concentration_model_subhalos: the concentration-mass relation applied to subhalos,
+    see concentration_models.py for a complete list of available models
+    :param kwargs_concentration_model_subhalos: keyword arguments for the subhalo MC relation
+    NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
+    :param concentration_model_subhalos: the concentration-mass relation applied to field halos,
+    see concentration_models.py for a complete list of available models
+    :param kwargs_concentration_model_fieldhalos: keyword arguments for the field halo MC relation
+    NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
+    :param truncation_model_subhalos: the truncation model applied to subhalos, see truncation_models for a complete list
+    :param kwargs_trunction_model_subhalos: keyword arguments for the truncation model applied to subhalos
+    :param truncation_model_fieldhalos: the truncation model applied to field halos, see truncation_models for a
+    complete list
+    :param kwargs_truncation_model_fieldhalos: keyword arguments for the truncation model applied to field halos
+    :param shmf_log_slope: the logarithmic slope of the subhalo mass function pivoting around 10^8 M_sun
+    :param cone_opening_angle_arcsec: the opening angle of the rendering volume in arcsec
+    :param log_m_host: log base 10 of the host halo mass [M_sun]
+    :param r_tidal: the core radius of the host halo in units of the host halo scale radius. Subhalos are distributed
+    in 3D with a cored NFW profile with this core radius
+    :param geometry_type: string that specifies the geometry of the rendering volume; options include
+    DOUBLE_CONE, CONE, CYLINDER
+    :param kwargs_cosmo: keyword arguments that specify the cosmology, see Cosmology/cosmology.py
+    :param uldm_plaw: sets the exponent for the core size/halo mass relation in ULDM
+    :param flucs: bool; turns of/off fluctuations in the host halo density profile
+    :param flucs_shape: the geometry in which to render fluctuations, options include 'aperture', 'ring', 'ellipse'
+    :param flucs_args: keyword arguments for the specified geometry, see realization_extensions
+    :param n_cut: maximum number of fluctuations to render; amplitudes of individual fluctuations get suppressed by
+    sqrt(n_cut / n_total) if n_total > n_cut, where n_total is the number of expected fluctuations given the de-Broglie
+    wavelength and the area in which the fluctuations area rendered
+    :param r_ein: The characteristic angular used to convert fluctuations in convergence to fluctuations in mass
+    :return: a realization of halos and fluctuations modeled as Gaussians in ULDM
     """
+
     # constants
     m22 = 10**(log10_m_uldm + 22)
     log_m0 = np.log10(1.6e10 * m22**(-4/3))
 
     # FIRST WE CREATE AN INSTANCE OF PYHALO, WHICH SETS THE COSMOLOGY
     pyhalo = pyHalo(z_lens, z_source, kwargs_cosmo)
 
     #compute M_min as described in documentation
     log_m_min = MinHaloMassULDM(log10_m_uldm, pyhalo.astropy_cosmo, log_mlow)
-
+    kwargs_density_profile = {}
     kwargs_density_profile['log10_m_uldm'] = log10_m_uldm
-    kwargs_density_profile['scale_nfw'] = scale_nfw
+    kwargs_density_profile['scale_nfw'] = False
     kwargs_density_profile['uldm_plaw'] = uldm_plaw
     kwargs_wdm = {'z_lens': z_lens, 'z_source': z_source, 'log_mc': log_m0, 'sigma_sub': sigma_sub,
                   'log_mlow': log_m_min, 'log_mhigh': log_mhigh,
                   'mass_function_model_subhalos': mass_function_model_subhalos,
                   'kwargs_mass_function_subhalos': kwargs_mass_function_subhalos,
                   'mass_function_model_fieldhalos': mass_function_model_fieldhalos,
                   'kwargs_mass_function_fieldhalos': kwargs_mass_function_fieldhalos,
@@ -487,66 +516,83 @@
         uldm_realization = ext.add_ULDM_fluctuations(de_Broglie_wavelength=lambda_dB,
                                 fluctuation_amplitude=fluctuation_amplitude,
                                 fluctuation_size=lambda_dB * fluctuation_size_scale,
                                 fluctuation_size_variance=lambda_dB * fluctuation_size_scale * fluctuation_size_dispersion,
                                 n_fluc_scale=n_fluc_scale,
                                 shape=flucs_shape,
                                 args=flucs_args,
-                                n_cut=n_cut, rescale_fluc_amp=rescale_fluc_amp)
+                                n_cut=n_cut)
         return uldm_realization
     else:
         return uldm_no_fluctuations
 
 def SIDM_core_collapse(z_lens, z_source, mass_ranges_subhalos, mass_ranges_field_halos,
         probabilities_subhalos, probabilities_field_halos, kwargs_sub_function=None,
         kwargs_field_function=None, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
         concentration_model_subhalos='DIEMERJOYCE19', kwargs_concentration_model_subhalos={},
         concentration_model_fieldhalos='DIEMERJOYCE19', kwargs_concentration_model_fieldhalos={},
         truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_trunction_model_subhalos={},
         truncation_model_fieldhalos='TRUNCATION_RN', kwargs_truncation_model_fieldhalos={},
         shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3,  r_tidal=0.25,
-        LOS_normalization=1.0, two_halo_contribution=True, delta_power_law_index=0.0,
-        geometry_type='DOUBLE_CONE', kwargs_cosmo=None, collapsed_halo_profile='SPL_CORE',
+        LOS_normalization=1.0, geometry_type='DOUBLE_CONE', kwargs_cosmo=None, collapsed_halo_profile='SPL_CORE',
         kwargs_collapsed_profile={'x_core_halo': 0.05, 'x_match': 3.0, 'log_slope_halo': 3.0}):
 
     """
+    Generates realizations of SIDM given the fraction of core-collapsed halos as a function of halo mass
 
-    :param z_lens:
-    :param z_source:
-    :param mass_ranges_subhalos:
-    :param mass_ranges_field_halos:
-    :param probabilities_subhalos:
-    :param probabilities_field_halos:
-    :param kwargs_sub_function:
-    :param kwargs_field_function:
-    :param sigma_sub:
-    :param log_mlow:
-    :param log_mhigh:
-    :param concentration_model_subhalos:
-    :param kwargs_concentration_model_subhalos:
-    :param concentration_model_fieldhalos:
-    :param kwargs_concentration_model_fieldhalos:
-    :param truncation_model_subhalos:
-    :param kwargs_trunction_model_subhalos:
-    :param truncation_model_fieldhalos:
-    :param kwargs_truncation_model_fieldhalos:
-    :param shmf_log_slope:
-    :param cone_opening_angle_arcsec:
-    :param log_m_host:
-    :param r_tidal:
-    :param LOS_normalization:
-    :param two_halo_contribution:
-    :param delta_power_law_index:
-    :param geometry_type:
-    :param kwargs_cosmo:
-    :param collapsed_halo_profile:
-    :param kwargs_collapsed_profile:
-    :return:
+    :param z_lens: main deflector redshift
+    :param z_source: source redshift
+    :param mass_ranges_subhalos: a list of mass ranges for subhalo collapse, e.g.
+    mass_ranges_subhalos = [[6, 8], [8, 9], ...]
+    :param mass_ranges_field_halos: a list of mass ranges for subhalo collapse, e.g.
+    mass_ranges_field_halos = [[6, 8], [8, 9], ...]
+    :param probabilities_subhalos: a list of functions, or a list of the fraction of collapsed subhalos in each mass bin
+    :param probabilities_field_halos: a list of functions, or a list of the fraction of collapsed field halos in each
+    mass bin
+    :param kwargs_sub_function: if probabilities_subhalos is a list of functions, specifies keyword arguments
+    for each function
+    :param kwargs_field_function: if probabilities_field_halos is a list of functions, specifies keyword arguments
+    for each function
+    :param sigma_sub: amplitude of the subhalo mass function at 10^8 solar masses in units [# of halos / kpc^2]
+    :param log_mlow: log base 10 of the minimum halo mass to render
+    :param log_mhigh: log base 10 of the maximum halo mass to render
+    :param mass_function_model_subhalos: mass function model for subhalos, see mass_function_models.py for a list
+    :param kwargs_mass_function_subhalos: keyword arguments for the mass function model
+    :param mass_function_model_fieldhalos: mass function model for field halos, see mass_function_models.py for a list
+    :param kwargs_mass_function_fieldhalos: keyword arguments for the mass function model
+    :param concentration_model_subhalos: the concentration-mass relation applied to subhalos,
+    see concentration_models.py for a complete list of available models
+    :param kwargs_concentration_model_subhalos: keyword arguments for the subhalo MC relation
+    NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
+    :param concentration_model_subhalos: the concentration-mass relation applied to field halos,
+    see concentration_models.py for a complete list of available models
+    :param kwargs_concentration_model_fieldhalos: keyword arguments for the field halo MC relation
+    NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
+    :param truncation_model_subhalos: the truncation model applied to subhalos, see truncation_models for a complete list
+    :param kwargs_trunction_model_subhalos: keyword arguments for the truncation model applied to subhalos
+    :param truncation_model_fieldhalos: the truncation model applied to field halos, see truncation_models for a
+    complete list
+    :param kwargs_truncation_model_fieldhalos: keyword arguments for the truncation model applied to field halos
+    :param shmf_log_slope: the logarithmic slope of the subhalo mass function pivoting around 10^8 M_sun
+    :param cone_opening_angle_arcsec: the opening angle of the rendering volume in arcsec
+    :param log_m_host: log base 10 of the host halo mass [M_sun]
+    :param r_tidal: the core radius of the host halo in units of the host halo scale radius. Subhalos are distributed
+    in 3D with a cored NFW profile with this core radius
+    :param LOS_normalization: rescales the amplitude of the line-of-sight mass function
+    :param geometry_type: string that specifies the geometry of the rendering volume; options include
+    DOUBLE_CONE, CONE, CYLINDER
+    :param kwargs_cosmo: keyword arguments that specify the cosmology, see Cosmology/cosmology.py
+    :param collapsed_halo_profile: string that sets the density profile of core-collapsed halos
+    currently implemented models are SPL_CORE and GNFW (see example notebook)
+    :param kwargs_collapsed_profile: keyword arguments for the collapsed profile (see example notebook)
+    :return: a realization of dark matter structure in SIDM
     """
 
+    two_halo_contribution = True
+    delta_power_law_index = 0.0
     cdm = CDM(z_lens, z_source, sigma_sub, log_mlow, log_mhigh,
         concentration_model_subhalos, kwargs_concentration_model_subhalos,
         concentration_model_fieldhalos, kwargs_concentration_model_fieldhalos,
         truncation_model_subhalos, kwargs_trunction_model_subhalos,
         truncation_model_fieldhalos, kwargs_truncation_model_fieldhalos,
         shmf_log_slope, cone_opening_angle_arcsec, log_m_host,  r_tidal,
         LOS_normalization, two_halo_contribution, delta_power_law_index,
```

### Comparing `pyhalo-0.2.0/pyHalo/pyhalo.py` & `pyhalo-0.2.1/pyHalo/pyhalo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/pyHalo/realization_extensions.py` & `pyhalo-0.2.1/pyHalo/realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/pyHalo/single_realization.py` & `pyhalo-0.2.1/pyHalo/single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/pyHalo/truncation_models.py` & `pyhalo-0.2.1/pyHalo/truncation_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/pyHalo/utilities.py` & `pyhalo-0.2.1/pyHalo/utilities.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/pyHalo.egg-info/PKG-INFO` & `pyhalo-0.2.1/pyHalo.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.0/pyHalo.egg-info/SOURCES.txt` & `pyhalo-0.2.1/pyHalo.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
@@ -30,14 +29,50 @@
 pyHalo.egg-info/PKG-INFO
 pyHalo.egg-info/SOURCES.txt
 pyHalo.egg-info/dependency_links.txt
 pyHalo.egg-info/entry_points.txt
 pyHalo.egg-info/not-zip-safe
 pyHalo.egg-info/requires.txt
 pyHalo.egg-info/top_level.txt
+pyHalo/Cosmology/__init__.py
+pyHalo/Cosmology/cosmology.py
+pyHalo/Cosmology/geometry.py
+pyHalo/Halos/__init__.py
+pyHalo/Halos/concentration.py
+pyHalo/Halos/halo_base.py
+pyHalo/Halos/lens_cosmo.py
+pyHalo/Halos/tidal_truncation.py
+pyHalo/Halos/util.py
+pyHalo/Halos/HaloModels/NFW.py
+pyHalo/Halos/HaloModels/PTMass.py
+pyHalo/Halos/HaloModels/PsuedoJaffe.py
+pyHalo/Halos/HaloModels/TNFW.py
+pyHalo/Halos/HaloModels/TNFWemulator.py
+pyHalo/Halos/HaloModels/ULDM.py
+pyHalo/Halos/HaloModels/__init__.py
+pyHalo/Halos/HaloModels/gaussian.py
+pyHalo/Halos/HaloModels/generalized_nfw.py
+pyHalo/Halos/HaloModels/powerlaw.py
+pyHalo/Rendering/__init__.py
+pyHalo/Rendering/correlated_structure.py
+pyHalo/Rendering/halo_population.py
+pyHalo/Rendering/line_of_sight.py
+pyHalo/Rendering/rendering_class_base.py
+pyHalo/Rendering/subhalos.py
+pyHalo/Rendering/two_halo.py
+pyHalo/Rendering/MassFunctions/__init__.py
+pyHalo/Rendering/MassFunctions/delta_function.py
+pyHalo/Rendering/MassFunctions/density_peaks.py
+pyHalo/Rendering/MassFunctions/mass_function_base.py
+pyHalo/Rendering/MassFunctions/util.py
+pyHalo/Rendering/SpatialDistributions/__init__.py
+pyHalo/Rendering/SpatialDistributions/base.py
+pyHalo/Rendering/SpatialDistributions/correlated.py
+pyHalo/Rendering/SpatialDistributions/nfw.py
+pyHalo/Rendering/SpatialDistributions/uniform.py
 pyhalo/__init__.py
 pyhalo/defaults.py
 pyhalo/pyhalo.py
 pyhalo/single_realization.py
 pyhalo.egg-info/PKG-INFO
 pyhalo.egg-info/SOURCES.txt
 pyhalo.egg-info/dependency_links.txt
@@ -62,14 +97,15 @@
 tests/test_halos/test_concentrations.py
 tests/test_halos/test_gaussian.py
 tests/test_halos/test_general_nfw.py
 tests/test_halos/test_lenscosmo.py
 tests/test_halos/test_nfw_halo.py
 tests/test_halos/test_pjaffe.py
 tests/test_halos/test_point_mass.py
+tests/test_halos/test_powerlaw_profile.py
 tests/test_halos/test_tnfw_halo.py
 tests/test_halos/test_truncation.py
 tests/test_halos/test_uldm.py
 tests/test_halos/test_util.py
 tests/test_rendering/__init__.py
 tests/test_rendering/test_2halo.py
 tests/test_rendering/test_los.py
```

### Comparing `pyhalo-0.2.0/pyproject.toml` & `pyhalo-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhalo"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Daniel Gilman", email="daniel.gilman@utoronto.ca" },
 ]
 description = "A python package for generating populations of dark matter halos"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyhalo-0.2.0/setup.py` & `pyhalo-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,41 +15,42 @@
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
 
 setup(
     author="Daniel Gilman",
-    author_email='gilmanda@ucla.edu',
+    version='0.2.1',
+    author_email='daniel.gilman@utoronto.ca',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
+        'Development Status :: 5 - Stable',
+        'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
-        "Programming Language :: Python :: 2",
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     description="A tool for rendering full mass distributions for gravitational lensing simulations",
     entry_points={
         'console_scripts': [
             'pyHalo=pyHalo.cli:main',
         ],
     },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='pyHalo',
     name='pyhalo',
-    packages=find_packages(include=['pyHalo']),
+    packages=find_packages(),
+    package_dir={'lenstronomy': 'lenstronomy'},
+    #packages=find_packages(include=['pyHalo']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/dangilman/pyHalo',
-    version='0.2.0',
     zip_safe=False,
 )
```

### Comparing `pyhalo-0.2.0/tests/test_concentration_models.py` & `pyhalo-0.2.1/tests/test_concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_cosmology/test_cone_geometry.py` & `pyhalo-0.2.1/tests/test_cosmology/test_cone_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_cosmology/test_cosmo.py` & `pyhalo-0.2.1/tests/test_cosmology/test_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_cosmology/test_cylinder_geometry.py` & `pyhalo-0.2.1/tests/test_cosmology/test_cylinder_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_halos/test_adiabatic_tides.py` & `pyhalo-0.2.1/tests/test_halos/test_adiabatic_tides.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 class TestAdiabaticTides(object):
 
     def setup_method(self):
         self.lens_cosmo_instance = LensCosmo(0.5, 1.5)
         log10_galaxy_rs, log10_galaxy_m, host_dynamical_time = np.log10(0.5), np.log10(0.25), 1.0
         self.att = AdiabaticTidesTruncation(self.lens_cosmo_instance,
-                                            13.3, 0.5, log10_galaxy_rs, log10_galaxy_m, mass_loss_interp=DummyInterp())
+                                            13.3, 0.5, log10_galaxy_rs, log10_galaxy_m,
+                                            mass_loss_interp=DummyInterp())
 
 
     def test_rt(self):
 
         mass = 10 ** 8.0
         x = 0.1
         y = 0.5
```

### Comparing `pyhalo-0.2.0/tests/test_halos/test_concentrations.py` & `pyhalo-0.2.1/tests/test_halos/test_concentrations.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_halos/test_gaussian.py` & `pyhalo-0.2.1/tests/test_halos/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_halos/test_general_nfw.py` & `pyhalo-0.2.1/tests/test_halos/test_general_nfw.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,46 +58,71 @@
         y = 1.0
         r3d = 100
         is_subhalo = False
         gamma_inner = 2.2
         gamma_outer = 3.2
         x_match = 3.5
         unique_tag = 1.0
-        kwargs_profile = {'gamma_inner': gamma_inner, 'gamma_outer': gamma_outer, 'x_match': x_match}
+        kwargs_profile = {'gamma_inner': gamma_inner, 'gamma_outer': gamma_outer, 'x_match': x_match,
+                          'evaluate_mc_at_zlens': True}
         gnfw = GeneralNFWFieldHalo(m, x, y, r3d, self.zhalo, is_subhalo, self.lens_cosmo, kwargs_profile,
                                    self.truncation_class, self.concentration_class, unique_tag)
         nfw = NFWFieldHalo(m, x, y, r3d, self.zhalo, is_subhalo, self.lens_cosmo, kwargs_profile,
                                    self.truncation_class, self.concentration_class, unique_tag)
 
         kwargs_gnfw = gnfw.lenstronomy_params[0][0]
         kwargs_nfw = nfw.lenstronomy_params[0][0]
         rmatch = x_match * kwargs_nfw['Rs']
         m3d_nfw = self.nfw_profile_lenstronomy.mass_3d_lens(rmatch, kwargs_nfw['Rs'],
                                                             kwargs_nfw['alpha_Rs'])
         m3d = self.gnfw_profile_lenstronomy.mass_3d_lens(rmatch, kwargs_gnfw['Rs'],
                                                          kwargs_gnfw['alpha_Rs'],
                                                          kwargs_gnfw['gamma_inner'], kwargs_gnfw['gamma_outer'])
-        npt.assert_almost_equal(m3d_nfw/m3d, 1.0, 2)
+        npt.assert_almost_equal(m3d_nfw/m3d, 1.0, 4)
+
+        m = 10 ** 7.3
+        x = 0.5
+        y = 1.0
+        r3d = 100
+        is_subhalo = False
+        gamma_inner = 1.5
+        gamma_outer = 2.89
+        x_match = 4.0
+        unique_tag = 1.0
+        kwargs_profile = {'gamma_inner': gamma_inner, 'gamma_outer': gamma_outer, 'x_match': x_match}
+        gnfw = GeneralNFWFieldHalo(m, x, y, r3d, self.zhalo, is_subhalo, self.lens_cosmo, kwargs_profile,
+                                   self.truncation_class, self.concentration_class, unique_tag)
+        nfw = NFWFieldHalo(m, x, y, r3d, self.zhalo, is_subhalo, self.lens_cosmo, kwargs_profile,
+                           self.truncation_class, self.concentration_class, unique_tag)
+
+        kwargs_gnfw = gnfw.lenstronomy_params[0][0]
+        kwargs_nfw = nfw.lenstronomy_params[0][0]
+        rmatch = x_match * kwargs_nfw['Rs']
+        m3d_nfw = self.nfw_profile_lenstronomy.mass_3d_lens(rmatch, kwargs_nfw['Rs'],
+                                                            kwargs_nfw['alpha_Rs'])
+        m3d = self.gnfw_profile_lenstronomy.mass_3d_lens(rmatch, kwargs_gnfw['Rs'],
+                                                         kwargs_gnfw['alpha_Rs'],
+                                                         kwargs_gnfw['gamma_inner'], kwargs_gnfw['gamma_outer'])
+        npt.assert_almost_equal(m3d_nfw / m3d, 1.0, 4)
 
     def test_concentration_redshift_eval(self):
         m = 10 ** 8
         x = 0.5
         y = 1.0
         r3d = 100
         is_subhalo = False
         gamma_inner = 1.25
         gamma_outer = 3.3
         x_match = 2.5
         unique_tag = 1.0
         kwargs_profile = {'gamma_inner': gamma_inner, 'gamma_outer': gamma_outer, 'x_match': x_match,
-                          'evaluate_mc_at_zlens': False, 'c_scatter': False, 'c_scatter_dex': 0.2}
+                          'evaluate_mc_at_zlens': False,}
         gnfw = GeneralNFWFieldHalo(m, x, y, r3d, self.zhalo, is_subhalo, self.lens_cosmo, kwargs_profile,
                                    self.truncation_class, self.concentration_class, unique_tag)
         gnfw_subhalo = GeneralNFWSubhalo(m, x, y, r3d, self.zhalo, is_subhalo, self.lens_cosmo, kwargs_profile,
                                    self.truncation_class, self.concentration_class, unique_tag)
         c = gnfw.profile_args[0]
         c_sub = gnfw_subhalo.profile_args[0]
         npt.assert_equal(False, c==c_sub)
 
-
 if __name__ == '__main__':
     pytest.main()
```

### Comparing `pyhalo-0.2.0/tests/test_halos/test_lenscosmo.py` & `pyhalo-0.2.1/tests/test_halos/test_lenscosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_halos/test_nfw_halo.py` & `pyhalo-0.2.1/tests/test_halos/test_nfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_halos/test_pjaffe.py` & `pyhalo-0.2.1/tests/test_halos/test_pjaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_halos/test_point_mass.py` & `pyhalo-0.2.1/tests/test_halos/test_point_mass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_halos/test_tnfw_halo.py` & `pyhalo-0.2.1/tests/test_halos/test_tnfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_halos/test_truncation.py` & `pyhalo-0.2.1/tests/test_halos/test_truncation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import pytest
 from pyHalo.Halos.lens_cosmo import LensCosmo
 from pyHalo.Cosmology.cosmology import Cosmology
 import numpy.testing as npt
 from pyHalo.Halos.tidal_truncation import TruncationRN, TruncationRoche, TruncationSplashBack
 from pyHalo.truncation_models import truncation_models
 from astropy.cosmology import FlatLambdaCDM
+import os
+
 
 class TestTruncation(object):
 
     def setup_method(self):
 
         astropy = FlatLambdaCDM(70.0, 0.3)
         cosmo = Cosmology(astropy)
         self.lenscosmo = LensCosmo(0.5, 1.5, cosmo)
 
     def test_load_models(self):
 
         model_name_list = ['TRUNCATION_R50', 'TRUNCATION_RN', 'TRUNCATION_ROCHE', 'TRUNCATION_ROCHE_GILMAN2020',
-                           'ADIABATIC_TIDES', 'SPLASHBACK']
+                           'SPLASHBACK']
         kwargs_model_list = [{}, {'LOS_truncation_factor': 50.}, {'RocheNorm': 1.0, 'm_power': 1./3, 'RocheNu': 2.0/3.0}, {},
-                             {'log_m_host': 13.0, 'z_host': 0.5}, {}]
+                             {}]
         for model,kwargs in zip(model_name_list, kwargs_model_list):
             mod, kw = truncation_models(model)
             kwargs.update(kw)
             kwargs['lens_cosmo'] = self.lenscosmo
             _ = mod(**kwargs)
 
     def test_truncation_RN(self):
```

### Comparing `pyhalo-0.2.0/tests/test_halos/test_uldm.py` & `pyhalo-0.2.1/tests/test_halos/test_uldm.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_halos/test_util.py` & `pyhalo-0.2.1/tests/test_halos/test_util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_mass_function_models.py` & `pyhalo-0.2.1/tests/test_mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_preset_models.py` & `pyhalo-0.2.1/tests/test_preset_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_pyhalo_base.py` & `pyhalo-0.2.1/tests/test_pyhalo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_realization_extensions.py` & `pyhalo-0.2.1/tests/test_realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_rendering/test_2halo.py` & `pyhalo-0.2.1/tests/test_rendering/test_2halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_rendering/test_los.py` & `pyhalo-0.2.1/tests/test_rendering/test_los.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_base_functions.py` & `pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_base_functions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_delta_function.py` & `pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_sheth_tormen.py` & `pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_sheth_tormen.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_rendering/test_population.py` & `pyhalo-0.2.1/tests/test_rendering/test_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_correlated.py` & `pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_nfw.py` & `pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_uniform.py` & `pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_rendering/test_subhalos.py` & `pyhalo-0.2.1/tests/test_rendering/test_subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_single_realization.py` & `pyhalo-0.2.1/tests/test_single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.0/tests/test_utilities.py` & `pyhalo-0.2.1/tests/test_utilities.py`

 * *Files identical despite different names*

