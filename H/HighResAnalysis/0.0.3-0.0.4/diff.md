# Comparing `tmp/HighResAnalysis-0.0.3.tar.gz` & `tmp/HighResAnalysis-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HighResAnalysis-0.0.3.tar", last modified: Mon May 22 12:51:03 2023, max compression
+gzip compressed data, was "HighResAnalysis-0.0.4.tar", last modified: Wed May 24 08:54:01 2023, max compression
```

## Comparing `HighResAnalysis-0.0.3.tar` & `HighResAnalysis-0.0.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.047952 HighResAnalysis-0.0.3/
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.039248 HighResAnalysis-0.0.3/HighResAnalysis/
--rw-r--r--   0 hits       (501) staff       (20)       22 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)   319156 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/_modidx.py
--rw-r--r--   0 hits       (501) staff       (20)     4272 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/analyse.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.042796 HighResAnalysis-0.0.3/HighResAnalysis/cern/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     3085 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/adc.py
--rw-r--r--   0 hits       (501) staff       (20)      921 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/calibration.py
--rw-r--r--   0 hits       (501) staff       (20)     3984 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/converter.py
--rw-r--r--   0 hits       (501) staff       (20)     3889 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/event_alignment.py
--rw-r--r--   0 hits       (501) staff       (20)     1324 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/raw.py
--rw-r--r--   0 hits       (501) staff       (20)     1611 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/ref.py
--rw-r--r--   0 hits       (501) staff       (20)     7345 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/convert.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.044185 HighResAnalysis-0.0.3/HighResAnalysis/mod/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)    15122 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/dut_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     4883 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/efficiency.py
--rw-r--r--   0 hits       (501) staff       (20)      439 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/ref_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     1838 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/reference.py
--rw-r--r--   0 hits       (501) staff       (20)    12333 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/residuals.py
--rw-r--r--   0 hits       (501) staff       (20)      880 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/reso_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     3576 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/resolution.py
--rw-r--r--   0 hits       (501) staff       (20)      567 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/tel_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     2161 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/telescope.py
--rw-r--r--   0 hits       (501) staff       (20)     2463 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/track_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     4297 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/tracks.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.045275 HighResAnalysis-0.0.3/HighResAnalysis/plotting/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     5770 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/binning.py
--rw-r--r--   0 hits       (501) staff       (20)    71626 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/draw.py
--rw-r--r--   0 hits       (501) staff       (20)    17384 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/fit.py
--rw-r--r--   0 hits       (501) staff       (20)    13156 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/html.py
--rw-r--r--   0 hits       (501) staff       (20)     2473 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/info.py
--rw-r--r--   0 hits       (501) staff       (20)     3057 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/latex.py
--rw-r--r--   0 hits       (501) staff       (20)     8211 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/save.py
--rw-r--r--   0 hits       (501) staff       (20)    15920 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/utils.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.047243 HighResAnalysis-0.0.3/HighResAnalysis/src/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     5893 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/analysis.py
--rw-r--r--   0 hits       (501) staff       (20)     2377 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/batch_analysis.py
--rw-r--r--   0 hits       (501) staff       (20)     4056 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/bins.py
--rw-r--r--   0 hits       (501) staff       (20)    10064 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/calibration.py
--rw-r--r--   0 hits       (501) staff       (20)    18450 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/converter.py
--rw-r--r--   0 hits       (501) staff       (20)    14848 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/currents.py
--rw-r--r--   0 hits       (501) staff       (20)     6652 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/cut.py
--rw-r--r--   0 hits       (501) staff       (20)     5153 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/dut.py
--rw-r--r--   0 hits       (501) staff       (20)    36228 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/dut_analysis.py
--rw-r--r--   0 hits       (501) staff       (20)    12991 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/proteus.py
--rw-r--r--   0 hits       (501) staff       (20)      739 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/raw.py
--rw-r--r--   0 hits       (501) staff       (20)    11867 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/run.py
--rw-r--r--   0 hits       (501) staff       (20)     5600 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/scan.py
--rw-r--r--   0 hits       (501) staff       (20)     5869 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/spreadsheet.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.047583 HighResAnalysis-0.0.3/HighResAnalysis/utility/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/utility/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     1979 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/utility/affine_transformations.py
--rw-r--r--   0 hits       (501) staff       (20)    21164 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/utility/utils.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.040299 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.041872 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 hits       (501) staff       (20)     1865 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 hits       (501) staff       (20)     1691 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)       52 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/entry_points-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/not-zip-safe-checkpoint
--rw-r--r--   0 hits       (501) staff       (20)      136 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)       16 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)     3349 2023-05-22 12:51:02.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 hits       (501) staff       (20)     2429 2023-05-22 12:51:03.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-05-22 12:51:02.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 hits       (501) staff       (20)      110 2023-05-22 12:51:02.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/entry_points.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/not-zip-safe
--rw-r--r--   0 hits       (501) staff       (20)      145 2023-05-22 12:51:02.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/requires.txt
--rw-r--r--   0 hits       (501) staff       (20)       16 2023-05-22 12:51:02.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/top_level.txt
--rw-rw-r--   0 hits       (501) staff       (20)    11337 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.3/LICENSE
--rw-rw-r--   0 hits       (501) staff       (20)      111 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.3/MANIFEST.in
--rw-r--r--   0 hits       (501) staff       (20)     3349 2023-05-22 12:51:03.047801 HighResAnalysis-0.0.3/PKG-INFO
--rw-r--r--   0 hits       (501) staff       (20)     2501 2023-05-22 12:45:33.000000 HighResAnalysis-0.0.3/README.md
--rw-r--r--   0 hits       (501) staff       (20)     1131 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/settings.ini
--rw-r--r--   0 hits       (501) staff       (20)       38 2023-05-22 12:51:03.047994 HighResAnalysis-0.0.3/setup.cfg
--rw-rw-r--   0 hits       (501) staff       (20)     2560 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.3/setup.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 08:54:01.127556 HighResAnalysis-0.0.4/
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 08:54:01.117754 HighResAnalysis-0.0.4/HighResAnalysis/
+-rw-r--r--   0 hits       (501) staff       (20)       22 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)   319156 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/_modidx.py
+-rw-r--r--   0 hits       (501) staff       (20)     4272 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/analyse.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 08:54:01.121955 HighResAnalysis-0.0.4/HighResAnalysis/cern/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/cern/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     3085 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/cern/adc.py
+-rw-r--r--   0 hits       (501) staff       (20)      921 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/cern/calibration.py
+-rw-r--r--   0 hits       (501) staff       (20)     3984 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/cern/converter.py
+-rw-r--r--   0 hits       (501) staff       (20)     3889 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/cern/event_alignment.py
+-rw-r--r--   0 hits       (501) staff       (20)     1324 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/cern/raw.py
+-rw-r--r--   0 hits       (501) staff       (20)     1611 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/cern/ref.py
+-rw-r--r--   0 hits       (501) staff       (20)     7345 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/convert.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 08:54:01.123392 HighResAnalysis-0.0.4/HighResAnalysis/mod/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)    15122 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/dut_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     4883 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/efficiency.py
+-rw-r--r--   0 hits       (501) staff       (20)      439 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/ref_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     1838 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/reference.py
+-rw-r--r--   0 hits       (501) staff       (20)    12333 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/residuals.py
+-rw-r--r--   0 hits       (501) staff       (20)      880 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/reso_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     3576 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/resolution.py
+-rw-r--r--   0 hits       (501) staff       (20)      567 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/tel_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     2161 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/telescope.py
+-rw-r--r--   0 hits       (501) staff       (20)     2463 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/track_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     4297 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/mod/tracks.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 08:54:01.124495 HighResAnalysis-0.0.4/HighResAnalysis/plotting/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/plotting/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     5770 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/plotting/binning.py
+-rw-r--r--   0 hits       (501) staff       (20)    71626 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/plotting/draw.py
+-rw-r--r--   0 hits       (501) staff       (20)    17384 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/plotting/fit.py
+-rw-r--r--   0 hits       (501) staff       (20)    13156 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/plotting/html.py
+-rw-r--r--   0 hits       (501) staff       (20)     2473 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/plotting/info.py
+-rw-r--r--   0 hits       (501) staff       (20)     3057 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/plotting/latex.py
+-rw-r--r--   0 hits       (501) staff       (20)     8211 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/plotting/save.py
+-rw-r--r--   0 hits       (501) staff       (20)    15920 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/plotting/utils.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 08:54:01.126743 HighResAnalysis-0.0.4/HighResAnalysis/src/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     5893 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/analysis.py
+-rw-r--r--   0 hits       (501) staff       (20)     2377 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/batch_analysis.py
+-rw-r--r--   0 hits       (501) staff       (20)     4056 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/bins.py
+-rw-r--r--   0 hits       (501) staff       (20)    10064 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/calibration.py
+-rw-r--r--   0 hits       (501) staff       (20)    18466 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/converter.py
+-rw-r--r--   0 hits       (501) staff       (20)    14848 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/currents.py
+-rw-r--r--   0 hits       (501) staff       (20)     6652 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/cut.py
+-rw-r--r--   0 hits       (501) staff       (20)     5153 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/dut.py
+-rw-r--r--   0 hits       (501) staff       (20)    36222 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/dut_analysis.py
+-rw-r--r--   0 hits       (501) staff       (20)    12991 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/proteus.py
+-rw-r--r--   0 hits       (501) staff       (20)      739 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/raw.py
+-rw-r--r--   0 hits       (501) staff       (20)    11867 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/run.py
+-rw-r--r--   0 hits       (501) staff       (20)     5600 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/scan.py
+-rw-r--r--   0 hits       (501) staff       (20)     5869 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/src/spreadsheet.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 08:54:01.127137 HighResAnalysis-0.0.4/HighResAnalysis/utility/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/utility/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     1979 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/utility/affine_transformations.py
+-rw-r--r--   0 hits       (501) staff       (20)    21180 2023-05-24 08:53:39.000000 HighResAnalysis-0.0.4/HighResAnalysis/utility/utils.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 08:54:01.118963 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 08:54:01.120807 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 hits       (501) staff       (20)     1865 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 hits       (501) staff       (20)     1691 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)       52 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/.ipynb_checkpoints/entry_points-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/.ipynb_checkpoints/not-zip-safe-checkpoint
+-rw-r--r--   0 hits       (501) staff       (20)      136 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)       16 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)     5508 2023-05-24 08:54:01.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 hits       (501) staff       (20)     2429 2023-05-24 08:54:01.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-05-24 08:54:01.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 hits       (501) staff       (20)      110 2023-05-24 08:54:01.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/entry_points.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/not-zip-safe
+-rw-r--r--   0 hits       (501) staff       (20)      145 2023-05-24 08:54:01.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/requires.txt
+-rw-r--r--   0 hits       (501) staff       (20)       16 2023-05-24 08:54:01.000000 HighResAnalysis-0.0.4/HighResAnalysis.egg-info/top_level.txt
+-rw-rw-r--   0 hits       (501) staff       (20)    11337 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.4/LICENSE
+-rw-rw-r--   0 hits       (501) staff       (20)      111 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.4/MANIFEST.in
+-rw-r--r--   0 hits       (501) staff       (20)     5508 2023-05-24 08:54:01.127398 HighResAnalysis-0.0.4/PKG-INFO
+-rw-r--r--   0 hits       (501) staff       (20)     4660 2023-05-24 08:48:11.000000 HighResAnalysis-0.0.4/README.md
+-rw-r--r--   0 hits       (501) staff       (20)     1131 2023-05-24 08:48:34.000000 HighResAnalysis-0.0.4/settings.ini
+-rw-r--r--   0 hits       (501) staff       (20)       38 2023-05-24 08:54:01.127600 HighResAnalysis-0.0.4/setup.cfg
+-rw-rw-r--   0 hits       (501) staff       (20)     2560 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.4/setup.py
```

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/_modidx.py` & `HighResAnalysis-0.0.4/HighResAnalysis/_modidx.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/analyse.py` & `HighResAnalysis-0.0.4/HighResAnalysis/analyse.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/cern/adc.py` & `HighResAnalysis-0.0.4/HighResAnalysis/cern/adc.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/cern/calibration.py` & `HighResAnalysis-0.0.4/HighResAnalysis/cern/calibration.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/cern/converter.py` & `HighResAnalysis-0.0.4/HighResAnalysis/cern/converter.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/cern/event_alignment.py` & `HighResAnalysis-0.0.4/HighResAnalysis/cern/event_alignment.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/cern/raw.py` & `HighResAnalysis-0.0.4/HighResAnalysis/cern/raw.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/cern/ref.py` & `HighResAnalysis-0.0.4/HighResAnalysis/cern/ref.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/convert.py` & `HighResAnalysis-0.0.4/HighResAnalysis/convert.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/mod/dut_cuts.py` & `HighResAnalysis-0.0.4/HighResAnalysis/mod/dut_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/mod/efficiency.py` & `HighResAnalysis-0.0.4/HighResAnalysis/mod/efficiency.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/mod/reference.py` & `HighResAnalysis-0.0.4/HighResAnalysis/mod/reference.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/mod/residuals.py` & `HighResAnalysis-0.0.4/HighResAnalysis/mod/residuals.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/mod/reso_cuts.py` & `HighResAnalysis-0.0.4/HighResAnalysis/mod/reso_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/mod/resolution.py` & `HighResAnalysis-0.0.4/HighResAnalysis/mod/resolution.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/mod/tel_cuts.py` & `HighResAnalysis-0.0.4/HighResAnalysis/mod/tel_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/mod/telescope.py` & `HighResAnalysis-0.0.4/HighResAnalysis/mod/telescope.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/mod/track_cuts.py` & `HighResAnalysis-0.0.4/HighResAnalysis/mod/track_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/mod/tracks.py` & `HighResAnalysis-0.0.4/HighResAnalysis/mod/tracks.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/plotting/binning.py` & `HighResAnalysis-0.0.4/HighResAnalysis/plotting/binning.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/plotting/draw.py` & `HighResAnalysis-0.0.4/HighResAnalysis/plotting/draw.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/plotting/fit.py` & `HighResAnalysis-0.0.4/HighResAnalysis/plotting/fit.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/plotting/html.py` & `HighResAnalysis-0.0.4/HighResAnalysis/plotting/html.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/plotting/info.py` & `HighResAnalysis-0.0.4/HighResAnalysis/plotting/info.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/plotting/latex.py` & `HighResAnalysis-0.0.4/HighResAnalysis/plotting/latex.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/plotting/save.py` & `HighResAnalysis-0.0.4/HighResAnalysis/plotting/save.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/plotting/utils.py` & `HighResAnalysis-0.0.4/HighResAnalysis/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/analysis.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/analysis.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/batch_analysis.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/batch_analysis.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/bins.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/bins.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/calibration.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/calibration.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/converter.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # %% ../../nbs/37_src.converter.ipynb 3
 import uproot
 from numpy import all, ones, count_nonzero, array  # noqa
 from uproot import ReadOnlyDirectory
 from uproot.models import TTree
 from pathlib import Path
 import awkward as aw  
-from datetime import time, timedelta
+from datetime import timedelta
+from time import time
 from inspect import signature
 from subprocess import check_call
 import h5py
 
 from .proteus import Proteus
 from .run import Run, Analysis, init_batch, DUT, Batch
 from .analysis import BeamTest
```

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/currents.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/currents.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/cut.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/cut.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/dut.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/dut.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/dut_analysis.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/dut_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # %% ../../nbs/29_src.dut_analysis.ipynb 2
 #!/usr/bin/env python
 
 # %% ../../nbs/29_src.dut_analysis.ipynb 3
 import h5py
 from typing import Any
 from pathlib import Path
-from datetime import timedelta, time, datetime
+from datetime import timedelta, datetime
 from numpy import zeros, array, mean, sqrt
 from fastcore.utils import *
 
 import HighResAnalysis.cern.converter
 import HighResAnalysis.src.converter
 
 import HighResAnalysis.plotting.latex as tex
```

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/proteus.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/proteus.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/raw.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/raw.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/run.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/run.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/scan.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/scan.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/src/spreadsheet.py` & `HighResAnalysis-0.0.4/HighResAnalysis/src/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/utility/affine_transformations.py` & `HighResAnalysis-0.0.4/HighResAnalysis/utility/affine_transformations.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis/utility/utils.py` & `HighResAnalysis-0.0.4/HighResAnalysis/utility/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 from numpy import sqrt, array, arange, mean, exp, concatenate, zeros, log2, log10, array_split, ndarray, full, frombuffer
 from progressbar import Bar, ETA, FileTransferSpeed, Percentage, ProgressBar, SimpleProgress, Widget
 import h5py
 import pickle
 from copy import deepcopy
 from inspect import signature
 from functools import wraps
-from datetime import timedelta, datetime, time
+from datetime import timedelta, datetime
+from time import time
 from multiprocessing import Pool, cpu_count
 from hashlib import md5, sha256
 from pathlib import Path
 
 from ..plotting.utils import info, critical, add_to_info, get_kw, remove_file
 
 # %% ../../nbs/28_utility.utils.ipynb 3
```

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `HighResAnalysis-0.0.4/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt` & `HighResAnalysis-0.0.4/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/HighResAnalysis.egg-info/SOURCES.txt` & `HighResAnalysis-0.0.4/HighResAnalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/LICENSE` & `HighResAnalysis-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.3/settings.ini` & `HighResAnalysis-0.0.4/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = HighResAnalysis
 lib_name = HighResAnalysis
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = HighResAnalysis
 nbs_path = nbs
 recursive = True
```

### Comparing `HighResAnalysis-0.0.3/setup.py` & `HighResAnalysis-0.0.4/setup.py`

 * *Files identical despite different names*

