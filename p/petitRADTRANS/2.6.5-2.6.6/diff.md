# Comparing `tmp/petitRADTRANS-2.6.5.tar.gz` & `tmp/petitRADTRANS-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petitRADTRANS-2.6.5.tar", last modified: Wed May 24 09:16:41 2023, max compression
+gzip compressed data, was "petitRADTRANS-2.6.6.tar", last modified: Wed May 24 09:30:25 2023, max compression
```

## Comparing `petitRADTRANS-2.6.5.tar` & `petitRADTRANS-2.6.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.059461 petitRADTRANS-2.6.5/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1062 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/LICENSE
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1171 2023-05-24 09:16:41.059573 petitRADTRANS-2.6.5/PKG-INFO
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)      901 2023-05-24 09:13:47.000000 petitRADTRANS-2.6.5/README.rst
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.032605 petitRADTRANS-2.6.5/petitRADTRANS/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1960 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/__file_conversion.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)      420 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    17117 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/_read_opacities.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.036401 petitRADTRANS-2.6.5/petitRADTRANS/ccf/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/ccf/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    31295 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/ccf/ccf.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3945 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/ccf/ccf_core.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.037678 petitRADTRANS-2.6.5/petitRADTRANS/cli/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/cli/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     8878 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/cli/eso_etc_cli.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    16595 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/cli/eso_skycalc_cli.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.038645 petitRADTRANS-2.6.5/petitRADTRANS/config/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       29 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/config/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2408 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/config/configuration.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.040444 petitRADTRANS-2.6.5/petitRADTRANS/containers/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/containers/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    56238 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/containers/planet.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)   125896 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/containers/spectral_model.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    32228 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/fort_input.f90
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3936 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/fort_rebin.f90
--rwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)   124384 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/fort_spec.f90
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     9998 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/nat_cst.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    15593 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/physics.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.041580 petitRADTRANS-2.6.5/petitRADTRANS/poor_mans_nonequ_chem/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       55 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/poor_mans_nonequ_chem/__init__.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.042246 petitRADTRANS-2.6.5/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       56 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     4272 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/chem_fortran_util.f90
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.042805 petitRADTRANS-2.6.5/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       63 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     4326 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/poor_mans_nonequ_chem.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     6934 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/pyth_input.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)   106780 2023-05-24 09:05:05.000000 petitRADTRANS-2.6.5/petitRADTRANS/radtrans.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.050274 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/
--rwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)      362 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     6826 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/chemistry.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    24928 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/cloud_cond.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    24346 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/data.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    39312 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/models.py
--rwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2516 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/parameter.py
--rwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1661 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/plot_style.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    30315 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/plotting.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    21787 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/preparing.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3126 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/rebin_give_width.f90
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)   101888 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/retrieval.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    29261 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/retrieval_config.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    11997 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/retrieval/util.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    13417 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/petitRADTRANS/utils.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       18 2023-05-24 08:38:56.000000 petitRADTRANS-2.6.5/petitRADTRANS/version.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.035218 petitRADTRANS-2.6.5/petitRADTRANS.egg-info/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1171 2023-05-24 09:16:41.000000 petitRADTRANS-2.6.5/petitRADTRANS.egg-info/PKG-INFO
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2390 2023-05-24 09:16:41.000000 petitRADTRANS-2.6.5/petitRADTRANS.egg-info/SOURCES.txt
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        1 2023-05-24 09:16:41.000000 petitRADTRANS-2.6.5/petitRADTRANS.egg-info/dependency_links.txt
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        1 2023-05-24 09:16:41.000000 petitRADTRANS-2.6.5/petitRADTRANS.egg-info/not-zip-safe
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       84 2023-05-24 09:16:41.000000 petitRADTRANS-2.6.5/petitRADTRANS.egg-info/requires.txt
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       20 2023-05-24 09:16:41.000000 petitRADTRANS-2.6.5/petitRADTRANS.egg-info/top_level.txt
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)      184 2023-05-24 09:16:41.059979 petitRADTRANS-2.6.5/setup.cfg
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3055 2023-05-24 09:13:47.000000 petitRADTRANS-2.6.5/setup.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-24 09:16:41.059180 petitRADTRANS-2.6.5/tests/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3008 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/_test_CO_line_lists.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3070 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/_test_H2O_line_lists.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3263 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/_test_TiO_line_lists.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2628 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/_test_data.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1698 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/_test_high_res.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3567 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/_test_line_shapes_alkalis.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1190 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/context.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    42081 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/reference_files_generators.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3695 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/test_chemistry.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)      536 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/test_fortran_modules.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1449 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/test_planet.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    14456 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/test_radtrans_correlated_k.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     9466 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/test_radtrans_correlated_k_scattering.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3139 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/test_radtrans_correlated_k_surface_scattering.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    15440 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/test_radtrans_line_by_line.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2967 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/test_radtrans_line_by_line_sampling.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    11355 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/test_retrieval.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2660 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/test_utility_functions.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    14324 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.5/tests/utils.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.842266 petitRADTRANS-2.6.6/
+-rw-r--r--   0 molliere (1984917825) 1357073302     1062 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/LICENSE
+-rw-r--r--   0 molliere (1984917825) 1357073302     1171 2023-05-24 09:30:25.842386 petitRADTRANS-2.6.6/PKG-INFO
+-rw-r--r--   0 molliere (1984917825) 1357073302      901 2023-05-24 09:29:38.000000 petitRADTRANS-2.6.6/README.rst
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.819787 petitRADTRANS-2.6.6/petitRADTRANS/
+-rw-r--r--   0 molliere (1984917825) 1357073302     1960 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/__file_conversion.py
+-rw-r--r--   0 molliere (1984917825) 1357073302      420 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    17117 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/_read_opacities.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.822239 petitRADTRANS-2.6.6/petitRADTRANS/ccf/
+-rw-r--r--   0 molliere (1984917825) 1357073302        0 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/ccf/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    31295 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/ccf/ccf.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3945 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/ccf/ccf_core.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.823007 petitRADTRANS-2.6.6/petitRADTRANS/cli/
+-rw-r--r--   0 molliere (1984917825) 1357073302        0 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/cli/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     8878 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/cli/eso_etc_cli.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    16595 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/cli/eso_skycalc_cli.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.823718 petitRADTRANS-2.6.6/petitRADTRANS/config/
+-rw-r--r--   0 molliere (1984917825) 1357073302       29 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/config/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     2408 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/config/configuration.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.824732 petitRADTRANS-2.6.6/petitRADTRANS/containers/
+-rw-r--r--   0 molliere (1984917825) 1357073302        0 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/containers/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    56238 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/containers/planet.py
+-rw-r--r--   0 molliere (1984917825) 1357073302   125896 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/containers/spectral_model.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    32228 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/fort_input.f90
+-rw-r--r--   0 molliere (1984917825) 1357073302     3936 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/fort_rebin.f90
+-rwxr-xr-x   0 molliere (1984917825) 1357073302   124384 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/fort_spec.f90
+-rw-r--r--   0 molliere (1984917825) 1357073302     9998 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/nat_cst.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    15599 2023-05-24 09:23:44.000000 petitRADTRANS-2.6.6/petitRADTRANS/physics.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.825781 petitRADTRANS-2.6.6/petitRADTRANS/poor_mans_nonequ_chem/
+-rw-r--r--   0 molliere (1984917825) 1357073302       55 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/poor_mans_nonequ_chem/__init__.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.826501 petitRADTRANS-2.6.6/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/
+-rw-r--r--   0 molliere (1984917825) 1357073302       56 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     4272 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/chem_fortran_util.f90
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.827123 petitRADTRANS-2.6.6/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/
+-rw-r--r--   0 molliere (1984917825) 1357073302       63 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     4326 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/poor_mans_nonequ_chem.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     6934 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/pyth_input.py
+-rw-r--r--   0 molliere (1984917825) 1357073302   106780 2023-05-24 09:05:05.000000 petitRADTRANS-2.6.6/petitRADTRANS/radtrans.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.834259 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/
+-rwxr-xr-x   0 molliere (1984917825) 1357073302      362 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     6826 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/chemistry.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    24928 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/cloud_cond.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    24346 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/data.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    39312 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/models.py
+-rwxr-xr-x   0 molliere (1984917825) 1357073302     2516 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/parameter.py
+-rwxr-xr-x   0 molliere (1984917825) 1357073302     1661 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/plot_style.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    30315 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/plotting.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    21787 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/preparing.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3126 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/rebin_give_width.f90
+-rw-r--r--   0 molliere (1984917825) 1357073302   101888 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/retrieval.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    29261 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/retrieval_config.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    11997 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/retrieval/util.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    13417 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/petitRADTRANS/utils.py
+-rw-r--r--   0 molliere (1984917825) 1357073302       18 2023-05-24 09:27:15.000000 petitRADTRANS-2.6.6/petitRADTRANS/version.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.821424 petitRADTRANS-2.6.6/petitRADTRANS.egg-info/
+-rw-r--r--   0 molliere (1984917825) 1357073302     1171 2023-05-24 09:30:25.000000 petitRADTRANS-2.6.6/petitRADTRANS.egg-info/PKG-INFO
+-rw-r--r--   0 molliere (1984917825) 1357073302     2390 2023-05-24 09:30:25.000000 petitRADTRANS-2.6.6/petitRADTRANS.egg-info/SOURCES.txt
+-rw-r--r--   0 molliere (1984917825) 1357073302        1 2023-05-24 09:30:25.000000 petitRADTRANS-2.6.6/petitRADTRANS.egg-info/dependency_links.txt
+-rw-r--r--   0 molliere (1984917825) 1357073302        1 2023-05-24 09:30:25.000000 petitRADTRANS-2.6.6/petitRADTRANS.egg-info/not-zip-safe
+-rw-r--r--   0 molliere (1984917825) 1357073302       84 2023-05-24 09:30:25.000000 petitRADTRANS-2.6.6/petitRADTRANS.egg-info/requires.txt
+-rw-r--r--   0 molliere (1984917825) 1357073302       20 2023-05-24 09:30:25.000000 petitRADTRANS-2.6.6/petitRADTRANS.egg-info/top_level.txt
+-rw-r--r--   0 molliere (1984917825) 1357073302      184 2023-05-24 09:30:25.842796 petitRADTRANS-2.6.6/setup.cfg
+-rw-r--r--   0 molliere (1984917825) 1357073302     3055 2023-05-24 09:29:47.000000 petitRADTRANS-2.6.6/setup.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2023-05-24 09:30:25.841979 petitRADTRANS-2.6.6/tests/
+-rw-r--r--   0 molliere (1984917825) 1357073302        0 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3008 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/_test_CO_line_lists.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3070 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/_test_H2O_line_lists.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3263 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/_test_TiO_line_lists.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     2628 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/_test_data.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     1698 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/_test_high_res.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3567 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/_test_line_shapes_alkalis.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     1190 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/context.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    42081 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/reference_files_generators.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3695 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/test_chemistry.py
+-rw-r--r--   0 molliere (1984917825) 1357073302      536 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/test_fortran_modules.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     1449 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/test_planet.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    14456 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/test_radtrans_correlated_k.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     9466 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/test_radtrans_correlated_k_scattering.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3139 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/test_radtrans_correlated_k_surface_scattering.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    15440 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/test_radtrans_line_by_line.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     2967 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/test_radtrans_line_by_line_sampling.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    11355 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/test_retrieval.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     2660 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/test_utility_functions.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    14324 2023-05-23 14:33:01.000000 petitRADTRANS-2.6.6/tests/utils.py
```

### Comparing `petitRADTRANS-2.6.5/LICENSE` & `petitRADTRANS-2.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/PKG-INFO` & `petitRADTRANS-2.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petitRADTRANS
-Version: 2.6.5
+Version: 2.6.6
 Summary: Exoplanet spectral synthesis tool for retrievals
 Home-page: https://gitlab.com/mauricemolli/petitRADTRANS
 Author: Paul Mollière
 Author-email: molliere@mpia.de
 License: MIT License
 License-File: LICENSE
```

### Comparing `petitRADTRANS-2.6.5/README.rst` & `petitRADTRANS-2.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/__file_conversion.py` & `petitRADTRANS-2.6.6/petitRADTRANS/__file_conversion.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/_read_opacities.py` & `petitRADTRANS-2.6.6/petitRADTRANS/_read_opacities.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/ccf/ccf.py` & `petitRADTRANS-2.6.6/petitRADTRANS/ccf/ccf.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/ccf/ccf_core.py` & `petitRADTRANS-2.6.6/petitRADTRANS/ccf/ccf_core.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/cli/eso_etc_cli.py` & `petitRADTRANS-2.6.6/petitRADTRANS/cli/eso_etc_cli.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/cli/eso_skycalc_cli.py` & `petitRADTRANS-2.6.6/petitRADTRANS/cli/eso_skycalc_cli.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/config/configuration.py` & `petitRADTRANS-2.6.6/petitRADTRANS/config/configuration.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/containers/planet.py` & `petitRADTRANS-2.6.6/petitRADTRANS/containers/planet.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/containers/spectral_model.py` & `petitRADTRANS-2.6.6/petitRADTRANS/containers/spectral_model.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/fort_input.f90` & `petitRADTRANS-2.6.6/petitRADTRANS/fort_input.f90`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/fort_rebin.f90` & `petitRADTRANS-2.6.6/petitRADTRANS/fort_rebin.f90`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/fort_spec.f90` & `petitRADTRANS-2.6.6/petitRADTRANS/fort_spec.f90`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/nat_cst.py` & `petitRADTRANS-2.6.6/petitRADTRANS/nat_cst.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/physics.py` & `petitRADTRANS-2.6.6/petitRADTRANS/physics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 os.environ["OMP_NUM_THREADS"] = "1"
 import numpy as np
 import copy as cp
 
 from scipy.interpolate import interp1d,CubicSpline
-from petitRADTRANS import poor_mans_nonequ_chem as pm
 
 import petitRADTRANS.nat_cst as nc
 
 
 def doppler_shift(wavelength_0, velocity):
     """Calculate the Doppler-shifted wavelength for electromagnetic waves.
 
@@ -191,14 +190,17 @@
             C/O for the nabla_ad interpolation
         FeH : float
             metallicity for the nabla_ad interpolation
     Returns:
         Tret : np.ndarray
             The temperature as a function of atmospheric pressure.
     """
+
+    from petitRADTRANS import poor_mans_nonequ_chem as pm
+
     # Go grom bar to cgs
     press_cgs = press * 1e6
 
     # Calculate the optical depth
     tau = delta * press_cgs ** alpha
 
     # This is the eddington temperature
```

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/chem_fortran_util.f90` & `petitRADTRANS-2.6.6/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/chem_fortran_util.f90`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/poor_mans_nonequ_chem.py` & `petitRADTRANS-2.6.6/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/poor_mans_nonequ_chem.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/pyth_input.py` & `petitRADTRANS-2.6.6/petitRADTRANS/pyth_input.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/radtrans.py` & `petitRADTRANS-2.6.6/petitRADTRANS/radtrans.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/chemistry.py` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/chemistry.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/cloud_cond.py` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/cloud_cond.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/data.py` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/data.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/models.py` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/models.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/parameter.py` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/parameter.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/plot_style.py` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/plot_style.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/plotting.py` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/plotting.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/preparing.py` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/preparing.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/rebin_give_width.f90` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/rebin_give_width.f90`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/retrieval.py` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/retrieval.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/retrieval_config.py` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/retrieval_config.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/retrieval/util.py` & `petitRADTRANS-2.6.6/petitRADTRANS/retrieval/util.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS/utils.py` & `petitRADTRANS-2.6.6/petitRADTRANS/utils.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS.egg-info/PKG-INFO` & `petitRADTRANS-2.6.6/petitRADTRANS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petitRADTRANS
-Version: 2.6.5
+Version: 2.6.6
 Summary: Exoplanet spectral synthesis tool for retrievals
 Home-page: https://gitlab.com/mauricemolli/petitRADTRANS
 Author: Paul Mollière
 Author-email: molliere@mpia.de
 License: MIT License
 License-File: LICENSE
```

### Comparing `petitRADTRANS-2.6.5/petitRADTRANS.egg-info/SOURCES.txt` & `petitRADTRANS-2.6.6/petitRADTRANS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/setup.py` & `petitRADTRANS-2.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 
 def setup_function():
     # from petitRADTRANS.version import version  # future, this cannot be done right now due to the imports in __init__
 
     setup(
         name='petitRADTRANS',
-        version='2.6.5',
+        version='2.6.6',
         description='Exoplanet spectral synthesis tool for retrievals',
         long_description=open(os.path.join(
           os.path.dirname(__file__), 'README.rst')).read(),
         # long_description_content_type='test/x-rst',
         url='https://gitlab.com/mauricemolli/petitRADTRANS',
         author='Paul Mollière',
         author_email='molliere@mpia.de',
```

### Comparing `petitRADTRANS-2.6.5/tests/_test_CO_line_lists.py` & `petitRADTRANS-2.6.6/tests/_test_CO_line_lists.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/_test_H2O_line_lists.py` & `petitRADTRANS-2.6.6/tests/_test_H2O_line_lists.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/_test_TiO_line_lists.py` & `petitRADTRANS-2.6.6/tests/_test_TiO_line_lists.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/_test_data.py` & `petitRADTRANS-2.6.6/tests/_test_data.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/_test_high_res.py` & `petitRADTRANS-2.6.6/tests/_test_high_res.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/_test_line_shapes_alkalis.py` & `petitRADTRANS-2.6.6/tests/_test_line_shapes_alkalis.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/context.py` & `petitRADTRANS-2.6.6/tests/context.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/reference_files_generators.py` & `petitRADTRANS-2.6.6/tests/reference_files_generators.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/test_chemistry.py` & `petitRADTRANS-2.6.6/tests/test_chemistry.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/test_fortran_modules.py` & `petitRADTRANS-2.6.6/tests/test_fortran_modules.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/test_planet.py` & `petitRADTRANS-2.6.6/tests/test_planet.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/test_radtrans_correlated_k.py` & `petitRADTRANS-2.6.6/tests/test_radtrans_correlated_k.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/test_radtrans_correlated_k_scattering.py` & `petitRADTRANS-2.6.6/tests/test_radtrans_correlated_k_scattering.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/test_radtrans_correlated_k_surface_scattering.py` & `petitRADTRANS-2.6.6/tests/test_radtrans_correlated_k_surface_scattering.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/test_radtrans_line_by_line.py` & `petitRADTRANS-2.6.6/tests/test_radtrans_line_by_line.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/test_radtrans_line_by_line_sampling.py` & `petitRADTRANS-2.6.6/tests/test_radtrans_line_by_line_sampling.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/test_retrieval.py` & `petitRADTRANS-2.6.6/tests/test_retrieval.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/test_utility_functions.py` & `petitRADTRANS-2.6.6/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.6.5/tests/utils.py` & `petitRADTRANS-2.6.6/tests/utils.py`

 * *Files identical despite different names*

