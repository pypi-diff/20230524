# Comparing `tmp/pysiml-0.2.9.dev202305021032-py3-none-any.whl.zip` & `tmp/pysiml-0.2.9.dev202305240600-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,31 @@
-Zip file size: 151913 bytes, number of entries: 113
+Zip file size: 171441 bytes, number of entries: 137
 -rw-r--r--  2.0 unx     1520 b- defN 80-Jan-01 00:00 pyproject.toml
 -rw-r--r--  2.0 unx      638 b- defN 80-Jan-01 00:00 siml/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 siml/__main__/__init__.py
 -rw-r--r--  2.0 unx      900 b- defN 80-Jan-01 00:00 siml/__main__/convert_interim_data.py
 -rw-r--r--  2.0 unx     1400 b- defN 80-Jan-01 00:00 siml/__main__/convert_raw_data.py
 -rw-r--r--  2.0 unx     1742 b- defN 80-Jan-01 00:00 siml/__main__/optimize.py
 -rw-r--r--  2.0 unx     8663 b- defN 80-Jan-01 00:00 siml/__main__/plot_losses.py
 -rw-r--r--  2.0 unx      927 b- defN 80-Jan-01 00:00 siml/__main__/prepare_preprocess_converters.py
 -rw-r--r--  2.0 unx      717 b- defN 80-Jan-01 00:00 siml/__main__/preprocess_interim_data.py
 -rw-r--r--  2.0 unx     1376 b- defN 80-Jan-01 00:00 siml/__main__/train.py
 -rw-r--r--  2.0 unx     3961 b- defN 80-Jan-01 00:00 siml/__main__/visualize_graph.py
+-rw-r--r--  2.0 unx      139 b- defN 80-Jan-01 00:00 siml/base/siml_const.py
+-rw-r--r--  2.0 unx      579 b- defN 80-Jan-01 00:00 siml/base/siml_enums.py
+-rw-r--r--  2.0 unx      228 b- defN 80-Jan-01 00:00 siml/base/siml_typing.py
 -rw-r--r--  2.0 unx       57 b- defN 80-Jan-01 00:00 siml/config.py
 -rw-r--r--  2.0 unx     3520 b- defN 80-Jan-01 00:00 siml/data_parallel.py
--rw-r--r--  2.0 unx    26681 b- defN 80-Jan-01 00:00 siml/datasets.py
--rw-r--r--  2.0 unx    27000 b- defN 80-Jan-01 00:00 siml/inferer.py
--rw-r--r--  2.0 unx     1466 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_assignment.py
--rw-r--r--  2.0 unx     3734 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_calculator.py
--rw-r--r--  2.0 unx     2064 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_selector.py
--rw-r--r--  2.0 unx       58 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_type.py
+-rw-r--r--  2.0 unx    25525 b- defN 80-Jan-01 00:00 siml/datasets.py
+-rw-r--r--  2.0 unx    26560 b- defN 80-Jan-01 00:00 siml/inferer.py
+-rw-r--r--  2.0 unx       84 b- defN 80-Jan-01 00:00 siml/loss_operations/__init__.py
+-rw-r--r--  2.0 unx     1463 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_assignment.py
+-rw-r--r--  2.0 unx     4057 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_calculator.py
+-rw-r--r--  2.0 unx     1960 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_calculator_builder.py
+-rw-r--r--  2.0 unx     2045 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_selector.py
 -rw-r--r--  2.0 unx     1364 b- defN 80-Jan-01 00:00 siml/mains.py
 -rw-r--r--  2.0 unx     2724 b- defN 80-Jan-01 00:00 siml/networks/__init__.py
 -rw-r--r--  2.0 unx    11337 b- defN 80-Jan-01 00:00 siml/networks/abstract_equivariant_gnn.py
 -rw-r--r--  2.0 unx     6505 b- defN 80-Jan-01 00:00 siml/networks/abstract_gcn.py
 -rw-r--r--  2.0 unx     1007 b- defN 80-Jan-01 00:00 siml/networks/activation.py
 -rw-r--r--  2.0 unx     4565 b- defN 80-Jan-01 00:00 siml/networks/activations.py
 -rw-r--r--  2.0 unx      715 b- defN 80-Jan-01 00:00 siml/networks/array2diagmat.py
@@ -63,53 +67,73 @@
 -rw-r--r--  2.0 unx     3260 b- defN 80-Jan-01 00:00 siml/networks/tcn.py
 -rw-r--r--  2.0 unx     5969 b- defN 80-Jan-01 00:00 siml/networks/tensor_operations.py
 -rw-r--r--  2.0 unx     1415 b- defN 80-Jan-01 00:00 siml/networks/threshold.py
 -rw-r--r--  2.0 unx      782 b- defN 80-Jan-01 00:00 siml/networks/time_norm.py
 -rw-r--r--  2.0 unx     1882 b- defN 80-Jan-01 00:00 siml/networks/translator.py
 -rw-r--r--  2.0 unx     1034 b- defN 80-Jan-01 00:00 siml/networks/upper_limit.py
 -rw-r--r--  2.0 unx     6940 b- defN 80-Jan-01 00:00 siml/optimize.py
--rw-r--r--  2.0 unx      125 b- defN 80-Jan-01 00:00 siml/path_like_objects/__init__.py
--rw-r--r--  2.0 unx     1119 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_directory.py
--rw-r--r--  2.0 unx     5982 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_file.py
--rw-r--r--  2.0 unx     5523 b- defN 80-Jan-01 00:00 siml/postprocessor.py
--rw-r--r--  2.0 unx    25936 b- defN 80-Jan-01 00:00 siml/prepost.py
--rw-r--r--  2.0 unx      148 b- defN 80-Jan-01 00:00 siml/preprocessing/__init__.py
--rw-r--r--  2.0 unx    20772 b- defN 80-Jan-01 00:00 siml/preprocessing/converter.py
--rw-r--r--  2.0 unx     9702 b- defN 80-Jan-01 00:00 siml/preprocessing/scalers_composition.py
--rw-r--r--  2.0 unx    10594 b- defN 80-Jan-01 00:00 siml/preprocessing/scaling_converter.py
+-rw-r--r--  2.0 unx      159 b- defN 80-Jan-01 00:00 siml/path_like_objects/__init__.py
+-rw-r--r--  2.0 unx     2735 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_directory.py
+-rw-r--r--  2.0 unx      736 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_file_builder.py
+-rw-r--r--  2.0 unx      289 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_files/__init__.py
+-rw-r--r--  2.0 unx     3245 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_files/checkpoint_file.py
+-rw-r--r--  2.0 unx     2268 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_files/interface.py
+-rw-r--r--  2.0 unx     3776 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_files/numpy_file.py
+-rw-r--r--  2.0 unx     2733 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_files/pickle_file.py
+-rw-r--r--  2.0 unx     2850 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_files/yaml_file.py
+-rw-r--r--  2.0 unx    12361 b- defN 80-Jan-01 00:00 siml/prepost.py
+-rw-r--r--  2.0 unx      160 b- defN 80-Jan-01 00:00 siml/preprocessing/__init__.py
+-rw-r--r--  2.0 unx    21038 b- defN 80-Jan-01 00:00 siml/preprocessing/converter.py
+-rw-r--r--  2.0 unx     9465 b- defN 80-Jan-01 00:00 siml/preprocessing/scalers_composition.py
+-rw-r--r--  2.0 unx    11050 b- defN 80-Jan-01 00:00 siml/preprocessing/scaling_converter.py
 -rw-r--r--  2.0 unx      176 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/__init__.py
 -rw-r--r--  2.0 unx     1405 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/__init__.py
 -rw-r--r--  2.0 unx      592 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/identity_scaler.py
 -rw-r--r--  2.0 unx      738 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/interface_scaler.py
 -rw-r--r--  2.0 unx     2038 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/isoam_scaler.py
 -rw-r--r--  2.0 unx     1403 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/max_abs_scaler.py
 -rw-r--r--  2.0 unx      465 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/min_max_scaler.py
 -rw-r--r--  2.0 unx     1926 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/sparse_standard_scaler.py
 -rw-r--r--  2.0 unx      570 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/standard_scaler.py
 -rw-r--r--  2.0 unx      865 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/user_defined_scaler.py
 -rw-r--r--  2.0 unx     1012 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scaler_result_save.py
--rw-r--r--  2.0 unx     4326 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scaler_wrapper.py
--rw-r--r--  2.0 unx    49064 b- defN 80-Jan-01 00:00 siml/setting.py
+-rw-r--r--  2.0 unx     4367 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scaler_wrapper.py
+-rw-r--r--  2.0 unx      154 b- defN 80-Jan-01 00:00 siml/services/__init__.py
+-rw-r--r--  2.0 unx     2342 b- defN 80-Jan-01 00:00 siml/services/environment.py
+-rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 siml/services/inference/__init__.py
+-rw-r--r--  2.0 unx     2587 b- defN 80-Jan-01 00:00 siml/services/inference/core_inferer.py
+-rw-r--r--  2.0 unx     1709 b- defN 80-Jan-01 00:00 siml/services/inference/data_loader_builder.py
+-rw-r--r--  2.0 unx     2613 b- defN 80-Jan-01 00:00 siml/services/inference/engine_bulider.py
+-rw-r--r--  2.0 unx     4660 b- defN 80-Jan-01 00:00 siml/services/inference/inner_setting.py
+-rw-r--r--  2.0 unx     4716 b- defN 80-Jan-01 00:00 siml/services/inference/metrics_builder.py
+-rw-r--r--  2.0 unx      203 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/__init__.py
+-rw-r--r--  2.0 unx     5159 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/post_fem_data.py
+-rw-r--r--  2.0 unx     6246 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/postprocessor.py
+-rw-r--r--  2.0 unx     8781 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/save_processor.py
+-rw-r--r--  2.0 unx      682 b- defN 80-Jan-01 00:00 siml/services/inference/record_object.py
+-rw-r--r--  2.0 unx     2574 b- defN 80-Jan-01 00:00 siml/services/model_builder.py
+-rw-r--r--  2.0 unx     4978 b- defN 80-Jan-01 00:00 siml/services/model_selector.py
+-rw-r--r--  2.0 unx     7124 b- defN 80-Jan-01 00:00 siml/services/path_rules.py
+-rw-r--r--  2.0 unx    50226 b- defN 80-Jan-01 00:00 siml/setting.py
 -rw-r--r--  2.0 unx    11036 b- defN 80-Jan-01 00:00 siml/siml_manager.py
--rw-r--r--  2.0 unx      147 b- defN 80-Jan-01 00:00 siml/siml_variables/__init__.py
--rw-r--r--  2.0 unx      648 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/__init__.py
+-rw-r--r--  2.0 unx      163 b- defN 80-Jan-01 00:00 siml/siml_variables/__init__.py
+-rw-r--r--  2.0 unx      594 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/__init__.py
 -rw-r--r--  2.0 unx     1573 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/interface_wrapper.py
 -rw-r--r--  2.0 unx     1398 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/ndarray_wrapper.py
--rw-r--r--  2.0 unx     1862 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/sparce_array_wrapper.py
--rw-r--r--  2.0 unx     3509 b- defN 80-Jan-01 00:00 siml/siml_variables/tensor_variables/tensor_variables.py
+-rw-r--r--  2.0 unx     1809 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/sparce_array_wrapper.py
+-rw-r--r--  2.0 unx     4156 b- defN 80-Jan-01 00:00 siml/siml_variables/tensor_variables/tensor_variables.py
 -rw-r--r--  2.0 unx    13021 b- defN 80-Jan-01 00:00 siml/study.py
 -rw-r--r--  2.0 unx    34886 b- defN 80-Jan-01 00:00 siml/trainer.py
 -rw-r--r--  2.0 unx      211 b- defN 80-Jan-01 00:00 siml/update_functions/__init__.py
 -rw-r--r--  2.0 unx     1774 b- defN 80-Jan-01 00:00 siml/update_functions/element_batch_update.py
 -rw-r--r--  2.0 unx     3623 b- defN 80-Jan-01 00:00 siml/update_functions/pseudo_batch_update.py
 -rw-r--r--  2.0 unx     2702 b- defN 80-Jan-01 00:00 siml/update_functions/standard_update.py
 -rw-r--r--  2.0 unx      429 b- defN 80-Jan-01 00:00 siml/update_functions/update_interface.py
 -rw-r--r--  2.0 unx    23027 b- defN 80-Jan-01 00:00 siml/util.py
--rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 siml/utils/__init__.py
--rw-r--r--  2.0 unx     6090 b- defN 80-Jan-01 00:00 siml/utils/fem_data_utils.py
--rw-r--r--  2.0 unx     2147 b- defN 80-Jan-01 00:00 siml/utils/path_utils.py
--rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305021032.dist-info/LICENSE
--rw-r--r--  2.0 unx     1638 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305021032.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305021032.dist-info/WHEEL
--rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305021032.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    10109 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202305021032.dist-info/RECORD
-113 files, 552017 bytes uncompressed, 135821 bytes compressed:  75.4%
+-rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 siml/utils/__init__.py
+-rw-r--r--  2.0 unx     7682 b- defN 80-Jan-01 00:00 siml/utils/fem_data_utils.py
+-rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305240600.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1638 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305240600.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305240600.dist-info/WHEEL
+-rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305240600.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    12471 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202305240600.dist-info/RECORD
+137 files, 604936 bytes uncompressed, 151519 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -27,36 +27,48 @@
 
 Filename: siml/__main__/train.py
 Comment: 
 
 Filename: siml/__main__/visualize_graph.py
 Comment: 
 
+Filename: siml/base/siml_const.py
+Comment: 
+
+Filename: siml/base/siml_enums.py
+Comment: 
+
+Filename: siml/base/siml_typing.py
+Comment: 
+
 Filename: siml/config.py
 Comment: 
 
 Filename: siml/data_parallel.py
 Comment: 
 
 Filename: siml/datasets.py
 Comment: 
 
 Filename: siml/inferer.py
 Comment: 
 
+Filename: siml/loss_operations/__init__.py
+Comment: 
+
 Filename: siml/loss_operations/loss_assignment.py
 Comment: 
 
 Filename: siml/loss_operations/loss_calculator.py
 Comment: 
 
-Filename: siml/loss_operations/loss_selector.py
+Filename: siml/loss_operations/loss_calculator_builder.py
 Comment: 
 
-Filename: siml/loss_operations/loss_type.py
+Filename: siml/loss_operations/loss_selector.py
 Comment: 
 
 Filename: siml/mains.py
 Comment: 
 
 Filename: siml/networks/__init__.py
 Comment: 
@@ -204,18 +216,33 @@
 
 Filename: siml/path_like_objects/__init__.py
 Comment: 
 
 Filename: siml/path_like_objects/siml_directory.py
 Comment: 
 
-Filename: siml/path_like_objects/siml_file.py
+Filename: siml/path_like_objects/siml_file_builder.py
+Comment: 
+
+Filename: siml/path_like_objects/siml_files/__init__.py
+Comment: 
+
+Filename: siml/path_like_objects/siml_files/checkpoint_file.py
 Comment: 
 
-Filename: siml/postprocessor.py
+Filename: siml/path_like_objects/siml_files/interface.py
+Comment: 
+
+Filename: siml/path_like_objects/siml_files/numpy_file.py
+Comment: 
+
+Filename: siml/path_like_objects/siml_files/pickle_file.py
+Comment: 
+
+Filename: siml/path_like_objects/siml_files/yaml_file.py
 Comment: 
 
 Filename: siml/prepost.py
 Comment: 
 
 Filename: siml/preprocessing/__init__.py
 Comment: 
@@ -261,14 +288,62 @@
 
 Filename: siml/preprocessing/siml_scalers/scaler_result_save.py
 Comment: 
 
 Filename: siml/preprocessing/siml_scalers/scaler_wrapper.py
 Comment: 
 
+Filename: siml/services/__init__.py
+Comment: 
+
+Filename: siml/services/environment.py
+Comment: 
+
+Filename: siml/services/inference/__init__.py
+Comment: 
+
+Filename: siml/services/inference/core_inferer.py
+Comment: 
+
+Filename: siml/services/inference/data_loader_builder.py
+Comment: 
+
+Filename: siml/services/inference/engine_bulider.py
+Comment: 
+
+Filename: siml/services/inference/inner_setting.py
+Comment: 
+
+Filename: siml/services/inference/metrics_builder.py
+Comment: 
+
+Filename: siml/services/inference/postprocessing/__init__.py
+Comment: 
+
+Filename: siml/services/inference/postprocessing/post_fem_data.py
+Comment: 
+
+Filename: siml/services/inference/postprocessing/postprocessor.py
+Comment: 
+
+Filename: siml/services/inference/postprocessing/save_processor.py
+Comment: 
+
+Filename: siml/services/inference/record_object.py
+Comment: 
+
+Filename: siml/services/model_builder.py
+Comment: 
+
+Filename: siml/services/model_selector.py
+Comment: 
+
+Filename: siml/services/path_rules.py
+Comment: 
+
 Filename: siml/setting.py
 Comment: 
 
 Filename: siml/siml_manager.py
 Comment: 
 
 Filename: siml/siml_variables/__init__.py
@@ -315,26 +390,23 @@
 
 Filename: siml/utils/__init__.py
 Comment: 
 
 Filename: siml/utils/fem_data_utils.py
 Comment: 
 
-Filename: siml/utils/path_utils.py
-Comment: 
-
-Filename: pysiml-0.2.9.dev202305021032.dist-info/LICENSE
+Filename: pysiml-0.2.9.dev202305240600.dist-info/LICENSE
 Comment: 
 
-Filename: pysiml-0.2.9.dev202305021032.dist-info/METADATA
+Filename: pysiml-0.2.9.dev202305240600.dist-info/METADATA
 Comment: 
 
-Filename: pysiml-0.2.9.dev202305021032.dist-info/WHEEL
+Filename: pysiml-0.2.9.dev202305240600.dist-info/WHEEL
 Comment: 
 
-Filename: pysiml-0.2.9.dev202305021032.dist-info/entry_points.txt
+Filename: pysiml-0.2.9.dev202305240600.dist-info/entry_points.txt
 Comment: 
 
-Filename: pysiml-0.2.9.dev202305021032.dist-info/RECORD
+Filename: pysiml-0.2.9.dev202305240600.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyproject.toml

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysiml"
-version = "0.2.9.dev202305021032"
+version = "0.2.9.dev202305240600"
 description = "SiML - a Simulation ML library"
 license = "Apache-2.0"
 authors = ["RICOS Co. Ltd."]
 readme = "README.md"
 repository = "https://github.com/ricosjp/pysiml"
 documentation = "https://ricosjp.github.io/pysiml/"
 packages = [
```

## siml/datasets.py

```diff
@@ -1,17 +1,17 @@
 import multiprocessing as multi
+import pathlib
 
-import femio
-from ignite.utils import convert_tensor
 import numpy as np
 import torch
+from ignite.utils import convert_tensor
 from tqdm import tqdm
 
-from .utils import fem_data_utils
-from . import util
+from siml import util
+from siml.preprocessing import RawConverter, ScalersComposition
 
 
 class BaseDataset(torch.utils.data.Dataset):
 
     def __init__(
             self, x_variable_names, y_variable_names, directories, *,
             supports=None, num_workers=0, allow_no_data=False,
@@ -37,14 +37,15 @@
 
         if self.recursive:
             data_directories = []
             for directory in directories:
                 data_directories += util.collect_data_directories(
                     directory, required_file_names=required_file_names,
                     allow_no_data=allow_no_data)
+
             self.data_directories = np.unique(data_directories)
         else:
             self.data_directories = directories
 
         list_y_variable_names = self._get_list_variable_names(
             self.y_variable_names)
         if len(self.data_directories) > 0:
@@ -173,52 +174,32 @@
         return self._load_data(data_directory)
 
 
 class PreprocessDataset(BaseDataset):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.prepost_converter = kwargs.get('prepost_converter')
-        self.raw_data_stem = kwargs.get('raw_data_stem', None)
-        self.conversion_function = kwargs.get('conversion_function', None)
-        self.load_function = kwargs.get('load_function', None)
-        self.conversion_setting = kwargs.get('conversion_setting', None)
-        return
+        self.raw_converter: RawConverter \
+            = kwargs.get("raw_converter")
+        self.scalers: ScalersComposition \
+            = kwargs.get("scalers")
 
     def __getitem__(self, i):
         data_directory = self.data_directories[i]
         return self._preprocess_data(data_directory)
 
-    def _preprocess_data(self, raw_data_directory):
-        if self.conversion_setting.skip_femio:
-            dict_data = {}
-            fem_data = None
-        else:
-            fem_data = femio.FEMData.read_directory(
-                self.conversion_setting.file_type, raw_data_directory,
-                save=False)
-            wrapped_data = fem_data_utils.FemDataWrapper(fem_data)
-            dict_data = wrapped_data.extract_variables(
-                self.conversion_setting.mandatory,
-                optional_variables=self.conversion_setting.optional
-            )
-
-        if self.conversion_function is not None:
-            dict_data.update(self.conversion_function(
-                fem_data, raw_data_directory))
-
-        if self.load_function is not None:
-            data_files = util.collect_files(
-                raw_data_directory,
-                self.conversion_setting.required_file_names)
-            loaded_dict_data, _ = self.load_function(
-                data_files, raw_data_directory)
-            dict_data.update(loaded_dict_data)
-
-        converted_dict_data = self.prepost_converter.preprocess(dict_data)
+    def _preprocess_data(self, raw_data_directory: pathlib.Path):
+        dict_data = self.raw_converter.convert_single_data(
+            raw_path=raw_data_directory,
+            return_results=True
+        )
+        dict_data = dict_data[str(raw_data_directory)]
+        converted_dict_data = self.scalers.transform_dict(
+            dict_data
+        )
         x_data = self._merge_data(
             converted_dict_data, self.x_variable_names)
 
         if np.all([
                 y_variable_names in converted_dict_data
                 for y_variable_names in self.y_variable_names]):
             y_data = self._merge_data(
@@ -282,22 +263,20 @@
         return self.data[i]
 
 
 class SimplifiedDataset(BaseDataset):
 
     def __init__(
             self, x_variable_names, y_variable_names, raw_dict_x,
-            prepost_converter,
             *, answer_raw_dict_y=None, num_workers=0, **kwargs):
         self.x_variable_names = x_variable_names
         self.y_variable_names = y_variable_names
         self.raw_dict_x = raw_dict_x
         self.answer_raw_dict_y = answer_raw_dict_y
         self.num_workers = num_workers
-        self.prepost_converter = prepost_converter
 
         self.x_dict_mode = isinstance(self.x_variable_names, dict)
         self.y_dict_mode = isinstance(self.y_variable_names, dict)
 
         if self.x_dict_mode:
             self.first_variable_name = list(
                 self.x_variable_names.values())[0][0]
@@ -305,23 +284,22 @@
             self.first_variable_name = self.x_variable_names[0]
         return
 
     def __len__(self):
         return 1
 
     def __getitem__(self, i):
-        converted_dict_data = self.prepost_converter.preprocess(
-            self.raw_dict_x)
+        dict_data = self.raw_dict_x
         x_data = self._merge_data(
-            converted_dict_data, self.x_variable_names)
+            dict_data,
+            self.x_variable_names
+        )
         if self.answer_raw_dict_y is not None:
-            converted_dict_data.update(self.prepost_converter.preprocess(
-                self.answer_raw_dict_y))
-            y_data = self._merge_data(
-                converted_dict_data, self.y_variable_names)
+            dict_data.update(self.answer_raw_dict_y)
+            y_data = self._merge_data(dict_data, self.y_variable_names)
         else:
             y_data = None
 
         return {
             'x': x_data, 't': y_data, 'data_directory': None}
```

## siml/inferer.py

```diff
@@ -1,197 +1,459 @@
-import io
+from __future__ import annotations
 import pathlib
-import shutil
-import time
-from typing import Callable
+from typing import Callable, Optional, Union
 
-import ignite
 import numpy as np
-import pandas as pd
-import torch
 from torch import Tensor
+from torch.utils.data import DataLoader
 
-from . import datasets
-from . import networks
-from . import postprocessor
-from . import prepost
-from . import setting
-from . import siml_manager
-from . import util
-from .utils import path_utils
+from siml import datasets, setting
+from siml.base.siml_const import SimlConstItems
+from siml.loss_operations import LossCalculatorBuilder
+from siml.path_like_objects import SimlDirectory, SimlFileBuilder
+from siml.preprocessing import ScalersComposition
+from siml.preprocessing.converter import (
+    ILoadFunction, IConvertFunction, RawConverter)
+from siml.services import ModelEnvironmentSetting, ModelSelectorBuilder
+from siml.services.inference import (
+    CoreInferer, InferenceDataLoaderBuilder, InnerInfererSetting,
+    PostPredictionRecord
+)
+from siml.services.inference.postprocessing import (
+    IInfererSaveFunction, SaveProcessor, PostProcessor,
+    PostFEMDataConverter, IFEMDataAdditionFunction
+)
 
 
-class Inferer(siml_manager.SimlManager):
+class WholeInferProcessor:
+    def __init__(
+        self,
+        main_setting: setting.MainSetting,
+        model_path: Optional[pathlib.Path] = None,
+        converter_parameters_pkl: Optional[pathlib.Path] = None,
+        conversion_function: Optional[IConvertFunction] = None,
+        load_function: Optional[ILoadFunction] = None,
+        data_addition_function: Optional[IFEMDataAdditionFunction] = None,
+        save_function: Optional[IInfererSaveFunction] = None,
+        user_loss_function_dic:
+        dict[str, Callable[[Tensor, Tensor], Tensor]] = None
+    ) -> dict:
+
+        self.raw_converter = RawConverter(
+            main_setting=main_setting,
+            conversion_function=conversion_function,
+            load_function=load_function
+        )
+
+        _inner_setting = InnerInfererSetting(
+            main_setting=main_setting,
+            force_model_path=model_path,
+            force_converter_parameters_pkl=converter_parameters_pkl
+        )
+        pkl_path = _inner_setting.get_converter_parameters_pkl_path()
+        self.scalers = ScalersComposition.create_from_file(
+            converter_parameters_pkl=pkl_path,
+            key=main_setting.get_crypt_key()
+        )
+
+        self.inferer = Inferer(
+            main_setting=main_setting,
+            model_path=model_path,
+            scalers=self.scalers,
+            load_function=load_function,
+            data_addition_function=data_addition_function,
+            save_function=save_function,
+            user_loss_function_dic=user_loss_function_dic
+        )
+
+    def run(
+        self,
+        data_directories: Union[list[pathlib.Path], pathlib.Path],
+        output_directory_base: Optional[pathlib.Path] = None,
+        perform_preprocess: bool = True,
+        save: Optional[bool] = None
+    ) -> dict:
+        """run whole inference processes.
+
+        Parameters
+        ----------
+        data_directories : Union[list[pathlib.Path], pathlib.Path]
+            pathes to data
+        output_directory_base : Optional[pathlib.Path], optional
+            path to parent directory of cases, by default None
+        perform_preprocess : bool, optional
+            If True, perform preprocessing and scaling, by default True
+        save : Optional[bool], optional
+            If True, save items, by default None
+
+        Returns
+        -------
+        dict
+            dictionary of results
+        """
+        if perform_preprocess:
+            return self._run_with_preprocess(
+                data_directories=data_directories,
+                output_directory_base=output_directory_base,
+                save=save
+            )
+        else:
+            return self.inferer.infer(
+                data_directories=data_directories,
+                output_directory_base=output_directory_base,
+                save=save
+            )
+
+    def _run_with_preprocess(
+        self,
+        data_directories: Union[list[pathlib.Path], pathlib.Path],
+        output_directory_base: Optional[pathlib.Path] = None,
+        save: Optional[bool] = None
+    ) -> dict:
+        if isinstance(data_directories, pathlib.Path):
+            data_directories = [data_directories]
+
+        inner_setting = self.inferer._inner_setting
+        conversion_setting = inner_setting.conversion_setting
+        dataset = datasets.PreprocessDataset(
+            inner_setting.trainer_setting.input_names,
+            inner_setting.trainer_setting.output_names,
+            data_directories,
+            supports=inner_setting.trainer_setting.support_inputs,
+            num_workers=0,
+            allow_no_data=True,
+            decrypt_key=inner_setting.get_crypt_key(),
+            raw_converter=self.raw_converter,
+            scalers=self.scalers,
+            required_file_names=conversion_setting.required_file_names,
+            conversion_setting=conversion_setting
+        )
+        return self.inferer.infer_dataset(
+            dataset, output_directory_base=output_directory_base, save=save
+        )
+
+    def run_dict_data(
+        self,
+        raw_dict_x: dict,
+        *,
+        answer_raw_dict_y: Optional[dict] = None,
+        perform_preprocess: bool = True
+    ) -> dict:
+        """_summary_
+
+        Parameters
+        ----------
+        raw_dict_x : dict
+            Dict of raw x data.
+        answer_raw_dict_y : Optional[dict], optional
+            Dict of raw answer y data, by default None
+        perform_preprocess : bool, optional
+            If True, perform scaling. by default True
+
+        Returns
+        -------
+        dict
+            dictionary of result
+        """
+
+        if perform_preprocess:
+            scaled_dict_x = self.scalers.transform_dict(raw_dict_x)
+            if answer_raw_dict_y is not None:
+                scaled_dict_answer = self.scalers.transform_dict(
+                    answer_raw_dict_y
+                )
+            else:
+                scaled_dict_answer = None
+
+            results = self.inferer.infer_dict_data(
+                scaled_dict_x, scaled_dict_answer=scaled_dict_answer
+            )
+            return results
+        else:
+            return self.inferer.infer_dict_data(
+                raw_dict_x, scaled_dict_answer=answer_raw_dict_y
+            )
+
+
+class Inferer():
 
     @classmethod
-    def read_settings(cls, settings_yaml, **kwargs):
+    def read_settings_file(
+        cls,
+        settings_yaml: pathlib.Path,
+        model_path: Optional[pathlib.Path] = None,
+        converter_parameters_pkl: Optional[pathlib.Path] = None,
+        **kwargs
+    ) -> Inferer:
         """Read settings.yaml to generate Inferer object.
 
         Parameters
         ----------
-        settings_yaml: str or pathlib.Path
-            setting.yaml file name.
+        settings_yaml : pathlib.Path
+            Path to yaml file of setting
+        model_path : Optional[pathlib.Path], optional
+            If fed, overwrite path to model file, by default None
+        converter_parameters_pkl : Optional[pathlib.Path], optional
+            If fed, overwrite path to pkl file of scaling parameters,
+             by default None
 
         Returns
-        --------
-        siml.Inferer
+        -------
+        Inferer
+            Inferer object
         """
         main_setting = setting.MainSetting.read_settings_yaml(settings_yaml)
-        return cls(main_setting, **kwargs)
+        return cls(
+            main_setting=main_setting,
+            model_path=model_path,
+            converter_parameters_pkl=converter_parameters_pkl,
+            **kwargs
+        )
 
     @classmethod
-    def from_model_directory(cls,
-                             model_directory,
-                             decrypt_key=None,
-                             infer_epoch: int = None,
-                             **kwargs):
+    def from_model_directory(
+        cls,
+        model_directory: pathlib.Path,
+        converter_parameters_pkl: Optional[pathlib.Path] = None,
+        model_select_method: str = "best",
+        decrypt_key: bytes = None,
+        infer_epoch: int = None,
+        **kwargs
+    ):
         """Load model data from a deployed directory.
 
         Parameters
         ----------
         model_directory: str or pathlib.Path
             Model directory created with Inferer.deploy().
+        model_path : Optional[pathlib.Path], optional
+            If fed, overwrite path to model file, by default None
+        converter_parameters_pkl : Optional[pathlib.Path], optional
+            If fed, overwrite path to pkl file of scaling parameters,
+             by default None
         decrypt_key: bytes, optional
             Key to decrypt model data. If not fed, and the data is encrypted,
             ValueError is raised.
+        model_select_method: str, optional
+            method name to select model. By default, best
         infer_epoch: int, optional
             If fed, model which corresponds to infer_epoch is used.
 
         Returns
         --------
         siml.Inferer
+            Inferer object
         """
-        model_directory = pathlib.Path(model_directory)
-        if (model_directory / 'settings.yml').is_file():
-            main_setting = setting.MainSetting.read_settings_yaml(
-                model_directory / 'settings.yml')
-        elif (model_directory / 'settings.yml.enc').is_file():
-            main_setting = setting.MainSetting.read_settings_yaml(
-                util.decrypt_file(
-                    decrypt_key, model_directory / 'settings.yml.enc',
-                    return_stringio=True))
-        else:
-            raise ValueError('No setting yaml file found')
 
-        obj = cls(main_setting, **kwargs)
-        obj.setting.inferer.model_key = decrypt_key
-
-        if (model_directory / 'model').is_file():
-            obj.setting.inferer.model = model_directory / 'model'
-        elif (model_directory / 'model.enc').is_file():
-            obj.setting.inferer.model = model_directory / 'model.enc'
-        else:
-            method = 'best' if infer_epoch is None else 'specified'
-            obj.setting.inferer.model = \
-                obj._select_snapshot(model_directory,
-                                     method=method,
-                                     infer_epoch=infer_epoch)
-
-        # Prefer pkl file under model_directory over setting one
-        if (model_directory / 'preprocessors.pkl').is_file():
-            obj.setting.inferer.converter_parameters_pkl \
-                = model_directory / 'preprocessors.pkl'
-        elif (model_directory / 'preprocessors.pkl.enc').is_file():
-            obj.setting.inferer.converter_parameters_pkl \
-                = model_directory / 'preprocessors.pkl.enc'
-        elif obj.setting.inferer.converter_parameters_pkl is not None:
-            pass
-        else:
-            raise ValueError('No preprocessor pickle file found')
+        siml_directory = SimlDirectory(model_directory)
+        if converter_parameters_pkl is None:
+            pickle_file = siml_directory.find_pickle_file(
+                "preprocessors", allow_missing=True
+            )
 
+            if pickle_file is None:
+                raise ValueError(
+                    f"Not found pickle file in a directory: {model_directory}."
+                    "Set converter_parameters_pkl argument explicitly."
+                )
+            pickle_file_path = pickle_file.file_path
+        else:
+            pickle_file_path = converter_parameters_pkl
+
+        setting_file = siml_directory.find_yaml_file('settings')
+        selector = ModelSelectorBuilder.create(model_select_method)
+        model_path = selector.select_model(
+            model_directory,
+            infer_epoch=infer_epoch
+        )
+
+        main_setting = setting.MainSetting.read_settings_yaml(
+            setting_file.file_path,
+            decrypt_key=decrypt_key,
+        )
+
+        obj = cls(
+            main_setting=main_setting,
+            model_path=model_path.file_path,
+            converter_parameters_pkl=pickle_file_path,
+            decrypt_key=decrypt_key,
+            **kwargs
+        )
         return obj
 
     def __init__(
-            self, settings, *,
-            model=None, converter_parameters_pkl=None, save=None,
-            conversion_function=None, load_function=None,
-            data_addition_function=None, postprocess_function=None,
-            save_function=None,
-            optuna_trial=None,
-            user_loss_fundtion_dic:
-            dict[str, Callable[[Tensor, Tensor], Tensor]] = None):
+        self,
+        main_setting: setting.MainSetting,
+        *,
+        scalers: ScalersComposition = None,
+        model_path: Optional[pathlib.Path] = None,
+        converter_parameters_pkl: Optional[pathlib.Path] = None,
+        load_function: ILoadFunction = None,
+        data_addition_function: IFEMDataAdditionFunction = None,
+        save_function: IInfererSaveFunction = None,
+        user_loss_function_dic:
+        dict[str, Callable[[Tensor, Tensor], Tensor]] = None,
+        decrypt_key: Optional[bytes] = None
+    ) -> None:
         """Initialize Inferer object.
 
         Parameters
         ----------
-        settings: siml.MainSetting
-        model: pathlib.Path, optional
-            If fed, overwrite self.setting.inferer.model.
-        converter_parameters_pkl: pathlib.Path, optional
-            If fed, overwrite self.setting.inferer.converter_parameters_pkl
+        main_setting: siml.MainSetting
+        model_path : Optional[pathlib.Path], optional
+            If fed, overwrite path to model file, by default None
+        converter_parameters_pkl : Optional[pathlib.Path], optional
+            If fed, overwrite path to pkl file of scaling parameters,
+             by default None
         save: bool, optional
             If fed, overwrite self.setting.inferer.save
-        conversion_function: function, optional
-            Conversion function to preprocess raw data. It should receive
-            two parameters, fem_data and raw_directory. If not fed,
-            no additional conversion occurs.
         load_function: function, optional
             Function to load data, which take list of pathlib.Path objects
             (as required files) and pathlib.Path object (as data directory)
             and returns data_dictionary and fem_data (can be None) to be saved.
         data_addition_function: function, optional
             Function to add some data at simulation data writing phase.
             If not fed, no data addition occurs.
         postprocess_function: function, optional
             Function to make postprocess of the inference data.
             If not fed, no additional postprocess will be performed.
         save_function: function, optional
             Function to save results. If not fed the default save function
             will be used.
         """
-        if isinstance(settings, pathlib.Path) or isinstance(
-                settings, io.TextIOBase):
-            self.setting = setting.MainSetting.read_settings_yaml(
-                settings)
-        elif isinstance(settings, setting.MainSetting):
-            self.setting = settings
-        else:
-            raise ValueError(
-                f"Unknown type for settings: {settings.__class__}")
-        self.user_loss_function_dic = user_loss_fundtion_dic
-        self.optuna_trial = optuna_trial
+        self._inner_setting = InnerInfererSetting(
+            main_setting=main_setting,
+            force_model_path=model_path,
+            force_converter_parameters_pkl=converter_parameters_pkl,
+            decrypt_key=decrypt_key
+        )
 
-        self.conversion_function = conversion_function
         self.load_function = load_function
         self.data_addition_function = data_addition_function
-        self.postprocess_function = postprocess_function
         self.save_function = save_function
+        if scalers is None:
+            self._scalers = self._inner_setting.load_scalers()
+        else:
+            self._scalers = scalers
 
-        self.inference_mode = True
-        if model is not None:
-            self.setting.inferer.model = model
-        if converter_parameters_pkl is not None:
-            self.setting.inferer.converter_parameters_pkl \
-                = converter_parameters_pkl
-        if save is not None:
-            self.setting.inferer.save = save
-
-        return
+        fem_data_creator = PostFEMDataConverter(
+            inferer_setting=self._inner_setting.inferer_setting,
+            conversion_setting=self._inner_setting.conversion_setting,
+            load_function=load_function,
+            data_addition_function=data_addition_function
+        )
+
+        self._model_env = self._create_model_env_setting()
+        self._collate_fn = self._create_collate_fn()
+        self._dataloader_builder = self._create_data_loader_builder()
+        self._core_inferer = self._create_core_inferer(
+            fem_data_creator,
+            user_loss_function_dic
+        )
+        self._save_processor = SaveProcessor(
+            inner_setting=self._inner_setting,
+            user_save_function=save_function
+        )
+
+    def _create_model_env_setting(self) -> ModelEnvironmentSetting:
+        trainer_setting = self._inner_setting.trainer_setting
+        _model_env = ModelEnvironmentSetting(
+            gpu_id=trainer_setting.gpu_id,
+            seed=trainer_setting.seed,
+            data_parallel=trainer_setting.data_parallel,
+            model_parallel=trainer_setting.model_parallel,
+            time_series=trainer_setting.time_series
+        )
+        return _model_env
+
+    def _create_collate_fn(self):
+        trainer_setting = self._inner_setting.trainer_setting
+        input_is_dict = trainer_setting.inputs.is_dict
+        output_is_dict = trainer_setting.outputs.is_dict
+
+        input_time_series_keys = \
+            trainer_setting.inputs.get_time_series_keys()
+        output_time_series_keys = \
+            trainer_setting.outputs.get_time_series_keys()
+
+        input_time_slices = trainer_setting.inputs.time_slice
+        output_time_slices = trainer_setting.outputs.time_slice
+        element_wise = trainer_setting.determine_element_wise()
+
+        collate_fn = datasets.CollateFunctionGenerator(
+            time_series=trainer_setting.time_series,
+            dict_input=input_is_dict,
+            dict_output=output_is_dict,
+            use_support=trainer_setting.support_inputs,
+            element_wise=element_wise,
+            data_parallel=trainer_setting.data_parallel,
+            input_time_series_keys=input_time_series_keys,
+            output_time_series_keys=output_time_series_keys,
+            input_time_slices=input_time_slices,
+            output_time_slices=output_time_slices
+        )
+        return collate_fn
+
+    def _create_core_inferer(
+        self,
+        fem_data_creator: PostFEMDataConverter,
+        user_loss_function_dic: dict = None
+    ) -> CoreInferer:
+        post_processor = PostProcessor(
+            inner_setting=self._inner_setting,
+            fem_data_converter=fem_data_creator,
+            scalers=self._scalers
+        )
+        loss_function = LossCalculatorBuilder.create(
+            trainer_setting=self._inner_setting.trainer_setting,
+            allow_no_answer=True,
+            user_loss_function_dic=user_loss_function_dic
+        )
+        _core_inferer = CoreInferer(
+            trainer_setting=self._inner_setting.trainer_setting,
+            model_setting=self._inner_setting.model_setting,
+            env_setting=self._model_env,
+            snapshot_file=self._inner_setting.get_snapshot_file_path(),
+            prepare_batch_function=self._collate_fn.prepare_batch,
+            loss_function=loss_function,
+            post_processor=post_processor,
+            decrypt_key=self._inner_setting.get_crypt_key()
+        )
+        return _core_inferer
+
+    def _create_data_loader_builder(self) -> InferenceDataLoaderBuilder:
+        dataloader_builder = InferenceDataLoaderBuilder(
+            trainer_setting=self._inner_setting.trainer_setting,
+            collate_fn=self._collate_fn,
+            decrypt_key=self._inner_setting.get_crypt_key()
+        )
+        return dataloader_builder
 
     def infer(
-            self, *, data_directories=None, model=None,
-            perform_preprocess=None, output_directory_base=None,
-            output_all=False):
+        self,
+        *,
+        data_directories: list[pathlib.Path] = None,
+        output_directory_base: Optional[pathlib.Path] = None,
+        output_all: bool = False,
+        save: Optional[bool] = None
+    ):
         """Perform infererence.
 
         Parameters
         ----------
         data_directories: list[pathlib.Path], optional
             List of data directories. Data is searched recursively.
             The default is an empty list.
-        model: pathlib.Path, optional
-            If fed, overwrite self.setting.inferer.model.
-        perform_preprocess: bool, optional
-            If fed, overwrite self.setting.inferer.perform_preprocess
         output_directory_base: pathlib.Path, optional
             If fed, overwrite self.setting.inferer.output_directory_base
         output_all: bool, optional. Dafault False
             If True, return all of results \
                 including not preprocessed predicted data
-
+        save: bool, optional. Default None
+            If fed, overwrite save option in main setting
 
         Returns
         -------
         inference_results: list[Dict]
             Inference results contains:
                 - dict_x: input and variables
                 - dict_y: inferred variables
@@ -202,72 +464,130 @@
                 - output_directory: Output directory path
                 - data_directory: Input directory path
                 - inference_time: Inference time
         """
         if data_directories is not None:
             if isinstance(data_directories, pathlib.Path):
                 data_directories = [data_directories]
-            self.setting.inferer.data_directories = data_directories
-        if model is not None:
-            self.setting.inferer.model = model
-        if perform_preprocess is not None:
-            self.setting.inferer.perform_preprocess = perform_preprocess
+        else:
+            data_directories = \
+                self._inner_setting.inferer_setting.data_directories
         if output_directory_base is not None:
-            self.setting.inferer.output_directory_base = output_directory_base
-
-        self._prepare_inference()
-        self.date_string = util.date_string()
-        inference_state = self.inferer.run(self.inference_loader)
-
-        if self.setting.inferer.save:
-            self.save(inference_state.metrics['results'])
+            # HACK: Improve it to make setting class immutable
+            self._inner_setting.main_setting.inferer.output_directory_base \
+                = output_directory_base
+
+        inference_loader = self._dataloader_builder.create(
+            data_directories=data_directories
+        )
+        inference_state = self._core_inferer.run(inference_loader)
+
+        do_save = save if save is not None \
+            else self._inner_setting.inferer_setting.save
+        if do_save:
+            self._save_processor.run(inference_state)
 
         if output_all:
             return inference_state
         else:
-            return inference_state.metrics['results']
+            return self._format_results(inference_state.metrics)
+
+    def infer_dataset(
+        self,
+        preprocess_dataset: datasets.PreprocessDataset,
+        output_directory_base: Optional[pathlib.Path] = None,
+        save: Optional[bool] = None
+    ) -> list[dict]:
+        """_summary_
+
+        Parameters
+        ----------
+        preprocess_dataset : datasets.PreprocessDataset
+            dataset of preprocessed data
+        output_directory_base : Optional[pathlib.Path], optional
+            base output directory, by default None
+        save : Optional[bool], optional
+            If fed, overwrite save option. by default None
+
+        Returns
+        -------
+        inference_results: list[Dict]
+            Inference results contains:
+                - dict_x: input and variables
+                - dict_y: inferred variables
+                - dict_answer: answer variables (None if not found)
+                - loss: Loss value (scaled)
+                - raw_loss: Loss in a raw scale
+                - fem_data: FEMData object
+                - output_directory: Output directory path
+                - data_directory: Input directory path
+                - inference_time: Inference time
+
+        """
 
-    def infer_simplified_model(
-            self, model_path, raw_dict_x, *, answer_raw_dict_y=None):
+        if output_directory_base is not None:
+            # HACK: Improve it to make setting class immutable
+            self._inner_setting.main_setting.inferer.output_directory_base \
+                = output_directory_base
+
+        inference_loader = DataLoader(
+            preprocess_dataset,
+            collate_fn=self._collate_fn,
+            batch_size=1,
+            shuffle=False,
+            num_workers=0
+        )
+        inference_state = self._core_inferer.run(inference_loader)
+
+        do_save = save if save is not None \
+            else self._inner_setting.inferer_setting.save
+        if do_save:
+            self._save_processor.run(inference_state)
+
+        return self._format_results(inference_state.metrics)
+
+    def infer_dict_data(
+        self,
+        scaled_dict_x: dict,
+        *,
+        scaled_dict_answer: Optional[dict] = None
+    ):
         """
         Infer with simplified model.
 
         Parameters
         ----------
-        model_path: pathlib.Path
-            Model file or directory name.
-        raw_dict_x: dict
-            Dict of raw x data.
-        answer_raw_dict_y: dict, optional
-            Dict of answer raw y data.
+        scaled_dict_x: dict
+            Dict of scaled x data.
+        scaled_dict_answer: dict, optional
+            Dict of answer scaled y data.
 
         Returns
         -------
         inference_result: Dict
             Inference results contains:
                 - dict_x: input and answer variables
                 - dict_y: inferred variables
                 - loss: Loss value (scaled)
                 - raw_loss: Loss in a raw scale
                 - fem_data: FEMData object
                 - output_directory: Output directory path
                 - data_directory: Input directory path
                 - inference_time: Inference time
         """
-        if model_path is not None:
-            self.setting.inferer.model = model_path
+        inference_loader = self._dataloader_builder.create(
+            raw_dict_x=scaled_dict_x,
+            answer_raw_dict_y=scaled_dict_answer
+        )
+        inference_state = self._core_inferer.run(inference_loader)
+
+        if self._inner_setting.inferer_setting.save:
+            self._save_processor.run(inference_state)
 
-        self._prepare_inference(
-            raw_dict_x=raw_dict_x, answer_raw_dict_y=answer_raw_dict_y)
-        self.date_string = util.date_string()
-        inference_state = self.inferer.run(self.inference_loader)
-
-        if self.setting.inferer.save:
-            self.save(inference_state.metrics['results'])
-        return inference_state.metrics['results'][0]
+        return self._format_results(inference_state.metrics)
 
     def infer_parameter_study(
             self, model, data_directories, *, n_interpolation=100,
             converter_parameters_pkl=None):
         """
         Infer with performing parameter study. Parameter study is done with the
         data generated by interpolating the input data_directories.
@@ -320,363 +640,84 @@
                 for i in range(n_interpolation + 1)], axis=1)
             for x_variable_name in min_input_dict.keys()}
         output_dict = self.infer_simplified_model(
             model, interpolated_input_dict,
             converter_parameters_pkl=converter_parameters_pkl)[0]
         return interpolated_input_dict, output_dict
 
-    def save(self, results):
-        """Save inference results information.
-
-        Parameters
-        ----------
-        results: Dict
-            Inference results.
-        """
-        output_directory = self._determine_output_directory()
-        output_directory.mkdir(parents=True, exist_ok=True)
-        setting.write_yaml(
-            self.setting, output_directory / 'settings.yml',
-            key=self.setting.inferer.model_key)
-        self._write_log(output_directory, results)
-        return
-
-    def _write_log(self, output_directory, results):
-        column_names = [
-            'loss', 'raw_loss', 'output_directory', 'data_directory',
-            'inference_time']
-
-        log_dict = {}
-        for column_name in column_names:
-            log_dict.update({column_name: [r[column_name] for r in results]})
-
-        pd.DataFrame(log_dict).to_csv(
-            output_directory / 'infer.csv', index=None)
-        return
-
-    def deploy(self, output_directory, *, model=None, encrypt_key=None):
+    def deploy(
+        self,
+        output_directory: pathlib.Path,
+        encrypt_key: bytes = None
+    ):
         """Deploy model information.
 
         Parameters
         ----------
         output_directory: pathlib.Path
             Output directory path.
-        model: pathlib.Path, optional
-            If fed, overwrite self.setting.inferer.model.
         encrypt_key: bytes, optional
             Key to encrypt model data. If not fed, the model data will not be
             encrypted.
         """
-        if model is not None:
-            self.setting.inferer.model = model
-        if model.is_dir():
-            snapshot = self._select_snapshot(
-                self.setting.inferer.model,
-                method=self.setting.trainer.snapshot_choise_method)
-        else:
-            snapshot = model
-
         output_directory.mkdir(parents=True, exist_ok=True)
+        enc_ext = ".enc" if encrypt_key is not None else ""
 
-        if encrypt_key is None:
-            output_model = output_directory / 'model'
-            if output_model.exists():
-                raise ValueError(f"{output_model} already exists")
-            shutil.copyfile(snapshot, output_model)
-
-            output_pkl = output_directory / 'preprocessors.pkl'
-            if output_pkl.exists():
-                raise ValueError(f"{output_pkl} already exists")
-            shutil.copyfile(
-                self.setting.inferer.converter_parameters_pkl,
-                output_pkl)
-
-            output_setting = output_directory / 'settings.yml'
-            if output_setting.exists():
-                raise ValueError(f"{output_setting} already exists")
-            setting.write_yaml(self.setting, output_setting)
+        # TODO: should deep copy to avoid side-effect
+        main_setting = self._inner_setting.main_setting
 
-        else:
-
-            output_model = output_directory / 'model.enc'
-            if output_model.exists():
-                raise ValueError(f"{output_model} already exists")
-            self._encrypt_file(
-                encrypt_key, snapshot, output_directory / 'model.enc')
-
-            output_pkl = output_directory / 'preprocessors.pkl.enc'
-            if output_pkl.exists():
-                raise ValueError(f"{output_pkl} already exists")
-            self._encrypt_file(
-                encrypt_key, self.setting.inferer.converter_parameters_pkl,
-                output_pkl)
-
-            output_setting = output_directory / 'settings.yml.enc'
-            if output_setting.exists():
-                raise ValueError(f"{output_setting} already exists")
-            setting.write_yaml(self.setting, output_setting, key=encrypt_key)
+        # output name
+        output_model_name = \
+            SimlConstItems.DEPLOYED_MODEL_NAME + f".pth{enc_ext}"
+        output_model_path = SimlFileBuilder.checkpoint_file(
+            output_directory / output_model_name
+        )
+        output_pkl = SimlFileBuilder.pickle_file(
+            output_directory / f'preprocessors.pkl{enc_ext}'
+        )
+        output_setting_yaml = SimlFileBuilder.yaml_file(
+            output_directory / 'settings.yml'
+        )
+        # Overwrite Setting
+        main_setting.inferer.model = output_model_path.file_path
+
+        # Model
+        snapshot_file = self._inner_setting.get_snapshot_file_path()
+        siml_path = SimlFileBuilder.checkpoint_file(snapshot_file)
+        model_data = siml_path.load(device="cpu", decrypt_key=encrypt_key)
+        output_model_path.save(model_data, encrypt_key=encrypt_key)
+
+        # pickle
+        pkl_path = self._inner_setting.get_converter_parameters_pkl_path()
+        pkl_path = SimlFileBuilder.pickle_file(pkl_path)
+        pkl_data = pkl_path.load(decrypt_key=encrypt_key)
+        output_pkl.save(
+            pkl_data, encrypt_key=encrypt_key
+        )
 
+        # yaml
+        setting.write_yaml(
+            main_setting,
+            output_setting_yaml.file_path,
+            key=encrypt_key
+        )
         return
 
-    def _encrypt_file(self, key, input_file_name, output_file_name):
-        with open(input_file_name, "rb") as f:
-            data = f.read()
-            binary = io.BytesIO(data)
-            util.encrypt_file(key, output_file_name, binary)
-        return
-
-    def _prepare_inference(
-            self, *,
-            raw_dict_x=None, answer_raw_dict_y=None, allow_no_data=True):
-
-        # Define model
-        if self.setting.inferer.model is None:
-            if self.setting.trainer.pretrain_directory is None:
-                raise ValueError(
-                    'No pretrain directory is specified for inference.')
-            else:
-                model = pathlib.Path(self.setting.trainer.pretrain_directory)
-        else:
-            model = pathlib.Path(self.setting.inferer.model)
-        self.setting.trainer.restart_directory = None
-
-        model = pathlib.Path(model)
-        if model.is_dir():
-            self.setting.trainer.pretrain_directory = model
-            self._update_setting_if_needed()
-            model_file = None
-        elif model.is_file():
-            model_file = model
-        else:
-            raise ValueError(f"Model does not exist: {model}")
-
-        self.model = networks.Network(
-            self.setting.model, self.setting.trainer)
-        self._select_device(gpu_id=self.setting.inferer.gpu_id)
-        self._load_pretrained_model_if_needed(model_file=model_file)
-
-        self.element_wise = self._determine_element_wise()
-        self.loss = self._create_loss_function(allow_no_answer=True)
-        if self.setting.inferer.converter_parameters_pkl is None:
-            self.setting.inferer.converter_parameters_pkl \
-                = self.setting.data.preprocessed_root / 'preprocessors.pkl'
-        self.prepost_converter = prepost.Converter(
-            self.setting.inferer.converter_parameters_pkl,
-            key=self.setting.inferer.model_key)
-
-        self.inference_loader = self._get_inferernce_loader(
-            raw_dict_x, answer_raw_dict_y, allow_no_data=allow_no_data)
-        self.inferer = self._create_inferer()
-        return
-
-    def _get_inferernce_loader(
-            self, raw_dict_x=None, answer_raw_dict_y=None,
-            allow_no_data=True):
-        input_is_dict = isinstance(
-            self.setting.trainer.inputs.variables, dict)
-        output_is_dict = isinstance(
-            self.setting.trainer.outputs.variables, dict)
-        if isinstance(self.setting.trainer.inputs.time_series, dict):
-            input_time_series_keys = [
-                k for k, v in self.setting.trainer.inputs.time_series.items()
-                if np.any(v)]
-        else:
-            input_time_series_keys = []
-        if isinstance(self.setting.trainer.outputs.time_series, dict):
-            output_time_series_keys = [
-                k for k, v in self.setting.trainer.outputs.time_series.items()
-                if np.any(v)]
-        else:
-            output_time_series_keys = []
-        input_time_slices = self.setting.trainer.inputs.time_slice
-        output_time_slices = self.setting.trainer.outputs.time_slice
-        self.collate_fn = datasets.CollateFunctionGenerator(
-            time_series=self.setting.trainer.time_series,
-            dict_input=input_is_dict, dict_output=output_is_dict,
-            use_support=self.setting.trainer.support_inputs,
-            element_wise=self.element_wise,
-            data_parallel=self.setting.trainer.data_parallel,
-            input_time_series_keys=input_time_series_keys,
-            output_time_series_keys=output_time_series_keys,
-            input_time_slices=input_time_slices,
-            output_time_slices=output_time_slices)
-        self.prepare_batch = self.collate_fn.prepare_batch
-
-        setting = self.setting
-        if setting.data.encrypt_key is not None:
-            key = setting.data.encrypt_key
-        elif setting.inferer.model_key is not None:
-            key = setting.inferer.model_key
-        elif setting.trainer.model_key is not None:
-            key = setting.trainer.model_key
-        else:
-            key = None
-
-        if raw_dict_x is not None:
-            inference_dataset = datasets.SimplifiedDataset(
-                setting.trainer.input_names,
-                setting.trainer.output_names,
-                raw_dict_x=raw_dict_x, answer_raw_dict_y=answer_raw_dict_y,
-                prepost_converter=self.prepost_converter,
-                allow_no_data=allow_no_data,
-                num_workers=0)
-        elif setting.inferer.perform_preprocess:
-            inference_dataset = datasets.PreprocessDataset(
-                setting.trainer.input_names,
-                setting.trainer.output_names,
-                setting.inferer.data_directories,
-                supports=setting.trainer.support_inputs,
-                num_workers=0,
-                required_file_names=setting.conversion.required_file_names,
-                decrypt_key=key,
-                prepost_converter=self.prepost_converter,
-                conversion_setting=setting.conversion,
-                conversion_function=self.conversion_function,
-                allow_no_data=allow_no_data,
-                load_function=self.load_function)
-        else:
-            inference_dataset = datasets.LazyDataset(
-                setting.trainer.input_names,
-                setting.trainer.output_names,
-                setting.inferer.data_directories,
-                supports=setting.trainer.support_inputs,
-                num_workers=0,
-                allow_no_data=allow_no_data,
-                decrypt_key=key)
-
-        inference_loader = torch.utils.data.DataLoader(
-            inference_dataset, collate_fn=self.collate_fn,
-            batch_size=1, shuffle=False, num_workers=0)
-        return inference_loader
-
-    def _create_inferer(self):
-
-        def _inference(engine, batch):
-            self.model.eval()
-            x, y = self.prepare_batch(
-                batch, device=self.device,
-                output_device=self.output_device,
-                support_device=self.device,
-                non_blocking=self.setting.trainer.non_blocking)
-            with torch.no_grad():
-                start_time = time.time()
-                y_pred = self.model(x)
-                end_time = time.time()
-                elapsed_time = end_time - start_time
-
-            assert len(batch['data_directories']) == 1
-            data_directory = batch['data_directories'][0]
-            loss = self.loss(y_pred, y, original_shapes=x['original_shapes'])
-            print('--')
-            print(f"              Data: {data_directory}")
-            print(f"Inference time [s]: {elapsed_time:.5e}")
-            if loss is not None:
-                print(f"              Loss: {loss}")
-            print('--')
-
-            return y_pred, y, {
-                'x': x, 'original_shapes': x['original_shapes'],
-                'data_directory': data_directory,
-                'inference_time': elapsed_time}
-
-        evaluator_engine = ignite.engine.Engine(_inference)
-
-        metrics = {'results': postprocessor.Postprocessor(inferer=self)}
-
-        for name, metric in metrics.items():
-            metric.attach(evaluator_engine, name)
-        return evaluator_engine
-
-    def _separate_data(self, data, descriptions, *, axis=-1):
-        if isinstance(data, dict):
-            return {
-                key:
-                self._separate_data(
-                    data[key], descriptions.variables[key], axis=axis)
-                for key in data.keys()}
-        if len(data) == 0:
-            return {}
-
-        data_dict = {}
-        index = 0
-        data = np.swapaxes(data, 0, axis)
-        for description in descriptions.variables:
-            dim = description.dim
-            data_dict.update({
-                description.name:
-                np.swapaxes(data[index:index+dim], 0, axis)})
-            index += dim
-        return data_dict
-
-    def _determine_output_directory(self, data_directory=None):
-        if data_directory is None:
-            data_directory = ''
-        if self.setting.inferer.output_directory is not None:
-            return self.setting.inferer.output_directory
-
-        subdirectory = self._determine_subdirectory()
-        base = self.setting.inferer.output_directory_base / subdirectory
-        if 'preprocessed' in str(data_directory):
-            output_directory = path_utils.determine_output_directory(
-                data_directory, base, 'preprocessed')
-        elif 'interim' in str(data_directory):
-            output_directory = path_utils.determine_output_directory(
-                data_directory, base, 'interim')
-        elif 'raw' in str(data_directory):
-            output_directory = path_utils.determine_output_directory(
-                data_directory, base, 'raw')
-        else:
-            output_directory = base
-        return output_directory
-
-    def _determine_subdirectory(self):
-        if self.setting.inferer.model is not None:
-            model = pathlib.Path(self.setting.inferer.model)
-            if model.is_dir():
-                model_name = model.name
-            else:
-                model_name = model.parent.name
-        elif self.setting.trainer.name is not None:
-            model_name = self.setting.trainer.name
-        else:
-            model_name = 'unknown'
-        return f"{model_name}_{self.date_string}"
-
-    def _determine_write_simulation_base(self, data_directory):
-        if self.setting.inferer.write_simulation_base is None:
-            if self.setting.inferer.perform_preprocess:
-                # Assume the given data is raw data
-                return data_directory
-            else:
-                if 'preprocessed' in str(data_directory):
-                    raw_candidate = pathlib.Path(
-                        str(data_directory).replace('preprocessed', 'raw'))
-                    if raw_candidate.is_dir():
-                        return raw_candidate
-                    else:
-                        interim_candidate = pathlib.Path(
-                            str(data_directory).replace(
-                                'preprocessed', 'interim'))
-                        if interim_candidate.is_dir():
-                            return interim_candidate
-                        else:
-                            return None
-                else:
-                    return None
-
-        if 'preprocessed' in str(data_directory):
-            write_simulation_base = path_utils.determine_output_directory(
-                data_directory,
-                self.setting.inferer.write_simulation_base,
-                'preprocessed')
-
-        elif 'interim' in str(data_directory):
-            write_simulation_base = path_utils.determine_output_directory(
-                data_directory,
-                self.setting.inferer.write_simulation_base,
-                'interim')
-        elif 'raw' in str(data_directory):
-            write_simulation_base = data_directory
-        else:
-            write_simulation_base \
-                = self.setting.inferer.write_simulation_base
-        return write_simulation_base
+    def _format_results(self, metrics: dict) -> list[dict]:
+        results = []
+        records: list[PostPredictionRecord] = metrics.pop("post_results")
+        for i, val in enumerate(records):
+            _data = {
+                name: getattr(val, name)
+                for name in PostPredictionRecord._fields
+            }
+            for name, item in metrics.items():
+                _data.update({name: item[i]})
+
+            each_output_directory = \
+                self._inner_setting.get_output_directory(
+                    val.inference_start_datetime,
+                    data_directory=val.data_directory,
+                )
+            _data.update({"output_directory": each_output_directory})
+            results.append(_data)
+        return results
```

## siml/loss_operations/loss_assignment.py

```diff
@@ -13,16 +13,17 @@
                     variable_name: str) -> str:
         raise NotImplementedError()
 
 
 class LossAssignmentCreator():
     @classmethod
     def create(
-            self,
-            loss_setting: Union[dict, str]) -> ILossAssignment:
+        self,
+        loss_setting: Union[dict, str]
+    ) -> ILossAssignment:
         if type(loss_setting) is dict:
             return DictLossAssignment(loss_setting)
 
         if type(loss_setting) is str:
             return StrLossAssignment(loss_setting)
 
         raise NotImplementedError(
```

## siml/loss_operations/loss_calculator.py

```diff
@@ -1,29 +1,44 @@
-from typing import Callable, Union
+import abc
+from typing import Callable, Union, Optional
 import torch
 from torch import Tensor
 
 from siml import util
+from siml.base.siml_enums import LossType
 from .loss_assignment import ILossAssignment
 from .loss_assignment import LossAssignmentCreator
 from .loss_selector import LossFunctionSelector
 
 
-class LossCalculator:
+class ILossCalculator(metaclass=abc.ABCMeta):
+    @abc.abstractmethod
+    def __call__(
+        self,
+        y_pred: torch.Tensor,
+        y: torch.Tensor,
+        original_shapes: Optional[tuple] = None,
+        **kwargs
+    ) -> torch.Tensor:
+        raise NotImplementedError()
+
+
+class LossCalculator(ILossCalculator):
 
     def __init__(
-            self,
-            *,
-            loss_setting: Union[dict, str] = 'mse',
-            time_series: bool = False,
-            output_is_dict: bool = False,
-            output_skips=None,
-            output_dims=None,
-            user_loss_function_dic:
-            dict[str, Callable[[Tensor, Tensor], Tensor]] = None):
+        self,
+        *,
+        loss_setting: Union[dict, str] = LossType.MSE.value,
+        time_series: bool = False,
+        output_is_dict: bool = False,
+        output_skips=None,
+        output_dims=None,
+        user_loss_function_dic:
+        dict[str, Callable[[Tensor, Tensor], Tensor]] = None
+    ) -> None:
 
         self.loss_assignment = LossAssignmentCreator.create(loss_setting)
         self.loss_core = CoreLossCalculator(
             loss_assignment=self.loss_assignment,
             user_loss_function_dic=user_loss_function_dic
         )
 
@@ -88,19 +103,20 @@
 
         self.loss_selector = LossFunctionSelector(
             loss_assignment,
             user_loss_function_dic=user_loss_function_dic
         )
         return
 
-    def __call__(self,
-                 input_tensor: Tensor,
-                 target_tensor: Tensor,
-                 variable_name: str = None
-                 ) -> Tensor:
+    def __call__(
+        self,
+        input_tensor: Tensor,
+        target_tensor: Tensor,
+        variable_name: str = None
+    ) -> Tensor:
         """Calculate loss value
 
         Args:
             input_tensor (Tensor): tensor of prediction
             target_tensor (Tensor): tensor of target
             variable_name (str, optional):
              name of variable. Defaults to None.
```

## siml/loss_operations/loss_selector.py

```diff
@@ -1,12 +1,13 @@
 from torch import Tensor
 from typing import Callable
 import torch.nn.functional as functional
 
-from .loss_type import LossType
+from siml.base.siml_enums import LossType
+
 from .loss_assignment import ILossAssignment
 
 
 class LossFunctionSelector():
     """
     Resposibility: Select loss function for each variable name
     """
@@ -20,17 +21,18 @@
 
         self.loss_assignment = loss_assignment
         self.func_name_to_func_obj = self._create_loss_function_dict(
             user_loss_function_dic
         )
         self._check_loss_functions()
 
-    def get_loss_function(self,
-                          variable_name: str
-                          ) -> Callable[[Tensor, Tensor], Tensor]:
+    def get_loss_function(
+        self,
+        variable_name: str
+    ) -> Callable[[Tensor, Tensor], Tensor]:
         loss_name = self.loss_assignment[variable_name]
         return self.func_name_to_func_obj[loss_name]
 
     def _check_loss_functions(self) -> None:
         for loss_name in self.loss_assignment.loss_names:
             if loss_name not in self.func_name_to_func_obj.keys():
                 raise ValueError(f"Unknown loss function name: {loss_name}")
@@ -50,14 +52,14 @@
 
         Returns:
             dict[str, Callable[[Tensor, Tensor], Tensor]]:
              Key is function name and value is function object
         """
 
         name_to_function = {
-            LossType.mse.name: functional.mse_loss
+            LossType.MSE.value: functional.mse_loss
         }
 
         if user_loss_function_dic is not None:
             name_to_function.update(user_loss_function_dic)
 
         return name_to_function
```

## siml/path_like_objects/__init__.py

```diff
@@ -1,2 +1,2 @@
 from .siml_directory import SimlDirectory  # NOQA
-from .siml_file import ISimlFile, SimlFileBulider, SimlFileExtType  # NOQA
+from .siml_file_builder import SimlFileBuilder, ISimlNumpyFile, ISimlPickleFile, ISimlCheckpointFile  # NOQA
```

## siml/path_like_objects/siml_directory.py

```diff
@@ -1,44 +1,105 @@
 import pathlib
-from typing import Union
+from typing import Union, Callable, Any
 
-from .siml_file import ISimlFile, SimlFileBulider
+from siml.base.siml_enums import SimlFileExtType
+
+from .siml_file_builder import (
+    ISimlNumpyFile, ISimlYamlFile, ISimlPickleFile, SimlFileBuilder
+)
 
 
 class SimlDirectory:
     def __init__(self, path: pathlib.Path) -> None:
         self._path = path
 
     def __str__(self) -> str:
         return f"SimlDirectory: {self._path}"
 
     @property
     def path(self) -> pathlib.Path:
         return self._path
 
+    def find_pickle_file(
+        self,
+        file_base_name: str,
+        *,
+        allow_missing: bool = False
+    ) -> Union[ISimlPickleFile, None]:
+        extensions = [
+            SimlFileExtType.PKL,
+            SimlFileExtType.PKLENC
+        ]
+
+        return self._find_file(
+            file_base_name=file_base_name,
+            extensions=extensions,
+            builder=SimlFileBuilder.pickle_file,
+            allow_missing=allow_missing
+        )
+
+    def find_yaml_file(
+        self,
+        file_base_name: str,
+        *,
+        allow_missing: bool = False
+    ) -> Union[ISimlYamlFile, None]:
+        extensions = [
+            SimlFileExtType.YAML,
+            SimlFileExtType.YAMLENC,
+            SimlFileExtType.YML,
+            SimlFileExtType.YMLENC
+        ]
+
+        return self._find_file(
+            file_base_name=file_base_name,
+            extensions=extensions,
+            builder=SimlFileBuilder.yaml_file,
+            allow_missing=allow_missing
+        )
+
     def find_variable_file(
         self,
         variable_name: str,
         *,
         allow_missing: bool = False
-    ) -> Union[ISimlFile, None]:
+    ) -> Union[ISimlNumpyFile, None]:
+
+        extensions = [
+            SimlFileExtType.NPY,
+            SimlFileExtType.NPYENC,
+            SimlFileExtType.NPZ,
+            SimlFileExtType.NPZENC
+        ]
+        return self._find_file(
+            variable_name,
+            extensions,
+            SimlFileBuilder.numpy_file,
+            allow_missing=allow_missing
+        )
 
-        extenstions = [".npy", ".npy.enc", ".npz", ".npz.enc"]
-        for ext in extenstions:
-            path = (self._path / (variable_name + ext))
+    def _find_file(
+        self,
+        file_base_name: str,
+        extensions: list[SimlFileExtType],
+        builder: Callable[[pathlib.Path], Any],
+        *,
+        allow_missing: bool = False
+    ):
+        for ext in extensions:
+            path: pathlib.Path = (self._path / (file_base_name + ext.value))
             if path.exists():
-                return SimlFileBulider.create(path)
+                return builder(path)
 
         if allow_missing:
             return None
 
         raise ValueError(
-            f"Unknown extension or file not found for {variable_name}"
+            f"Unknown extension or file not found for {file_base_name}"
         )
 
     def exist_variable_file(self, variable_name: str) -> bool:
         _file = self.find_variable_file(variable_name, allow_missing=True)
-
         if _file is None:
             return False
         else:
             return True
```

## siml/prepost.py

```diff
@@ -1,73 +1,18 @@
 """Module for preprocessing."""
 
 import datetime as dt
 import itertools as it
-from typing import Union
 
 import femio
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.sparse as sp
 
 from siml import util
-from siml.utils import fem_data_utils
-from siml.preprocessing import ScalersComposition
-from siml.siml_variables import ArrayDataType
-
-
-def add_difference(
-        fem_data, dict_data, reference_dict_data, prefix='difference'):
-    if reference_dict_data is None:
-        return fem_data
-    intersections = set(
-        dict_data.keys()).intersection(reference_dict_data.keys())
-    if len(intersections) == 0:
-        return fem_data
-
-    difference_dict_data = {
-        intersection:
-        np.reshape(
-            dict_data[intersection], reference_dict_data[intersection].shape)
-        - reference_dict_data[intersection]
-        for intersection in intersections}
-
-    wrapped_data = fem_data_utils.FemDataWrapper(fem_data)
-    wrapped_data.update_fem_data(
-        difference_dict_data, prefix=prefix
-    )
-
-    return wrapped_data.fem_data
-
-
-def add_abs_difference(
-        fem_data, dict_data, reference_dict_data, prefix='difference_abs'):
-    if reference_dict_data is None:
-        return fem_data
-    intersections = set(
-        dict_data.keys()).intersection(reference_dict_data.keys())
-    if len(intersections) == 0:
-        return fem_data
-
-    difference_dict_data = {
-        intersection:
-        np.abs(
-            np.reshape(
-                dict_data[intersection],
-                reference_dict_data[intersection].shape)
-            - reference_dict_data[intersection])
-        for intersection in intersections}
-
-    wrapped_data = fem_data_utils.FemDataWrapper(fem_data)
-    wrapped_data.update_fem_data(
-        difference_dict_data,
-        prefix=prefix
-    )
-
-    return wrapped_data.fem_data
 
 
 def concatenate_preprocessed_data(
         preprocessed_base_directories, output_directory_base, variable_names,
         *, ratios=(.9, .05, .05), overwrite=False,
         finished_file='preprocessed'):
     """Concatenate preprocessed data in the element direction.
@@ -126,300 +71,14 @@
         if test_length > 0:
             np.save(
                 output_directory_base / f"validation/{variable_name}.npy",
                 data[indices[train_length+validation_length:]])
     return
 
 
-class Converter:
-
-    def __init__(self, converter_parameters_pkl, key=None):
-        self.converters = ScalersComposition.create_from_file(
-            converter_parameters_pkl=converter_parameters_pkl,
-            key=key
-        )
-
-    def preprocess(self, dict_data_x: dict):
-        input_dict = {
-            name: v for name, v in dict_data_x.items()
-            if name in self.converters.get_variable_names()
-        }
-
-        converted_dict_data_x = self.converters.transform_dict(input_dict)
-        if len(converted_dict_data_x) == 0:
-            raise ValueError(
-                'No converted data found. '
-                'Check the preprocessed directory set correctly.')
-        return converted_dict_data_x
-
-    def postprocess(
-            self, dict_data_x: dict, dict_data_y: dict, output_directory=None,
-            *,
-            dict_data_y_answer=None,
-            overwrite=False, save_x=False, write_simulation=False,
-            write_npy=True, write_simulation_stem=None,
-            write_simulation_base=None, read_simulation_type='fistr',
-            save_function=None,
-            write_simulation_type='fistr', skip_femio=False,
-            load_function=None, convert_to_order1=False,
-            data_addition_function=None, required_file_names=[],
-            less_output=False, perform_inverse=True,
-            skip_fem_data_creation=False, **kwargs):
-        """Postprocess data with inversely converting them.
-
-        Parameters
-        ----------
-        dict_data_x: dict
-            Dict of input data.
-        dict_data_y: dict
-            Dict of output data.
-        output_directory: pathlib.Path, optional
-            Output directory path.
-        dict_data_y_answer: dict
-            Dict of expected output data.
-        overwrite: bool, optional
-            If True, overwrite data.
-        save_x: bool, optional
-            If True, save input values in addition to output values.
-        write_simulation: bool, optional
-            If True, write simulation data file(s) based on the inference.
-        write_npy: bool, optional
-            If True, write npy files of inferences.
-        write_simulation_base: pathlib.Path, optional
-            Base of simulation data to be used for write_simulation option.
-            If not fed, try to find from the input directories.
-        read_simulation_type: str, optional
-            Simulation file type to read simulation base.
-        write_simulation_type: str, optional
-            Simulation file type to write.
-        skip_femio: bool, optional
-            If True, skip femio to read simulation base.
-        load_function: callable, optional
-            Load function taking data_files and data_directory as inputs,
-            and returns data_dict and fem_data.
-        required_file_names: list[str], optional
-            Required file names for load function.
-        less_output: bool, optional
-            If True, output less variables in FEMData object.
-        data_addition_function: callable, optional
-            Function to add some data to existing fem_data.
-        skip_fem_data_creation: bool, optional
-            If True, skip fem_data object creation.
-
-        Returns
-        --------
-            inversed_dict_data_x: dict
-                Inversed input data.
-            inversed_dict_data_y: dict
-                Inversed output data.
-            inversed_dict_answer: dict
-                Inversed answer data. None when the answer not available.
-            fem_data: femio.FEMData
-                FEMData object with input and output data.
-        """
-        _dict_data_x = self._format_dict_shape(dict_data_x)
-        _dict_data_y = self._format_dict_shape(dict_data_y)
-        _dict_data_y_answer = self._format_dict_shape(dict_data_y_answer)
-
-        if perform_inverse:
-            _dict_data_x = self._inverse_process(_dict_data_x)
-            _dict_data_y = self._inverse_process(_dict_data_y)
-            _dict_data_y_answer = self._inverse_process(_dict_data_y_answer)
-
-        # Save data
-        if skip_fem_data_creation or write_simulation_base is None \
-                or not write_simulation_base.exists():
-            fem_data = None
-        else:
-            try:
-                fem_data = self._create_fem_data(
-                    _dict_data_x, _dict_data_y,
-                    dict_data_answer=_dict_data_y_answer,
-                    write_simulation_base=write_simulation_base,
-                    write_simulation_stem=write_simulation_stem,
-                    read_simulation_type=read_simulation_type,
-                    data_addition_function=data_addition_function,
-                    skip_femio=skip_femio, load_function=load_function,
-                    convert_to_order1=convert_to_order1,
-                    required_file_names=required_file_names)
-            except ValueError as e:
-                print(
-                    f"{e}\n"
-                    'Could not read FEMData object, set None\n'
-                    f"write_simulation_base: {write_simulation_base}\n"
-                    f"write_simulation_stem: {write_simulation_stem}\n"
-                    f"read_simulation_type: {read_simulation_type}\n"
-                )
-                fem_data = None
-                write_simulation_base = None
-                write_simulation = False
-        if output_directory is not None:
-            if write_npy:
-                if save_x:
-                    self.save(_dict_data_x, output_directory)
-                self.save(_dict_data_y, output_directory)
-            if write_simulation:
-                if write_simulation_base is None:
-                    raise ValueError('No write_simulation_base fed.')
-                self._write_simulation(
-                    output_directory, fem_data, overwrite=overwrite,
-                    write_simulation_type=write_simulation_type,
-                    less_output=less_output)
-            if save_function is not None:
-                save_function(
-                    output_directory, fem_data, overwrite=overwrite,
-                    write_simulation_type=write_simulation_type)
-
-        return _dict_data_x, _dict_data_y, \
-            _dict_data_y_answer, fem_data
-
-    def _inverse_process(
-        self,
-        dict_data: Union[dict[str, ArrayDataType], None]
-    ) -> dict[str, ArrayDataType]:
-        if dict_data is None:
-            return {}
-
-        dict_data_answer = self.converters.inverse_transform_dict(dict_data)
-        return dict_data_answer
-
-    def _format_dict_shape(
-        self,
-        dict_data: Union[dict, None]
-    ) -> Union[dict[str, ArrayDataType], None]:
-        # This function should be deprecated
-        # It is not appropriate to overwrite value for variable name
-        if dict_data is None:
-            return None
-
-        if len(dict_data) == 0:
-            return None
-
-        if isinstance(list(dict_data.values())[0], dict):
-            return_dict_data = {
-                variable_name: data
-                for value in dict_data.values()
-                for variable_name, data in value.items()
-                if variable_name in self.converters.get_variable_names()
-            }
-        else:
-            return_dict_data = {
-                variable_name: data
-                for variable_name, data in dict_data.items()
-                if variable_name in self.converters.get_variable_names()
-            }
-        return return_dict_data
-
-    def _create_fem_data(
-            self, dict_data_x, dict_data_y, write_simulation_base, *,
-            dict_data_answer=None,
-            write_simulation_stem=None,
-            read_simulation_type='fistr', data_addition_function=None,
-            skip_femio=False, load_function=None,
-            required_file_names=[], convert_to_order1=False):
-        if not skip_femio:
-            fem_data = femio.FEMData.read_directory(
-                read_simulation_type, write_simulation_base,
-                stem=write_simulation_stem, save=False,
-                read_mesh_only=False)
-        elif load_function:
-            if len(required_file_names) == 0:
-                raise ValueError(
-                    'Please specify required_file_names when skip_femio '
-                    'is True.')
-            data_files = util.collect_files(
-                write_simulation_base, required_file_names)
-            data_dict, fem_data = load_function(
-                data_files, write_simulation_base)
-            wrapped_fem_data = fem_data_utils.FemDataWrapper(fem_data)
-            wrapped_fem_data.update_fem_data(data_dict, allow_overwrite=True)
-            fem_data = wrapped_fem_data.fem_data
-        else:
-            raise ValueError(
-                'When skip_femio is True, please feed load_function.')
-
-        if convert_to_order1:
-            fem_data = fem_data.to_first_order()
-
-        wrapped_fem_data = fem_data_utils.FemDataWrapper(fem_data)
-        wrapped_fem_data.update_fem_data(dict_data_x, prefix='input_')
-        if dict_data_answer is not None:
-            wrapped_fem_data.update_fem_data(
-                dict_data_answer, prefix='answer_'
-            )
-        wrapped_fem_data.update_fem_data(dict_data_y, prefix='predicted_')
-
-        fem_data = wrapped_fem_data.fem_data
-        fem_data = add_difference(
-            fem_data, dict_data_y, dict_data_answer, prefix='difference_')
-        fem_data = add_abs_difference(
-            fem_data, dict_data_y, dict_data_answer, prefix='difference_abs_')
-        if data_addition_function is not None:
-            fem_data = data_addition_function(fem_data, write_simulation_base)
-
-        return fem_data
-
-    def _write_simulation(
-            self, output_directory, fem_data, *,
-            write_simulation_type='fistr', overwrite=False, less_output=False):
-        if write_simulation_type == 'fistr':
-            ext = ''
-        elif write_simulation_type == 'ucd':
-            ext = '.inp'
-        elif write_simulation_type == 'vtk':
-            ext = '.vtk'
-        elif write_simulation_type in ['polyvtk', 'vtu']:
-            ext = '.vtu'
-        else:
-            raise ValueError(
-                f"Unexpected write_simulation_type: {write_simulation_type}")
-        if less_output:
-            nodal_data = {}
-            for key in fem_data.nodal_data.keys():
-                if 'answer_' in key or 'predicted_' in key \
-                        or 'difference_' in key:
-                    nodal_data.update({
-                        key: fem_data.nodal_data.get_attribute_data(key)})
-                else:
-                    pass
-            fem_data.nodal_data.reset()
-
-            elemental_data = {}
-            for key in fem_data.elemental_data.keys():
-                if 'answer_' in key or 'predicted_' in key \
-                        or 'difference_' in key:
-                    elemental_data.update({
-                        key: fem_data.elemental_data.get_attribute_data(key)})
-                else:
-                    pass
-            if 'face' in fem_data.elemental_data:
-                face = fem_data.elemental_data['face']
-                has_face = True
-            else:
-                has_face = False
-            fem_data.elemental_data.reset()
-            fem_data.nodal_data.update_data(fem_data.nodes.ids, nodal_data)
-            fem_data.elemental_data.update_data(
-                fem_data.elements.ids, elemental_data)
-            if has_face:
-                fem_data.elemental_data['face'] = face
-
-        fem_data.write(
-            write_simulation_type, output_directory / ('mesh' + ext),
-            overwrite=overwrite)
-        return
-
-    def save(self, data_dict, output_directory):
-        if not output_directory.exists():
-            output_directory.mkdir(parents=True, exist_ok=True)
-        for variable_name, data in data_dict.items():
-            np.save(output_directory / f"{variable_name}.npy", data)
-        return
-
-
 def normalize_adjacency_matrix(adj):
     """Symmetrically normalize adjacency matrix.
 
     Parameters
     ----------
     adj: scipy.sparse.coo_matrix
         Adjacency matrix in COO expression.
```

## siml/preprocessing/__init__.py

```diff
@@ -1,3 +1,3 @@
-from . import converter  # NOQA
+from .converter import RawConverter  # NOQA
 from .scaling_converter import ScalingConverter  # NOQA
 from .scalers_composition import ScalersComposition  # NOQA
```

## siml/preprocessing/converter.py

```diff
@@ -5,15 +5,17 @@
 from operator import or_
 from typing import Dict, Tuple, Union
 
 import femio
 import numpy as np
 
 from siml import setting, util
-from siml.utils import fem_data_utils, path_utils
+from siml.utils import fem_data_utils
+from siml.services.path_rules import SimlPathRules
+from siml.base.siml_enums import DirectoryType
 
 
 class IConvertFunction(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def __call__(
         self,
         fem_data: femio.FEMData,
@@ -63,56 +65,58 @@
         load_function: ILoadFunction,
         filter_function: IFilterFunction,
         *,
         save_function: ISaveFunction = None,
         output_directory: pathlib.Path = None,
         raise_when_overwrite: bool = False,
         force_renew: bool = False,
-        save_results: bool = True
+        return_results: bool = False
     ) -> None:
 
         self.setting = setting
         self.raw_path = raw_path
         self.load_function = load_function
         self.save_function = save_function
 
         self.filter_function = filter_function
         self._output_directory = output_directory
         self.force_renew = force_renew
         self.raise_when_overwrite = raise_when_overwrite
-        self.save_results = save_results
+        self.return_results = return_results
 
-        if self.save_results and (self.save_function is None):
+        save_results = (not return_results)
+        if save_results and (self.save_function is None):
             raise ValueError(
                 "save_function is None when save_results option is True."
             )
 
     @property
     @cache
     def output_directory(self) -> pathlib.Path:
         if self._output_directory is not None:
             return self._output_directory
         else:
-            return path_utils.determine_output_directory(
+            rules = SimlPathRules()
+            return rules.determine_output_directory(
                 self.raw_path,
                 self.setting.output_base_directory,
-                'raw'
+                allowed_type=DirectoryType.RAW
             )
 
     def run(self) -> Union[None, dict]:
 
         values = self._convert()
         if values is None:
             print(
                 f"Conversion process for {self.raw_path} has failed"
             )
             return None
 
         dict_data, fem_data = values
-        if not self.save_results:
+        if self.return_results:
             return dict_data
 
         self.save_function(
             fem_data,
             dict_data,
             self.output_directory,
             self.force_renew
@@ -164,14 +168,17 @@
     def _check_directory(self) -> bool:
 
         # check raw path
         valid_raw_path = self._check_raw_path()
         if not valid_raw_path:
             return False
 
+        if self.return_results:
+            return True
+
         # check output directory
         valid_output_directory = self._check_output_direcotry()
         return valid_output_directory
 
     def _check_raw_path(self) -> bool:
         # Check raw_path
         if self.raw_path.is_file():
@@ -297,59 +304,59 @@
                 "cannot set at the same time"
             )
 
     def convert(
         self,
         raw_directory: pathlib.Path = None,
         *,
-        save_results: bool = True
+        return_results: bool = False
     ) -> dict[str, Union[dict, None]]:
         """Perform conversion.
 
         Parameters
         ----------
         raw_directory: pathlib.Path, optional
             Raw data directory name. If not fed, self.setting.data.raw is used
             instead.
 
-        save_results: bool, optional
+        return_results: bool, optional
             If True, save results and dump files
 
         Returns
         -------
         dict[str, Union[dict, None]]:
             key is a path to raw directory.
-            If save_results is True, values is a list of None.
-            If save_results is False, values is a dictionary
+            If return_results is False, values is a list of None.
+            If return_results is True, values is a dictionary
              of converted values.
         """
         print(f"# process: {self.max_process}")
         raw_directories = self._search_raw_directories(raw_directory)
         chunksize = max(len(raw_directories) // self.max_process // 16, 1)
 
         with multi.Pool(self.max_process) as pool:
             results = pool.map(
                 partial(
                     self.convert_single_data,
-                    save_results=save_results
+                    return_results=return_results
                 ),
                 raw_directories,
                 chunksize=chunksize
             )
 
         flatten_results = reduce(lambda x, y: x | y, results)
         return flatten_results
 
     def convert_single_data(
         self,
         raw_path: pathlib.Path,
         *,
         output_directory: pathlib.Path = None,
         raise_when_overwrite: bool = False,
-        save_results: bool = True
+        return_results: bool = False
     ) -> dict[str, Union[dict, None]]:
         """Convert single directory.
 
         Parameters
         ----------
         raw_path: pathlib.Path
             Input data path of raw data.
@@ -359,33 +366,32 @@
             If True, raise when the output directory exists. The default is
             False.
 
         Returns
         -------
         dict[str, Union[dict, None]]:
             key is a path to raw directory.
-            If save_results is True, values is a list of None.
-            If save_results is False, values is a dictionary
+            If return_results is False, values is a list of None.
+            If return_results is True, values is a dictionary
              of converted values.
         """
-
         load_function = self._create_load_function()
         save_function = self._create_save_function()
         filter_function = self._create_filter_function()
 
         single_converter = SingleDataConverter(
             setting=self.setting,
             raw_path=raw_path,
             load_function=load_function,
             save_function=save_function,
             filter_function=filter_function,
             output_directory=output_directory,
             raise_when_overwrite=raise_when_overwrite,
             force_renew=self.force_renew,
-            save_results=save_results
+            return_results=return_results
         )
 
         result = single_converter.run()
         return {str(raw_path): result}
 
     def _search_raw_directories(
         self,
```

## siml/preprocessing/scalers_composition.py

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 import multiprocessing as multi
 import warnings
 import pathlib
 from typing import Optional, Union, Final
 
 from siml import util
-from siml.path_like_objects import ISimlFile, SimlFileBulider, SimlFileExtType
+from siml.path_like_objects import SimlFileBuilder, ISimlNumpyFile
 from siml.siml_variables import ArrayDataType
 
 from .siml_scalers import SimlScalerWrapper
 
 
 class ScalersComposition():
     REGISTERED_KEY: Final[str] = "variable_name_to_scalers"
@@ -17,21 +17,15 @@
     @classmethod
     def create_from_file(
         cls,
         converter_parameters_pkl: pathlib.Path,
         max_process: Optional[int] = None,
         key: Optional[bytes] = None
     ) -> ScalersComposition:
-        siml_file = SimlFileBulider.create(converter_parameters_pkl)
-        if siml_file.get_file_extension() not in [
-                SimlFileExtType.PKLENC.value, SimlFileExtType.PKL.value]:
-            raise ValueError(
-                f"Input file: {converter_parameters_pkl} is not understandable"
-            )
-
+        siml_file = SimlFileBuilder.pickle_file(converter_parameters_pkl)
         parameters: dict = siml_file.load(
             decrypt_key=key
         )
         variable_name_to_scalers = parameters.pop(
             cls.REGISTERED_KEY, None
         )
         scalers_dict = ScalersComposition._load_scalers(parameters, key=key)
@@ -129,17 +123,17 @@
         # add relationship
         dumped_dict[self.REGISTERED_KEY] \
             = self._variable_name_to_scaler
         return dumped_dict
 
     def lazy_partial_fit(
         self,
-        scaler_name_to_files: dict[str, list[ISimlFile]]
+        scaler_name_to_files: dict[str, list[ISimlNumpyFile]]
     ) -> None:
-        preprocessor_inputs: list[tuple[str, list[ISimlFile]]] \
+        preprocessor_inputs: list[tuple[str, list[ISimlNumpyFile]]] \
             = [
                 (name, files)
                 for name, files in scaler_name_to_files.items()
         ]
 
         with multi.Pool(self.max_process) as pool:
             results = pool.starmap(
@@ -158,15 +152,15 @@
         scaler = self.get_scaler(variable_name)
         transformed_data = scaler.transform(data)
         return transformed_data
 
     def transform_file(
         self,
         variable_name: str,
-        siml_file: ISimlFile
+        siml_file: ISimlNumpyFile
     ) -> ArrayDataType:
 
         loaded_data = siml_file.load(
             decrypt_key=self._decrypt_key
         )
         scaler = self.get_scaler(variable_name)
         transformed_data = scaler.transform(loaded_data)
@@ -221,15 +215,15 @@
             converted_data = scaler.inverse_transform(data)
             converted_dict_data[variable_name] = converted_data
         return converted_dict_data
 
     def _lazy_partial_fit(
         self,
         variable_name: str,
-        data_files: list[ISimlFile]
+        data_files: list[ISimlNumpyFile]
     ) -> tuple[str, SimlScalerWrapper]:
         scaler = self.get_scaler(variable_name)
 
         scaler.lazy_partial_fit(data_files)
         return (variable_name, scaler)
 
     @staticmethod
```

## siml/preprocessing/scaling_converter.py

```diff
@@ -1,19 +1,21 @@
+from __future__ import annotations
 import multiprocessing as multi
 import pathlib
 import pickle
 from functools import partial
 from typing import Optional
 
 import pydantic
 import pydantic.dataclasses as dc
 from siml import setting, util
-from siml.path_like_objects import ISimlFile, SimlDirectory
-from siml.utils import path_utils
+from siml.path_like_objects import SimlDirectory, ISimlNumpyFile
 from siml.siml_variables import ArrayDataType
+from siml.services.path_rules import SimlPathRules
+from siml.base.siml_enums import DirectoryType
 
 from .siml_scalers import IScalingSaveFunction, DefaultSaveFunction
 from .scalers_composition import ScalersComposition
 
 
 class Config:
     init = True
@@ -23,15 +25,14 @@
 
 @dc.dataclass(config=Config)
 class PreprocessInnerSettings():
     preprocess_dict: dict
     interim_directories: list[pathlib.Path]
     preprocessed_root: pathlib.Path
     recursive: bool = True
-    str_replace: str = 'interim'
     REQUIRED_FILE_NAMES: Optional[list[str]] = None
     FINISHED_FILE: str = 'preprocessed'
     PREPROCESSORS_PKL_NAME: str = 'preprocessors.pkl'
 
     # cached value
     cached_interim_directories: Optional[list[SimlDirectory]] = None
 
@@ -79,15 +80,15 @@
 
     def collect_interim_directories(self) -> list[SimlDirectory]:
         return self.cached_interim_directories
 
     def get_scaler_fitting_files(
         self,
         variable_name: str
-    ) -> list[ISimlFile]:
+    ) -> list[ISimlNumpyFile]:
 
         preprocess_setting = self.preprocess_dict[variable_name]
         siml_directories = self.collect_interim_directories()
 
         data_files = [
             siml_dir.find_variable_file(variable_name)
             for siml_dir in siml_directories
@@ -99,79 +100,95 @@
             ]
         return data_files
 
     def get_output_directory(
         self,
         data_directory: pathlib.Path
     ) -> pathlib.Path:
-        output_directory = path_utils.determine_output_directory(
+        rules = SimlPathRules()
+        output_directory = rules.determine_output_directory(
             data_directory,
             self.preprocessed_root,
-            self.str_replace
+            allowed_type=DirectoryType.INTERIM
         )
         return output_directory
 
 
 class ScalingConverter:
     """
     This is Facade Class for scaling process
     """
     @classmethod
     def read_settings(cls, settings_yaml: pathlib.Path, **args):
         main_setting = setting.MainSetting.read_settings_yaml(
             settings_yaml, replace_preprocessed=False)
         return cls(main_setting, **args)
 
+    @classmethod
+    def read_pkl(
+        cls,
+        main_setting: setting.MainSetting,
+        converter_parameters_pkl: pathlib.Path,
+        key: bytes = None,
+    ):
+        scalers = ScalersComposition.create_from_file(
+            converter_parameters_pkl=converter_parameters_pkl,
+            key=key
+        )
+        return cls(
+            main_setting=main_setting,
+            scalers=scalers
+        )
+
     def __init__(
         self,
         main_setting: setting.MainSetting,
         *,
         force_renew: bool = False,
         save_func: Optional[IScalingSaveFunction] = None,
         max_process: int = None,
         allow_missing: bool = False,
         recursive: bool = True,
-        str_replace: str = 'interim',
+        scalers: Optional[ScalersComposition] = None
     ) -> None:
         """
         Initialize ScalingConverter
 
         Parameters
         ----------
             main_setting (setting.MainSetting): setting class
             force_renew: bool, optional
                 If True, renew npy files even if they are alerady exist.
             recursive: bool, optional
                 If True, search data recursively.
             save_func: callable, optional
                 Callback function to customize save data. It should accept
                 output_directory, variable_name, and transformed_data.
-            str_replace: str, optional
-                String to replace data directory in order to convert
-                from interim data to preprocessed data.
             max_process: int, optional
                 The maximum number of processes.
             allow_missing: bool, optional
                 If True, continue even if some of variables are missing.
         """
 
         self._setting = PreprocessInnerSettings(
             preprocess_dict=main_setting.preprocess,
             interim_directories=main_setting.data.interim,
             preprocessed_root=main_setting.data.preprocessed_root,
-            recursive=recursive,
-            str_replace=str_replace
+            recursive=recursive
         )
 
-        self._scalers: ScalersComposition \
-            = ScalersComposition.create_from_dict(
-                preprocess_dict=main_setting.preprocess,
-                max_process=max_process,
-                key=main_setting.data.encrypt_key
-            )
+        if scalers is None:
+            self._scalers: ScalersComposition \
+                = ScalersComposition.create_from_dict(
+                    preprocess_dict=main_setting.preprocess,
+                    max_process=max_process,
+                    key=main_setting.data.encrypt_key
+                )
+        else:
+            self._scalers = scalers
 
         self._decrypt_key = main_setting.data.encrypt_key
         self.max_process = max_process
         self.force_renew = force_renew
         self.save_func = self._initialize_save_function(save_func)
         self.allow_missing = allow_missing
```

## siml/preprocessing/siml_scalers/scaler_wrapper.py

```diff
@@ -2,15 +2,16 @@
 import gc
 from typing import Optional, Union
 import warnings
 
 import numpy as np
 import scipy.sparse as sp
 
-from siml.path_like_objects import ISimlFile, SimlFileExtType
+from siml.base.siml_enums import SimlFileExtType
+from siml.path_like_objects import ISimlNumpyFile
 from siml.preprocessing.siml_scalers import ISimlScaler, scale_functions
 from siml.siml_variables import ArrayDataType, create_siml_arrray
 
 
 class SimlScalerWrapper(ISimlScaler):
     @classmethod
     def create(cls, dict_data: dict, key: Optional[bytes] = None):
@@ -98,15 +99,15 @@
             skip_nan=False,
             use_diagonal=False
         )
         return result
 
     def lazy_partial_fit(
         self,
-        data_files: list[ISimlFile]
+        data_files: list[ISimlNumpyFile]
     ) -> None:
         for data_file in data_files:
             print(f"Start load data: {data_file}")
             print(dt.datetime.now())
             data = self._load_file(data_file)
             print(f"Start partial_fit: {data_file}")
             print(dt.datetime.now())
@@ -127,20 +128,20 @@
             'componentwise': self.componentwise,
             'preprocess_converter': vars(self.converter)
         }
         return dumped_dict
 
     def _load_file(
         self,
-        siml_file: ISimlFile
+        siml_file: ISimlNumpyFile
     ) -> ArrayDataType:
 
         loaded_data = siml_file.load(decrypt_key=self.key)
 
-        if siml_file.get_file_extension() in [
+        if siml_file.file_extension in [
                 SimlFileExtType.NPZENC.value, SimlFileExtType.NPZ.value]:
             if not sp.issparse(loaded_data):
                 raise ValueError(
                     f"Data type not understood for: {siml_file.file_path}"
                 )
 
         return loaded_data
```

## siml/setting.py

```diff
@@ -1,19 +1,21 @@
 import dataclasses as dc
-from enum import Enum
 import io
 import os
-from pathlib import Path
 import typing
+from enum import Enum
+from pathlib import Path
+from typing import Optional
 
 import numpy as np
 import optuna
 import yaml
 
-from . import util
+from siml import util
+from siml.path_like_objects import SimlFileBuilder
 
 
 @dc.dataclass
 class TypedDataClass:
 
     @classmethod
     def read_settings_yaml(cls, settings_yaml):
@@ -340,14 +342,18 @@
             return {
                 dict_key: dict_value.collect_values(key, default=default)
                 for dict_key, dict_value in data.items()}
         else:
             raise ValueError(f"Unexpected data: {data}")
 
     @property
+    def is_dict(self):
+        return isinstance(self.variables, dict)
+
+    @property
     def names(self):
         return self.collect_values('name')
 
     @property
     def dims(self):
         return self.collect_values('dim', default=1)
 
@@ -369,14 +375,21 @@
         if isinstance(s, list):
             return s[0]
         elif isinstance(s, dict):
             return {k: v[0] for k, v in s.items()}
         else:
             raise ValueError(f"Invalid format: {s}")
 
+    def get_time_series_keys(self):
+        if not isinstance(self.time_series, dict):
+            return []
+        return [
+            k for k, v in self.time_series.items() if np.any(v)
+        ]
+
     def to_dict(self):
         if isinstance(self.variables, dict):
             ret_dict = {}
             for value in self.variables.values():
                 ret_dict.update(value.to_dict())
             return ret_dict
         elif isinstance(self.variables, list):
@@ -674,14 +687,22 @@
 
     @property
     def variable_information(self):
         out_dict = self.inputs.to_dict()
         out_dict.update(self.outputs.to_dict())
         return out_dict
 
+    def determine_element_wise(self) -> bool:
+        if self.time_series:
+            return False
+        if self.element_wise or self.simplified_model:
+            return True
+
+        return False
+
     def update_output_directory(self, *, id_=None, base=None):
         if base is None:
             base = Path(self.output_directory_base)
         else:
             base = Path(base)
         if id_ is None:
             id_string = ''
@@ -772,14 +793,16 @@
     perform_inverse: bool = True
     return_all_results: bool = True
     model_key: bytes = dc.field(
         default=None, metadata={'allow_none': True})
     gpu_id: int = -1
     less_output: bool = False
     skip_fem_data_creation: bool = False
+    infer_epoch: int = dc.field(
+        default=None, metadata={'allow_none': True})
 
 
 @dc.dataclass
 class BlockSetting(TypedDataClass):
     name: str = 'Block'
     is_first: bool = False
     is_last: bool = False
@@ -1142,23 +1165,34 @@
     model: ModelSetting = ModelSetting()
     optuna: OptunaSetting = OptunaSetting()
     study: StudySetting = StudySetting()
     replace_preprocessed: bool = False
     misc: dict = dc.field(default_factory=dict)
 
     @classmethod
-    def read_settings_yaml(cls, settings_yaml, replace_preprocessed=False):
-        dict_settings = util.load_yaml(settings_yaml)
-        if isinstance(settings_yaml, Path):
-            name = settings_yaml.stem
+    def read_settings_yaml(
+        cls,
+        settings_yaml: Path,
+        replace_preprocessed=False,
+        *,
+        decrypt_key: Optional[bytes] = None
+    ):
+
+        siml_file = SimlFileBuilder.yaml_file(settings_yaml)
+        dict_settings = siml_file.load(decrypt_key=decrypt_key)
+        if not siml_file.is_encrypted:
+            name = siml_file.file_path.stem
         else:
             name = None
+
         return cls.read_dict_settings(
-            dict_settings, name=name,
-            replace_preprocessed=replace_preprocessed)
+            dict_settings,
+            name=name,
+            replace_preprocessed=replace_preprocessed
+        )
 
     @classmethod
     def read_dict_settings(
             cls, dict_settings, *, name=None, replace_preprocessed=False):
         if 'trainer' in dict_settings \
                 and 'name' not in dict_settings['trainer']:
             if name is None:
@@ -1238,14 +1272,26 @@
                     != str(self.data.train[0]):
                 print(
                     'self.data.preprocessed differs from self.data.train. '
                     'Replaced.')
                 self.data.preprocessed = [self.data.train[0].parent]
         return
 
+    def get_crypt_key(self):
+        if self.data.encrypt_key is not None:
+            return self.data.encrypt_key
+
+        if self.inferer.model_key is not None:
+            return self.inferer.model_key
+
+        if self.trainer.model_key is not None:
+            return self.trainer.model_key
+
+        return None
+
     def update_with_dict(self, new_dict):
         original_dict = dc.asdict(self)
         return MainSetting.read_dict_settings(
             self._update_with_dict(original_dict, new_dict))
 
     def _update_with_dict(self, original_setting, new_setting):
         if isinstance(new_setting, str) or isinstance(new_setting, float) \
```

## siml/siml_variables/__init__.py

```diff
@@ -1,3 +1,3 @@
 # flake8: noqa
 from .array_variables import ArrayDataType, create_siml_arrray
-from .tensor_variables.tensor_variables import siml_tensor_variables
+from .tensor_variables.tensor_variables import siml_tensor_variables, ISimlVariables
```

## siml/siml_variables/array_variables/__init__.py

```diff
@@ -1,25 +1,23 @@
 # flake8: noqa
-from typing import Union
+from typing import get_args
 
-import numpy as np
 import scipy.sparse as sp
+import numpy as np
+
+from siml.base.siml_typing import ArrayDataType
 
 from .interface_wrapper import ISimlArray
 from .ndarray_wrapper import NdArrayWrapper
 from .sparce_array_wrapper import SparseArrayWrapper, SparseArrayType
 
-ArrayDataType = Union[
-    np.ndarray, sp.coo_matrix, sp.csr_matrix, sp.csc_matrix
-]
-
 
 def create_siml_arrray(
     data: ArrayDataType
 ) -> ISimlArray:
     if isinstance(data, np.ndarray):
         return NdArrayWrapper(data)
 
-    if isinstance(data, (sp.coo_matrix, sp.csr_matrix, sp.csc_matrix)):
+    if isinstance(data, get_args(SparseArrayType)):
         return SparseArrayWrapper(data)
 
     raise ValueError(f"Unsupported data type: {data.__class__}")
```

## siml/siml_variables/array_variables/sparce_array_wrapper.py

```diff
@@ -1,17 +1,15 @@
 import datetime as dt
-from typing import Union, Callable
+from typing import Callable
 import warnings
 
-import scipy.sparse as sp
+from siml.base.siml_typing import SparseArrayType
 
 from .interface_wrapper import ISimlArray
 
-SparseArrayType = Union[sp.coo_matrix, sp.csr_matrix, sp.csc_matrix]
-
 
 class SparseArrayWrapper(ISimlArray):
     def __init__(
         self,
         data: SparseArrayType
     ) -> None:
         self.data = data
```

## siml/siml_variables/tensor_variables/tensor_variables.py

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
-from typing import TypeVar
+from typing import TypeVar, Any
 
 import torch
+import numpy as np
 
 BuiltInVars = TypeVar(
     'BuiltInVars',
     torch.Tensor, dict, list
 )
 
 
@@ -19,14 +20,20 @@
 
     def slice(self, loss_slice: slice) -> ISimlVariables:
         raise NotImplementedError()
 
     def send(self, device: str) -> ISimlVariables:
         raise NotImplementedError()
 
+    def min_len(self) -> int:
+        raise NotImplementedError()
+
+    def to_numpy(self) -> Any:
+        raise NotImplementedError()
+
 
 def siml_tensor_variables(values: BuiltInVars) -> ISimlVariables:
     if isinstance(values, torch.Tensor):
         return TensorSimlVariables(values)
     if isinstance(values, dict):
         return DictSimlVariables(values)
     if isinstance(values, list):
@@ -63,14 +70,20 @@
         tmp = self._x[loss_slice]
         return TensorSimlVariables(tmp)
 
     def send(self, device: str) -> TensorSimlVariables:
         tmp = self._x.to(device)
         return TensorSimlVariables(tmp)
 
+    def min_len(self) -> int:
+        return len(self._x)
+
+    def to_numpy(self) -> Any:
+        return self._x.cpu().detach().numpy()
+
 
 class DictSimlVariables(ISimlVariables):
     def __init__(self, value: dict):
         self._x = {k: siml_tensor_variables(v) for k, v in value.items()}
 
     def __str__(self) -> str:
         txt = ""
@@ -86,14 +99,20 @@
         tmp = {k: v.slice(loss_slice) for k, v in self._x.items()}
         return DictSimlVariables(tmp)
 
     def send(self, device: str) -> TensorSimlVariables:
         tmp = {k: v.send(device) for k, v in self._x.items()}
         return DictSimlVariables(tmp)
 
+    def min_len(self) -> int:
+        return np.min([x.min_len() for x in self._x.values()])
+
+    def to_numpy(self) -> Any:
+        return {k: v.to_numpy() for k, v in self._x.items()}
+
 
 class ListSimlVaraiables(ISimlVariables):
     def __init__(self, value: list[torch.Tensor]):
         self._x = [siml_tensor_variables(v) for v in value]
 
     def __str__(self) -> str:
         values = [str(v) for v in self._x]
@@ -107,7 +126,13 @@
     def slice(self, loss_slice: slice) -> ListSimlVaraiables:
         tmp = [v.slice(loss_slice) for v in self._x]
         return ListSimlVaraiables(tmp)
 
     def send(self, device: str) -> ListSimlVaraiables:
         tmp = [v.send(device) for v in self._x]
         return ListSimlVaraiables(tmp)
+
+    def min_len(self) -> int:
+        return np.min([x.min_len() for x in self._x])
+
+    def to_numpy(self) -> Any:
+        return [v.to_numpy() for v in self._x]
```

## siml/trainer.py

```diff
@@ -27,15 +27,15 @@
 
 class Trainer(siml_manager.SimlManager):
 
     def __init__(self,
                  settings,
                  *,
                  optuna_trial=None,
-                 user_loss_fundtion_dic:
+                 user_loss_function_dic:
                  dict[str, Callable[[Tensor, Tensor], Tensor]] = None):
         """Initialize SimlManager object.
 
         Parameters
         ----------
         settings: siml.setting.MainSetting object or pathlib.Path
             Setting descriptions.
@@ -54,15 +54,15 @@
                 settings)
         elif isinstance(settings, setting.MainSetting):
             self.setting = settings
         else:
             raise ValueError(
                 f"Unknown type for settings: {settings.__class__}")
         self.inference_mode = False
-        self.user_loss_function_dic = user_loss_fundtion_dic
+        self.user_loss_function_dic = user_loss_function_dic
 
         self._update_setting_if_needed()
         self.optuna_trial = optuna_trial
         return
 
     def train(self):
         """Perform training.
```

## siml/utils/__init__.py

```diff
@@ -1,3 +1 @@
-
-from . import path_utils  # NOQA
 from . import fem_data_utils  # NOQA
```

## siml/utils/fem_data_utils.py

```diff
@@ -144,14 +144,74 @@
             else:
                 variable_name = prefix + key
         else:
             variable_name = prefix + key
 
         return variable_name
 
+    def add_difference(
+        self,
+        dict_data: dict,
+        reference_dict_data: dict,
+        prefix: str = 'difference'
+    ) -> None:
+        if reference_dict_data is None:
+            return
+
+        intersections = \
+            set(dict_data.keys()).intersection(reference_dict_data.keys())
+        if len(intersections) == 0:
+            return
+
+        difference_dict_data = {
+            intersection:
+            np.reshape(
+                dict_data[intersection],
+                reference_dict_data[intersection].shape
+            )
+            - reference_dict_data[intersection]
+            for intersection in intersections
+        }
+
+        self.update_fem_data(
+            difference_dict_data,
+            prefix=prefix
+        )
+
+    def add_abs_difference(
+        self,
+        dict_data: dict,
+        reference_dict_data: dict,
+        prefix: str = 'difference_abs'
+    ) -> None:
+        if reference_dict_data is None:
+            return
+
+        intersections = \
+            set(dict_data.keys()).intersection(reference_dict_data.keys())
+        if len(intersections) == 0:
+            return
+
+        difference_dict_data = {
+            intersection:
+            np.abs(
+                np.reshape(
+                    dict_data[intersection],
+                    reference_dict_data[intersection].shape
+                )
+                - reference_dict_data[intersection]
+            )
+            for intersection in intersections
+        }
+
+        self.update_fem_data(
+            difference_dict_data,
+            prefix=prefix
+        )
+
 
 def reshape_data_if_needed(value: np.ndarray):
     """Reshape numpy.ndarray-like to be writable to visualization files.
 
     Parameters
     ----------
     value: numpy.ndarray
```

## Comparing `siml/postprocessor.py` & `siml/services/inference/metrics_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,178 @@
+from __future__ import annotations
+from typing import Union
 
-from ignite.metrics.metric import Metric, reinit__is_reduced
 import numpy as np
 import torch
+from ignite.metrics.metric import Metric, reinit__is_reduced
 
-from . import datasets
+from siml import setting
+from siml.loss_operations import ILossCalculator
 
+from .record_object import PredictionRecord, PostPredictionRecord
 
-class Postprocessor(Metric):
 
-    def __init__(self, inferer):
+class MetricsBuilder():
+    def __init__(
+        self,
+        trainer_setting: setting.TrainerSetting,
+        loss_function: ILossCalculator
+    ) -> None:
+
+        self._trainer_setting = trainer_setting
+        self.loss_function = loss_function
+
+    def create(self) -> dict[str, Metric]:
+        metrics = {
+            'post_results': PostResultsMetrics(),
+            'loss': LossMetrics(
+                loss_function=self.loss_function
+            ),
+            'raw_loss': RawLossMetrics(
+                trainer_setting=self._trainer_setting,
+                loss_function=self.loss_function
+            )
+        }
+        return metrics
+
+
+class PostResultsMetrics(Metric):
+    def __init__(
+        self
+    ) -> None:
         super().__init__()
-        self.inferer = inferer
-        return
 
     @reinit__is_reduced
     def reset(self):
         self._results = []
         return
 
     @reinit__is_reduced
-    def update(self, data):
+    def update(self, output):
+        record: PostPredictionRecord = output[2]["post_result"]
+        self._results.append(record)
+        return
+
+    def compute(self):
+        return self._results
+
+
+class LossMetrics(Metric):
+    def __init__(
+        self,
+        loss_function: ILossCalculator
+    ) -> None:
+        super().__init__()
+        self.loss_function = loss_function
+
+    @reinit__is_reduced
+    def reset(self):
+        self._results = []
+        return
 
-        y_pred, y = data[0], data[1]
-        x = data[2]['x']
-        data_directory = data[2]['data_directory']
-        inference_time = data[2]['inference_time']
-        loss = self.inferer.loss(
-            y_pred, y, x['original_shapes'])
+    @reinit__is_reduced
+    def update(self, output):
+        y_pred = output[0]
+        y = output[1]
+        record: PredictionRecord = output[2]["result"]
+        loss = self.loss_function(
+            y_pred,
+            y,
+            original_shapes=record.original_shapes
+        )
         if loss is not None:
-            loss = loss.cpu().detach().numpy()
+            print(f"              Loss: {loss}")
 
-        dict_var_x = self.inferer._separate_data(
-            self._to_numpy(x['x']), self.inferer.setting.trainer.inputs)
-        dict_var_y = self.inferer._separate_data(
-            self._to_numpy(y), self.inferer.setting.trainer.outputs)
-        dict_var_y_pred = self.inferer._separate_data(
-            self._to_numpy(y_pred), self.inferer.setting.trainer.outputs)
-
-        output_directory = self.inferer._determine_output_directory(
-            data_directory)
-        write_simulation_base = self.inferer._determine_write_simulation_base(
-            data_directory)
-
-        setting = self.inferer.setting
-        inversed_dict_x, inversed_dict_y, inversed_dict_answer, fem_data \
-            = self.inferer.prepost_converter.postprocess(
-                dict_var_x, dict_var_y_pred,
-                output_directory=output_directory,
-                dict_data_y_answer=dict_var_y,
-                skip_femio=setting.conversion.skip_femio,
-                load_function=self.inferer.load_function,
-                data_addition_function=self.inferer.data_addition_function,
-                overwrite=setting.inferer.overwrite,
-                save_x=setting.inferer.save,
-                write_simulation=setting.inferer.write_simulation,
-                write_npy=setting.inferer.write_npy,
-                write_simulation_stem=setting.inferer.write_simulation_stem,
-                write_simulation_base=write_simulation_base,
-                read_simulation_type=setting.inferer.read_simulation_type,
-                write_simulation_type=setting.inferer.write_simulation_type,
-                save_function=self.inferer.save_function,
-                convert_to_order1=setting.inferer.convert_to_order1,
-                required_file_names=setting.conversion.required_file_names,
-                less_output=setting.inferer.less_output,
-                perform_inverse=setting.inferer.perform_inverse,
-                skip_fem_data_creation=setting.inferer.skip_fem_data_creation)
-        raw_loss = self._compute_raw_loss(
-            inversed_dict_answer, inversed_dict_y, x['original_shapes'])
+            loss = loss.cpu().detach().numpy().item()
+        self._results.append(loss)
+        return
 
-        if self.inferer.postprocess_function is not None:
-            inversed_dict_x, inversed_dict_y, fem_data \
-                = self.inferer.postprocess_function(
-                    inversed_dict_x, inversed_dict_y, fem_data)
-
-        if self.inferer.setting.inferer.return_all_results:
-            self._results.append({
-                'dict_x': inversed_dict_x, 'dict_y': inversed_dict_y,
-                'dict_answer': inversed_dict_answer,
-                'fem_data': fem_data,
-                'loss': loss,
-                'raw_loss': raw_loss,
-                'output_directory': output_directory,
-                'data_directory': data_directory,
-                'inference_time': inference_time})
-        else:
-            # Keep only small data to save memory
-            self._results.append({
-                'loss': loss,
-                'raw_loss': raw_loss,
-                'output_directory': output_directory,
-                'data_directory': data_directory,
-                'inference_time': inference_time})
+    def compute(self):
+        return self._results
+
+
+class RawLossMetrics(Metric):
+
+    def __init__(
+        self,
+        trainer_setting: setting.TrainerSetting,
+        loss_function: ILossCalculator
+    ) -> None:
+        super().__init__()
+        self._trainer_setting = trainer_setting
+        self.loss_function = loss_function
+
+    @reinit__is_reduced
+    def reset(self):
+        self._results = []
         return
 
-    def _to_numpy(self, x):
-        if isinstance(x, (datasets.DataDict, dict)):
-            return {
-                key: value.cpu().detach().numpy() for key, value in x.items()}
-        else:
-            return x.cpu().detach().numpy()
+    @reinit__is_reduced
+    def update(self, output):
+        post_result: PostPredictionRecord = output[2]["post_result"]
+        raw_loss = self._compute_raw_loss(
+            post_result.dict_answer,
+            post_result.dict_y,
+            post_result.original_shapes
+        )
+
+        if raw_loss is not None:
+            raw_loss = raw_loss.item()
+        self._results.append(raw_loss)
+        return
 
     def compute(self):
         return self._results
 
-    def _compute_raw_loss(self, dict_answer, dict_y, original_shapes=None):
+    def _compute_raw_loss(
+        self,
+        dict_answer: dict[str, np.ndarray],
+        dict_y: dict[str, np.ndarray],
+        original_shapes: tuple = None
+    ) -> Union[np.ndarray, None]:
+
         if dict_answer is None:
             return None  # No answer
+
         y_keys = dict_y.keys()
         if not np.all([y_key in dict_answer for y_key in y_keys]):
             return None  # No answer
 
-        if isinstance(self.inferer.setting.trainer.output_names, dict):
-            output_names = self.inferer.setting.trainer.output_names
+        if isinstance(self._trainer_setting.output_names, dict):
+            output_names = self._trainer_setting.output_names
             y_raw_pred = self._reshape_dict(output_names, dict_y)
             y_raw_answer = self._reshape_dict(output_names, dict_answer)
         else:
             y_raw_pred = torch.from_numpy(
-                np.concatenate([dict_y[k] for k in dict_y.keys()], axis=-1))
+                np.concatenate(
+                    [dict_y[k] for k in dict_y.keys()],
+                    axis=-1
+                )
+            )
             y_raw_answer = torch.from_numpy(
                 np.concatenate(
-                    [dict_answer[k] for k in dict_y.keys()], axis=-1))
+                    [dict_answer[k] for k in dict_y.keys()],
+                    axis=-1
+                )
+            )
 
-        raw_loss = self.inferer.loss(
+        raw_loss = self.loss_function(
             y_raw_pred, y_raw_answer, original_shapes=original_shapes)
         if raw_loss is None:
             return None
         else:
             return raw_loss.numpy()
 
-    def _reshape_dict(self, dict_names, data_dict):
+    def _reshape_dict(
+        self,
+        dict_names: list[str],
+        data_dict: dict
+    ) -> dict[str: torch.Tensor]:
         return {
             key:
-            torch.from_numpy(np.concatenate([
-                data_dict[variable_name] for variable_name in value]))
+            torch.from_numpy(
+                np.concatenate([
+                    data_dict[variable_name] for variable_name in value
+                ])
+            )
             for key, value in dict_names.items()
             if key in data_dict.keys()}
```

## Comparing `pysiml-0.2.9.dev202305021032.dist-info/LICENSE` & `pysiml-0.2.9.dev202305240600.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pysiml-0.2.9.dev202305021032.dist-info/METADATA` & `pysiml-0.2.9.dev202305240600.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysiml
-Version: 0.2.9.dev202305021032
+Version: 0.2.9.dev202305240600
 Summary: SiML - a Simulation ML library
 Home-page: https://github.com/ricosjp/pysiml
 License: Apache-2.0
 Author: RICOS Co. Ltd.
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

