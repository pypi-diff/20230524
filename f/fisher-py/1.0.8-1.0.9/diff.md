# Comparing `tmp/fisher_py-1.0.8.tar.gz` & `tmp/fisher_py-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fisher_py-1.0.8.tar", last modified: Mon Oct 25 19:24:16 2021, max compression
+gzip compressed data, was "fisher_py-1.0.9.tar", last modified: Sat Dec 25 18:01:10 2021, max compression
```

## Comparing `fisher_py-1.0.8.tar` & `fisher_py-1.0.9.tar`

### file list

```diff
@@ -1,111 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.957355 fisher_py-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2021-10-25 19:24:09.000000 fisher_py-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-25 19:24:09.000000 fisher_py-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2021-10-25 19:24:16.957355 fisher_py-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2021-10-25 19:24:09.000000 fisher_py-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.949355 fisher_py-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-10-25 19:24:09.000000 fisher_py-1.0.8/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25605 2021-10-25 19:24:09.000000 fisher_py-1.0.8/examples/raw_file_reader_example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.949355 fisher_py-1.0.8/fisher_py/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.953355 fisher_py-1.0.8/fisher_py/data/
--rw-r--r--   0 runner    (1001) docker     (121)      957 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.953355 fisher_py-1.0.8/fisher_py/data/business/
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/barcode_status_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/bracket_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/cached_scan_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)    14283 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/centroid_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.957355 fisher_py-1.0.8/fisher_py/data/business/chromatogram_signal/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/chromatogram_signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/chromatogram_signal/chromatogram_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    10753 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/chromatogram_signal_cls.py
--rw-r--r--   0 runner    (1001) docker     (121)     8287 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/chromatogram_trace_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/data_units.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/generic_data_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4900 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/header_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     5929 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/instrument_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/instrument_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3213 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/label_peak.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/log_entry.py
--rw-r--r--   0 runner    (1001) docker     (121)     4340 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/mass_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     4196 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/mass_to_frequency_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/noise_and_baseline.py
--rw-r--r--   0 runner    (1001) docker     (121)     4741 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/range.py
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/range_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3158 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/reaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     5502 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/run_header.py
--rw-r--r--   0 runner    (1001) docker     (121)     9758 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/sample_information.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/sample_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    21095 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/scan.py
--rw-r--r--   0 runner    (1001) docker     (121)    11751 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/scan_statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)    10979 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/segmented_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/sequence_file_writer_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/simple_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/spectrum_packet_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/status_log_values.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/tolerance_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1542 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/trace_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/business/tune_data_values.py
--rw-r--r--   0 runner    (1001) docker     (121)     1964 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/common_core_data_object.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/file_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     7080 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/file_header.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/file_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_accurate_mass.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.957355 fisher_py-1.0.8/fisher_py/data/filter_enums/
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/activation_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/compensation_voltage_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/detector_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/energy_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/event_accurate_mass.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/field_free_region_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      713 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/ionization_mode_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/mass_analyzer_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/ms_order_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/polarity_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/scan_data_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/scan_mode_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/sector_scan_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/source_fragmentation_value_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/filter_enums/tri_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     6372 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/ft_average_options.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/peak_options.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/raw_file_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/scan_dependent_details.py
--rw-r--r--   0 runner    (1001) docker     (121)    21038 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/scan_event.py
--rw-r--r--   0 runner    (1001) docker     (121)    31090 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/scan_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4550 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/sequence_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/sequence_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      170 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/source_fragmentation_info_valid_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/data/tolerance_units.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.957355 fisher_py-1.0.8/fisher_py/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/exceptions/core_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/exceptions/raw_file_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.957355 fisher_py-1.0.8/fisher_py/mass_precision_estimator/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/mass_precision_estimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/mass_precision_estimator/estimator_results.py
--rw-r--r--   0 runner    (1001) docker     (121)     4140 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/mass_precision_estimator/precision_estimate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.957355 fisher_py-1.0.8/fisher_py/net_wrapping/
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/net_wrapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/net_wrapping/net_wrapper_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    17743 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/raw_file.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.957355 fisher_py-1.0.8/fisher_py/raw_file_reader/
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/raw_file_reader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.957355 fisher_py-1.0.8/fisher_py/raw_file_reader/data_model/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/raw_file_reader/data_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4418 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/raw_file_reader/data_model/wrapped_run_header.py
--rw-r--r--   0 runner    (1001) docker     (121)    38443 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/raw_file_reader/raw_file_access.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/raw_file_reader/raw_file_reader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/raw_file_reader/scan_dependents.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-10-25 19:24:09.000000 fisher_py-1.0.8/fisher_py/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:24:16.949355 fisher_py-1.0.8/fisher_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2021-10-25 19:24:16.000000 fisher_py-1.0.8/fisher_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3860 2021-10-25 19:24:16.000000 fisher_py-1.0.8/fisher_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-25 19:24:16.000000 fisher_py-1.0.8/fisher_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-10-25 19:24:16.000000 fisher_py-1.0.8/fisher_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-10-25 19:24:16.000000 fisher_py-1.0.8/fisher_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-25 19:24:16.957355 fisher_py-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      860 2021-10-25 19:24:09.000000 fisher_py-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.981466 fisher_py-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2021-12-25 18:00:58.000000 fisher_py-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-12-25 18:00:58.000000 fisher_py-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3751 2021-12-25 18:01:10.981466 fisher_py-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3177 2021-12-25 18:00:58.000000 fisher_py-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.961466 fisher_py-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2021-12-25 18:00:58.000000 fisher_py-1.0.9/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25605 2021-12-25 18:00:58.000000 fisher_py-1.0.9/examples/raw_file_reader_example.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.965466 fisher_py-1.0.9/fisher_py/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.965466 fisher_py-1.0.9/fisher_py/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.969466 fisher_py-1.0.9/fisher_py/data/business/
+-rw-r--r--   0 runner    (1001) docker     (121)     1977 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/barcode_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/bracket_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/cached_scan_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14283 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/centroid_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.969466 fisher_py-1.0.9/fisher_py/data/business/chromatogram_signal/
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/chromatogram_signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/chromatogram_signal/chromatogram_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10753 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/chromatogram_signal_cls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8287 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/chromatogram_trace_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/data_units.py
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/generic_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4900 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/header_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5929 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/instrument_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/instrument_selection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3213 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/label_peak.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1396 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4340 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/mass_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4196 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/mass_to_frequency_converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/noise_and_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4741 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/range.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/range_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3158 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5502 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/run_header.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9758 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/sample_information.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/sample_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21095 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11751 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/scan_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10979 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/segmented_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/sequence_file_writer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/simple_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/spectrum_packet_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/status_log_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/tolerance_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1542 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/trace_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/business/tune_data_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1964 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/common_core_data_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1482 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/file_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7080 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/file_header.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/file_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_accurate_mass.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.973466 fisher_py-1.0.9/fisher_py/data/filter_enums/
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/activation_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/compensation_voltage_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/detector_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/energy_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/event_accurate_mass.py
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/field_free_region_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/ionization_mode_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/mass_analyzer_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/ms_order_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/polarity_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/scan_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/scan_mode_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/sector_scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/source_fragmentation_value_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/filter_enums/tri_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6372 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/ft_average_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/peak_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/raw_file_classification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1048 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/scan_dependent_details.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21038 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/scan_event.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31090 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/scan_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4550 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/sequence_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/sequence_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/source_fragmentation_info_valid_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/data/tolerance_units.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.977466 fisher_py-1.0.9/fisher_py/dll/
+-rw-r--r--   0 runner    (1001) docker     (121)    60928 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/OpenMcdf.dll
+-rw-r--r--   0 runner    (1001) docker     (121)    51085 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/OpenMcdf.xml
+-rw-r--r--   0 runner    (1001) docker     (121)    44544 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.BackgroundSubtraction.dll
+-rw-r--r--   0 runner    (1001) docker     (121)    23404 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.BackgroundSubtraction.pdb
+-rw-r--r--   0 runner    (1001) docker     (121)   108555 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.BackgroundSubtraction.xml
+-rw-r--r--   0 runner    (1001) docker     (121)   404480 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.Data.dll
+-rw-r--r--   0 runner    (1001) docker     (121)   165480 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.Data.pdb
+-rw-r--r--   0 runner    (1001) docker     (121)  1433699 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.Data.xml
+-rw-r--r--   0 runner    (1001) docker     (121)    11264 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.MassPrecisionEstimator.dll
+-rw-r--r--   0 runner    (1001) docker     (121)     3424 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.MassPrecisionEstimator.pdb
+-rw-r--r--   0 runner    (1001) docker     (121)    12090 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.MassPrecisionEstimator.xml
+-rw-r--r--   0 runner    (1001) docker     (121)   643584 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.RawFileReader.dll
+-rw-r--r--   0 runner    (1001) docker     (121)   271748 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.RawFileReader.pdb
+-rw-r--r--   0 runner    (1001) docker     (121)  1577841 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/dll/ThermoFisher.CommonCore.RawFileReader.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.981466 fisher_py-1.0.9/fisher_py/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/exceptions/core_exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/exceptions/raw_file_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.981466 fisher_py-1.0.9/fisher_py/mass_precision_estimator/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/mass_precision_estimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2500 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/mass_precision_estimator/estimator_results.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4140 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/mass_precision_estimator/precision_estimate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.981466 fisher_py-1.0.9/fisher_py/net_wrapping/
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/net_wrapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/net_wrapping/net_wrapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17743 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/raw_file.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.981466 fisher_py-1.0.9/fisher_py/raw_file_reader/
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/raw_file_reader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.981466 fisher_py-1.0.9/fisher_py/raw_file_reader/data_model/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/raw_file_reader/data_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4418 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/raw_file_reader/data_model/wrapped_run_header.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38443 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/raw_file_reader/raw_file_access.py
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/raw_file_reader/raw_file_reader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1955 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/raw_file_reader/scan_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-12-25 18:00:58.000000 fisher_py-1.0.9/fisher_py/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 18:01:10.965466 fisher_py-1.0.9/fisher_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3751 2021-12-25 18:01:10.000000 fisher_py-1.0.9/fisher_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4610 2021-12-25 18:01:10.000000 fisher_py-1.0.9/fisher_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-25 18:01:10.000000 fisher_py-1.0.9/fisher_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-12-25 18:01:10.000000 fisher_py-1.0.9/fisher_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-12-25 18:01:10.000000 fisher_py-1.0.9/fisher_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-25 18:01:10.981466 fisher_py-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2021-12-25 18:00:58.000000 fisher_py-1.0.9/setup.py
```

### Comparing `fisher_py-1.0.8/LICENSE` & `fisher_py-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/PKG-INFO` & `fisher_py-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisher_py
-Version: 1.0.8
+Version: 1.0.9
 Summary: This python module allows to extract data from the RAW-file-format produces by devices from Thermo Fisher Scientific.
 Home-page: https://github.com/ethz-institute-of-microbiology/fisher_py
 Author: ethz-institute-of-microbiology
 Author-email: dominik.werner@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fisher_py-1.0.8/README.md` & `fisher_py-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/examples/raw_file_reader_example.py` & `fisher_py-1.0.9/examples/raw_file_reader_example.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/__init__.py` & `fisher_py-1.0.9/fisher_py/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/__init__.py` & `fisher_py-1.0.9/fisher_py/data/business/__init__.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/cached_scan_provider.py` & `fisher_py-1.0.9/fisher_py/data/business/cached_scan_provider.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/centroid_stream.py` & `fisher_py-1.0.9/fisher_py/data/business/centroid_stream.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/chromatogram_signal/chromatogram_data.py` & `fisher_py-1.0.9/fisher_py/data/business/chromatogram_signal/chromatogram_data.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/chromatogram_signal_cls.py` & `fisher_py-1.0.9/fisher_py/data/business/chromatogram_signal_cls.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/chromatogram_trace_settings.py` & `fisher_py-1.0.9/fisher_py/data/business/chromatogram_trace_settings.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/header_item.py` & `fisher_py-1.0.9/fisher_py/data/business/header_item.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/instrument_data.py` & `fisher_py-1.0.9/fisher_py/data/business/instrument_data.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/instrument_selection.py` & `fisher_py-1.0.9/fisher_py/data/business/instrument_selection.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/label_peak.py` & `fisher_py-1.0.9/fisher_py/data/business/label_peak.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/log_entry.py` & `fisher_py-1.0.9/fisher_py/data/business/log_entry.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/mass_options.py` & `fisher_py-1.0.9/fisher_py/data/business/mass_options.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/mass_to_frequency_converter.py` & `fisher_py-1.0.9/fisher_py/data/business/mass_to_frequency_converter.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/noise_and_baseline.py` & `fisher_py-1.0.9/fisher_py/data/business/noise_and_baseline.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/range.py` & `fisher_py-1.0.9/fisher_py/data/business/range.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/range_factory.py` & `fisher_py-1.0.9/fisher_py/data/business/range_factory.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/reaction.py` & `fisher_py-1.0.9/fisher_py/data/business/reaction.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/run_header.py` & `fisher_py-1.0.9/fisher_py/data/business/run_header.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/sample_information.py` & `fisher_py-1.0.9/fisher_py/data/business/sample_information.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/scan.py` & `fisher_py-1.0.9/fisher_py/data/business/scan.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/scan_statistics.py` & `fisher_py-1.0.9/fisher_py/data/business/scan_statistics.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/segmented_scan.py` & `fisher_py-1.0.9/fisher_py/data/business/segmented_scan.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/sequence_file_writer_factory.py` & `fisher_py-1.0.9/fisher_py/data/business/sequence_file_writer_factory.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/simple_scan.py` & `fisher_py-1.0.9/fisher_py/data/business/simple_scan.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/spectrum_packet_type.py` & `fisher_py-1.0.9/fisher_py/data/business/spectrum_packet_type.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/status_log_values.py` & `fisher_py-1.0.9/fisher_py/data/business/status_log_values.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/trace_type.py` & `fisher_py-1.0.9/fisher_py/data/business/trace_type.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/business/tune_data_values.py` & `fisher_py-1.0.9/fisher_py/data/business/tune_data_values.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/common_core_data_object.py` & `fisher_py-1.0.9/fisher_py/data/common_core_data_object.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/file_error.py` & `fisher_py-1.0.9/fisher_py/data/file_error.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/file_header.py` & `fisher_py-1.0.9/fisher_py/data/file_header.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/filter_enums/__init__.py` & `fisher_py-1.0.9/fisher_py/data/filter_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/filter_enums/activation_type.py` & `fisher_py-1.0.9/fisher_py/data/filter_enums/activation_type.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/filter_enums/ionization_mode_type.py` & `fisher_py-1.0.9/fisher_py/data/filter_enums/ionization_mode_type.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/ft_average_options.py` & `fisher_py-1.0.9/fisher_py/data/ft_average_options.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/scan_dependent_details.py` & `fisher_py-1.0.9/fisher_py/data/scan_dependent_details.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/scan_event.py` & `fisher_py-1.0.9/fisher_py/data/scan_event.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/scan_filter.py` & `fisher_py-1.0.9/fisher_py/data/scan_filter.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/sequence_file_writer.py` & `fisher_py-1.0.9/fisher_py/data/sequence_file_writer.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/data/sequence_info.py` & `fisher_py-1.0.9/fisher_py/data/sequence_info.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/mass_precision_estimator/estimator_results.py` & `fisher_py-1.0.9/fisher_py/mass_precision_estimator/estimator_results.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/mass_precision_estimator/precision_estimate.py` & `fisher_py-1.0.9/fisher_py/mass_precision_estimator/precision_estimate.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/net_wrapping/__init__.py` & `fisher_py-1.0.9/fisher_py/net_wrapping/__init__.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/net_wrapping/net_wrapper_base.py` & `fisher_py-1.0.9/fisher_py/net_wrapping/net_wrapper_base.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/raw_file.py` & `fisher_py-1.0.9/fisher_py/raw_file.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/raw_file_reader/data_model/wrapped_run_header.py` & `fisher_py-1.0.9/fisher_py/raw_file_reader/data_model/wrapped_run_header.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/raw_file_reader/raw_file_access.py` & `fisher_py-1.0.9/fisher_py/raw_file_reader/raw_file_access.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/raw_file_reader/raw_file_reader_adapter.py` & `fisher_py-1.0.9/fisher_py/raw_file_reader/raw_file_reader_adapter.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/raw_file_reader/scan_dependents.py` & `fisher_py-1.0.9/fisher_py/raw_file_reader/scan_dependents.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py/utils.py` & `fisher_py-1.0.9/fisher_py/utils.py`

 * *Files identical despite different names*

### Comparing `fisher_py-1.0.8/fisher_py.egg-info/PKG-INFO` & `fisher_py-1.0.9/fisher_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisher-py
-Version: 1.0.8
+Version: 1.0.9
 Summary: This python module allows to extract data from the RAW-file-format produces by devices from Thermo Fisher Scientific.
 Home-page: https://github.com/ethz-institute-of-microbiology/fisher_py
 Author: ethz-institute-of-microbiology
 Author-email: dominik.werner@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fisher_py-1.0.8/fisher_py.egg-info/SOURCES.txt` & `fisher_py-1.0.9/fisher_py.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -76,14 +76,28 @@
 fisher_py/data/filter_enums/ms_order_type.py
 fisher_py/data/filter_enums/polarity_type.py
 fisher_py/data/filter_enums/scan_data_type.py
 fisher_py/data/filter_enums/scan_mode_type.py
 fisher_py/data/filter_enums/sector_scan_type.py
 fisher_py/data/filter_enums/source_fragmentation_value_type.py
 fisher_py/data/filter_enums/tri_state.py
+fisher_py/dll/OpenMcdf.dll
+fisher_py/dll/OpenMcdf.xml
+fisher_py/dll/ThermoFisher.CommonCore.BackgroundSubtraction.dll
+fisher_py/dll/ThermoFisher.CommonCore.BackgroundSubtraction.pdb
+fisher_py/dll/ThermoFisher.CommonCore.BackgroundSubtraction.xml
+fisher_py/dll/ThermoFisher.CommonCore.Data.dll
+fisher_py/dll/ThermoFisher.CommonCore.Data.pdb
+fisher_py/dll/ThermoFisher.CommonCore.Data.xml
+fisher_py/dll/ThermoFisher.CommonCore.MassPrecisionEstimator.dll
+fisher_py/dll/ThermoFisher.CommonCore.MassPrecisionEstimator.pdb
+fisher_py/dll/ThermoFisher.CommonCore.MassPrecisionEstimator.xml
+fisher_py/dll/ThermoFisher.CommonCore.RawFileReader.dll
+fisher_py/dll/ThermoFisher.CommonCore.RawFileReader.pdb
+fisher_py/dll/ThermoFisher.CommonCore.RawFileReader.xml
 fisher_py/exceptions/__init__.py
 fisher_py/exceptions/core_exception.py
 fisher_py/exceptions/raw_file_exception.py
 fisher_py/mass_precision_estimator/__init__.py
 fisher_py/mass_precision_estimator/estimator_results.py
 fisher_py/mass_precision_estimator/precision_estimate.py
 fisher_py/net_wrapping/__init__.py
```

### Comparing `fisher_py-1.0.8/setup.py` & `fisher_py-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='fisher_py',
-    version='1.0.8',
+    version='1.0.9',
     author='ethz-institute-of-microbiology',
     author_email='dominik.werner@live.com',
     description='This python module allows to extract data from the RAW-file-format produces by devices from Thermo Fisher Scientific.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ethz-institute-of-microbiology/fisher_py',
     packages=setuptools.find_packages(),
```

