# Comparing `tmp/warrenapp-0.1.2.tar.gz` & `tmp/warrenapp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warrenapp-0.1.2.tar", last modified: Tue May 16 17:30:55 2023, max compression
+gzip compressed data, was "warrenapp-0.1.3.tar", last modified: Wed May 24 18:40:30 2023, max compression
```

## Comparing `warrenapp-0.1.2.tar` & `warrenapp-0.1.3.tar`

### file list

```diff
@@ -1,59 +1,64 @@
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.454624 warrenapp-0.1.2/
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1521 2023-05-04 20:41:15.000000 warrenapp-0.1.2/LICENSE
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     3615 2023-05-16 17:30:55.454624 warrenapp-0.1.2/PKG-INFO
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1405 2023-05-05 00:01:17.000000 warrenapp-0.1.2/README.md
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1351 2023-05-16 17:24:45.000000 warrenapp-0.1.2/pyproject.toml
--rw-rw-r--   0 sweav     (1001) sweav     (1001)       38 2023-05-16 17:30:55.454624 warrenapp-0.1.2/setup.cfg
--rw-r--r--   0 sweav     (1001) sweav     (1001)      245 2023-05-04 23:54:39.000000 warrenapp-0.1.2/setup.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.446624 warrenapp-0.1.2/src/
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.446624 warrenapp-0.1.2/src/warrenapp/
--rw-r--r--   0 sweav     (1001) sweav     (1001)       24 2023-05-04 20:41:15.000000 warrenapp-0.1.2/src/warrenapp/__init__.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      281 2023-05-04 23:54:00.000000 warrenapp-0.1.2/src/warrenapp/apps.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.446624 warrenapp-0.1.2/src/warrenapp/badelf_tools/
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     4776 2023-05-08 18:36:02.000000 warrenapp-0.1.2/src/warrenapp/badelf_tools/acf.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)    20158 2023-05-04 20:41:15.000000 warrenapp-0.1.2/src/warrenapp/badelf_tools/badelf_algorithm_functions.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)    14535 2023-05-10 15:37:41.000000 warrenapp-0.1.2/src/warrenapp/badelf_tools/utilities.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     5179 2023-05-08 18:36:04.000000 warrenapp-0.1.2/src/warrenapp/models.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.446624 warrenapp-0.1.2/src/warrenapp/workflows/
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1177 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/__init__.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.454624 warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/
--rw-r--r--   0 sweav     (1001) sweav     (1001)      187 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/__init__.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)      828 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/prepop_relaxation_static_hse.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)      816 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/prepop_relaxation_static_pbesol.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     1778 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/relaxation_static_base.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.454624 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/
--rw-r--r--   0 sweav     (1001) sweav     (1001)      752 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/__init__.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      807 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/badelf_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      622 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/badelf_pbesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      637 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/bader_badelf_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      650 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/bader_badelf_pbesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      651 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/bader_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      742 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/bader_pbesol.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)    15145 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/base.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      903 2023-05-04 23:50:58.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/elf_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      921 2023-05-16 17:22:25.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/elf_pbesol.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     3958 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/prebader_badelf_dft.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)    14056 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.454624 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/
--rw-r--r--   0 sweav     (1001) sweav     (1001)      296 2023-05-04 20:41:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/__init__.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      963 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      545 2023-05-04 23:52:02.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/hsesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     4621 2023-05-05 00:04:23.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      503 2023-05-04 23:52:02.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/pbe_metal.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      443 2023-05-04 23:52:02.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/pbesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      702 2023-05-04 23:52:02.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/scan.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.454624 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/
--rw-r--r--   0 sweav     (1001) sweav     (1001)      364 2023-05-08 17:14:12.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/__init__.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)      874 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/hse.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)      457 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/hsesol.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)      772 2023-05-10 15:37:41.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/pbe.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)      482 2023-05-10 15:37:41.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/pbe_metal.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)      575 2023-05-10 15:37:41.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/pbesol.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)      445 2023-05-10 15:37:41.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/scan.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     2136 2023-05-08 21:19:01.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/seeded_hse.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.446624 warrenapp-0.1.2/src/warrenapp.egg-info/
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     3615 2023-05-16 17:30:55.000000 warrenapp-0.1.2/src/warrenapp.egg-info/PKG-INFO
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     2127 2023-05-16 17:30:55.000000 warrenapp-0.1.2/src/warrenapp.egg-info/SOURCES.txt
--rw-rw-r--   0 sweav     (1001) sweav     (1001)        1 2023-05-16 17:30:55.000000 warrenapp-0.1.2/src/warrenapp.egg-info/dependency_links.txt
--rw-rw-r--   0 sweav     (1001) sweav     (1001)        8 2023-05-16 17:30:55.000000 warrenapp-0.1.2/src/warrenapp.egg-info/requires.txt
--rw-rw-r--   0 sweav     (1001) sweav     (1001)       10 2023-05-16 17:30:55.000000 warrenapp-0.1.2/src/warrenapp.egg-info/top_level.txt
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-24 18:40:30.029661 warrenapp-0.1.3/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1521 2023-05-04 20:41:15.000000 warrenapp-0.1.3/LICENSE
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     3452 2023-05-24 18:40:30.029661 warrenapp-0.1.3/PKG-INFO
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     1242 2023-05-24 18:39:07.000000 warrenapp-0.1.3/README.md
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     1351 2023-05-24 18:38:00.000000 warrenapp-0.1.3/pyproject.toml
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)       38 2023-05-24 18:40:30.029661 warrenapp-0.1.3/setup.cfg
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      245 2023-05-04 23:54:39.000000 warrenapp-0.1.3/setup.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-24 18:40:30.021661 warrenapp-0.1.3/src/
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-24 18:40:30.021661 warrenapp-0.1.3/src/warrenapp/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)       24 2023-05-04 20:41:15.000000 warrenapp-0.1.3/src/warrenapp/__init__.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      281 2023-05-04 23:54:00.000000 warrenapp-0.1.3/src/warrenapp/apps.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-24 18:40:30.021661 warrenapp-0.1.3/src/warrenapp/badelf_tools/
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     4776 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/badelf_tools/acf.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)    20158 2023-05-04 20:41:15.000000 warrenapp-0.1.3/src/warrenapp/badelf_tools/badelf_algorithm_functions.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)    14535 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/badelf_tools/utilities.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-24 18:40:30.021661 warrenapp-0.1.3/src/warrenapp/inputs/
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      309 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/inputs/warren_potcar_mappings.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     5179 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/models.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-24 18:40:30.021661 warrenapp-0.1.3/src/warrenapp/workflows/
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     1351 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/__init__.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-24 18:40:30.025661 warrenapp-0.1.3/src/warrenapp/workflows/nested_dft/
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      500 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/nested_dft/__init__.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     2755 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/nested_dft/double_relaxation_static_base.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     1300 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/nested_dft/prepop_relaxation_static_hse_hse.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     1520 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/nested_dft/prepop_relaxation_static_pbesol_hse.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     1128 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/nested_dft/prepop_relaxation_static_pbesol_hse_hse.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      816 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/nested_dft/prepop_relaxation_static_pbesol_pbesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     1990 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/nested_dft/relaxation_static_base.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-24 18:40:30.025661 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      752 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/__init__.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      807 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/badelf_hse.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      622 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/badelf_pbesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      637 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/bader_badelf_hse.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      650 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/bader_badelf_pbesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      651 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/bader_hse.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      742 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/bader_pbesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)    15988 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/base.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      903 2023-05-04 23:50:58.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/elf_hse.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      921 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/elf_pbesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     3958 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/prebader_badelf_dft.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)    14056 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-24 18:40:30.025661 warrenapp-0.1.3/src/warrenapp/workflows/relaxation/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      296 2023-05-04 20:41:15.000000 warrenapp-0.1.3/src/warrenapp/workflows/relaxation/__init__.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     1246 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/relaxation/hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      545 2023-05-04 23:52:02.000000 warrenapp-0.1.3/src/warrenapp/workflows/relaxation/hsesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     4738 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/relaxation/pbe.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      503 2023-05-04 23:52:02.000000 warrenapp-0.1.3/src/warrenapp/workflows/relaxation/pbe_metal.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      443 2023-05-04 23:52:02.000000 warrenapp-0.1.3/src/warrenapp/workflows/relaxation/pbesol.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      702 2023-05-04 23:52:02.000000 warrenapp-0.1.3/src/warrenapp/workflows/relaxation/scan.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-24 18:40:30.029661 warrenapp-0.1.3/src/warrenapp/workflows/static_energy/
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      364 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/static_energy/__init__.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      874 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/static_energy/hse.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      457 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/static_energy/hsesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      772 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/static_energy/pbe.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      482 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/static_energy/pbe_metal.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      575 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/static_energy/pbesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      445 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/static_energy/scan.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     2136 2023-05-24 18:38:00.000000 warrenapp-0.1.3/src/warrenapp/workflows/static_energy/seeded_hse.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-24 18:40:30.021661 warrenapp-0.1.3/src/warrenapp.egg-info/
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     3452 2023-05-24 18:40:30.000000 warrenapp-0.1.3/src/warrenapp.egg-info/PKG-INFO
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     2405 2023-05-24 18:40:30.000000 warrenapp-0.1.3/src/warrenapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)        1 2023-05-24 18:40:30.000000 warrenapp-0.1.3/src/warrenapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)        8 2023-05-24 18:40:30.000000 warrenapp-0.1.3/src/warrenapp.egg-info/requires.txt
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)       10 2023-05-24 18:40:30.000000 warrenapp-0.1.3/src/warrenapp.egg-info/top_level.txt
```

### Comparing `warrenapp-0.1.2/LICENSE` & `warrenapp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/PKG-INFO` & `warrenapp-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warrenapp
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Warrenapp is an extension of the Simulated Materials Ecosystem (Simmate), a package designed to ease computational materials research. The WarrenApp adds several custom workflows and settings.
 Author-email: Sam Weaver <sweav@unc.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Sam M. Weaver
         All rights reserved.
         
@@ -48,20 +48,18 @@
 </p>
 
 ### Requirements
 This extension is built off of [Simmate](https://github.com/jacksund/simmate). In order to use it you must have the base Simmate package installed.
 
 Tutorials are at: https://jacksund.github.io/simmate/getting_started/overview/
 
-Additionally, several components of this package don't work with Python 3.11 yet. Make sure your environment is on Python 3.10
-
 ### How to Install
-1. If you don't already have Simmate installed, follow the instructions to [install Simmate](https://jacksund.github.io/simmate/getting_started/installation/quick_start/) making sure to install Python 3.10
+1. If you don't already have Simmate installed, follow the instructions to [install Simmate](https://jacksund.github.io/simmate/getting_started/installation/quick_start/)
 ``` shell
-conda create -n my_env -c conda-forge python=3.10 simmate
+conda create -n my_env -c conda-forge python=3.11 simmate
 conda activate my_env
 simmate database reset
 ```
 2. Install the warrenapp using pip
 ``` shell
 pip install warrenapp
 ```
```

### Comparing `warrenapp-0.1.2/README.md` & `warrenapp-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 </p>
 
 ### Requirements
 This extension is built off of [Simmate](https://github.com/jacksund/simmate). In order to use it you must have the base Simmate package installed.
 
 Tutorials are at: https://jacksund.github.io/simmate/getting_started/overview/
 
-Additionally, several components of this package don't work with Python 3.11 yet. Make sure your environment is on Python 3.10
-
 ### How to Install
-1. If you don't already have Simmate installed, follow the instructions to [install Simmate](https://jacksund.github.io/simmate/getting_started/installation/quick_start/) making sure to install Python 3.10
+1. If you don't already have Simmate installed, follow the instructions to [install Simmate](https://jacksund.github.io/simmate/getting_started/installation/quick_start/)
 ``` shell
-conda create -n my_env -c conda-forge python=3.10 simmate
+conda create -n my_env -c conda-forge python=3.11 simmate
 conda activate my_env
 simmate database reset
 ```
 2. Install the warrenapp using pip
 ``` shell
 pip install warrenapp
 ```
```

### Comparing `warrenapp-0.1.2/pyproject.toml` & `warrenapp-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend= "setuptools.build_meta"
 
 [project]
 name = "warrenapp"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = ["simmate"]
 description = "The Warrenapp is an extension of the Simulated Materials Ecosystem (Simmate), a package designed to ease computational materials research. The WarrenApp adds several custom workflows and settings."
 readme = "README.md"
 requires-python=">=3.10"
 authors = [{ name = "Sam Weaver", email = "sweav@unc.edu" }]
 license = { file = "LICENSE" }
```

### Comparing `warrenapp-0.1.2/src/warrenapp/badelf_tools/acf.py` & `warrenapp-0.1.3/src/warrenapp/badelf_tools/acf.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/badelf_tools/badelf_algorithm_functions.py` & `warrenapp-0.1.3/src/warrenapp/badelf_tools/badelf_algorithm_functions.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/badelf_tools/utilities.py` & `warrenapp-0.1.3/src/warrenapp/badelf_tools/utilities.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/models.py` & `warrenapp-0.1.3/src/warrenapp/models.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/__init__.py` & `warrenapp-0.1.3/src/warrenapp/workflows/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from .nested_dft import (
-    Nested__Warren__RelaxationStaticHse,
-    Nested__Warren__RelaxationStaticPbesol,
+    Nested__Warren__RelaxationStaticHseHse,
+    Nested__Warren__RelaxationStaticPbeHse,
+    Nested__Warren__RelaxationStaticPbeHseHse,
+    Nested__Warren__RelaxationStaticPbePbe,
+    Relaxation__Warren__HseWithWavecar,
+    Relaxation__Warren__PbeWithWavecar,
 )
 from .population_analysis import (
     PopulationAnalysis__Warren__BadelfHse,
     PopulationAnalysis__Warren__BadelfPbesol,
     PopulationAnalysis__Warren__BaderBadelfHse,
     PopulationAnalysis__Warren__BaderBadelfPbesol,
     PopulationAnalysis__Warren__BaderHse,
```

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/prepop_relaxation_static_hse.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/bader_hse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding: utf-8 -*-
-from warrenapp.workflows.nested_dft.relaxation_static_base import RelaxationStaticBase
+
+# from warrenapp.workflows.population_analysis.bader_pbe import (
+#     StaticEnergy__Warren__PrebaderPbe,
+# )
+from warrenapp.workflows.population_analysis.base import VaspBaderBase
 from warrenapp.workflows.population_analysis.prebader_badelf_dft import (
-    StaticEnergy__Warren__PrebadelfHse,
+    StaticEnergy__Warren__PrebaderHse,
 )
-from warrenapp.workflows.relaxation.pbesol import Relaxation__Warren__Pbesol
 
 
-# This workflow will run
-class Nested__Warren__RelaxationStaticHse(RelaxationStaticBase):
+class PopulationAnalysis__Warren__BaderHse(VaspBaderBase):
     """
-    Runs a PBEsol quality structure relaxation, an HSE quality static energy
-    calculation.
+    Runs a static energy calculation using an extra-fine FFT grid using vasp
+    and then carries out Bader analysis on the resulting charge density.
+    Uses the Warren lab HSE settings.
     """
 
-    static_energy_workflow = StaticEnergy__Warren__PrebadelfHse
-    # We use pbesol as our default relaxation functional because it doesn't take
-    # much more time than pbe and is considered to be more accurate for solids
-    # (Phys. Rev. Lett. 102, 039902 (2009))
-    relaxation_workflow = Relaxation__Warren__Pbesol
+    static_energy_prebader = StaticEnergy__Warren__PrebaderHse
```

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/prepop_relaxation_static_pbesol.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/badelf_pbesol.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # -*- coding: utf-8 -*-
 
-from warrenapp.workflows.nested_dft.relaxation_static_base import RelaxationStaticBase
+from warrenapp.workflows.population_analysis.base import VaspBadElfBase
 from warrenapp.workflows.population_analysis.prebader_badelf_dft import (
     StaticEnergy__Warren__PrebadelfPbesol,
 )
-from warrenapp.workflows.relaxation.pbesol import Relaxation__Warren__Pbesol
 
 
-class Nested__Warren__RelaxationStaticPbesol(RelaxationStaticBase):
+class PopulationAnalysis__Warren__BadelfPbesol(VaspBadElfBase):
     """
-    Runs a PBEsol quality structure relaxation, a PBEsol quality static energy
-    calculation.
-
+    Runs a static energy calculation using an extra-fine FFT grid and then
+    carries out Bader analysis on the resulting charge density using the ELFCAR
+    as a reference when partitioning. Uses the PBE functional and settings from
+    the Warren Lab.
     """
 
-    static_energy_workflow = StaticEnergy__Warren__PrebadelfPbesol
-    # We use pbesol as our default relaxation functional because it doesn't take
-    # much more time than pbe and is considered to be more accurate for solids
-    # (Phys. Rev. Lett. 102, 039902 (2009))
-    relaxation_workflow = Relaxation__Warren__Pbesol
+    static_energy_prebadelf = StaticEnergy__Warren__PrebadelfPbesol
```

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/relaxation_static_base.py` & `warrenapp-0.1.3/src/warrenapp/workflows/nested_dft/relaxation_static_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
 
+import os
+import shutil
 from pathlib import Path
 
 from simmate.engine import Workflow
 from simmate.toolkit import Structure
 
 
 class RelaxationStaticBase(Workflow):
@@ -26,28 +28,33 @@
         cls,
         structure: Structure,
         command: str = None,
         source: dict = None,
         directory: Path = None,
         **kwargs,
     ):
-        # run a relaxation at PBE quality
+        # run a relaxation
         relaxation_directory = directory / "relaxation"
         relaxation_result = cls.relaxation_workflow.run(
             structure=structure,
             command=command,
             source=source,
             directory=relaxation_directory,
         ).result()
 
         static_energy_directory = directory / "static_energy"
         # run a static energy and bader/badelf analysis using the same structure
         # as above.
         # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
         # We need to make a new directory because only one vasp workflow can
         # be run in each directory.
+        os.mkdir(static_energy_directory)
+        shutil.copyfile(
+            relaxation_directory / "WAVECAR", static_energy_directory / "WAVECAR"
+        )
         static_energy_result = cls.static_energy_workflow.run(
             structure=relaxation_result,
             command=command,
             source=source,
             directory=static_energy_directory,
+            # copy_previous_directory=True,
         )
```

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/__init__.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/badelf_hse.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/badelf_hse.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/badelf_pbesol.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/bader_badelf_pbesol.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: utf-8 -*-
 
-from warrenapp.workflows.population_analysis.base import VaspBadElfBase
+
+from simmate.engine.workflow import Workflow
+
+from warrenapp.workflows.population_analysis.base import VaspBaderBadElfBase
 from warrenapp.workflows.population_analysis.prebader_badelf_dft import (
     StaticEnergy__Warren__PrebadelfPbesol,
 )
 
 
-class PopulationAnalysis__Warren__BadelfPbesol(VaspBadElfBase):
+class PopulationAnalysis__Warren__BaderBadelfPbesol(VaspBaderBadElfBase):
     """
-    Runs a static energy calculation using an extra-fine FFT grid and then
-    carries out Bader analysis on the resulting charge density using the ELFCAR
-    as a reference when partitioning. Uses the PBE functional and settings from
-    the Warren Lab.
+    Runs a static energy calculation using an extra-fine FFT grid using vasp
+    and then carries out Badelf and Bader analysis on the resulting charge density.
+    Uses the Warren lab settings Pbesol settings.
     """
 
-    static_energy_prebadelf = StaticEnergy__Warren__PrebadelfPbesol
+    static_energy_prebadelf: Workflow = StaticEnergy__Warren__PrebadelfPbesol
```

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/bader_badelf_hse.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/bader_badelf_hse.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/bader_badelf_pbesol.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/bader_pbesol.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 
-
-from simmate.engine.workflow import Workflow
-
-from warrenapp.workflows.population_analysis.base import VaspBaderBadElfBase
-from warrenapp.workflows.population_analysis.prebader_badelf_dft import (
+from warrenapp.workflows.population_analysis.badelf_pbesol import (
     StaticEnergy__Warren__PrebadelfPbesol,
 )
+from warrenapp.workflows.population_analysis.base import VaspBaderBase
+from warrenapp.workflows.population_analysis.prebader_badelf_dft import (
+    StaticEnergy__Warren__PrebaderPbesol,
+)
 
 
-class PopulationAnalysis__Warren__BaderBadelfPbesol(VaspBaderBadElfBase):
+class PopulationAnalysis__Warren__BaderPbesol(VaspBaderBase):
     """
     Runs a static energy calculation using an extra-fine FFT grid using vasp
-    and then carries out Badelf and Bader analysis on the resulting charge density.
+    and then carries out Bader analysis on the resulting charge density.
     Uses the Warren lab settings Pbesol settings.
     """
 
-    static_energy_prebadelf: Workflow = StaticEnergy__Warren__PrebadelfPbesol
+    static_energy_prebader = StaticEnergy__Warren__PrebaderPbesol
+    static_energy_prebadelf = StaticEnergy__Warren__PrebadelfPbesol
```

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/base.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -374,7 +374,27 @@
             # Run bader
             PopulationAnalysis__Warren__Bader.run(
                 directory=directory,
             ).result()
             # Copy bader files
             for file in bader_files:
                 shutil.copy(directory / file, directory / "bader")
+
+
+# We want to define the settings that will be used when updating static energy
+# workflows for prebader or prebadelf DFT calculations. We do that here so
+# that we don't need to do it in every inheriting class.
+prebader_incar_settings = dict(
+    NGXF__density_a=40,
+    NGYF__density_b=40,
+    NGZF__density_c=40,
+    LAECHG=True,  # write core charge density to AECCAR0 and valence to AECCAR2
+)
+prebadelf_incar_settings = dict(
+    NGX__density_a=40,  # Note that these set the FFT grid while the pre-Bader task sets the
+    NGY__density_b=40,  # fine FFT grid (e.g. useds NGX instead of NGXF)
+    NGZ__density_c=40,
+    LELF=True,  # Writes the ELFCAR
+    NPAR=1,  # Must be set if LELF is set
+    PREC="Single",  # ensures CHGCAR grid matches ELFCAR grid
+    LAECHG=True,  # write core charge density to AECCAR0 and valence to AECCAR2
+)
```

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/elf_hse.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/elf_hse.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/elf_pbesol.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/elf_pbesol.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/prebader_badelf_dft.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/prebader_badelf_dft.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from warrenapp.workflows.static_energy.hse import StaticEnergy__Warren__Hse
 from warrenapp.workflows.static_energy.pbesol import StaticEnergy__Warren__Pbesol
 
 # We want to define the settings that will be used when updating static energy
 # workflows for prebader or prebadelf DFT calculations. We do that here so
 # that we don't need to do it in every inheriting class.
 prebader_incar_settings = dict(
-    NGXF__density_a=10,
-    NGYF__density_b=10,
-    NGZF__density_c=10,
+    NGXF__density_a=40,
+    NGYF__density_b=40,
+    NGZF__density_c=40,
     LAECHG=True,  # write core charge density to AECCAR0 and valence to AECCAR2
 )
 prebadelf_incar_settings = dict(
-    NGX__density_a=10,  # Note that these set the FFT grid while the pre-Bader task sets the
-    NGY__density_b=10,  # fine FFT grid (e.g. useds NGX instead of NGXF)
-    NGZ__density_c=10,
+    NGX__density_a=40,  # Note that these set the FFT grid while the pre-Bader task sets the
+    NGY__density_b=40,  # fine FFT grid (e.g. useds NGX instead of NGXF)
+    NGZ__density_c=40,
     LELF=True,  # Writes the ELFCAR
     NPAR=1,  # Must be set if LELF is set
     PREC="Single",  # ensures CHGCAR grid matches ELFCAR grid
     LAECHG=True,  # write core charge density to AECCAR0 and valence to AECCAR2
 )
```

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py` & `warrenapp-0.1.3/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/relaxation/hse.py` & `warrenapp-0.1.3/src/warrenapp/workflows/relaxation/hse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # -*- coding: utf-8 -*-
 
+from warrenapp.inputs.warren_potcar_mappings import HSE_POTCAR_MAPPINGS
 from warrenapp.workflows.relaxation.pbe import Relaxation__Warren__Pbe
 
 
 class Relaxation__Warren__Hse(Relaxation__Warren__Pbe):
     """
     Runs a VASP relaxation calculation using Warren Lab HSE settings.
     """
 
     description_doc_short = "Warren Lab presets for HSE geometry optimization"
+    # some potcars don't work with HSE in VASP 5.x.x. I change them here
+    # in the hopes that they will work properly.
+    potcar_mappings = HSE_POTCAR_MAPPINGS
 
     incar = Relaxation__Warren__Pbe.incar.copy()
     incar.update(
         ALGO="Damped",  # We use Damped because it is the recommended setting by
         # by VASP (https://www.vasp.at/wiki/index.php/LHFCALC)
         HFSCREEN=0.2,
         ICHARG=1,
         LHFCALC=True,
         PRECFOCK="Fast",
-        TIME=0.5,  # This is the recommended setting when using the Damped tag.
-        # VASP also suggests lowering it if convergence isn't reached which I may
-        # need to incorporate into an error handler.
+        TIME=0.2,  # This is lower than the recommended setting (0.5) when using the
+        # Damped tag because calculations struggle to converge.
+        # VASP also suggests lowering it if convergence isn't reached so there
+        # is precedence for this.
         VDW_S8=2.310,  # these three tags are necessary for IVDW 12 with HSE06
         VDW_A1=0.383,
         VDW_A2=5.685,
     )
```

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/relaxation/hsesol.py` & `warrenapp-0.1.3/src/warrenapp/workflows/relaxation/hsesol.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/relaxation/pbe.py` & `warrenapp-0.1.3/src/warrenapp/workflows/relaxation/pbe.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,40 +32,40 @@
     TripleProduct,
     Unconverged,
     Walltime,
     Zbrent,
     Zheev,
     Zpotrf,
 )
-from simmate.apps.vasp.inputs.potcar_mappings import PBE_ELEMENT_MAPPINGS
+from simmate.apps.vasp.inputs.potcar_mappings import PBE_POTCAR_MAPPINGS
 from simmate.apps.vasp.workflows.base import VaspWorkflow
 
 
 class Relaxation__Warren__Pbe(VaspWorkflow):
     """
     Runs a VASP geometry optimization using preferred settings from the Warren lab.
 
     """
 
     description_doc_short = "Warren Lab's presets for PBE optimization"
 
     functional = "PBE"
-    potcar_mappings = PBE_ELEMENT_MAPPINGS
+    potcar_mappings = PBE_POTCAR_MAPPINGS
     # For now I'm keeping the matproj default element mappings, but I will likely
     # update these for future calculations.
 
     incar = dict(
         ALGO="Fast",
-        EDIFF__per_atom=5.0e-05,
+        EDIFF__per_atom=1e-05,  # This is slightly higher quality than the settings in Simmate (5e-05)
         ENCUT=520,  # Should set dynamically in future
         IBRION=2,
         ISIF=3,
         ISMEAR=0,  # Gaussian smearing
         ISPIN=2,
-        KSPACING=0.4,
+        KSPACING=0.25,  # This is probably on the edge of good quality
         LASPH=True,
         LORBIT=11,
         LREAL="Auto",
         LWAVE=False,
         NELM=150,
         NSW=99,
         PREC="Accurate",
```

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/relaxation/scan.py` & `warrenapp-0.1.3/src/warrenapp/workflows/relaxation/scan.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/static_energy/hse.py` & `warrenapp-0.1.3/src/warrenapp/workflows/static_energy/hse.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/static_energy/pbe.py` & `warrenapp-0.1.3/src/warrenapp/workflows/static_energy/pbe.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/static_energy/pbesol.py` & `warrenapp-0.1.3/src/warrenapp/workflows/static_energy/pbesol.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp/workflows/static_energy/seeded_hse.py` & `warrenapp-0.1.3/src/warrenapp/workflows/static_energy/seeded_hse.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.2/src/warrenapp.egg-info/PKG-INFO` & `warrenapp-0.1.3/src/warrenapp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warrenapp
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Warrenapp is an extension of the Simulated Materials Ecosystem (Simmate), a package designed to ease computational materials research. The WarrenApp adds several custom workflows and settings.
 Author-email: Sam Weaver <sweav@unc.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Sam M. Weaver
         All rights reserved.
         
@@ -48,20 +48,18 @@
 </p>
 
 ### Requirements
 This extension is built off of [Simmate](https://github.com/jacksund/simmate). In order to use it you must have the base Simmate package installed.
 
 Tutorials are at: https://jacksund.github.io/simmate/getting_started/overview/
 
-Additionally, several components of this package don't work with Python 3.11 yet. Make sure your environment is on Python 3.10
-
 ### How to Install
-1. If you don't already have Simmate installed, follow the instructions to [install Simmate](https://jacksund.github.io/simmate/getting_started/installation/quick_start/) making sure to install Python 3.10
+1. If you don't already have Simmate installed, follow the instructions to [install Simmate](https://jacksund.github.io/simmate/getting_started/installation/quick_start/)
 ``` shell
-conda create -n my_env -c conda-forge python=3.10 simmate
+conda create -n my_env -c conda-forge python=3.11 simmate
 conda activate my_env
 simmate database reset
 ```
 2. Install the warrenapp using pip
 ``` shell
 pip install warrenapp
 ```
```

### Comparing `warrenapp-0.1.2/src/warrenapp.egg-info/SOURCES.txt` & `warrenapp-0.1.3/src/warrenapp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,22 @@
 src/warrenapp.egg-info/SOURCES.txt
 src/warrenapp.egg-info/dependency_links.txt
 src/warrenapp.egg-info/requires.txt
 src/warrenapp.egg-info/top_level.txt
 src/warrenapp/badelf_tools/acf.py
 src/warrenapp/badelf_tools/badelf_algorithm_functions.py
 src/warrenapp/badelf_tools/utilities.py
+src/warrenapp/inputs/warren_potcar_mappings.py
 src/warrenapp/workflows/__init__.py
 src/warrenapp/workflows/nested_dft/__init__.py
-src/warrenapp/workflows/nested_dft/prepop_relaxation_static_hse.py
-src/warrenapp/workflows/nested_dft/prepop_relaxation_static_pbesol.py
+src/warrenapp/workflows/nested_dft/double_relaxation_static_base.py
+src/warrenapp/workflows/nested_dft/prepop_relaxation_static_hse_hse.py
+src/warrenapp/workflows/nested_dft/prepop_relaxation_static_pbesol_hse.py
+src/warrenapp/workflows/nested_dft/prepop_relaxation_static_pbesol_hse_hse.py
+src/warrenapp/workflows/nested_dft/prepop_relaxation_static_pbesol_pbesol.py
 src/warrenapp/workflows/nested_dft/relaxation_static_base.py
 src/warrenapp/workflows/population_analysis/__init__.py
 src/warrenapp/workflows/population_analysis/badelf_hse.py
 src/warrenapp/workflows/population_analysis/badelf_pbesol.py
 src/warrenapp/workflows/population_analysis/bader_badelf_hse.py
 src/warrenapp/workflows/population_analysis/bader_badelf_pbesol.py
 src/warrenapp/workflows/population_analysis/bader_hse.py
```

