# Comparing `tmp/dspeed-1.0.1.tar.gz` & `tmp/dspeed-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspeed-1.0.1.tar", last modified: Wed May 24 14:14:02 2023, max compression
+gzip compressed data, was "dspeed-1.1.0.tar", last modified: Wed May 24 15:37:41 2023, max compression
```

## Comparing `dspeed-1.0.1.tar` & `dspeed-1.1.0.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:14:02.480001 dspeed-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 14:13:53.000000 dspeed-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-24 14:14:02.480001 dspeed-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-24 14:13:53.000000 dspeed-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-24 14:13:53.000000 dspeed-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-24 14:14:02.480001 dspeed-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 14:13:53.000000 dspeed-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:14:02.472001 dspeed-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:14:02.472001 dspeed-1.0.1/src/dspeed/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 14:14:02.000000 dspeed-1.0.1/src/dspeed/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    72374 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processing_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:14:02.476001 dspeed-1.0.1/src/dspeed/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/bl_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/dplms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/dwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/fftw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/gaussian_filter1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/linear_slope_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/log_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/min_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/moving_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/multi_a_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/multi_t_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/param_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/peak_snr_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/pole_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/presum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/pulse_injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/soft_pileup_corr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/time_over_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/time_point_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/trap_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/wiener_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/processors/windower.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:14:02.476001 dspeed-1.0.1/src/dspeed/vis/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-05-24 14:13:53.000000 dspeed-1.0.1/src/dspeed/vis/waveform_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:14:02.472001 dspeed-1.0.1/src/dspeed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-24 14:14:02.000000 dspeed-1.0.1/src/dspeed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-24 14:14:02.000000 dspeed-1.0.1/src/dspeed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:14:02.000000 dspeed-1.0.1/src/dspeed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 14:14:02.000000 dspeed-1.0.1/src/dspeed.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:14:02.000000 dspeed-1.0.1/src/dspeed.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-24 14:14:02.000000 dspeed-1.0.1/src/dspeed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 14:14:02.000000 dspeed-1.0.1/src/dspeed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:14:02.480001 dspeed-1.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:14:02.480001 dspeed-1.0.1/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/configs/icpc-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/configs/numpy-parsing.json
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/configs/sipm-dplms-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/configs/sipm-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:14:02.480001 dspeed-1.0.1/tests/processors/
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/processors/dplms_noise_mat.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/processors/test_dplms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/processors/test_dwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/processors/test_fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/processors/test_get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/processors/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/test_build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/test_list_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/test_numpy_constants_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/test_processing_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:14:02.480001 dspeed-1.0.1/tests/vis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:14:02.480001 dspeed-1.0.1/tests/vis/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/vis/configs/hpge-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-24 14:13:53.000000 dspeed-1.0.1/tests/vis/test_waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.246807 dspeed-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 15:37:33.000000 dspeed-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-24 15:37:41.246807 dspeed-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-24 15:37:33.000000 dspeed-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-24 15:37:33.000000 dspeed-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-24 15:37:41.246807 dspeed-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 15:37:33.000000 dspeed-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.234807 dspeed-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.238807 dspeed-1.1.0/src/dspeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72618 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processing_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.242807 dspeed-1.1.0/src/dspeed/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/bl_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/dplms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/fftw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/gaussian_filter1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/linear_slope_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/log_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/moving_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/multi_a_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/multi_t_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/param_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/peak_snr_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/pole_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/presum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/pulse_injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/soft_pileup_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/time_over_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/time_point_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/trap_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/wiener_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/windower.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.242807 dspeed-1.1.0/src/dspeed/vis/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/vis/waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.238807 dspeed-1.1.0/src/dspeed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.242807 dspeed-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.242807 dspeed-1.1.0/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/configs/icpc-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/configs/numpy-parsing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/configs/sipm-dplms-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/configs/sipm-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.246807 dspeed-1.1.0/tests/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/dplms_noise_mat.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_dplms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_fftw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_list_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_numpy_constants_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_processing_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.246807 dspeed-1.1.0/tests/vis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.246807 dspeed-1.1.0/tests/vis/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/vis/configs/hpge-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/vis/test_waveform_browser.py
```

### Comparing `dspeed-1.0.1/LICENSE` & `dspeed-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/PKG-INFO` & `dspeed-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspeed
-Version: 1.0.1
+Version: 1.1.0
 Summary: Fast Digital Signal Processing for particle detectors in Python
 Home-page: https://github.com/legend-exp/dspeed
 Author: Ian Guinn
 Author-email: iguinn@email.unc.edu
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dspeed-1.0.1/README.md` & `dspeed-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/setup.cfg` & `dspeed-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/build_dsp.py` & `dspeed-1.1.0/src/dspeed/build_dsp.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/cli.py` & `dspeed-1.1.0/src/dspeed/cli.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/errors.py` & `dspeed-1.1.0/src/dspeed/errors.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/logging.py` & `dspeed-1.1.0/src/dspeed/logging.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processing_chain.py` & `dspeed-1.1.0/src/dspeed/processing_chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,29 +9,28 @@
 import itertools as it
 import json
 import logging
 import re
 from abc import ABCMeta, abstractmethod
 from copy import deepcopy
 from dataclasses import dataclass
-from typing import Any, Union
+from typing import Any
 
 import lgdo
 import numpy as np
+from lgdo import LGDO
 from lgdo.lgdo_utils import expand_path
 from numba import vectorize
 from pint import Quantity, Unit
 
 from .errors import DSPFatal, ProcessingChainError
 from .units import unit_registry as ureg
 
 log = logging.getLogger(__name__)
 
-LGDO = Union[lgdo.Scalar, lgdo.Array, lgdo.VectorOfVectors, lgdo.Struct]
-
 # Filler value for variables to be automatically deduced later
 auto = "auto"
 
 # Map from ast interpreter operations to functions to call and format string
 ast_ops_dict = {
     ast.Add: (np.add, "{}+{}"),
     ast.Sub: (np.subtract, "{}-{}"),
@@ -125,30 +124,30 @@
         unit: str | Unit = auto,
         is_coord: bool = auto,
     ) -> None:
         """
         Parameters
         ----------
         proc_chain
-            ProcessingChain that contains this variable
+            :class:`ProcessingChain` that contains this variable.
         name
-            Name of variable used to look it up
+            Name of variable used to look it up.
         shape
-            Shape of variable, without buffer_len dimension
+            Shape of variable, without `buffer_len` dimension.
         dtype
-            Data type of variable
+            Data type of variable.
         grid
             Coordinate grid associated with variable. This contains the
             period and offset of the variable. For variables where
-            is_coord is True, use this to perform unit conversions
+            is_coord is True, use this to perform unit conversions.
         unit
             Unit associated with variable during I/O.
         is_coord
-            If True, variable represents an array index and can be converted
-            into a unitted number using grid
+            If ``True``, variable represents an array index and can be converted
+            into a unitted number using grid.
         """
         assert isinstance(proc_chain, ProcessingChain) and isinstance(name, str)
         self.proc_chain = proc_chain
         self.name = name
 
         # ndarray containing data buffer of size block_width x shape
         # list of ndarrays in different coordinate systems if is_coord is true
@@ -339,15 +338,15 @@
         """
         Parameters
         ----------
         block_width
             number of entries to simultaneously process.
         buffer_len
             length of input and output buffers. Should be a multiple of
-            `block_width`
+            `block_width`.
         """
         # Dictionary from name to scratch data buffers as ProcChainVar
         self._vars_dict = {}
         # list of processors with variables they are called on
         self._proc_managers = []
         # lists of I/O managers that handle copying data to/from external memory buffers
         self._input_managers = []
@@ -1079,23 +1078,29 @@
             arr_grid = param.grid if param.grid is not auto else None
             if not grid:
                 grid = arr_grid
 
             # check if arr_dims can be broadcast to match fun_dims
             for i in range(max(len(fun_dims), len(arr_dims))):
                 fd = fun_dims[-i - 1] if i < len(fun_dims) else None
-                ad = arr_dims[-i - 1] if i < len(arr_dims) else None
+                ad = (
+                    arr_dims[-i - 1]
+                    if i < len(arr_dims)
+                    else self.proc_chain._block_width
+                    if i == len(arr_dims)
+                    else None
+                )
 
                 if isinstance(fd, str):
                     if fd in dims_dict:
                         this_dim = dims_dict[fd]
                         if not ad or this_dim.length != ad:
                             raise ProcessingChainError(
                                 f"failed to broadcast array dimensions for "
-                                f"{func.__name}. Could not find consistent value "
+                                f"{func.__name__}. Could not find consistent value "
                                 f"for dimension {fd}"
                             )
                         if not this_dim.grid:
                             dims_dict[fd].grid = arr_grid
                         elif arr_grid and arr_grid != this_dim.grid:
                             log.debug(
                                 f"arrays of dimension {fd} for "
@@ -1160,14 +1165,15 @@
                 it.chain(zip(it.repeat(None), self.params), self.kw_params.items()),
                 dims_list,
                 self.types,
             )
         ):
             dim_list = outerdims.copy()
             for d in dims.split(","):
+                d = d.strip()
                 if not d:
                     continue
                 if d not in dims_dict:
                     # If it is an array lets get the length
                     if isinstance(param, np.ndarray):
                         dims_dict[d] = self.DimInfo(len(param), None)
                     else:
@@ -1307,19 +1313,20 @@
         ]
         self.kwargs = {}
 
         log.debug(f"added conversion: {self}")
 
 
 class IOManager(metaclass=ABCMeta):
-    """
-    Base class. IOManagers will be associated with a type of input/output
-    buffer, and must define a read and write for each one. __init__ methods
-    should update variable with any information from buffer, and check that
-    buffer and variable are compatible.
+    r"""Base class.
+
+    :class:`IOManager`\ s will be associated with a type of input/output
+    buffer, and must define a read and write for each one. ``__init__()``
+    methods should update variable with any information from buffer, and check
+    that buffer and variable are compatible.
     """
 
     @abstractmethod
     def read(self, start: int, end: int) -> None:
         pass
 
     @abstractmethod
@@ -1329,15 +1336,15 @@
     @abstractmethod
     def __str__(self) -> str:
         pass
 
 
 # Ok, this one's not LGDO
 class NumpyIOManager(IOManager):
-    """IO Manager for buffers that are numpy arrays"""
+    r""":class:`IOManager` for buffers that are :class:`numpy.ndarray`\ s."""
 
     def __init__(self, io_buf: np.ndarray, var: ProcChainVar) -> None:
         assert isinstance(io_buf, np.ndarray) and isinstance(var, ProcChainVar)
 
         var.update_auto(dtype=io_buf.dtype, shape=io_buf.shape[1:])
 
         if var.shape != io_buf.shape[1:] or var.dtype != io_buf.dtype:
@@ -1364,15 +1371,15 @@
         return (
             f"{self.var} linked to numpy.array(shape={self.io_buf.shape}, "
             f"dtype={self.io_buf.dtype})"
         )
 
 
 class LGDOArrayIOManager(IOManager):
-    """IO Manager for buffers that are lgdo Arrays"""
+    r"""IO Manager for buffers that are :class:`lgdo.Array`\ s."""
 
     def __init__(self, io_array: lgdo.Array, var: ProcChainVar) -> None:
         assert isinstance(io_array, lgdo.Array) and isinstance(var, ProcChainVar)
 
         unit = io_array.attrs.get("units", None)
         var.update_auto(dtype=io_array.dtype, shape=io_array.nda.shape[1:], unit=unit)
 
@@ -1416,15 +1423,15 @@
         )
 
     def __str__(self) -> str:
         return f"{self.var} linked to lgdo.Array(shape={self.io_array.nda.shape}, dtype={self.io_array.nda.dtype}, attrs={self.io_array.attrs})"
 
 
 class LGDOArrayOfEqualSizedArraysIOManager(IOManager):
-    """IO Manager for buffers that are numpy ArrayOfEqualSizedArrays"""
+    r""":class:`IOManager` for buffers that are :class:`lgdo.ArrayOfEqualSizedArray`\ s."""
 
     def __init__(self, io_array: np.ArrayOfEqualSizedArrays, var: ProcChainVar) -> None:
         assert isinstance(io_array, lgdo.ArrayOfEqualSizedArrays) and isinstance(
             var, ProcChainVar
         )
 
         unit = io_array.attrs.get("units", None)
@@ -1637,15 +1644,15 @@
         any value can be used.
 
     Returns
     -------
     (proc_chain, field_mask, lh5_out)
         - `proc_chain` -- :class:`ProcessingChain` object that is executed
         - `field_mask` -- list of input fields that are used
-        - `lh5_out` -- output :class:`~.lgdo.table.Table` containing processed
+        - `lh5_out` -- output :class:`~lgdo.table.Table` containing processed
           values
     """
     proc_chain = ProcessingChain(block_width, lh5_in.size)
 
     if isinstance(dsp_config, str):
         with open(expand_path(dsp_config)) as f:
             dsp_config = json.load(f)
```

### Comparing `dspeed-1.0.1/src/dspeed/processors/__init__.py` & `dspeed-1.1.0/src/dspeed/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/bl_subtract.py` & `dspeed-1.1.0/src/dspeed/processors/bl_subtract.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/convolutions.py` & `dspeed-1.1.0/src/dspeed/processors/convolutions.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/dplms.py` & `dspeed-1.1.0/src/dspeed/processors/dplms.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/dwt.py` & `dspeed-1.1.0/src/dspeed/processors/dwt.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/fftw.py` & `dspeed-1.1.0/src/dspeed/processors/fftw.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,60 +2,90 @@
 
 from typing import Callable
 
 import numpy as np
 from numba import guvectorize
 from pyfftw import FFTW
 
+from ..processing_chain import ProcChainVar
 from ..utils import numba_defaults_kwargs as nb_kwargs
 
 
-def dft(buf_in: np.ndarray, buf_out: np.ndarray) -> Callable:
+def dft(w_in: np.ndarray | ProcChainVar, w_out: np.ndarray | ProcChainVar) -> Callable:
     """Perform discrete Fourier transforms using the FFTW library.
 
-    Note
-    ----
-    This processor is composed of a factory function that is called using the
-    `init_args` argument. The input and output waveforms are passed using
-    `args`.
+    Parameters
+    ----------
+    w_in
+        the input waveform.
+    w_out
+        the output fourier transform.
+
+    JSON Configuration Example
+    --------------------------
+
+    .. code-block :: json
+
+        "wf_dft": {
+            "function": "dft",
+            "module": "dspeed.processors",
+            "args": ["wf", "wf_dft"],
+            "init_args": ["wf", "wf_dft"]
+        }
 
     Note
     ----
     FFTW optimizes the FFT algorithm based on the size of the arrays, with SIMD
     parallelized commands.  This optimization requires initialization, so this
     is a factory function that returns a Numba gufunc that performs the FFT.
     FFTW works on fixed memory buffers, so you must tell it what memory to use
     ahead of time.  When using this with
-    :class:`~.dsp.processing_chain.ProcessingChain`, to ensure the correct
-    buffers are used, call
-    :meth:`~.dsp.processing_chain.ProcessingChain.get_variable` to give it the
-    internal memory buffer directly. With :func:`~.dsp.build_dsp.build_dsp`,
-    you can just give it the name, and it will automatically happen. The
+    :class:`~.dsp.processing_chain.ProcessingChain`, the output waveform's size,
+    dtype and coordinate grid units can be set automatically.  The
     possible `dtypes` for the input/outputs are:
 
     =============================== ========= =============================== =============
     :class:`numpy.dtype`            Size      :class:`numpy.dtype`            Size
     ------------------------------- --------- ------------------------------- -------------
     ``float32``/``float``           :math:`n` ``complex64``                   :math:`n/2+1`
     ``float64``/``double``          :math:`n` ``complex128``                  :math:`n/2+1`
     ``float128``/``longdouble``     :math:`n` ``complex256``/``clongdouble``  :math:`n/2+1`
     ``complex64``                   :math:`n` ``complex64``                   :math:`n`
     ``complex128``                  :math:`n` ``complex128``                  :math:`n`
     ``complex256``/``clongdouble``  :math:`n` ``complex256``/``clongdouble``  :math:`n`
     =============================== ========= =============================== =============
     """
+    # if we have a ProcChainVar, set up the output and get numpy arrays
+    if isinstance(w_in, ProcChainVar) and isinstance(w_out, ProcChainVar):
+        c = w_in.dtype.kind
+        s = w_in.dtype.itemsize
+        if c == "f":
+            w_out.update_auto(
+                shape=w_in.shape[:-1] + (w_in.shape[-1] // 2 + 1,),
+                dtype=np.dtype(f"c{2*s}"),
+                period=1.0 / w_in.period / w_in.shape[-1],
+            )
+        elif c == "c":
+            w_out.update_auto(
+                shape=w_in.shape,
+                dtype=np.dtype(f"c{s}"),
+                period=1.0 / w_in.period / w_in.shape[-1],
+            )
+        w_in = w_in.buffer
+        w_out = w_out.buffer
+
     try:
-        dft_fun = FFTW(buf_in, buf_out, axes=(-1,), direction="FFTW_FORWARD")
+        dft_fun = FFTW(w_in, w_out, axes=(-1,), direction="FFTW_FORWARD")
     except ValueError:
         raise ValueError(
             "incompatible array types/shapes. See function documentation for allowed values"
         )
 
-    typesig = "void(" + str(buf_in.dtype) + "[:, :], " + str(buf_out.dtype) + "[:, :])"
-    sizesig = "(m, n)->(m, n)" if buf_in.shape == buf_out.shape else "(m, n),(m, l)"
+    typesig = "void(" + str(w_in.dtype) + "[:, :], " + str(w_out.dtype) + "[:, :])"
+    sizesig = "(m, n)->(m, n)" if w_in.shape == w_out.shape else "(m, n),(m, l)"
 
     @guvectorize(
         [typesig],
         sizesig,
         **nb_kwargs(
             cache=False,
             forceobj=True,
@@ -63,57 +93,87 @@
     )
     def dft(wf_in: np.ndarray, dft_out: np.ndarray) -> None:
         dft_fun(wf_in, dft_out)
 
     return dft
 
 
-def inv_dft(buf_in: np.ndarray, buf_out: np.ndarray) -> Callable:
+def inv_dft(w_in: np.ndarray, w_out: np.ndarray) -> Callable:
     """Perform inverse discrete Fourier transforms using the FFTW library.
 
-    Note
-    ----
-    This processor is composed of a factory function that is called using the
-    `init_args` argument. The input and output waveforms are passed using
-    `args`.
+    Parameters
+    ----------
+    w_in
+        the input fourier transformed waveform.
+    w_out
+        the output time-domain waveform.
+
+    JSON Configuration Example
+    --------------------------
+
+    .. code-block :: json
+
+        "wf_invdft": {
+            "function": "inv_dft",
+            "module": "dspeed.processors",
+            "args": ["wf_dft", "wf_invdft"],
+            "init_args": ["wf_dft", "wf_invdft"]
+        }
 
     Note
     ----
     FFTW optimizes the FFT algorithm based on the size of the arrays, with SIMD
     parallelized commands.  This optimization requires initialization, so this
     is a factory function that returns a Numba gufunc that performs the FFT.
     FFTW works on fixed memory buffers, so you must tell it what memory to use
     ahead of time.  When using this with
-    :class:`~.dsp.processing_chain.ProcessingChain`, to ensure the correct
-    buffers are used, call
-    :meth:`~.dsp.processing_chain.ProcessingChain.get_variable` to give it the
-    internal memory buffer directly. With :func:`~.dsp.build_dsp.build_dsp`,
-    you can just give it the name, and it will automatically happen. The
-    possible `dtypes` for the input/outputs are:
+    :class:`~.dsp.processing_chain.ProcessingChain`, the output waveform's size,
+    dtype and coordinate grid units can be set automatically.  The automated
+    behavior will produce a real output by default, unless you specify a complex
+    output. Possible `dtypes` for the input/outputs are:
 
     =============================== ============= =============================== =========
     :class:`numpy.dtype`            Size          :class:`numpy.dtype`            Size
     ------------------------------- ------------- ------------------------------- ---------
     ``complex64``                   :math:`n/2+1` ``float32``/``float``           :math:`n`
     ``complex128``                  :math:`n/2+1` ``float64``/``double``          :math:`n`
     ``complex256``/``clongdouble``  :math:`n/2+1` ``float128``/``longdouble``     :math:`n`
     ``complex64``                   :math:`n`     ``complex64``                   :math:`n`
     ``complex128``                  :math:`n`     ``complex128``                  :math:`n`
     ``complex256``/``clongdouble``  :math:`n`     ``complex256``/``clongdouble``  :math:`n`
     =============================== ============= =============================== =========
     """
+    # if we have a ProcChainVar, set up the output and get numpy arrays
+    if isinstance(w_in, ProcChainVar) and isinstance(w_out, ProcChainVar):
+        s = w_in.dtype.itemsize
+        if w_out.dtype == "auto":
+            w_out.update_auto(
+                shape=w_in.shape[:-1] + (2 * (w_in.shape[-1] - 1),),
+                dtype=np.dtype(f"f{s//2}"),
+                period=1.0 / w_in.period / w_in.shape[-1],
+            )
+        else:
+            w_out.update_auto(
+                shape=w_in.shape
+                if w_out.dtype.kind == "c"
+                else w_in.shape[:-1] + (2 * (w_in.shape[-1] - 1),),
+                period=1.0 / w_in.period / w_in.shape[-1],
+            )
+        w_in = w_in.buffer
+        w_out = w_out.buffer
+
     try:
-        idft_fun = FFTW(buf_in, buf_out, axes=(-1,), direction="FFTW_BACKWARD")
+        idft_fun = FFTW(w_in, w_out, axes=(-1,), direction="FFTW_BACKWARD")
     except ValueError:
         raise ValueError(
             "incompatible array types/shapes. See function documentation for allowed values"
         )
 
-    typesig = "void(" + str(buf_in.dtype) + "[:, :], " + str(buf_out.dtype) + "[:, :])"
-    sizesig = "(m, n)->(m, n)" if buf_in.shape == buf_out.shape else "(m, n),(m, l)"
+    typesig = "void(" + str(w_in.dtype) + "[:, :], " + str(w_out.dtype) + "[:, :])"
+    sizesig = "(m, n)->(m, n)" if w_in.shape == w_out.shape else "(m, n),(m, l)"
 
     @guvectorize(
         [typesig],
         sizesig,
         **nb_kwargs(
             cache=False,
             forceobj=True,
@@ -121,70 +181,96 @@
     )
     def inv_dft(wf_in: np.ndarray, dft_out: np.ndarray) -> None:
         idft_fun(wf_in, dft_out)
 
     return inv_dft
 
 
-def psd(buf_in: np.ndarray, buf_out: np.ndarray) -> Callable:
+def psd(w_in: np.ndarray, w_out: np.ndarray) -> Callable:
     """Perform discrete Fourier transforms using the FFTW library, and use it to get
     the power spectral density.
 
-    Note
-    ----
-    This processor is composed of a factory function that is called using the
-    `init_args` argument. The input and output waveforms are passed using
-    `args`.
+    Parameters
+    ----------
+    w_in
+        the input waveform.
+    w_out
+        the output fourier transform.
+
+    JSON Configuration Example
+    --------------------------
+
+    .. code-block :: json
+
+        "wf_psd": {
+            "function": "psd",
+            "module": "dspeed.processors",
+            "args": ["wf", "wf_psd"],
+            "init_args": ["wf", "wf_psd"]
+        }
 
     Note
     ----
     FFTW optimizes the FFT algorithm based on the size of the arrays, with SIMD
     parallelized commands.  This optimization requires initialization, so this
     is a factory function that returns a Numba gufunc that performs the FFT.
     FFTW works on fixed memory buffers, so you must tell it what memory to use
     ahead of time.  When using this with
-    :class:`~.dsp.processing_chain.ProcessingChain`, to ensure the correct
-    buffers are used, call
-    :meth:`~.dsp.processing_chain.ProcessingChain.get_variable` to give it the
-    internal memory buffer directly. With :func:`~.dsp.build_dsp.build_dsp`,
-    you can just give it the name, and it will automatically happen. The
+    :class:`~.dsp.processing_chain.ProcessingChain`, the output waveform's size,
+    dtype and coordinate grid units can be set automatically.  The
     possible `dtypes` for the input/outputs are:
 
     =============================== ========= ============================ =============
     :class:`numpy.dtype`            Size      :class:`numpy.dtype`         Size
     ------------------------------- --------- ---------------------------- -------------
     ``complex64``                   :math:`n` ``float32``/``float``        :math:`n`
     ``complex128``                  :math:`n` ``float64``/``double``       :math:`n`
     ``complex256``/``clongdouble``  :math:`n` ``float128``/``longdouble``  :math:`n`
     ``float32``/``float``           :math:`n` ``float32``/``float``        :math:`n/2+1`
     ``float64``/``double``          :math:`n` ``float64``/``double``       :math:`n/2+1`
     ``float128``/``longdouble``     :math:`n` ``float128``/``longdouble``  :math:`n/2+1`
     =============================== ========= ============================ =============
     """
+    # if we have a ProcChainVar, set up the output and get numpy arrays
+    if isinstance(w_in, ProcChainVar) and isinstance(w_out, ProcChainVar):
+        c = w_in.dtype.kind
+        s = w_in.dtype.itemsize
+        if c == "f":
+            w_out.update_auto(
+                shape=w_in.shape[:-1] + (w_in.shape[-1] // 2 + 1,),
+                dtype=np.dtype(f"f{s}"),
+                period=1.0 / w_in.period / w_in.shape[-1],
+            )
+        elif c == "c":
+            w_out.update_auto(
+                shape=w_in.shape,
+                dtype=np.dtype(f"f{s//2}"),
+                period=1.0 / w_in.period / w_in.shape[-1],
+            )
+        w_in = w_in.buffer
+        w_out = w_out.buffer
 
     # build intermediate array for the dft, which will be abs'd to get the PSD
-    buf_dft = np.ndarray(
-        buf_out.shape, np.dtype("complex" + str(buf_out.dtype.itemsize * 16))
-    )
+    w_dft = np.ndarray(w_out.shape, np.dtype(f"c{w_in.dtype.itemsize*2}"))
     try:
-        dft_fun = FFTW(buf_in, buf_dft, axes=(-1,), direction="FFTW_FORWARD")
+        dft_fun = FFTW(w_in, w_dft, axes=(-1,), direction="FFTW_FORWARD")
     except ValueError:
         raise ValueError(
             "incompatible array types/shapes. See function documentation for allowed values"
         )
 
-    typesig = "void(" + str(buf_in.dtype) + "[:, :], " + str(buf_out.dtype) + "[:, :])"
-    sizesig = "(m, n)->(m, n)" if buf_in.shape == buf_out.shape else "(m, n),(m, l)"
+    typesig = "void(" + str(w_in.dtype) + "[:, :], " + str(w_out.dtype) + "[:, :])"
+    sizesig = "(m, n)->(m, n)" if w_in.shape == w_out.shape else "(m, n),(m, l)"
 
     @guvectorize(
         [typesig],
         sizesig,
         **nb_kwargs(
             cache=False,
             forceobj=True,
         ),
     )
     def psd(wf_in: np.ndarray, psd_out: np.ndarray) -> None:
-        dft_fun(wf_in, buf_dft)
-        np.abs(buf_dft, psd_out)
+        dft_fun(wf_in, w_dft)
+        np.abs(w_dft, psd_out)
 
     return psd
```

### Comparing `dspeed-1.0.1/src/dspeed/processors/fixed_time_pickoff.py` & `dspeed-1.1.0/src/dspeed/processors/fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/gaussian_filter1d.py` & `dspeed-1.1.0/src/dspeed/processors/gaussian_filter1d.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/get_multi_local_extrema.py` & `dspeed-1.1.0/src/dspeed/processors/get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/histogram.py` & `dspeed-1.1.0/src/dspeed/processors/histogram.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/linear_slope_fit.py` & `dspeed-1.1.0/src/dspeed/processors/linear_slope_fit.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/log_check.py` & `dspeed-1.1.0/src/dspeed/processors/log_check.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/min_max.py` & `dspeed-1.1.0/src/dspeed/processors/min_max.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/moving_windows.py` & `dspeed-1.1.0/src/dspeed/processors/moving_windows.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/multi_a_filter.py` & `dspeed-1.1.0/src/dspeed/processors/multi_a_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/multi_t_filter.py` & `dspeed-1.1.0/src/dspeed/processors/multi_t_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/optimize.py` & `dspeed-1.1.0/src/dspeed/processors/optimize.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/param_lookup.py` & `dspeed-1.1.0/src/dspeed/processors/param_lookup.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/peak_snr_threshold.py` & `dspeed-1.1.0/src/dspeed/processors/peak_snr_threshold.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/pole_zero.py` & `dspeed-1.1.0/src/dspeed/processors/pole_zero.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/presum.py` & `dspeed-1.1.0/src/dspeed/processors/presum.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/pulse_injector.py` & `dspeed-1.1.0/src/dspeed/processors/pulse_injector.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/saturation.py` & `dspeed-1.1.0/src/dspeed/processors/saturation.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/soft_pileup_corr.py` & `dspeed-1.1.0/src/dspeed/processors/soft_pileup_corr.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/time_over_threshold.py` & `dspeed-1.1.0/src/dspeed/processors/time_over_threshold.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/time_point_thresh.py` & `dspeed-1.1.0/src/dspeed/processors/time_point_thresh.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/trap_filters.py` & `dspeed-1.1.0/src/dspeed/processors/trap_filters.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/upsampler.py` & `dspeed-1.1.0/src/dspeed/processors/upsampler.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/wiener_filter.py` & `dspeed-1.1.0/src/dspeed/processors/wiener_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/processors/windower.py` & `dspeed-1.1.0/src/dspeed/processors/windower.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/utils.py` & `dspeed-1.1.0/src/dspeed/utils.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed/vis/waveform_browser.py` & `dspeed-1.1.0/src/dspeed/vis/waveform_browser.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/src/dspeed.egg-info/PKG-INFO` & `dspeed-1.1.0/src/dspeed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspeed
-Version: 1.0.1
+Version: 1.1.0
 Summary: Fast Digital Signal Processing for particle detectors in Python
 Home-page: https://github.com/legend-exp/dspeed
 Author: Ian Guinn
 Author-email: iguinn@email.unc.edu
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dspeed-1.0.1/src/dspeed.egg-info/SOURCES.txt` & `dspeed-1.1.0/src/dspeed.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,12 +61,13 @@
 tests/configs/icpc-dsp-config.json
 tests/configs/numpy-parsing.json
 tests/configs/sipm-dplms-config.json
 tests/configs/sipm-dsp-config.json
 tests/processors/dplms_noise_mat.dat
 tests/processors/test_dplms.py
 tests/processors/test_dwt.py
+tests/processors/test_fftw.py
 tests/processors/test_fixed_time_pickoff.py
 tests/processors/test_get_multi_local_extrema.py
 tests/processors/test_histogram.py
 tests/vis/test_waveform_browser.py
 tests/vis/configs/hpge-dsp-config.json
```

### Comparing `dspeed-1.0.1/tests/configs/icpc-dsp-config.json` & `dspeed-1.1.0/tests/configs/icpc-dsp-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/configs/numpy-parsing.json` & `dspeed-1.1.0/tests/configs/numpy-parsing.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/configs/sipm-dplms-config.json` & `dspeed-1.1.0/tests/configs/sipm-dplms-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/configs/sipm-dsp-config.json` & `dspeed-1.1.0/tests/configs/sipm-dsp-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/conftest.py` & `dspeed-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/processors/dplms_noise_mat.dat` & `dspeed-1.1.0/tests/processors/dplms_noise_mat.dat`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/processors/test_dplms.py` & `dspeed-1.1.0/tests/processors/test_dplms.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/processors/test_dwt.py` & `dspeed-1.1.0/tests/processors/test_dwt.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/processors/test_fixed_time_pickoff.py` & `dspeed-1.1.0/tests/processors/test_fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/processors/test_get_multi_local_extrema.py` & `dspeed-1.1.0/tests/processors/test_get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/processors/test_histogram.py` & `dspeed-1.1.0/tests/processors/test_histogram.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/test_build_dsp.py` & `dspeed-1.1.0/tests/test_build_dsp.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/test_cli.py` & `dspeed-1.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/test_list_parsing.py` & `dspeed-1.1.0/tests/test_list_parsing.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/test_numpy_constants_parsing.py` & `dspeed-1.1.0/tests/test_numpy_constants_parsing.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/test_processing_chain.py` & `dspeed-1.1.0/tests/test_processing_chain.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/vis/configs/hpge-dsp-config.json` & `dspeed-1.1.0/tests/vis/configs/hpge-dsp-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.0.1/tests/vis/test_waveform_browser.py` & `dspeed-1.1.0/tests/vis/test_waveform_browser.py`

 * *Files identical despite different names*

