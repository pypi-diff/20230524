# Comparing `tmp/fonsim-0.4.0.tar.gz` & `tmp/fonsim-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fonsim-0.4.0.tar", last modified: Mon May 15 17:26:10 2023, max compression
+gzip compressed data, was "fonsim-0.4.1.tar", last modified: Wed May 24 13:16:17 2023, max compression
```

## Comparing `fonsim-0.4.0.tar` & `fonsim-0.4.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.024949 fonsim-0.4.0/
--rw-rw-r--   0 arend     (1000) arend     (1000)    34523 2022-05-16 00:07:54.000000 fonsim-0.4.0/LICENSE.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)     3060 2023-05-15 17:26:10.024949 fonsim-0.4.0/PKG-INFO
--rw-rw-r--   0 arend     (1000) arend     (1000)     2309 2023-05-08 14:23:04.000000 fonsim-0.4.0/README.md
--rw-rw-r--   0 arend     (1000) arend     (1000)      105 2022-05-16 00:07:54.000000 fonsim-0.4.0/pyproject.toml
--rw-rw-r--   0 arend     (1000) arend     (1000)       38 2023-05-15 17:26:10.024949 fonsim-0.4.0/setup.cfg
--rw-rw-r--   0 arend     (1000) arend     (1000)     1334 2023-05-10 00:14:35.000000 fonsim-0.4.0/setup.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.004949 fonsim-0.4.0/src/
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.008949 fonsim-0.4.0/src/fonsim/
--rw-rw-r--   0 arend     (1000) arend     (1000)      555 2023-05-05 15:10:16.000000 fonsim-0.4.0/src/fonsim/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      565 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/colors.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.012949 fonsim-0.4.0/src/fonsim/components/
--rw-rw-r--   0 arend     (1000) arend     (1000)      269 2023-05-08 18:37:27.000000 fonsim-0.4.0/src/fonsim/components/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     5574 2023-05-08 14:09:52.000000 fonsim-0.4.0/src/fonsim/components/actuators.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     5843 2023-05-05 15:10:16.000000 fonsim-0.4.0/src/fonsim/components/circulartube_autodiff.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     6566 2023-05-08 14:09:52.000000 fonsim-0.4.0/src/fonsim/components/containers.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     2831 2023-05-05 15:10:16.000000 fonsim-0.4.0/src/fonsim/components/containers_autodiff.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      923 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/components/dummy.py
--rw-rw-r--   0 arend     (1000) arend     (1000)    12333 2023-05-14 23:39:01.000000 fonsim-0.4.0/src/fonsim/components/restrictors.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     5680 2023-05-13 18:19:15.000000 fonsim-0.4.0/src/fonsim/components/sources.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      277 2023-05-08 14:23:04.000000 fonsim-0.4.0/src/fonsim/components/terminals.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     2211 2023-05-08 16:06:19.000000 fonsim-0.4.0/src/fonsim/components/valves.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.012949 fonsim-0.4.0/src/fonsim/constants/
--rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/constants/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      263 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/constants/norm.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      215 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/constants/physical.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.012949 fonsim-0.4.0/src/fonsim/conversion/
--rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/conversion/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      897 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/conversion/indexmatch.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.016949 fonsim-0.4.0/src/fonsim/core/
--rw-rw-r--   0 arend     (1000) arend     (1000)      287 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/core/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)    22530 2023-05-08 20:53:03.000000 fonsim-0.4.0/src/fonsim/core/component.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     1963 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/core/node.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      277 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/core/setnumpythreads.py
--rw-rw-r--   0 arend     (1000) arend     (1000)    42054 2023-05-08 16:32:15.000000 fonsim-0.4.0/src/fonsim/core/simulation.py
--rw-rw-r--   0 arend     (1000) arend     (1000)    19886 2023-05-14 23:39:01.000000 fonsim-0.4.0/src/fonsim/core/solver.py
--rw-rw-r--   0 arend     (1000) arend     (1000)    11114 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/core/system.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3995 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/core/terminal.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     4492 2023-05-08 14:23:04.000000 fonsim-0.4.0/src/fonsim/core/variable.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.016949 fonsim-0.4.0/src/fonsim/data/
--rw-rw-r--   0 arend     (1000) arend     (1000)      134 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/data/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3335 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/data/curve.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     4454 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/data/dataseries.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     4446 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/data/interpolate.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     6459 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/data/pvcurve.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     5365 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/data/writeout.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.016949 fonsim-0.4.0/src/fonsim/fluid/
--rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/fluid/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     1867 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/fluid/fallback.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3329 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/fluid/fluid.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.020949 fonsim-0.4.0/src/fonsim/fluids/
--rw-rw-r--   0 arend     (1000) arend     (1000)       52 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/fluids/Bingham.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      758 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/fluids/IdealCompressible.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      869 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/fluids/IdealIncompressible.py
--rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/fluids/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      693 2023-05-13 18:19:15.000000 fonsim-0.4.0/src/fonsim/notice_beta.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.020949 fonsim-0.4.0/src/fonsim/resources/
--rw-rw-r--   0 arend     (1000) arend     (1000)      979 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/resources/Measurement_60mm_balloon_actuator_01.csv
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.020949 fonsim-0.4.0/src/fonsim/visual/
--rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/visual/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     1977 2023-05-08 14:09:52.000000 fonsim-0.4.0/src/fonsim/visual/plotting.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.020949 fonsim-0.4.0/src/fonsim/wave/
--rw-rw-r--   0 arend     (1000) arend     (1000)       75 2022-05-16 00:07:54.000000 fonsim-0.4.0/src/fonsim/wave/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     5357 2023-05-05 15:10:16.000000 fonsim-0.4.0/src/fonsim/wave/custom.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     1365 2023-03-23 19:19:04.000000 fonsim-0.4.0/src/fonsim/wave/wave.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.008949 fonsim-0.4.0/src/fonsim.egg-info/
--rw-rw-r--   0 arend     (1000) arend     (1000)     3060 2023-05-15 17:26:09.000000 fonsim-0.4.0/src/fonsim.egg-info/PKG-INFO
--rw-rw-r--   0 arend     (1000) arend     (1000)     1989 2023-05-15 17:26:10.000000 fonsim-0.4.0/src/fonsim.egg-info/SOURCES.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)        1 2023-05-15 17:26:09.000000 fonsim-0.4.0/src/fonsim.egg-info/dependency_links.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)       72 2023-05-15 17:26:09.000000 fonsim-0.4.0/src/fonsim.egg-info/requires.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)        7 2023-05-15 17:26:09.000000 fonsim-0.4.0/src/fonsim.egg-info/top_level.txt
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-15 17:26:10.024949 fonsim-0.4.0/tests/
--rw-rw-r--   0 arend     (1000) arend     (1000)     1309 2023-05-08 14:09:52.000000 fonsim-0.4.0/tests/test_basic.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     4153 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_component_autocall.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3015 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_custom.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3238 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_dataseries.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      711 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_indexmatch.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3893 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_interpolate.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     1751 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_node.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3205 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_pvcurve.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     5311 2023-05-08 14:09:52.000000 fonsim-0.4.0/tests/test_simulation_and_solver.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     4594 2023-05-13 18:19:15.000000 fonsim-0.4.0/tests/test_solver_infinite_flow.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     7373 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_system.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     2684 2023-03-23 19:19:04.000000 fonsim-0.4.0/tests/test_terminal.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     1253 2023-05-08 14:23:04.000000 fonsim-0.4.0/tests/test_variable.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.904641 fonsim-0.4.1/
+-rw-rw-r--   0 arend     (1000) arend     (1000)    34523 2022-05-16 00:07:54.000000 fonsim-0.4.1/LICENSE.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3313 2023-05-24 13:16:17.904641 fonsim-0.4.1/PKG-INFO
+-rw-rw-r--   0 arend     (1000) arend     (1000)     2562 2023-05-24 12:53:35.000000 fonsim-0.4.1/README.md
+-rw-rw-r--   0 arend     (1000) arend     (1000)      105 2022-05-16 00:07:54.000000 fonsim-0.4.1/pyproject.toml
+-rw-rw-r--   0 arend     (1000) arend     (1000)       38 2023-05-24 13:16:17.904641 fonsim-0.4.1/setup.cfg
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1334 2023-05-24 13:14:25.000000 fonsim-0.4.1/setup.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.856627 fonsim-0.4.1/src/
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.864629 fonsim-0.4.1/src/fonsim/
+-rw-rw-r--   0 arend     (1000) arend     (1000)      555 2023-05-05 15:10:16.000000 fonsim-0.4.1/src/fonsim/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      565 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/colors.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.872631 fonsim-0.4.1/src/fonsim/components/
+-rw-rw-r--   0 arend     (1000) arend     (1000)      269 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/components/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5574 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/components/actuators.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5843 2023-05-05 15:10:16.000000 fonsim-0.4.1/src/fonsim/components/circulartube_autodiff.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     6566 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/components/containers.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     2831 2023-05-05 15:10:16.000000 fonsim-0.4.1/src/fonsim/components/containers_autodiff.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      923 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/components/dummy.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)    12333 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/components/restrictors.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5680 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/components/sources.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      277 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/components/terminals.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     2211 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/components/valves.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.872631 fonsim-0.4.1/src/fonsim/constants/
+-rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.1/src/fonsim/constants/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      263 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/constants/norm.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      215 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/constants/physical.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.876633 fonsim-0.4.1/src/fonsim/conversion/
+-rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.1/src/fonsim/conversion/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      897 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/conversion/indexmatch.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.880634 fonsim-0.4.1/src/fonsim/core/
+-rw-rw-r--   0 arend     (1000) arend     (1000)      287 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/core/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)    22530 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/core/component.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1963 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/core/node.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      277 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/core/setnumpythreads.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)    42054 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/core/simulation.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)    20184 2023-05-24 13:09:59.000000 fonsim-0.4.1/src/fonsim/core/solver.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)    11114 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/core/system.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3995 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/core/terminal.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     4492 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/core/variable.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.884635 fonsim-0.4.1/src/fonsim/data/
+-rw-rw-r--   0 arend     (1000) arend     (1000)      134 2022-05-16 00:07:54.000000 fonsim-0.4.1/src/fonsim/data/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3335 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/data/curve.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     4454 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/data/dataseries.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     4446 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/data/interpolate.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     6459 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/data/pvcurve.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5365 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/data/writeout.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.888636 fonsim-0.4.1/src/fonsim/fluid/
+-rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.1/src/fonsim/fluid/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1867 2022-05-16 00:07:54.000000 fonsim-0.4.1/src/fonsim/fluid/fallback.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3329 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/fluid/fluid.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.888636 fonsim-0.4.1/src/fonsim/fluids/
+-rw-rw-r--   0 arend     (1000) arend     (1000)       52 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/fluids/Bingham.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      758 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/fluids/IdealCompressible.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      869 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/fluids/IdealIncompressible.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.1/src/fonsim/fluids/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      693 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/notice_beta.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.888636 fonsim-0.4.1/src/fonsim/resources/
+-rw-rw-r--   0 arend     (1000) arend     (1000)      979 2022-05-16 00:07:54.000000 fonsim-0.4.1/src/fonsim/resources/Measurement_60mm_balloon_actuator_01.csv
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.892638 fonsim-0.4.1/src/fonsim/visual/
+-rw-rw-r--   0 arend     (1000) arend     (1000)        0 2022-05-16 00:07:54.000000 fonsim-0.4.1/src/fonsim/visual/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1977 2023-05-15 17:30:22.000000 fonsim-0.4.1/src/fonsim/visual/plotting.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.892638 fonsim-0.4.1/src/fonsim/wave/
+-rw-rw-r--   0 arend     (1000) arend     (1000)       75 2022-05-16 00:07:54.000000 fonsim-0.4.1/src/fonsim/wave/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5357 2023-05-05 15:10:16.000000 fonsim-0.4.1/src/fonsim/wave/custom.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1365 2023-03-23 19:19:04.000000 fonsim-0.4.1/src/fonsim/wave/wave.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.868630 fonsim-0.4.1/src/fonsim.egg-info/
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3313 2023-05-24 13:16:17.000000 fonsim-0.4.1/src/fonsim.egg-info/PKG-INFO
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1989 2023-05-24 13:16:17.000000 fonsim-0.4.1/src/fonsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)        1 2023-05-24 13:16:17.000000 fonsim-0.4.1/src/fonsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)       72 2023-05-24 13:16:17.000000 fonsim-0.4.1/src/fonsim.egg-info/requires.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)        7 2023-05-24 13:16:17.000000 fonsim-0.4.1/src/fonsim.egg-info/top_level.txt
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-24 13:16:17.900640 fonsim-0.4.1/tests/
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1309 2023-05-15 17:30:22.000000 fonsim-0.4.1/tests/test_basic.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     4153 2023-03-23 19:19:04.000000 fonsim-0.4.1/tests/test_component_autocall.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3015 2023-03-23 19:19:04.000000 fonsim-0.4.1/tests/test_custom.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3238 2023-03-23 19:19:04.000000 fonsim-0.4.1/tests/test_dataseries.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      711 2023-03-23 19:19:04.000000 fonsim-0.4.1/tests/test_indexmatch.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3893 2023-03-23 19:19:04.000000 fonsim-0.4.1/tests/test_interpolate.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1751 2023-03-23 19:19:04.000000 fonsim-0.4.1/tests/test_node.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3205 2023-03-23 19:19:04.000000 fonsim-0.4.1/tests/test_pvcurve.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5311 2023-05-15 17:30:22.000000 fonsim-0.4.1/tests/test_simulation_and_solver.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     4594 2023-05-15 17:30:22.000000 fonsim-0.4.1/tests/test_solver_infinite_flow.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     7373 2023-03-23 19:19:04.000000 fonsim-0.4.1/tests/test_system.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     2684 2023-03-23 19:19:04.000000 fonsim-0.4.1/tests/test_terminal.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1253 2023-05-15 17:30:22.000000 fonsim-0.4.1/tests/test_variable.py
```

### Comparing `fonsim-0.4.0/LICENSE.txt` & `fonsim-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/PKG-INFO` & `fonsim-0.4.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,19 @@
-Metadata-Version: 2.1
-Name: fonsim
-Version: 0.4.0
-Summary: Fluidic Object-Oriented Network Simulator
-Home-page: http://fonsim.org
-Author: Arne Baeyens, Bert Van Raemdonck
-Author-email: info@fonsim.org
-License: AGPLv3
-Keywords: simulator,simulation,flow,fluids,fluidic,soft robot,soro,soft robotics,soft robots
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # FONSim
 [![PyPI version](https://badge.fury.io/py/fonsim.svg)](https://badge.fury.io/py/fonsim)
 [![Documentation Status](https://readthedocs.org/projects/fonsim/badge/?version=latest)](https://fonsim.readthedocs.io/en/latest/?badge=latest)
 ![coverage](https://gitlab.com/abaeyens/fonsim/badges/master/coverage.svg)
+[![DOI:10.1109/RoboSoft55895.2023.10122049](https://zenodo.org/badge/DOI/10.1109/RoboSoft55895.2023.10122049.svg)](https://doi.org/10.1109/RoboSoft55895.2023.10122049)
 #### _Fluidic Object-oriented Network SIMulator_
 
-An object-oriented Python 3 library designed for simulating pneumatic and hydraulic systems in soft robots.
-Find the full documentation on [fonsim.org](http://fonsim.org/).
+An object-oriented Python 3 package
+designed for simulating pneumatic and hydraulic systems in soft robots.
+It is being developed at the [KU Leuven soft robotics group](
+  https://softroboticsgroup.com).
+Full documentation: [fonsim.org](http://fonsim.org/).
 
 This project is available under the GNU Affero General Public License v3.0 (**agpl-3.0**) license.
 
 ### Installation
 The pre-packaged release version can be installed using `pip install fonsim`.
 See the [PyPI page](https://pypi.org/project/fonsim/) for more information.
```

### Comparing `fonsim-0.4.0/setup.py` & `fonsim-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fonsim",
-    version="0.4.0",
+    version="0.4.1",
     author="Arne Baeyens, Bert Van Raemdonck",
     author_email="info@fonsim.org",
     description="Fluidic Object-Oriented Network Simulator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://fonsim.org',
     keywords='simulator, simulation, flow, fluids, fluidic, soft robot, soro, soft robotics, soft robots',
```

### Comparing `fonsim-0.4.0/src/fonsim/__init__.py` & `fonsim-0.4.1/src/fonsim/__init__.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/colors.py` & `fonsim-0.4.1/src/fonsim/colors.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/components/actuators.py` & `fonsim-0.4.1/src/fonsim/components/actuators.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/components/circulartube_autodiff.py` & `fonsim-0.4.1/src/fonsim/components/circulartube_autodiff.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/components/containers.py` & `fonsim-0.4.1/src/fonsim/components/containers.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/components/containers_autodiff.py` & `fonsim-0.4.1/src/fonsim/components/containers_autodiff.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/components/dummy.py` & `fonsim-0.4.1/src/fonsim/components/dummy.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/components/restrictors.py` & `fonsim-0.4.1/src/fonsim/components/restrictors.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/components/sources.py` & `fonsim-0.4.1/src/fonsim/components/sources.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/components/valves.py` & `fonsim-0.4.1/src/fonsim/components/valves.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/conversion/indexmatch.py` & `fonsim-0.4.1/src/fonsim/conversion/indexmatch.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/core/component.py` & `fonsim-0.4.1/src/fonsim/core/component.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/core/node.py` & `fonsim-0.4.1/src/fonsim/core/node.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/core/simulation.py` & `fonsim-0.4.1/src/fonsim/core/simulation.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/core/solver.py` & `fonsim-0.4.1/src/fonsim/core/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,19 +202,23 @@
                 phi_correction = -np.linalg.solve(self.sim.H, residual)
             except np.linalg.LinAlgError as e:
                 # probably singular matrix or so
                 if self.sim.verbose: print(e)
                 return 0
             # Scale down the correction if it is so large
             # that it would push any arguments outside their allowed range
+            # todo: rewrite this to be more elegant and faster
             max_correction_pos = self.sim.phi_range[:, 0] - self.sim.phi[step, :]
             max_correction_neg = self.sim.phi_range[:, 1] - self.sim.phi[step, :]
-            rel_correction_pos = phi_correction / max_correction_pos
-            rel_correction_neg = phi_correction / max_correction_neg
-            times_too_large = max(np.amax(rel_correction_pos), np.amax(rel_correction_neg))
+            mask_pos = max_correction_pos != 0
+            mask_neg = max_correction_neg != 0
+            rel_correction = np.zeros((self.sim.nb_arguments, 2), dtype=float)
+            rel_correction[mask_pos, 0] = phi_correction[mask_pos] / max_correction_pos[mask_pos]
+            rel_correction[mask_neg, 1] = phi_correction[mask_neg] / max_correction_neg[mask_neg]
+            times_too_large = max(np.amax(rel_correction[:, 0]), np.amax(rel_correction[:, 1]))
             if alpha * times_too_large > 1:
                 # take 0.9 to keep a little distance from the limits
                 phi_correction *= 0.9 / times_too_large
             # Apply the correction
             self.sim.phi[step,:] = self.sim.phi[step,:] + alpha*phi_correction
         if self.sim.verbose:
             print(f'Exited without convergence with max_error {max_error:.1f}')
```

### Comparing `fonsim-0.4.0/src/fonsim/core/system.py` & `fonsim-0.4.1/src/fonsim/core/system.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/core/terminal.py` & `fonsim-0.4.1/src/fonsim/core/terminal.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/core/variable.py` & `fonsim-0.4.1/src/fonsim/core/variable.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/data/curve.py` & `fonsim-0.4.1/src/fonsim/data/curve.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/data/dataseries.py` & `fonsim-0.4.1/src/fonsim/data/dataseries.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/data/interpolate.py` & `fonsim-0.4.1/src/fonsim/data/interpolate.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/data/pvcurve.py` & `fonsim-0.4.1/src/fonsim/data/pvcurve.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/data/writeout.py` & `fonsim-0.4.1/src/fonsim/data/writeout.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/fluid/fallback.py` & `fonsim-0.4.1/src/fonsim/fluid/fallback.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/fluid/fluid.py` & `fonsim-0.4.1/src/fonsim/fluid/fluid.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/fluids/IdealCompressible.py` & `fonsim-0.4.1/src/fonsim/fluids/IdealCompressible.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/fluids/IdealIncompressible.py` & `fonsim-0.4.1/src/fonsim/fluids/IdealIncompressible.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/notice_beta.py` & `fonsim-0.4.1/src/fonsim/notice_beta.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/resources/Measurement_60mm_balloon_actuator_01.csv` & `fonsim-0.4.1/src/fonsim/resources/Measurement_60mm_balloon_actuator_01.csv`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/visual/plotting.py` & `fonsim-0.4.1/src/fonsim/visual/plotting.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/wave/custom.py` & `fonsim-0.4.1/src/fonsim/wave/custom.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim/wave/wave.py` & `fonsim-0.4.1/src/fonsim/wave/wave.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/src/fonsim.egg-info/PKG-INFO` & `fonsim-0.4.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fonsim
-Version: 0.4.0
+Version: 0.4.1
 Summary: Fluidic Object-Oriented Network Simulator
 Home-page: http://fonsim.org
 Author: Arne Baeyens, Bert Van Raemdonck
 Author-email: info@fonsim.org
 License: AGPLv3
 Keywords: simulator,simulation,flow,fluids,fluidic,soft robot,soro,soft robotics,soft robots
 Classifier: Development Status :: 4 - Beta
@@ -18,18 +18,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # FONSim
 [![PyPI version](https://badge.fury.io/py/fonsim.svg)](https://badge.fury.io/py/fonsim)
 [![Documentation Status](https://readthedocs.org/projects/fonsim/badge/?version=latest)](https://fonsim.readthedocs.io/en/latest/?badge=latest)
 ![coverage](https://gitlab.com/abaeyens/fonsim/badges/master/coverage.svg)
+[![DOI:10.1109/RoboSoft55895.2023.10122049](https://zenodo.org/badge/DOI/10.1109/RoboSoft55895.2023.10122049.svg)](https://doi.org/10.1109/RoboSoft55895.2023.10122049)
 #### _Fluidic Object-oriented Network SIMulator_
 
-An object-oriented Python 3 library designed for simulating pneumatic and hydraulic systems in soft robots.
-Find the full documentation on [fonsim.org](http://fonsim.org/).
+An object-oriented Python 3 package
+designed for simulating pneumatic and hydraulic systems in soft robots.
+It is being developed at the [KU Leuven soft robotics group](
+  https://softroboticsgroup.com).
+Full documentation: [fonsim.org](http://fonsim.org/).
 
 This project is available under the GNU Affero General Public License v3.0 (**agpl-3.0**) license.
 
 ### Installation
 The pre-packaged release version can be installed using `pip install fonsim`.
 See the [PyPI page](https://pypi.org/project/fonsim/) for more information.
```

### Comparing `fonsim-0.4.0/src/fonsim.egg-info/SOURCES.txt` & `fonsim-0.4.1/src/fonsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_basic.py` & `fonsim-0.4.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_component_autocall.py` & `fonsim-0.4.1/tests/test_component_autocall.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_custom.py` & `fonsim-0.4.1/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_dataseries.py` & `fonsim-0.4.1/tests/test_dataseries.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_indexmatch.py` & `fonsim-0.4.1/tests/test_indexmatch.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_interpolate.py` & `fonsim-0.4.1/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_node.py` & `fonsim-0.4.1/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_pvcurve.py` & `fonsim-0.4.1/tests/test_pvcurve.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_simulation_and_solver.py` & `fonsim-0.4.1/tests/test_simulation_and_solver.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_solver_infinite_flow.py` & `fonsim-0.4.1/tests/test_solver_infinite_flow.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_system.py` & `fonsim-0.4.1/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_terminal.py` & `fonsim-0.4.1/tests/test_terminal.py`

 * *Files identical despite different names*

### Comparing `fonsim-0.4.0/tests/test_variable.py` & `fonsim-0.4.1/tests/test_variable.py`

 * *Files identical despite different names*

