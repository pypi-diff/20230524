# Comparing `tmp/magnumnp-1.0.9.tar.gz` & `tmp/magnumnp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnumnp-1.0.9.tar", last modified: Wed May  3 15:33:07 2023, max compression
+gzip compressed data, was "magnumnp-1.1.0.tar", last modified: Wed May 24 18:29:56 2023, max compression
```

## Comparing `magnumnp-1.0.9.tar` & `magnumnp-1.1.0.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.837859 magnumnp-1.0.9/
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-03 15:32:50.000000 magnumnp-1.0.9/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    35069 2023-05-03 15:32:50.000000 magnumnp-1.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7091 2023-05-03 15:33:07.837859 magnumnp-1.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6598 2023-05-03 15:32:50.000000 magnumnp-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.832859 magnumnp-1.0.9/magnumnp/
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.834859 magnumnp-1.0.9/magnumnp/common/
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2485 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/decorated_tensor.py
--rw-rw-rw-   0 root         (0) root         (0)     8932 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/io.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     2044 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/material.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     6630 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/state.py
--rw-rw-rw-   0 root         (0) root         (0)    38962 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/tabulate.py
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/time_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     8878 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.835859 magnumnp-1.0.9/magnumnp/field_terms/
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5554 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/anisotropy.py
--rw-rw-rw-   0 root         (0) root         (0)     8338 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/demag.py
--rw-rw-rw-   0 root         (0) root         (0)     2248 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/demagPBC.py
--rw-rw-rw-   0 root         (0) root         (0)     7456 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/demag_nonequidistant.py
--rw-rw-rw-   0 root         (0) root         (0)     6605 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/dmi.py
--rw-rw-rw-   0 root         (0) root         (0)     3163 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     2110 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/exchangePBC.py
--rw-rw-rw-   0 root         (0) root         (0)     1862 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/external.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/field_terms.py
--rw-rw-rw-   0 root         (0) root         (0)     6325 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/oersted.py
--rw-rw-rw-   0 root         (0) root         (0)     4937 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/rkky.py
--rw-rw-rw-   0 root         (0) root         (0)     3263 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/spintorque.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.835859 magnumnp-1.0.9/magnumnp/loggers/
--rw-rw-rw-   0 root         (0) root         (0)      943 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/loggers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/loggers/field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     4018 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/loggers/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     7570 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/loggers/scalar_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.836860 magnumnp-1.0.9/magnumnp/solvers/
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/llg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.836860 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4420 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/rkf45.py
--rw-rw-rw-   0 root         (0) root         (0)     2247 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/scipy_ode.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/scipy_odeint.py
--rw-rw-rw-   0 root         (0) root         (0)     3256 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/torchdiffeq.py
--rw-rw-rw-   0 root         (0) root         (0)     3313 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.836860 magnumnp-1.0.9/magnumnp/utils/
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6669 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/utils/imaging_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1910 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/utils/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.832859 magnumnp-1.0.9/magnumnp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7091 2023-05-03 15:33:07.000000 magnumnp-1.0.9/magnumnp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1456 2023-05-03 15:33:07.000000 magnumnp-1.0.9/magnumnp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 15:33:07.000000 magnumnp-1.0.9/magnumnp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-03 15:33:07.000000 magnumnp-1.0.9/magnumnp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-03 15:33:07.000000 magnumnp-1.0.9/magnumnp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 15:33:07.837859 magnumnp-1.0.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1866 2023-05-03 15:33:01.000000 magnumnp-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.812390 magnumnp-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-24 18:29:41.000000 magnumnp-1.1.0/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    35069 2023-05-24 18:29:41.000000 magnumnp-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7118 2023-05-24 18:29:56.811390 magnumnp-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6625 2023-05-24 18:29:41.000000 magnumnp-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.808390 magnumnp-1.1.0/magnumnp/
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.809390 magnumnp-1.1.0/magnumnp/common/
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/decorated_tensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     8932 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/material.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     7251 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/state.py
+-rw-rw-rw-   0 root         (0) root         (0)    38962 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/tabulate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/time_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8878 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.810391 magnumnp-1.1.0/magnumnp/field_terms/
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/anisotropy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8459 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/demag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/demagPBC.py
+-rw-rw-rw-   0 root         (0) root         (0)     6698 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/demag_nonequidistant.py
+-rw-rw-rw-   0 root         (0) root         (0)     8592 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/dmi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/external.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/field_terms.py
+-rw-rw-rw-   0 root         (0) root         (0)     6357 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/oersted.py
+-rw-rw-rw-   0 root         (0) root         (0)     4936 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/rkky.py
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/spintorque.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.810391 magnumnp-1.1.0/magnumnp/loggers/
+-rw-rw-rw-   0 root         (0) root         (0)      943 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/loggers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/loggers/field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4018 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/loggers/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     7570 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/loggers/scalar_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.811390 magnumnp-1.1.0/magnumnp/solvers/
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/llg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.811390 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4420 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/rkf45.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/scipy_ode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/scipy_odeint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3256 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/torchdiffeq.py
+-rw-rw-rw-   0 root         (0) root         (0)     3312 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.811390 magnumnp-1.1.0/magnumnp/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6669 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/utils/imaging_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/utils/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.808390 magnumnp-1.1.0/magnumnp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7118 2023-05-24 18:29:56.000000 magnumnp-1.1.0/magnumnp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-05-24 18:29:56.000000 magnumnp-1.1.0/magnumnp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 18:29:56.000000 magnumnp-1.1.0/magnumnp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-24 18:29:56.000000 magnumnp-1.1.0/magnumnp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-24 18:29:56.000000 magnumnp-1.1.0/magnumnp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 18:29:56.812390 magnumnp-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2023-05-24 18:29:51.000000 magnumnp-1.1.0/setup.py
```

### Comparing `magnumnp-1.0.9/LICENSE` & `magnumnp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/PKG-INFO` & `magnumnp-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: magnumnp
-Version: 1.0.9
+Version: 1.1.0
 Summary: magnum.np finite-difference package for the solution of micromagnetic problems
 Home-page: http://gitlab.com/magnum.np/magnum.np
 Author: Florian Bruckner
 Author-email: florian.bruckner@univie.ac.at
 Project-URL: Documentation, https://magnum.np.gitlab.io/magnum.np/
 Project-URL: Changelog, https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-magnum.np 1.0.9
+magnum.np 1.1.0
 ===============
 
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
@@ -34,21 +34,21 @@
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
 The following demos are also stored on Google Colab, where they can directly be run without any local installation:
 
-   * [RKKY](demos/rkky.ipynb) ([Colab] (https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
-   * [Softmagnetic Composite](demos/softmagnetic_composite.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
-   * [Spin Orbit Torque](demos/sot.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
-   * [Standard Problem #4](demos/sp4.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
-   * [Standard Problem #5](demos/sp5.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
-   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
-   * [Standard Problem FMR](demos/sp_FMR.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
+   * [RKKY](demos/rkky/run.ipynb) ([Colab](https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
+   * [Softmagnetic Composite](demos/softmagnetic_composite/run.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
+   * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
+   * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
+   * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
+   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
+   * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
 
 
 
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
```

### Comparing `magnumnp-1.0.9/README.md` & `magnumnp-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-magnum.np 1.0.9
+magnum.np 1.1.0
 ===============
 
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
@@ -21,21 +21,21 @@
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
 The following demos are also stored on Google Colab, where they can directly be run without any local installation:
 
-   * [RKKY](demos/rkky.ipynb) ([Colab] (https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
-   * [Softmagnetic Composite](demos/softmagnetic_composite.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
-   * [Spin Orbit Torque](demos/sot.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
-   * [Standard Problem #4](demos/sp4.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
-   * [Standard Problem #5](demos/sp5.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
-   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
-   * [Standard Problem FMR](demos/sp_FMR.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
+   * [RKKY](demos/rkky/run.ipynb) ([Colab](https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
+   * [Softmagnetic Composite](demos/softmagnetic_composite/run.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
+   * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
+   * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
+   * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
+   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
+   * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
 
 
 
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
```

### Comparing `magnumnp-1.0.9/magnumnp/__init__.py` & `magnumnp-1.1.0/magnumnp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """magnum.np main module"""
 
-__version__ = '1.0.9'
+__version__ = '1.1.0'
 
 import magnumnp.common.logging as logging
 import torch
 torch.set_default_dtype(torch.float64)
 
 # monkey patch torch versions < 2.0 or on Windows
 try:
```

### Comparing `magnumnp-1.0.9/magnumnp/common/__init__.py` & `magnumnp-1.1.0/magnumnp/common/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/common/constants.py` & `magnumnp-1.1.0/magnumnp/common/constants.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/common/decorated_tensor.py` & `magnumnp-1.1.0/magnumnp/common/decorated_tensor.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,31 +26,36 @@
         self._cell_volumes = cell_volumes
         return super().__new__(self, x, *args, **kwargs)
 
     def avg(self, dim=(0,1,2)):
         if self.dim() <= 1: # e.g. [0,0,1]
             return self
         elif self.dim() == 2: # state.m[domain]
-            return (self * self._cell_volumes.unsqueeze(-1)).sum(dim=0) / self._cell_volumes.sum(dim=0)
+            return (self * self._cell_volumes).sum(dim=0) / self._cell_volumes.sum(dim=0)
         elif self.dim() == 3: # [nx,ny,nz]
-            return (self * self._cell_volumes).sum(dim=dim) / self._cell_volumes.sum()
+            return (self * self._cell_volumes.squeeze(-1)).sum(dim=dim) / self._cell_volumes.sum()
         else:                 # [nx,ny,nz,...]
-            return (self * self._cell_volumes.unsqueeze(-1)).sum(dim=dim) / self._cell_volumes.sum()
+            return (self * self._cell_volumes).sum(dim=dim) / self._cell_volumes.sum()
 
     def average(self, dim=(0,1,2)):
         return self.avg(dim)
 
     def normalize(self):
         self /= torch.linalg.norm(self, dim = -1, keepdim = True)
         self[...] = torch.nan_to_num(self, posinf=0, neginf=0)
         return self
 
     def __call__(self, t):
         return self
 
+    def __setitem__(self, key, value):
+        if hasattr(self, "_expanded"):
+            self.set_(self.clone())
+        super().__setitem__(key, value)
+
     def __getitem__(self, idx):
         item = super().__getitem__(idx)
 
         # update cell_volumes
         if isinstance(idx, tuple): # apply slicing
             if idx[0] == Ellipsis:
                 item._cell_volumes = self._cell_volumes
```

### Comparing `magnumnp-1.0.9/magnumnp/common/io.py` & `magnumnp-1.1.0/magnumnp/common/io.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/common/logging.py` & `magnumnp-1.1.0/magnumnp/common/logging.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/common/material.py` & `magnumnp-1.1.0/magnumnp/common/material.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/common/mesh.py` & `magnumnp-1.1.0/magnumnp/common/mesh.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,27 +13,21 @@
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 from magnumnp.common import logging
+import torch
 
 __all__ = ["Mesh"]
 
 class Mesh(object):
-    def __init__(self, n, dx, origin=(0,0,0)):
+    def __init__(self, n, dx, origin=(0,0,0), pbc=(0,0,0)):
         self.n = tuple(n)
         self.dx = tuple(dx)
         self.origin = tuple(origin)
-
-    @property
-    def cell_volume(self):
-        return self.dx[0] * self.dx[1] * self.dx[2]
-
-    @property
-    def volume(self):
-        return self.n[0] * self.n[1] * self.n[2] * self.cell_volume
+        self.pbc = tuple(pbc)
 
     def __str__(self):
-        str_dx = ["%g" % dx if isinstance(dx, (float, int)) else "XX" for dx in self.dx]
+        str_dx = ["%g" % dx if isinstance(dx, (int,float)) else "XX" for dx in self.dx]
         return "%dx%dx%d (size= %s x %s x %s)" % (*self.n, *str_dx)
```

### Comparing `magnumnp-1.0.9/magnumnp/common/state.py` & `magnumnp-1.1.0/magnumnp/common/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 import torch
 import os
+import subprocess
 import numpy as np
 from magnumnp.common import logging, DecoratedTensor, Material
 from magnumnp.common.io import write_vti, write_vtr
 
 __all__ = ["State"]
 
 complex_dtype = {
@@ -29,30 +30,31 @@
     torch.float32: torch.complex64,
     torch.float64: torch.complex128
     }
 
 class State(object):
     def __init__(self, mesh, t0 = 0., device = None, dtype = None):
         if device == None:
-            CUDA_DEVICE = os.environ.get('CUDA_DEVICE', '0')
-            self._device = torch.device(f"cuda:{CUDA_DEVICE}" if torch.cuda.is_available() else "cpu")
+            device_id = os.environ.get('CUDA_DEVICE')
+            if device_id == None:
+                device_id = get_gpu_with_least_memory()
+            self._device = torch.device(f"cuda:{device_id}" if int(device_id) >= 0 else "cpu")
         else:
             self._device = device
 
         #TODO: add scale parameter to fix paraview issue, and use characteristic length scales
-
         self._dtype = dtype or torch.get_default_dtype()
         self.mesh = mesh
 
         self._is_equidistant = all([isinstance(dx, (float, int)) for dx in mesh.dx])
         self.dx = [self._tensor(dx).expand(n) for n, dx in zip(mesh.n, mesh.dx)] # use state.dx when a torch.tensor is needed
 
         # compute cell_volumes (use expand for equidistant dimentions)
         dx, dy, dz = torch.meshgrid([self._tensor(dx) for dx in mesh.dx], indexing = "ij")
-        self._cell_volumes = (dx*dy*dz).expand(mesh.n)
+        self._cell_volumes = (dx*dy*dz).expand(mesh.n).unsqueeze(-1)
 
         self._material = Material(self)
         self.t = t0
 
         dtype_str = str(self._dtype).split('.')[1]
         logging.info_green("[State] running on device: %s (dtype = %s)" % (self._device, dtype_str))
         logging.info_green("[Mesh] %s" % mesh)
@@ -74,56 +76,59 @@
         if isinstance(values, dict):
             self._material = Material(self)
             for key, value in values.items():
                 self._material[key] = value
         else:
             raise ValueError("Dictionary needs to be provided to set material")
 
-    def _zeros(self, size, dtype = None, **kwargs):
+    def zeros(self, size, dtype = None, **kwargs):
         dtype = dtype or self._dtype
         return torch.zeros(size, dtype=dtype, device=self._device, **kwargs)
 
-    def _arange(self, start, end = None, step=1, dtype = None, **kwargs):
+    def arange(self, start, end = None, step=1, dtype = None, **kwargs):
         dtype = dtype or self._dtype
         if end == None:
            end = start
            start = 0
         return torch.arange(start, end, step, dtype=dtype, device=self._device, **kwargs)
 
-    def _linspace(self, start, end, steps, dtype = None, **kwargs):
+    def linspace(self, start, end, steps, dtype = None, **kwargs):
         dtype = dtype or self._dtype
         return torch.linspace(start, end, steps, dtype=dtype, device=self._device, **kwargs)
 
     # _tensor for internal use only
     def _tensor(self, data, dtype = None):
         dtype = dtype or self._dtype
         if isinstance(data, torch.Tensor):
             return data.to(dtype=dtype, device=self._device)
         else:
             return torch.tensor(data, dtype=dtype, device=self._device)
 
     # TODO: avoid unneeded DecoratedTensors (e.g. state.Tensor(0.))
     def Tensor(self, data, dtype = None, requires_grad = False):
+        dtype = dtype or self._dtype
+        if isinstance(data, DecoratedTensor) and data.dtype == dtype:
+            return data
+
         if isinstance(data, list) or isinstance(data, tuple) or isinstance(data, float) or isinstance(data, int) or isinstance(data, np.ndarray):
-            dtype = dtype or self._dtype
             t = DecoratedTensor(torch.tensor(data, dtype=dtype, device=self._device), self.cell_volumes)
             t.requires_grad = requires_grad
             return t
         elif isinstance(data, torch.Tensor):
             requires_grad = requires_grad or data.requires_grad
             return DecoratedTensor(data.requires_grad_(requires_grad), self.cell_volumes)
         elif callable(data):
             return lambda t: self.Tensor(data(t))
         else:
             raise TypeError("Unknown data of type '%s' (needs to be 'list', 'tuple', 'torch.Tensor', or 'function')!" % type(data))
 
     def Constant(self, c, dtype = None, requires_grad = False):
         dtype = dtype or self._dtype
         c = self.Tensor(c, dtype=dtype)
-        x = DecoratedTensor(self._zeros(self.mesh.n + c.shape, dtype=dtype), self.cell_volumes)
+        x = DecoratedTensor(self.zeros(self.mesh.n + c.shape, dtype=dtype), self.cell_volumes)
         x[...] = c
         x.requires_grad = requires_grad
         return x
 
     def SpatialCoordinate(self):
         x = self.dx[0].cumsum(0) - self.dx[0]/2. + self.mesh.origin[0]
         y = self.dx[1].cumsum(0) - self.dx[1]/2. + self.mesh.origin[1]
@@ -137,15 +142,15 @@
         value = self.Tensor(value)
         if len(value.shape) == 0: # convert dim=0 tensor into dim=1 tensor
             value = value.reshape(1)
         if len(value.shape) < 3: # expand homogeneous material to [nx,ny,nz,...] tensor-field
             shape = value.shape
             value = value.reshape((1,1,1) + tuple(shape))
             value = value.expand(self.mesh.n + tuple(shape))
-            value = value.clone() # need to clone here, since otherwise inplace modification of a single item will affect the whole tensor
+            value._expanded = True # annotate expanded tensor (clone will be before individual items are modified)
         elif len(value.shape) == 3: # scalar-field should have dimension [nx,ny,nz,1]
             value = value.unsqueeze(-1)
         else: # otherwise assume the dimention is correct!
             pass
         return value
 
     def write_vtk(self, fields, filename):
@@ -161,7 +166,26 @@
     @property
     def complex_dtype(self):
         return complex_dtype[self._dtype]
 
     @property
     def cell_volumes(self):
         return self._cell_volumes
+
+
+
+def get_gpu_with_least_memory():
+    if not torch.cuda.is_available():
+        return -1
+
+    import pynvml
+    pynvml.nvmlInit()
+    num_gpus = pynvml.nvmlDeviceGetCount()
+
+    gpu_memory = []
+    for i in range(num_gpus):
+        handle = pynvml.nvmlDeviceGetHandleByIndex(i)
+        mem_info = pynvml.nvmlDeviceGetMemoryInfo(handle)
+        gpu_memory.append(mem_info.used)
+
+    pynvml.nvmlShutdown()
+    return gpu_memory.index(min(gpu_memory))
```

### Comparing `magnumnp-1.0.9/magnumnp/common/tabulate.py` & `magnumnp-1.1.0/magnumnp/common/tabulate.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/common/time_interpolator.py` & `magnumnp-1.1.0/magnumnp/common/time_interpolator.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import torch
 from scipy import interpolate
 
 __all__ = ["TimeInterpolator"]
 
 class TimeInterpolator(object):
     def __init__(self, state, points):
-        self._tp = state.Tensor(list(points.keys()))
+        self._tp = state._tensor(list(points.keys()))
         self._fp = state._tensor(list(points.values()))
         self._state = state
 
     def __call__(self, t):
         i = torch.searchsorted(self._tp, t) # upper index
         i = torch.clamp(i, min=1, max=len(self._tp)-1) # extrapolate on bounds
         tp = self._tp
```

### Comparing `magnumnp-1.0.9/magnumnp/common/timer.py` & `magnumnp-1.1.0/magnumnp/common/timer.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/field_terms/__init__.py` & `magnumnp-1.1.0/magnumnp/field_terms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,24 @@
 
 from magnumnp.field_terms.anisotropy import *
 from magnumnp.field_terms.demag import *
 from magnumnp.field_terms.demag_nonequidistant import *
 from magnumnp.field_terms.demagPBC import *
 from magnumnp.field_terms.dmi import *
 from magnumnp.field_terms.exchange import *
-from magnumnp.field_terms.exchangePBC import *
 from magnumnp.field_terms.external import *
 from magnumnp.field_terms.field_terms import *
 from magnumnp.field_terms.oersted import *
 from magnumnp.field_terms.rkky import *
 from magnumnp.field_terms.spintorque import *
 
 __all__ = (anisotropy.__all__ +
            demag.__all__ +
            demag_nonequidistant.__all__ +
            demagPBC.__all__ +
            dmi.__all__ +
            exchange.__all__ +
-           exchangePBC.__all__ +
            external.__all__ +
            field_terms.__all__ +
            oersted.__all__ +
            rkky.__all__ +
            spintorque.__all__)
```

### Comparing `magnumnp-1.0.9/magnumnp/field_terms/anisotropy.py` & `magnumnp-1.1.0/magnumnp/field_terms/anisotropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,9 +108,9 @@
         h = torch.einsum('...a, ...ba-> ...b', h, R) # matmult transpose
         return torch.nan_to_num(-1./constants.mu_0/state.material["Ms"] * h, posinf=0, neginf=0)
 
     def E(self, state):
         R = self._R(state)
         mx, my, mz = torch.einsum('...a, ...ab-> ...b', state.m, R).unbind(dim=-1) # matmult
 
-        return (state.material[self.Kc1] * (mx**2 * my**2 + mx**2 * mz**2 + my**2 * mz**2).sum() +
-                state.material[self.Kc2] * (mx**2 * my**2 * mz**2).sum()) * state.mesh.cell_volume
+        return ((state.material[self.Kc1] * (mx**2 * my**2 + mx**2 * mz**2 + my**2 * mz**2) +
+                 state.material[self.Kc2] * (mx**2 * my**2 * mz**2)) * state.cell_volumes).sum()
```

### Comparing `magnumnp-1.0.9/magnumnp/field_terms/demagPBC.py` & `magnumnp-1.1.0/magnumnp/field_terms/demagPBC.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,28 +13,29 @@
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 from magnumnp.common import timedmethod, constants
+from .field_terms import LinearFieldTerm
 from math import pi
 import torch
 
 __all__ = ["DemagFieldPBC"]
 
-class DemagFieldPBC(object):
+class DemagFieldPBC(LinearFieldTerm):
     @timedmethod
     def h(self, state):
         m_fft = torch.fft.fftn(state.material["Ms"] * state.m, dim = [i for i in range(3) if state.mesh.n[i] > 1]).squeeze(-1) #TODO: use rfftn -> kz should be size N//2+1
         dx, dy, dz = state.mesh.dx
 
-        kx = (2. * pi * state._arange(state.mesh.n[0]) / state.mesh.n[0]).reshape(-1,1,1)
-        ky = (2. * pi * state._arange(state.mesh.n[1]) / state.mesh.n[1]).reshape(1,-1,1)
-        kz = (2. * pi * state._arange(state.mesh.n[2]) / state.mesh.n[2]).reshape(1,1,-1)
+        kx = (2. * pi * state.arange(state.mesh.n[0]) / state.mesh.n[0]).reshape(-1,1,1)
+        ky = (2. * pi * state.arange(state.mesh.n[1]) / state.mesh.n[1]).reshape(1,-1,1)
+        kz = (2. * pi * state.arange(state.mesh.n[2]) / state.mesh.n[2]).reshape(1,1,-1)
 
         div_fft = (1.-torch.exp(-1j*kx)) * m_fft[:,:,:,0] / dx \
                 + (1.-torch.exp(-1j*ky)) * m_fft[:,:,:,1] / dy \
                 + (1.-torch.exp(-1j*kz)) * m_fft[:,:,:,2] / dz
 
         u_fft = -div_fft / (4./dx**2*torch.sin(kx/2.)**2 + \
                             4./dy**2*torch.sin(ky/2.)**2 + \
@@ -44,10 +45,7 @@
         h_fft = torch.empty_like(m_fft)
         h_fft[:,:,:,0] = (1.-torch.exp(1j*kx)) * u_fft / dx
         h_fft[:,:,:,1] = (1.-torch.exp(1j*ky)) * u_fft / dy
         h_fft[:,:,:,2] = (1.-torch.exp(1j*kz)) * u_fft / dz
 
         h = torch.fft.ifftn(h_fft, dim = [i for i in range(3) if state.mesh.n[i] > 1])
         return h.real
-
-    def E(self, state):
-        return - 0.5 * constants.mu_0 * state.mesh.cell_volume * torch.sum(state.material["Ms"] * state.m * self.h(state))
```

### Comparing `magnumnp-1.0.9/magnumnp/field_terms/demag_nonequidistant.py` & `magnumnp-1.1.0/magnumnp/field_terms/oersted.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,132 +12,141 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
-from magnumnp.common import logging, timedmethod, constants, Timer
-from .field_terms import LinearFieldTerm
-from . import newell_f, newell_g, dipole_f, dipole_g, newell_N
+from magnumnp.common import logging, timedmethod, constants
+from .field_terms import FieldTerm
 import numpy as np
 import torch
-from time import time
+import torch.fft
+from torch import asinh, atan, sqrt, log, abs
 import os
+from time import time
 
-__all__ = ["DemagFieldNonEquidistant"]
+__all__ = ["OerstedField"]
 
-class DemagFieldNonEquidistant(LinearFieldTerm):
-    r"""
-    Demagneti_dstation Field:
+def krueger_g(points):
+    x = points[:,:,:,0]
+    y = points[:,:,:,1]
+    z = points[:,:,:,2]
+
+    R = sqrt(x**2 + y**2 + z**2)
+
+    res = (3.*x**2 + 3.*y**2 - 2.*z**2)*z*R/24.
+    res += np.pi*z/4.*abs(x*y*z)
+
+    mask = (x**2 + y**2).gt(0)
+    res[mask] += ((x**4 - 6.*x**2*y**2 + y**4)/24. * log(z+R))[mask]
+
+    mask = (y**2).gt(0)
+    res[mask] += (x*y/6. * (y**2 - 3.*z**2) * atan(x*z/(y*R)))[mask]
+
+    mask = (x**2).gt(0)
+    res[mask] += (x*y/6. * (x**2 - 3.*z**2) * atan(y*z/(x*R)))[mask]
+
+    mask = (y**2+z**2).gt(0)
+    res[mask] += (z/6. * x * (z**2 - 3.*y**2) * log(x+R))[mask]
+
+    mask = (x**2+z**2).gt(0)
+    res[mask] += (z/6. * y * (z**2 - 3.*x**2) * log(y+R))[mask]
+
+    return res
 
-    The dipole-dipole interaction gives rise to a long-range interaction.
-    The integral formulation of the corresponding Maxwell equations can
-    be represented as convolution of the magneti_dstation :math:`\vec{M} = M_s \; \vec{m}` with a proper
-    demagneti_dstation kernel :math:`\vec{N}`
+
+def dipole_g(points):
+    x = points[:,:,:,0]
+    y = points[:,:,:,1]
+    z = points[:,:,:,2]
+
+    R = sqrt(x**2 + y**2 + z**2)
+    res = -z/R**3
+    res[0,0,0] = 0.
+    return res
+
+
+class OerstedField(FieldTerm):
+    r"""
+    The Oersted field created by some current density :math:`\vec{j}` can be calculated by means of the Biot-Savart law
 
     .. math::
-        \vec{h}^\text{dem}_{\vec{i}} = \sum\limits_{\vec{j}} \vec{N}_{\vec{i} - \vec{j}} \, \vec{M}_{\vec{j}},
 
-    The convolution can be evaluated efficiently using an FFT method.
+        \vec{h}^\text{oersted}(\vec{x}) = \frac{1}{4 \pi} \int \vec{j}(\vec{x}') \times \frac{\vec{x}-\vec{x}'}{\vert \vec{x}-\vec{x}'\vert^3} \, d\vec{x}'.
+
+    The occuring equations look very similar to those of the demag field [krueger], and the occuring convolution can be efficiently calculated by means of an FFT method.
 
-    :param p: number of next neighbors for near field via Newell's equation (default = 20)
+    :param p: number of next neighbors for near field via Krueger's equations (default = 20)
     :type p: int, optional
     """
     def __init__(self, p = 20):
         self._p = p
 
-    def _init_N_component(self, state, i_dst, i_src, perm, func_near, func_far):
-        # rescale dx to avoid NaNs when using single precision
-        # TODO: add scale to state and rescale like in DemagField
-        dx = state.mesh.dx
-        z = (torch.cumsum(state.dx[2], dim=0) - state.dx[2][0])
-        dx_dst = state._tensor([[dx[0], dx[1], state.dx[2][i_dst]][ind] for ind in perm])
-        dx_src = state._tensor([[dx[0], dx[1], state.dx[2][i_src]][ind] for ind in perm])
-
+    def _init_K_component(self, state, perm, func_near, func_far):
         # dipole far-field
-        shape = [1 if n==1 else 2*n for n in state.mesh.n[:2] + (1,)]
-
-        ij = [torch.fft.fftshift(state._arange(n)) - n//2 for n in shape]
+        shape = [1 if n==1 else 2*n for n in state.mesh.n]
+        ij = [torch.fft.fftshift(state.arange(n)) - n//2 for n in shape]
         ij = torch.meshgrid(*ij,indexing='ij')
 
-        xyz = [[ij[0]*dx[0], ij[1]*dx[1], ij[2]*0. + z[i_dst]+state.dx[2][i_dst]/2. - (z[i_src]+state.dx[2][i_src]/2.)][ind] for ind in perm] # diff of cell centers
-        Nc = func_far(*xyz) * torch.prod(dx_src) / (4.*torch.pi)
+        r = torch.stack([ij[ind]*state.mesh.dx[ind] for ind in perm], dim=-1)
+        Kc = func_far(r) * np.prod(state.mesh.dx) / (4.*np.pi)
 
         # newell near-field
         n_near = np.minimum(state.mesh.n, self._p)
-        n_near[2] = 1
-        shape = [1 if n==1 else 2*n for n in n_near]
-        N_near = state._zeros(shape)
-        ij = [torch.fft.fftshift(state._arange(n)) - n//2 for n in shape]
+        K_near = state.zeros([1 if i==1 else 2*i for i in n_near])
+        ij = [torch.fft.fftshift(state.arange(n)) - n//2 for n in K_near.shape[:3]]
         ij = torch.meshgrid(*ij,indexing='ij')
 
-        xyz = [[ij[0]*dx[0], ij[1]*dx[1], z[i_dst] - z[i_src]][ind] for ind in perm] # diff of cell centers origins
-
-        N_near = -newell_N(func_near, *xyz, *dx_dst, *dx_src) / (4.*torch.pi*torch.prod(dx_dst))
+        for k in np.rollaxis(np.indices((3,)*3), 0, 4).reshape(27, -1) - 1:
+            r = torch.stack([(ij[ind] + k[ind])*state.mesh.dx[ind] for ind in perm], dim=-1)
+            K_near[:,:,:] += np.prod(2.-3*np.abs(k)) * func_near(r) / (4.*np.pi*np.prod(state.mesh.dx))
+
+        Kc[:n_near[0]   ,:n_near[1]   ,:n_near[2]   ] = K_near[:n_near[0]   ,:n_near[1]   ,:n_near[2]   ]
+        Kc[:n_near[0]   ,:n_near[1]   ,-n_near[2]+1:] = K_near[:n_near[0]   ,:n_near[1]   ,-n_near[2]+1:]
+        Kc[:n_near[0]   ,-n_near[1]+1:,:n_near[2]   ] = K_near[:n_near[0]   ,-n_near[1]+1:,:n_near[2]   ]
+        Kc[:n_near[0]   ,-n_near[1]+1:,-n_near[2]+1:] = K_near[:n_near[0]   ,-n_near[1]+1:,-n_near[2]+1:]
+        Kc[-n_near[0]+1:,:n_near[1]   ,:n_near[2]   ] = K_near[-n_near[0]+1:,:n_near[1]   ,:n_near[2]   ]
+        Kc[-n_near[0]+1:,:n_near[1]   ,-n_near[2]+1:] = K_near[-n_near[0]+1:,:n_near[1]   ,-n_near[2]+1:]
+        Kc[-n_near[0]+1:,-n_near[1]+1:,:n_near[2]   ] = K_near[-n_near[0]+1:,-n_near[1]+1:,:n_near[2]   ]
+        Kc[-n_near[0]+1:,-n_near[1]+1:,-n_near[2]+1:] = K_near[-n_near[0]+1:,-n_near[1]+1:,-n_near[2]+1:]
 
-        Nc[:n_near[0]   ,:n_near[1]   ,:n_near[2]   ] = N_near[:n_near[0]   ,:n_near[1]   ,:n_near[2]   ]
-        Nc[:n_near[0]   ,:n_near[1]   ,-n_near[2]+1:] = N_near[:n_near[0]   ,:n_near[1]   ,-n_near[2]+1:]
-        Nc[:n_near[0]   ,-n_near[1]+1:,:n_near[2]   ] = N_near[:n_near[0]   ,-n_near[1]+1:,:n_near[2]   ]
-        Nc[:n_near[0]   ,-n_near[1]+1:,-n_near[2]+1:] = N_near[:n_near[0]   ,-n_near[1]+1:,-n_near[2]+1:]
-        Nc[-n_near[0]+1:,:n_near[1]   ,:n_near[2]   ] = N_near[-n_near[0]+1:,:n_near[1]   ,:n_near[2]   ]
-        Nc[-n_near[0]+1:,:n_near[1]   ,-n_near[2]+1:] = N_near[-n_near[0]+1:,:n_near[1]   ,-n_near[2]+1:]
-        Nc[-n_near[0]+1:,-n_near[1]+1:,:n_near[2]   ] = N_near[-n_near[0]+1:,-n_near[1]+1:,:n_near[2]   ]
-        Nc[-n_near[0]+1:,-n_near[1]+1:,-n_near[2]+1:] = N_near[-n_near[0]+1:,-n_near[1]+1:,-n_near[2]+1:]
-
-        Nc = torch.fft.rfftn(Nc, dim = [i for i in range(2) if state.mesh.n[i] > 1])#.real#.clone()
-        return Nc
-
-    def _init_N(self, state):
-        if isinstance(state.mesh.dx[2], float):
-            logging.warning("mesh.dx[2] should not be constant when using DemagFieldNonEquidistant! Use the equidistant DemagField otherwise!")
-        if not all([isinstance(dx, float) for dx in state.mesh.dx[:2]]):
-            raise ValueError("Demag field only implemented for non-equidistant z-spacings. mesh.dx[0] and mesh.dx[1] need to be constant!")
+        return torch.fft.rfftn(Kc, dim = [i for i in range(3) if state.mesh.n[i] > 1])#.real.clone()
 
+    def _init_K(self, state):
         dtype = state._dtype
         state._dtype = torch.float64 # always use double precision
-
         time_kernel = time()
-        self._N = [None]*state.mesh.n[2]
-        for i_dst in range(state.mesh.n[2]):
-            self._N[i_dst] = [None]*state.mesh.n[2]
-            for i_src in range(i_dst+1):
-                Nxx = self._init_N_component(state, i_dst, i_src, [0,1,2], newell_f, dipole_f)
-                Nxy = self._init_N_component(state, i_dst, i_src, [0,1,2], newell_g, dipole_g)
-                Nxz = self._init_N_component(state, i_dst, i_src, [0,2,1], newell_g, dipole_g)
-                Nyy = self._init_N_component(state, i_dst, i_src, [1,2,0], newell_f, dipole_f)
-                Nyz = self._init_N_component(state, i_dst, i_src, [1,2,0], newell_g, dipole_g)
-                Nzz = self._init_N_component(state, i_dst, i_src, [2,0,1], newell_f, dipole_f)
-
-                self._N[i_dst][i_src] = [[ Nxx,  Nxy,  Nxz],
-                                         [ Nxy,  Nyy,  Nyz],
-                                         [ Nxz,  Nyz,  Nzz]]
-                self._N[i_src][i_dst] = [[ Nxx,  Nxy, -Nxz],
-                                         [ Nxy,  Nyy, -Nyz],
-                                         [-Nxz, -Nyz,  Nzz]]
-        logging.info(f"[DEMAG]: Time calculation of demag kernel = {time() - time_kernel} s")
+        Kxy = self._init_K_component(state, [0,1,2], krueger_g, dipole_g).to(dtype=dtype)
+        Kyz = self._init_K_component(state, [1,2,0], krueger_g, dipole_g).to(dtype=dtype)
+        Kxz = self._init_K_component(state, [2,0,1], krueger_g, dipole_g).to(dtype=dtype)
+
+        self._K = [[  0., -Kxy, +Kxz],
+                   [+Kxy,   0., -Kyz],
+                   [-Kxz, +Kyz,   0.]]
+
+        logging.info(f"[OERSTED]: Time calculation of oersted kernel = {time() - time_kernel} s")
         state._dtype = dtype # restore dtype
 
     @timedmethod
     def h(self, state):
-        if not hasattr(self, "_N"):
-            self._init_N(state)
+        if not hasattr(self, "_K"):
+            self._init_K(state)
 
-        m_pad_fft = torch.fft.rfftn(state.material["Ms"] * state.m, dim = [i for i in range(2) if state.mesh.n[i] > 1], s = [2*state.mesh.n[i] for i in range(2) if state.mesh.n[i] > 1])
-        hx = state._zeros(m_pad_fft.shape[:-1], dtype=state.complex_dtype)
-        hy = state._zeros(m_pad_fft.shape[:-1], dtype=state.complex_dtype)
-        hz = state._zeros(m_pad_fft.shape[:-1], dtype=state.complex_dtype)
-
-        for i_dst in range(state.mesh.n[2]):
-            for i_src in range(state.mesh.n[2]):
-                for ax in range(3):
-                    hx[:,:,i_src] += self._N[i_src][i_dst][0][ax][:,:,0]*m_pad_fft[:,:,i_dst,ax]
-                    hy[:,:,i_src] += self._N[i_src][i_dst][1][ax][:,:,0]*m_pad_fft[:,:,i_dst,ax]
-                    hz[:,:,i_src] += self._N[i_src][i_dst][2][ax][:,:,0]*m_pad_fft[:,:,i_dst,ax]
-
-        hx = torch.fft.irfftn(hx, dim = [i for i in range(2) if state.mesh.n[i] > 1])
-        hy = torch.fft.irfftn(hy, dim = [i for i in range(2) if state.mesh.n[i] > 1])
-        hz = torch.fft.irfftn(hz, dim = [i for i in range(2) if state.mesh.n[i] > 1])
+        hx = state.zeros(list(self._K[0][1].shape), dtype=state.complex_dtype)
+        hy = state.zeros(list(self._K[0][1].shape), dtype=state.complex_dtype)
+        hz = state.zeros(list(self._K[0][1].shape), dtype=state.complex_dtype)
+
+        for ax in range(3):
+            j_pad_fft1D = torch.fft.rfftn(state.j[:,:,:,ax], dim = [i for i in range(3) if state.mesh.n[i] > 1], s = [2*state.mesh.n[i] for i in range(3) if state.mesh.n[i] > 1])
+
+            hx += self._K[0][ax] * j_pad_fft1D
+            hy += self._K[1][ax] * j_pad_fft1D
+            hz += self._K[2][ax] * j_pad_fft1D
+
+        hx = torch.fft.irfftn(hx, dim = [i for i in range(3) if state.mesh.n[i] > 1])
+        hy = torch.fft.irfftn(hy, dim = [i for i in range(3) if state.mesh.n[i] > 1])
+        hz = torch.fft.irfftn(hz, dim = [i for i in range(3) if state.mesh.n[i] > 1])
 
         return torch.stack([hx[:state.mesh.n[0],:state.mesh.n[1],:state.mesh.n[2]],
                             hy[:state.mesh.n[0],:state.mesh.n[1],:state.mesh.n[2]],
                             hz[:state.mesh.n[0],:state.mesh.n[1],:state.mesh.n[2]]], dim=3)
```

### Comparing `magnumnp-1.0.9/magnumnp/field_terms/dmi.py` & `magnumnp-1.1.0/magnumnp/field_terms/dmi.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from magnumnp.common import timedmethod, constants
 import torch
 from .field_terms import LinearFieldTerm
 import numpy as np
 
 __all__ = ["DMIField", "InterfaceDMIField", "BulkDMIField", "D2dDMIField"]
 
+
 class DMIField(LinearFieldTerm):
     r"""
     General Dzyaloshinskii-Moriya interaction
 
     The general expression for the DMI field can be expressed as
 
     .. math::
@@ -55,42 +56,75 @@
         Ms = state.material["Ms"].torch_tensor
         m = state.m.torch_tensor
         h = self._h(m, D, Ms, state)
         return state.Tensor(h)
 
     @torch.compile
     def _h(self, m, D, Ms, state):
-        h = state._zeros(state.mesh.n + (3,))
+        h = state.zeros(state.mesh.n + (3,))
         # x
-        v = state._tensor(self._dmi_vector[0]).expand(m[1:,:,:].shape)
-        D_avg = torch.where(D[1:,:,:]*D[:-1,:,:] < 0,
-                            torch.sqrt(torch.sqrt(-D[1:,:,:]*D[:-1,:,:])*torch.abs(D[1:,:,:]+D[:-1,:,:]) / 2.), # TODO: is sign missing?
-                            2.*D[1:,:,:]*D[:-1,:,:]/(D[1:,:,:]+D[:-1,:,:]))
-        h[:-1,:,:] += D_avg * torch.linalg.cross(v, m[ 1:,:,:]) / (2.*state.mesh.dx[0])
-        h[ 1:,:,:] -= D_avg * torch.linalg.cross(v, m[:-1,:,:]) / (2.*state.mesh.dx[0])
+        if state.mesh.pbc[0] == 0:
+            v = state._tensor(self._dmi_vector[0]).expand(m[1:,:,:].shape)
+            D_avg = torch.where(D[1:,:,:]*D[:-1,:,:] < 0,
+                                torch.sqrt(torch.sqrt(-D[1:,:,:]*D[:-1,:,:])*torch.abs(D[1:,:,:]+D[:-1,:,:]) / 2.), # TODO: is sign missing?
+                                2.*D[1:,:,:]*D[:-1,:,:] / (D[1:,:,:]+D[:-1,:,:]))
+            h[:-1,:,:] += D_avg * torch.linalg.cross(v, m[ 1:,:,:]) / (2.*state.mesh.dx[0])
+            h[ 1:,:,:] -= D_avg * torch.linalg.cross(v, m[:-1,:,:]) / (2.*state.mesh.dx[0])
+        else:
+            v = state._tensor(self._dmi_vector[0]).expand(m.shape)
+            D_next = torch.roll(D, +1, dims=0)
+            D_avg = torch.where(D_next*D < 0,
+                                torch.sqrt(torch.sqrt(-D_next*D)*torch.abs(D_next+D) / 2.), # TODO: is sign missing?
+                                2.*D_next*D / (D_next+D))
+            h += D_avg * torch.linalg.cross(v, torch.roll(state.m, +1, dims=0)) / (2.*state.mesh.dx[0])
+
+            D_avg = torch.roll(D_avg, -1, dims=0)
+            h += D_avg * torch.linalg.cross(v, torch.roll(state.m, -1, dims=0)) / (2.*state.mesh.dx[0])
 
         # y
-        v = state._tensor(self._dmi_vector[1]).expand(m[:,1:,:].shape)
-        D_avg = torch.where(D[:,1:,:]*D[:,:-1,:] < 0,
-                            torch.sqrt(torch.sqrt(-D[:,1:,:]*D[:,:-1,:])*torch.abs(D[:,1:,:]+D[:,:-1,:]) / 2.),
-                            2.*D[:,1:,:]*D[:,:-1,:]/(D[:,1:,:]+D[:,:-1,:]))
-        h[:,:-1,:] += D_avg * torch.linalg.cross(v, m[:, 1:,:]) / (2.*state.mesh.dx[1])
-        h[:, 1:,:] -= D_avg * torch.linalg.cross(v, m[:,:-1,:]) / (2.*state.mesh.dx[1])
+        if state.mesh.pbc[1] == 0:
+            v = state._tensor(self._dmi_vector[1]).expand(m[:,1:,:].shape)
+            D_avg = torch.where(D[:,1:,:]*D[:,:-1,:] < 0,
+                                torch.sqrt(torch.sqrt(-D[:,1:,:]*D[:,:-1,:])*torch.abs(D[:,1:,:]+D[:,:-1,:]) / 2.),
+                                2.*D[:,1:,:]*D[:,:-1,:] / (D[:,1:,:]+D[:,:-1,:]))
+            h[:,:-1,:] += D_avg * torch.linalg.cross(v, m[:, 1:,:]) / (2.*state.mesh.dx[1])
+            h[:, 1:,:] -= D_avg * torch.linalg.cross(v, m[:,:-1,:]) / (2.*state.mesh.dx[1])
+        else:
+            v = state._tensor(self._dmi_vector[1]).expand(m.shape)
+            D_next = torch.roll(D, +1, dims=1)
+            D_avg = torch.where(D_next*D < 0,
+                                torch.sqrt(torch.sqrt(-D_next*D)*torch.abs(D_next+D) / 2.), # TODO: is sign missing?
+                                2.*D_next*D / (D_next+D))
+            h += D_avg * torch.linalg.cross(v, torch.roll(state.m, +1, dims=1)) / (2.*state.mesh.dx[1])
+
+            D_avg = torch.roll(D_avg, -1, dims=1)
+            h += D_avg * torch.linalg.cross(v, torch.roll(state.m, -1, dims=1)) / (2.*state.mesh.dx[1])
 
         # z
-        v = state._tensor(self._dmi_vector[2]).expand(m[:,:,1:].shape)
-        D_avg = torch.where(D[:,:,1:]*D[:,:,:-1] < 0,
-                            torch.sqrt(torch.sqrt(-D[:,:,1:]*D[:,:,:-1])*torch.abs(D[:,:,1:]+D[:,:,:-1]) / 2.),
-                            2.*D[:,:,1:]*D[:,:,:-1]/(D[:,:,1:]+D[:,:,:-1]))
-        h[:,:,:-1] += D_avg * torch.linalg.cross(v, m[:,:, 1:]) / (2.*state.mesh.dx[2])
-        h[:,:, 1:] -= D_avg * torch.linalg.cross(v, m[:,:,:-1]) / (2.*state.mesh.dx[2])
+        if state.mesh.pbc[2] == 0:
+            v = state._tensor(self._dmi_vector[2]).expand(m[:,:,1:].shape)
+            D_avg = torch.where(D[:,:,1:]*D[:,:,:-1] < 0,
+                                torch.sqrt(torch.sqrt(-D[:,:,1:]*D[:,:,:-1])*torch.abs(D[:,:,1:]+D[:,:,:-1]) / 2.),
+                                2.*D[:,:,1:]*D[:,:,:-1] / (D[:,:,1:]+D[:,:,:-1]))
+            h[:,:,:-1] += D_avg * torch.linalg.cross(v, m[:,:, 1:]) / (2.*state.mesh.dx[2])
+            h[:,:, 1:] -= D_avg * torch.linalg.cross(v, m[:,:,:-1]) / (2.*state.mesh.dx[2])
+        else:
+            v = state._tensor(self._dmi_vector[2]).expand(m.shape)
+            D_next = torch.roll(D, +1, dims=2)
+            D_avg = torch.where(D_next*D < 0,
+                                torch.sqrt(torch.sqrt(-D_next*D)*torch.abs(D_next+D) / 2.), # TODO: is sign missing?
+                                2.*D_next*D / (D_next+D))
+            h += D_avg * torch.linalg.cross(v, torch.roll(state.m, +1, dims=2)) / (2.*state.mesh.dx[2])
+
+            D_avg = torch.roll(D_avg, -1, dims=2)
+            h += D_avg * torch.linalg.cross(v, torch.roll(state.m, -1, dims=2)) / (2.*state.mesh.dx[2])
 
         h *= 2. / (constants.mu_0 * Ms)
-        h = torch.nan_to_num(h, posinf=0, neginf=0)
-        return h
+        return h.nan_to_num(posinf=0, neginf=0)
+
 
 class InterfaceDMIField(DMIField):
     r"""
     Interface Dzyaloshinskii-Moriya interaction
 
     .. math::
         \vec{h}^\text{dmii}(\vec{x}) = -\frac{2 \, D_i}{\mu_0 \, M_s} \; \left[ \nabla \left(\vec{e}_z \cdot \vec{m} \right) - \left(\nabla \cdot \vec{m} \right) \, \vec{e}_z\right],
```

### Comparing `magnumnp-1.0.9/magnumnp/field_terms/exchangePBC.py` & `magnumnp-1.1.0/magnumnp/field_terms/external.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,41 +14,50 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 from magnumnp.common import timedmethod, constants
 import torch
-from .field_terms import LinearFieldTerm
 
-__all__ = ["ExchangeFieldPBC"]
+__all__ = ["ExternalField"]
 
-class ExchangeFieldPBC(LinearFieldTerm):
-    parameters = ["A"]
+class ExternalField(object):
+    r"""
+    External Field
 
-    def __init__(self, domain=None, **kwargs):
-        self._domain = domain
-        super().__init__(**kwargs)
+    :param h: External Field
+    :type h: list or tuple or :class:`Tensor` or function
+
+    :Examples:
+
+    .. code::
+
+        # homogenious, constant field
+        external = ExternalField([Hx, 0, 0])
+
+        # homogenious, time-dependent field
+        external = ExternalField(lambda t: [Hx*t, 0, 0])
+
+        # inhomogenious, constant field
+        x, y, z = SpatialCoordinate(state)
+        h = torch.stack([x,y,z], dim=-1)
+        external = ExternalField(h)
+    """
+    def __init__(self, h):
+        self._h = h
 
     @timedmethod
     def h(self, state):
-        h = state._zeros(state.mesh.n + (3,))
+        h = state.Tensor(self._h)(state.t)
+        if len(h.shape) == 1:
+            h = h.expand(state.m.shape)
+        return h
+
+    def __setattr__(self, name, value):
+        if name == "h":
+            self._h = value
+        else:
+            super().__setattr__(name, value)
 
-        A = state.material[self.A]
-        if self._domain != None:
-            A = A * self._domain[:,:,:,None]
-
-        for dim in range(3):
-            if isinstance(A, torch.Tensor) and A.dim() == 4: # TODO: A could be a 1D tensor instead of a 4D tensor field
-                A_next = torch.roll(A, +1, dim) # N
-                A_avg = 2.*A_next*A/(A_next+A)
-                h += A_avg * (torch.roll(state.m, +1, dim) - state.m) / state.mesh.dx[dim]**2 # m_i+1 - m_i
-
-                A_avg = torch.roll(A_avg, -1, dim)
-                h += A_avg * (torch.roll(state.m, -1, dim) - state.m) / state.mesh.dx[dim]**2 # m_i-1 - m_i
-            else:
-                h += A * (torch.roll(state.m, +1, dim) - state.m) / state.mesh.dx[dim]**2 # m_i+1 - m_i
-                h += A * (torch.roll(state.m, -1, dim) - state.m) / state.mesh.dx[dim]**2 # m_i-1 - m_i
-
-        h *= 2. / (constants.mu_0 * state.material["Ms"])
-        h = torch.nan_to_num(h, posinf=0, neginf=0)
-        return state.Tensor(h)
+    def E(self, state):
+        return - constants.mu_0 * torch.sum(state.material["Ms"] * state.m * self.h(state) * state.cell_volumes)
```

### Comparing `magnumnp-1.0.9/magnumnp/field_terms/field_terms.py` & `magnumnp-1.1.0/magnumnp/field_terms/field_terms.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,9 +30,10 @@
             raise Warning("Got unknown parameters '%s'. Ignoring!" % unknown_params)
         params = {key:key for key in self.parameters}
         params.update(kwargs)
         for key, value in params.items():
             setattr(self, key, value)
 
 class LinearFieldTerm(FieldTerm):
-    def E(self, state):
-        return -0.5 * constants.mu_0 * state.mesh.cell_volume * torch.sum(state.material["Ms"] * state.m * self.h(state))
+    def E(self, state, domain = Ellipsis):
+        E = -0.5 * constants.mu_0 * state.material["Ms"] * state.m * self.h(state) * state.cell_volumes
+        return E[domain].sum()
```

### Comparing `magnumnp-1.0.9/magnumnp/field_terms/rkky.py` & `magnumnp-1.1.0/magnumnp/field_terms/rkky.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self._dir = dir #TODO: dir is ignored
         self._id1 = min(id1,id2)
         self._id2 = max(id1,id2)
         self._order = order
 
     @timedmethod
     def h(self, state):
-        h = state._zeros(state.mesh.n + (3,))
+        h = state.zeros(state.mesh.n + (3,))
         if self._order == 0:
             m1 = state.m[:,:,(self._id1,),:]
             m2 = state.m[:,:,(self._id2,),:]
         elif self._order == 1:
             m1 = 1.5 * state.m[:,:,(self._id1,),:] - 0.5 * state.m[:,:,(self._id1-1,),:]
             m2 = 1.5 * state.m[:,:,(self._id2,),:] - 0.5 * state.m[:,:,(self._id2+1,),:]
         elif self._order == 2:
```

### Comparing `magnumnp-1.0.9/magnumnp/field_terms/spintorque.py` & `magnumnp-1.1.0/magnumnp/field_terms/spintorque.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/loggers/__init__.py` & `magnumnp-1.1.0/magnumnp/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/loggers/field_logger.py` & `magnumnp-1.1.0/magnumnp/loggers/field_logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/loggers/logger.py` & `magnumnp-1.1.0/magnumnp/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/loggers/scalar_logger.py` & `magnumnp-1.1.0/magnumnp/loggers/scalar_logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/solvers/__init__.py` & `magnumnp-1.1.0/magnumnp/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/solvers/llg.py` & `magnumnp-1.1.0/magnumnp/solvers/llg.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     def relax(self, state, maxiter = 500, rtol = 1e-6, dt = 1e-11):
         t0 = state.t
         E0 = self.E(state)
 
         for i in range(maxiter):
             self._solver.step(state, dt, alpha = 1.0, rtol = rtol, atol = rtol) #, no_precession = True) # no_precession requires more iterations for SP4 demo!?
 
+            # dm = f(state, t, m, alpha = 1.0)
+            # |dm|.max()
             E = self.E(state)
             dE = torch.abs((E - E0)/E)
             logging.info_blue("[LLG] relax: t=%g dE=%g E=%g" % (state.t-t0, dE, E))
             if dE < rtol:
                 break
             E0 = E
```

### Comparing `magnumnp-1.0.9/magnumnp/solvers/ode_solvers/__init__.py` & `magnumnp-1.1.0/magnumnp/solvers/ode_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/solvers/ode_solvers/rkf45.py` & `magnumnp-1.1.0/magnumnp/solvers/ode_solvers/rkf45.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/solvers/ode_solvers/scipy_ode.py` & `magnumnp-1.1.0/magnumnp/solvers/ode_solvers/scipy_ode.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         state.t = t
         state.m = state.Tensor(m.reshape(state.mesh.n + (3,), order = "F"))
         f = self._f(state, **llg_args)
         return f.detach().cpu().numpy().flatten(order = "F")
 
     def step(self, state, dt, rtol = None, atol = None, **llg_args):
         if not self._initialized:
-            m = state.m.numpy().reshape(-1, order = 'F')
+            m = state.m.detach().cpu().numpy().reshape(-1, order = 'F')
             self._solver.set_initial_value(m, state.t.item())
             self._initialized = True
 
         self._solver.set_f_params(state, llg_args)
 
         t1 = self._solver.t + dt
         m1 = self._solver.integrate(t1)
```

### Comparing `magnumnp-1.0.9/magnumnp/solvers/ode_solvers/scipy_odeint.py` & `magnumnp-1.1.0/magnumnp/solvers/ode_solvers/scipy_odeint.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,20 +37,20 @@
     def _f_wrapper(self, t, m, state, llg_args):
         state.t = t * 1e-9 # scale time by 1e9 to prevent underflow error
         state.m = state.Tensor(m.reshape(state.mesh.n + (3,), order = "F"))
         f = self._f(state, **llg_args) * 1e-9
         return f.detach().cpu().numpy().flatten(order = "F")
 
     def step(self, state, dt, rtol = None, atol = None, **llg_args):
-        m0 = state.m.numpy().reshape(-1, order = 'F')
+        m0 = state.m.detach().cpu().numpy().reshape(-1, order = 'F')
 
         t1 = state.t + dt
         m1 = odeint(self._f_wrapper,
                     m0,
-                    [state.t*1e9, t1*1e9],
+                    [(state.t*1e9).detach().cpu().numpy(), (t1*1e9).detach().cpu().numpy()],
                     args = (state, llg_args),
                     rtol = rtol or self._rtol,
                     atol = atol or self._atol,
                     tfirst = True)[1]
 
         state.m = state.Tensor(m1.reshape(state.mesh.n + (3,), order = "F"))
         state.t = t1
```

### Comparing `magnumnp-1.0.9/magnumnp/solvers/ode_solvers/torchdiffeq.py` & `magnumnp-1.1.0/magnumnp/solvers/ode_solvers/torchdiffeq.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/solvers/string.py` & `magnumnp-1.1.0/magnumnp/solvers/string.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
         x_source = [0.]
         for i in range(1, (len(images))):
             w = (((Epath[i] + Epath[i-1])/2. - Emin) / (Emax - Emin) + 1.)**self._omega
             dm = torch.linalg.norm(images[i] - images[i-1])
             x_source.append(w * dm + x_source[-1])
         x_source = state._tensor(x_source)
-        x_target = state._linspace(x_source[0], x_source[-1], self._num_images)
+        x_target = state.linspace(x_source[0], x_source[-1], self._num_images)
 
         # start interpolation
         try:
             target_data = Interp1D(x_source, source_data, method = self._interpolation)(x_target)
         except:
             target_data = Interp1D(x_source, source_data, 'linear')(x_target)
```

### Comparing `magnumnp-1.0.9/magnumnp/utils/__init__.py` & `magnumnp-1.1.0/magnumnp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/utils/imaging_tools.py` & `magnumnp-1.1.0/magnumnp/utils/imaging_tools.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.9/magnumnp/utils/misc.py` & `magnumnp-1.1.0/magnumnp/utils/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 import torch
 
-__all__ = ["add_noise", "nsk"]
+__all__ = ["add_noise", "nsk", "hsl_to_rgb"]
 
 def add_noise(x, dev = 1.0, mean = 0.0):
    if torch.is_tensor(x):
         x += torch.empty_like(x).normal_(mean = mean, std = dev)
         x.normalize()
 
 def nsk(state): # TODO: document and improve interface
     m = state.m.mean(axis=2)
     dxm = torch.stack(torch.gradient(m, spacing = state.mesh.dx[0], dim = 0), dim = -1).squeeze(-1)
     dym = torch.stack(torch.gradient(m, spacing = state.mesh.dx[1], dim = 1), dim = -1).squeeze(-1)
-    return 1./(4.*pi) * (m * torch.linalg.cross(dxm, dym)).sum() * state.mesh.dx[0] * state.mesh.dx[1]
+    return 1./(4.*torch.pi) * (m * torch.linalg.cross(dxm, dym)).sum() * state.mesh.dx[0] * state.mesh.dx[1]
 
 
 def hsl_to_rgb(h, s, l): # TODO: document and improve interface
     def hue_to_rgb(p, q, t):
         t = torch.where(t < 0, t + 1, t)
         t = torch.where(t > 1, t - 1, t)
         return torch.where(t < 1/6, p + (q - p) * 6 * t,
```

### Comparing `magnumnp-1.0.9/magnumnp.egg-info/PKG-INFO` & `magnumnp-1.1.0/magnumnp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: magnumnp
-Version: 1.0.9
+Version: 1.1.0
 Summary: magnum.np finite-difference package for the solution of micromagnetic problems
 Home-page: http://gitlab.com/magnum.np/magnum.np
 Author: Florian Bruckner
 Author-email: florian.bruckner@univie.ac.at
 Project-URL: Documentation, https://magnum.np.gitlab.io/magnum.np/
 Project-URL: Changelog, https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-magnum.np 1.0.9
+magnum.np 1.1.0
 ===============
 
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
@@ -34,21 +34,21 @@
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
 The following demos are also stored on Google Colab, where they can directly be run without any local installation:
 
-   * [RKKY](demos/rkky.ipynb) ([Colab] (https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
-   * [Softmagnetic Composite](demos/softmagnetic_composite.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
-   * [Spin Orbit Torque](demos/sot.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
-   * [Standard Problem #4](demos/sp4.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
-   * [Standard Problem #5](demos/sp5.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
-   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
-   * [Standard Problem FMR](demos/sp_FMR.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
+   * [RKKY](demos/rkky/run.ipynb) ([Colab](https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
+   * [Softmagnetic Composite](demos/softmagnetic_composite/run.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
+   * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
+   * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
+   * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
+   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
+   * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
 
 
 
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
```

### Comparing `magnumnp-1.0.9/magnumnp.egg-info/SOURCES.txt` & `magnumnp-1.1.0/magnumnp.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 magnumnp/field_terms/__init__.py
 magnumnp/field_terms/anisotropy.py
 magnumnp/field_terms/demag.py
 magnumnp/field_terms/demagPBC.py
 magnumnp/field_terms/demag_nonequidistant.py
 magnumnp/field_terms/dmi.py
 magnumnp/field_terms/exchange.py
-magnumnp/field_terms/exchangePBC.py
 magnumnp/field_terms/external.py
 magnumnp/field_terms/field_terms.py
 magnumnp/field_terms/oersted.py
 magnumnp/field_terms/rkky.py
 magnumnp/field_terms/spintorque.py
 magnumnp/loggers/__init__.py
 magnumnp/loggers/field_logger.py
```

### Comparing `magnumnp-1.0.9/setup.py` & `magnumnp-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,29 @@
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='magnumnp',
-      version='v1.0.9',
+      version='v1.1.0',
       description='magnum.np finite-difference package for the solution of micromagnetic problems',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Florian Bruckner',
       author_email='florian.bruckner@univie.ac.at',
       url='http://gitlab.com/magnum.np/magnum.np',
       project_urls = {'Documentation': 'https://magnum.np.gitlab.io/magnum.np/',
                       'Changelog': 'https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG'
       },
       packages=['magnumnp', 'magnumnp.common', 'magnumnp.field_terms', 'magnumnp.loggers', 'magnumnp.solvers', 'magnumnp.solvers.ode_solvers', 'magnumnp.utils'],
       install_requires = [
-            'torch',
             'numpy',
+            'pynvml',
+            'pyvista',
             'scipy',
             'setproctitle',
-            'pyvista',
+            'torch',
+            'torchdiffeq',
             'xitorch',
-            'torchdiffeq'
             ]
      )
```

