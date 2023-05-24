# Comparing `tmp/HighResAnalysis-0.0.5.tar.gz` & `tmp/HighResAnalysis-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HighResAnalysis-0.0.5.tar", last modified: Wed May 24 09:35:57 2023, max compression
+gzip compressed data, was "HighResAnalysis-0.0.6.tar", last modified: Wed May 24 09:52:54 2023, max compression
```

## Comparing `HighResAnalysis-0.0.5.tar` & `HighResAnalysis-0.0.6.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:35:57.926888 HighResAnalysis-0.0.5/
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:35:57.918118 HighResAnalysis-0.0.5/HighResAnalysis/
--rw-r--r--   0 hits       (501) staff       (20)       22 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)   319156 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/_modidx.py
--rw-r--r--   0 hits       (501) staff       (20)     4272 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/analyse.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:35:57.921799 HighResAnalysis-0.0.5/HighResAnalysis/cern/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/cern/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     3085 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/cern/adc.py
--rw-r--r--   0 hits       (501) staff       (20)      921 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/cern/calibration.py
--rw-r--r--   0 hits       (501) staff       (20)     3984 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/cern/converter.py
--rw-r--r--   0 hits       (501) staff       (20)     3889 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/cern/event_alignment.py
--rw-r--r--   0 hits       (501) staff       (20)     1324 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/cern/raw.py
--rw-r--r--   0 hits       (501) staff       (20)     1611 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/cern/ref.py
--rw-r--r--   0 hits       (501) staff       (20)     7345 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/convert.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:35:57.923183 HighResAnalysis-0.0.5/HighResAnalysis/mod/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)    15122 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/dut_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     4883 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/efficiency.py
--rw-r--r--   0 hits       (501) staff       (20)      439 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/ref_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     1838 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/reference.py
--rw-r--r--   0 hits       (501) staff       (20)    12333 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/residuals.py
--rw-r--r--   0 hits       (501) staff       (20)      880 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/reso_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     3576 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/resolution.py
--rw-r--r--   0 hits       (501) staff       (20)      567 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/tel_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     2161 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/telescope.py
--rw-r--r--   0 hits       (501) staff       (20)     2463 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/track_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     4297 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/mod/tracks.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:35:57.924404 HighResAnalysis-0.0.5/HighResAnalysis/plotting/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/plotting/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     5770 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/plotting/binning.py
--rw-r--r--   0 hits       (501) staff       (20)    71626 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/plotting/draw.py
--rw-r--r--   0 hits       (501) staff       (20)    17384 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/plotting/fit.py
--rw-r--r--   0 hits       (501) staff       (20)    13156 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/plotting/html.py
--rw-r--r--   0 hits       (501) staff       (20)     2473 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/plotting/info.py
--rw-r--r--   0 hits       (501) staff       (20)     3057 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/plotting/latex.py
--rw-r--r--   0 hits       (501) staff       (20)     8211 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/plotting/save.py
--rw-r--r--   0 hits       (501) staff       (20)    15920 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/HighResAnalysis/plotting/utils.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:35:57.926245 HighResAnalysis-0.0.5/HighResAnalysis/src/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     5893 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/analysis.py
--rw-r--r--   0 hits       (501) staff       (20)     2377 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/batch_analysis.py
--rw-r--r--   0 hits       (501) staff       (20)     4056 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/bins.py
--rw-r--r--   0 hits       (501) staff       (20)    10064 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/calibration.py
--rw-r--r--   0 hits       (501) staff       (20)    18466 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/converter.py
--rw-r--r--   0 hits       (501) staff       (20)    14848 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/currents.py
--rw-r--r--   0 hits       (501) staff       (20)     6652 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/cut.py
--rw-r--r--   0 hits       (501) staff       (20)     5153 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/dut.py
--rw-r--r--   0 hits       (501) staff       (20)    36238 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/dut_analysis.py
--rw-r--r--   0 hits       (501) staff       (20)    12991 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/proteus.py
--rw-r--r--   0 hits       (501) staff       (20)      739 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/raw.py
--rw-r--r--   0 hits       (501) staff       (20)    11867 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/run.py
--rw-r--r--   0 hits       (501) staff       (20)     5600 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/scan.py
--rw-r--r--   0 hits       (501) staff       (20)     5869 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/src/spreadsheet.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:35:57.926570 HighResAnalysis-0.0.5/HighResAnalysis/utility/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/utility/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     1979 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/utility/affine_transformations.py
--rw-r--r--   0 hits       (501) staff       (20)    21180 2023-05-24 09:35:50.000000 HighResAnalysis-0.0.5/HighResAnalysis/utility/utils.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:35:57.919184 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:35:57.920885 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 hits       (501) staff       (20)     1865 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 hits       (501) staff       (20)     1691 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)       52 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/.ipynb_checkpoints/entry_points-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/.ipynb_checkpoints/not-zip-safe-checkpoint
--rw-r--r--   0 hits       (501) staff       (20)      136 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)       16 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)     5508 2023-05-24 09:35:57.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 hits       (501) staff       (20)     2429 2023-05-24 09:35:57.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-05-24 09:35:57.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 hits       (501) staff       (20)      110 2023-05-24 09:35:57.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/entry_points.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/not-zip-safe
--rw-r--r--   0 hits       (501) staff       (20)      145 2023-05-24 09:35:57.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/requires.txt
--rw-r--r--   0 hits       (501) staff       (20)       16 2023-05-24 09:35:57.000000 HighResAnalysis-0.0.5/HighResAnalysis.egg-info/top_level.txt
--rw-rw-r--   0 hits       (501) staff       (20)    11337 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.5/LICENSE
--rw-rw-r--   0 hits       (501) staff       (20)      111 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.5/MANIFEST.in
--rw-r--r--   0 hits       (501) staff       (20)     5508 2023-05-24 09:35:57.926757 HighResAnalysis-0.0.5/PKG-INFO
--rw-r--r--   0 hits       (501) staff       (20)     4660 2023-05-24 08:48:11.000000 HighResAnalysis-0.0.5/README.md
--rw-r--r--   0 hits       (501) staff       (20)     1131 2023-05-24 09:35:49.000000 HighResAnalysis-0.0.5/settings.ini
--rw-r--r--   0 hits       (501) staff       (20)       38 2023-05-24 09:35:57.926925 HighResAnalysis-0.0.5/setup.cfg
--rw-rw-r--   0 hits       (501) staff       (20)     2560 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.5/setup.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:52:54.926791 HighResAnalysis-0.0.6/
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:52:54.917501 HighResAnalysis-0.0.6/HighResAnalysis/
+-rw-r--r--   0 hits       (501) staff       (20)       22 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)   319156 2023-05-24 09:52:48.000000 HighResAnalysis-0.0.6/HighResAnalysis/_modidx.py
+-rw-r--r--   0 hits       (501) staff       (20)     4272 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/analyse.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:52:54.921084 HighResAnalysis-0.0.6/HighResAnalysis/cern/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/cern/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     3085 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/cern/adc.py
+-rw-r--r--   0 hits       (501) staff       (20)      921 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/cern/calibration.py
+-rw-r--r--   0 hits       (501) staff       (20)     4064 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/cern/converter.py
+-rw-r--r--   0 hits       (501) staff       (20)     3889 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/cern/event_alignment.py
+-rw-r--r--   0 hits       (501) staff       (20)     1324 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/cern/raw.py
+-rw-r--r--   0 hits       (501) staff       (20)     1611 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/cern/ref.py
+-rw-r--r--   0 hits       (501) staff       (20)     7345 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/convert.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:52:54.922565 HighResAnalysis-0.0.6/HighResAnalysis/mod/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)    15122 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/dut_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     4883 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/efficiency.py
+-rw-r--r--   0 hits       (501) staff       (20)      439 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/ref_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     1838 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/reference.py
+-rw-r--r--   0 hits       (501) staff       (20)    12333 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/residuals.py
+-rw-r--r--   0 hits       (501) staff       (20)      880 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/reso_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     3576 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/resolution.py
+-rw-r--r--   0 hits       (501) staff       (20)      567 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/tel_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     2161 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/telescope.py
+-rw-r--r--   0 hits       (501) staff       (20)     2463 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/track_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     4297 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/mod/tracks.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:52:54.923910 HighResAnalysis-0.0.6/HighResAnalysis/plotting/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/plotting/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     5770 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/plotting/binning.py
+-rw-r--r--   0 hits       (501) staff       (20)    71626 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/plotting/draw.py
+-rw-r--r--   0 hits       (501) staff       (20)    17384 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/plotting/fit.py
+-rw-r--r--   0 hits       (501) staff       (20)    13156 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/plotting/html.py
+-rw-r--r--   0 hits       (501) staff       (20)     2473 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/plotting/info.py
+-rw-r--r--   0 hits       (501) staff       (20)     3057 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/plotting/latex.py
+-rw-r--r--   0 hits       (501) staff       (20)     8211 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/plotting/save.py
+-rw-r--r--   0 hits       (501) staff       (20)    15920 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/plotting/utils.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:52:54.925994 HighResAnalysis-0.0.6/HighResAnalysis/src/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     5893 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/analysis.py
+-rw-r--r--   0 hits       (501) staff       (20)     2377 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/batch_analysis.py
+-rw-r--r--   0 hits       (501) staff       (20)     4056 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/bins.py
+-rw-r--r--   0 hits       (501) staff       (20)    10064 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/calibration.py
+-rw-r--r--   0 hits       (501) staff       (20)    18466 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/converter.py
+-rw-r--r--   0 hits       (501) staff       (20)    14848 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/currents.py
+-rw-r--r--   0 hits       (501) staff       (20)     6652 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/cut.py
+-rw-r--r--   0 hits       (501) staff       (20)     5153 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/dut.py
+-rw-r--r--   0 hits       (501) staff       (20)    36238 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/dut_analysis.py
+-rw-r--r--   0 hits       (501) staff       (20)    12991 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/proteus.py
+-rw-r--r--   0 hits       (501) staff       (20)      739 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/raw.py
+-rw-r--r--   0 hits       (501) staff       (20)    11867 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/run.py
+-rw-r--r--   0 hits       (501) staff       (20)     5600 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/scan.py
+-rw-r--r--   0 hits       (501) staff       (20)     5869 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/src/spreadsheet.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:52:54.926375 HighResAnalysis-0.0.6/HighResAnalysis/utility/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/utility/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     1979 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/utility/affine_transformations.py
+-rw-r--r--   0 hits       (501) staff       (20)    21180 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/HighResAnalysis/utility/utils.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:52:54.918554 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-24 09:52:54.920155 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 hits       (501) staff       (20)     1865 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 hits       (501) staff       (20)     1691 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)       52 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/.ipynb_checkpoints/entry_points-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/.ipynb_checkpoints/not-zip-safe-checkpoint
+-rw-r--r--   0 hits       (501) staff       (20)      136 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)       16 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)     5508 2023-05-24 09:52:54.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 hits       (501) staff       (20)     2429 2023-05-24 09:52:54.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-05-24 09:52:54.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 hits       (501) staff       (20)      110 2023-05-24 09:52:54.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/entry_points.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/not-zip-safe
+-rw-r--r--   0 hits       (501) staff       (20)      145 2023-05-24 09:52:54.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/requires.txt
+-rw-r--r--   0 hits       (501) staff       (20)       16 2023-05-24 09:52:54.000000 HighResAnalysis-0.0.6/HighResAnalysis.egg-info/top_level.txt
+-rw-rw-r--   0 hits       (501) staff       (20)    11337 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.6/LICENSE
+-rw-rw-r--   0 hits       (501) staff       (20)      111 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.6/MANIFEST.in
+-rw-r--r--   0 hits       (501) staff       (20)     5508 2023-05-24 09:52:54.926602 HighResAnalysis-0.0.6/PKG-INFO
+-rw-r--r--   0 hits       (501) staff       (20)     4660 2023-05-24 08:48:11.000000 HighResAnalysis-0.0.6/README.md
+-rw-r--r--   0 hits       (501) staff       (20)     1131 2023-05-24 09:52:47.000000 HighResAnalysis-0.0.6/settings.ini
+-rw-r--r--   0 hits       (501) staff       (20)       38 2023-05-24 09:52:54.926837 HighResAnalysis-0.0.6/setup.cfg
+-rw-rw-r--   0 hits       (501) staff       (20)     2560 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.6/setup.py
```

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/_modidx.py` & `HighResAnalysis-0.0.6/HighResAnalysis/_modidx.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/analyse.py` & `HighResAnalysis-0.0.6/HighResAnalysis/analyse.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/cern/adc.py` & `HighResAnalysis-0.0.6/HighResAnalysis/cern/adc.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/cern/calibration.py` & `HighResAnalysis-0.0.6/HighResAnalysis/cern/calibration.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/cern/converter.py` & `HighResAnalysis-0.0.6/HighResAnalysis/cern/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,27 +52,27 @@
         return [self.Raw.OutFilePath, self.Adc2Vcal.OutFilePath, self.Ref.OutFilePath] + super().aux_files
 
     @property
     def raw_files(self):
         return [self.EventAlignment.RefPath, self.Adc2Vcal.RawFilePath] + super().raw_files
 
     def init_raw(self):
-        from cern.raw import CERNRaw
+        from HighResAnalysis.cern.raw import CERNRaw
         return CERNRaw(self)
 
     def init_event_alignment(self):
-        from cern.event_alignment import EventAlignment
+        from HighResAnalysis.cern.event_alignment import EventAlignment
         return EventAlignment(self.Raw)
 
     def init_adc2vcal(self):
-        from cern.adc import Adc2Vcal
+        from HighResAnalysis.cern.adc import Adc2Vcal
         return Adc2Vcal(self)
 
     def init_ref(self):
-        from cern.ref import RefConverter
+        from HighResAnalysis.cern.ref import RefConverter
         return RefConverter(self)
 
     def init_duts(self):
         return super().init_duts() if self.DUTName is None else [DUT.from_name(self.DUTName, self.Run.Info)]
 
     def merge_root_files(self, force=False):
         """merge the telescope and DUT root files"""
@@ -86,15 +86,15 @@
         return self.Adc2Vcal.OutFilePath
 
     def get_time_stamp(self):
         return (array(uproot.open(self.time_stamp_file)['Event']['TimeStamp']) / 1000).astype('d')
 
     @property
     def calibration(self):
-        from cern.calibration import CERNCalibration
+        from HighResAnalysis.cern.calibration import CERNCalibration
         return CERNCalibration
 
 # %% ../../nbs/12_cern.converter.ipynb 5
 @call_parse
 def main(run:int=232,
         dut:int=0,
         tc:str=None):
```

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/cern/event_alignment.py` & `HighResAnalysis-0.0.6/HighResAnalysis/cern/event_alignment.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/cern/raw.py` & `HighResAnalysis-0.0.6/HighResAnalysis/cern/raw.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/cern/ref.py` & `HighResAnalysis-0.0.6/HighResAnalysis/cern/ref.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/convert.py` & `HighResAnalysis-0.0.6/HighResAnalysis/convert.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/mod/dut_cuts.py` & `HighResAnalysis-0.0.6/HighResAnalysis/mod/dut_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/mod/efficiency.py` & `HighResAnalysis-0.0.6/HighResAnalysis/mod/efficiency.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/mod/reference.py` & `HighResAnalysis-0.0.6/HighResAnalysis/mod/reference.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/mod/residuals.py` & `HighResAnalysis-0.0.6/HighResAnalysis/mod/residuals.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/mod/reso_cuts.py` & `HighResAnalysis-0.0.6/HighResAnalysis/mod/reso_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/mod/resolution.py` & `HighResAnalysis-0.0.6/HighResAnalysis/mod/resolution.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/mod/tel_cuts.py` & `HighResAnalysis-0.0.6/HighResAnalysis/mod/tel_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/mod/telescope.py` & `HighResAnalysis-0.0.6/HighResAnalysis/mod/telescope.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/mod/track_cuts.py` & `HighResAnalysis-0.0.6/HighResAnalysis/mod/track_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/mod/tracks.py` & `HighResAnalysis-0.0.6/HighResAnalysis/mod/tracks.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/plotting/binning.py` & `HighResAnalysis-0.0.6/HighResAnalysis/plotting/binning.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/plotting/draw.py` & `HighResAnalysis-0.0.6/HighResAnalysis/plotting/draw.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/plotting/fit.py` & `HighResAnalysis-0.0.6/HighResAnalysis/plotting/fit.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/plotting/html.py` & `HighResAnalysis-0.0.6/HighResAnalysis/plotting/html.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/plotting/info.py` & `HighResAnalysis-0.0.6/HighResAnalysis/plotting/info.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/plotting/latex.py` & `HighResAnalysis-0.0.6/HighResAnalysis/plotting/latex.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/plotting/save.py` & `HighResAnalysis-0.0.6/HighResAnalysis/plotting/save.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/plotting/utils.py` & `HighResAnalysis-0.0.6/HighResAnalysis/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/analysis.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/analysis.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/batch_analysis.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/batch_analysis.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/bins.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/bins.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/calibration.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/calibration.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/converter.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/converter.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/currents.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/currents.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/cut.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/cut.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/dut.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/dut.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/dut_analysis.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/dut_analysis.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/proteus.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/proteus.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/raw.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/raw.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/run.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/run.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/scan.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/scan.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/src/spreadsheet.py` & `HighResAnalysis-0.0.6/HighResAnalysis/src/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/utility/affine_transformations.py` & `HighResAnalysis-0.0.6/HighResAnalysis/utility/affine_transformations.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis/utility/utils.py` & `HighResAnalysis-0.0.6/HighResAnalysis/utility/utils.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `HighResAnalysis-0.0.6/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt` & `HighResAnalysis-0.0.6/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis.egg-info/PKG-INFO` & `HighResAnalysis-0.0.6/HighResAnalysis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HighResAnalysis
-Version: 0.0.5
+Version: 0.0.6
 Summary: Analysis of High Resolution Data from CERN and DESY beam tests
 Home-page: https://github.com/dmitryhits/HighResAnalysis
 Author: Dmitry Hits
 Author-email: dmitry.hits@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python alignment telescope testbeam
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `HighResAnalysis-0.0.5/HighResAnalysis.egg-info/SOURCES.txt` & `HighResAnalysis-0.0.6/HighResAnalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/LICENSE` & `HighResAnalysis-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/PKG-INFO` & `HighResAnalysis-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HighResAnalysis
-Version: 0.0.5
+Version: 0.0.6
 Summary: Analysis of High Resolution Data from CERN and DESY beam tests
 Home-page: https://github.com/dmitryhits/HighResAnalysis
 Author: Dmitry Hits
 Author-email: dmitry.hits@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python alignment telescope testbeam
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `HighResAnalysis-0.0.5/README.md` & `HighResAnalysis-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.5/settings.ini` & `HighResAnalysis-0.0.6/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = HighResAnalysis
 lib_name = HighResAnalysis
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = HighResAnalysis
 nbs_path = nbs
 recursive = True
```

### Comparing `HighResAnalysis-0.0.5/setup.py` & `HighResAnalysis-0.0.6/setup.py`

 * *Files identical despite different names*

