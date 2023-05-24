# Comparing `tmp/mlcvzoo_base-5.3.3.tar.gz` & `tmp/mlcvzoo_base-5.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_base-5.3.3.tar", max compression
+gzip compressed data, was "mlcvzoo_base-5.3.4.tar", max compression
```

## Comparing `mlcvzoo_base-5.3.3.tar` & `mlcvzoo_base-5.3.4.tar`

### file list

```diff
@@ -1,101 +1,102 @@
--rw-r--r--   0        0        0    11412 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/LICENSE
--rw-r--r--   0        0        0      546 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/README.md
--rw-r--r--   0        0        0      244 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/__init__.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/__init__.py
--rw-r--r--   0        0        0     1021 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/configuration.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/__init__.py
--rw-r--r--   0        0        0    11270 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation.py
--rw-r--r--   0        0        0      816 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_attributes.py
--rw-r--r--   0        0        0     2429 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_builder.py
--rw-r--r--   0        0        0    26777 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_class_mapper.py
--rw-r--r--   0        0        0     1130 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_parser.py
--rw-r--r--   0        0        0      975 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_writer.py
--rw-r--r--   0        0        0     6146 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/bounding_box.py
--rw-r--r--   0        0        0    13021 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/box.py
--rw-r--r--   0        0        0     2734 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/class_identifier.py
--rw-r--r--   0        0        0     5253 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/classification.py
--rw-r--r--   0        0        0     3941 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/dataset_info.py
--rw-r--r--   0        0        0     3268 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/ocr_perception.py
--rw-r--r--   0        0        0    11655 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/segmentation.py
--rw-r--r--   0        0        0      362 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/types.py
--rw-r--r--   0        0        0      906 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/exceptions.py
--rw-r--r--   0        0        0     5029 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/interfaces.py
--rw-r--r--   0        0        0    12243 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/model.py
--rw-r--r--   0        0        0     2333 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/registry.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/__init__.py
--rw-r--r--   0        0        0     8184 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/annotation_handler_config.py
--rw-r--r--   0        0        0     3942 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/class_mapping_config.py
--rw-r--r--   0        0        0      656 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/config_registry.py
--rw-r--r--   0        0        0      772 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/device_query.py
--rw-r--r--   0        0        0     1692 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/mlfow_config.py
--rw-r--r--   0        0        0     3093 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/model_config.py
--rw-r--r--   0        0        0     2589 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/reduction_mapping_config.py
--rw-r--r--   0        0        0     3889 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/replacement_config.py
--rw-r--r--   0        0        0     3939 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/structs.py
--rw-r--r--   0        0        0     7286 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/utils.py
--rw-r--r--   0        0        0      628 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/visualization_config.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/__init__.py
--rw-r--r--   0        0        0      256 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/__init__.py
--rw-r--r--   0        0        0     8663 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py
--rw-r--r--   0        0        0     7121 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py
--rw-r--r--   0        0        0     2458 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py
--rw-r--r--   0        0        0     8862 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py
--rw-r--r--   0        0        0     6066 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py
--rw-r--r--   0        0        0    14648 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_handler.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/__init__.py
--rw-r--r--   0        0        0     3289 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py
--rw-r--r--   0        0        0     8168 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py
--rw-r--r--   0        0        0    11628 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py
--rw-r--r--   0        0        0     7841 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py
--rw-r--r--   0        0        0    10617 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py
--rw-r--r--   0        0        0     9205 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/__init__.py
--rw-r--r--   0        0        0    14717 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py
--rw-r--r--   0        0        0     8684 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py
--rw-r--r--   0        0        0     4097 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py
--rw-r--r--   0        0        0      501 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/structs.py
--rw-r--r--   0        0        0    11234 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/utils.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/__init__.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/__init__.py
--rw-r--r--   0        0        0     2227 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/configuration.py
--rw-r--r--   0        0        0     6836 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/data_classes.py
--rw-r--r--   0        0        0    54097 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/metrics_computation.py
--rw-r--r--   0        0        0    12295 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/metrics_logging.py
--rw-r--r--   0        0        0     4134 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/model_evaluation.py
--rw-r--r--   0        0        0      633 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/structs.py
--rw-r--r--   0        0        0    15646 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/utils.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/__init__.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/mlflow/__init__.py
--rw-r--r--   0        0        0     7255 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/mlflow/mlflow_runner.py
--rw-r--r--   0        0        0     1676 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/mlflow/utils.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/__init__.py
--rw-r--r--   0        0        0      257 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/constants.py
--rw-r--r--   0        0        0    10705 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/model_registry.py
--rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/read_from_file/__init__.py
--rw-r--r--   0        0        0     1540 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/read_from_file/configuration.py
--rw-r--r--   0        0        0    10713 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/read_from_file/model.py
--rw-r--r--   0        0        0        0 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/__init__.py
--rw-r--r--   0        0        0     1078 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE
--rw-r--r--   0        0        0      138 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/README.md
--rw-r--r--   0        0        0      249 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/__init__.py
--rw-r--r--   0        0        0     1774 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py
--rw-r--r--   0        0        0     1117 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/LICENSE.txt
--rw-r--r--   0        0        0      108 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/README.md
--rw-r--r--   0        0        0      296 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/__init__.py
--rw-r--r--   0        0        0     2794 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/perspective.py
--rw-r--r--   0        0        0     3744 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE
--rw-r--r--   0        0        0      127 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/README.md
--rw-r--r--   0        0        0      249 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/__init__.py
--rw-r--r--   0        0        0     1649 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py
--rw-r--r--   0        0        0      488 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/__init__.py
--rw-r--r--   0        0        0     4725 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/annotation_utils.py
--rw-r--r--   0        0        0     2353 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/common_utils.py
--rw-r--r--   0        0        0    11836 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/draw_utils.py
--rw-r--r--   0        0        0     5992 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/file_utils.py
--rw-r--r--   0        0        0     5852 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/gpu_util.py
--rw-r--r--   0        0        0     3009 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/implicit_path_replacements.py
--rw-r--r--   0        0        0     2435 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/versioning_utils.py
--rw-r--r--   0        0        0     3811 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/xml_utils.py
--rw-r--r--   0        0        0     4007 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/pyproject.toml
--rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 mlcvzoo_base-5.3.3/setup.py
--rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 mlcvzoo_base-5.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/LICENSE
+-rw-r--r--   0        0        0      546 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/README.md
+-rw-r--r--   0        0        0      244 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/__init__.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/__init__.py
+-rw-r--r--   0        0        0     1021 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/configuration.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/__init__.py
+-rw-r--r--   0        0        0    11270 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation.py
+-rw-r--r--   0        0        0      816 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_attributes.py
+-rw-r--r--   0        0        0     2429 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_builder.py
+-rw-r--r--   0        0        0    26777 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_class_mapper.py
+-rw-r--r--   0        0        0     1130 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_parser.py
+-rw-r--r--   0        0        0      975 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_writer.py
+-rw-r--r--   0        0        0     6146 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/bounding_box.py
+-rw-r--r--   0        0        0    13021 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/box.py
+-rw-r--r--   0        0        0     2734 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/class_identifier.py
+-rw-r--r--   0        0        0     5253 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/classification.py
+-rw-r--r--   0        0        0     3941 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/dataset_info.py
+-rw-r--r--   0        0        0     3268 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/ocr_perception.py
+-rw-r--r--   0        0        0    11655 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/segmentation.py
+-rw-r--r--   0        0        0      362 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/types.py
+-rw-r--r--   0        0        0      906 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/exceptions.py
+-rw-r--r--   0        0        0     5029 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/interfaces.py
+-rw-r--r--   0        0        0    12243 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/model.py
+-rw-r--r--   0        0        0     2333 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/registry.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/__init__.py
+-rw-r--r--   0        0        0     8184 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/annotation_handler_config.py
+-rw-r--r--   0        0        0     3942 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/class_mapping_config.py
+-rw-r--r--   0        0        0      656 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/config_registry.py
+-rw-r--r--   0        0        0      772 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/device_query.py
+-rw-r--r--   0        0        0     1692 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/mlfow_config.py
+-rw-r--r--   0        0        0     3093 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/model_config.py
+-rw-r--r--   0        0        0     2589 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/reduction_mapping_config.py
+-rw-r--r--   0        0        0     3889 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/replacement_config.py
+-rw-r--r--   0        0        0     3939 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/structs.py
+-rw-r--r--   0        0        0     7286 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/utils.py
+-rw-r--r--   0        0        0      628 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/visualization_config.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/__init__.py
+-rw-r--r--   0        0        0     8663 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py
+-rw-r--r--   0        0        0     7121 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py
+-rw-r--r--   0        0        0     2458 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py
+-rw-r--r--   0        0        0     8862 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py
+-rw-r--r--   0        0        0     6066 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py
+-rw-r--r--   0        0        0    14648 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_handler.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/__init__.py
+-rw-r--r--   0        0        0     3289 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py
+-rw-r--r--   0        0        0     8168 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py
+-rw-r--r--   0        0        0    11628 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py
+-rw-r--r--   0        0        0     7841 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py
+-rw-r--r--   0        0        0    10617 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py
+-rw-r--r--   0        0        0     9205 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/__init__.py
+-rw-r--r--   0        0        0    14717 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py
+-rw-r--r--   0        0        0     8684 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py
+-rw-r--r--   0        0        0     4097 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py
+-rw-r--r--   0        0        0      501 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/structs.py
+-rw-r--r--   0        0        0    11234 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/utils.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/__init__.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/__init__.py
+-rw-r--r--   0        0        0     2227 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/configuration.py
+-rw-r--r--   0        0        0     6836 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/data_classes.py
+-rw-r--r--   0        0        0    54097 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/metrics_computation.py
+-rw-r--r--   0        0        0    12295 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/metrics_logging.py
+-rw-r--r--   0        0        0     4134 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/model_evaluation.py
+-rw-r--r--   0        0        0      633 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/structs.py
+-rw-r--r--   0        0        0    15646 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/utils.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/__init__.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/mlflow/__init__.py
+-rw-r--r--   0        0        0     7255 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/mlflow/mlflow_runner.py
+-rw-r--r--   0        0        0     1676 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/mlflow/utils.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/__init__.py
+-rw-r--r--   0        0        0      257 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/constants.py
+-rw-r--r--   0        0        0    10705 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/model_registry.py
+-rw-r--r--   0        0        0      196 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/read_from_file/__init__.py
+-rw-r--r--   0        0        0     1540 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/read_from_file/configuration.py
+-rw-r--r--   0        0        0    10713 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/read_from_file/model.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/py.typed
+-rw-r--r--   0        0        0        0 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/__init__.py
+-rw-r--r--   0        0        0     1078 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE
+-rw-r--r--   0        0        0      138 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/README.md
+-rw-r--r--   0        0        0      249 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/__init__.py
+-rw-r--r--   0        0        0     1774 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py
+-rw-r--r--   0        0        0     1117 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/LICENSE.txt
+-rw-r--r--   0        0        0      108 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/README.md
+-rw-r--r--   0        0        0      296 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/__init__.py
+-rw-r--r--   0        0        0     2794 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/perspective.py
+-rw-r--r--   0        0        0     3744 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE
+-rw-r--r--   0        0        0      127 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/README.md
+-rw-r--r--   0        0        0      249 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/__init__.py
+-rw-r--r--   0        0        0     1649 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py
+-rw-r--r--   0        0        0      488 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/__init__.py
+-rw-r--r--   0        0        0     4725 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/annotation_utils.py
+-rw-r--r--   0        0        0     2353 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/common_utils.py
+-rw-r--r--   0        0        0    11836 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/draw_utils.py
+-rw-r--r--   0        0        0     5992 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/file_utils.py
+-rw-r--r--   0        0        0     5852 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/gpu_util.py
+-rw-r--r--   0        0        0     3009 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/implicit_path_replacements.py
+-rw-r--r--   0        0        0     2435 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/versioning_utils.py
+-rw-r--r--   0        0        0     3811 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/xml_utils.py
+-rw-r--r--   0        0        0     4007 2023-05-24 07:50:46.943977 mlcvzoo_base-5.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 mlcvzoo_base-5.3.4/setup.py
+-rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 mlcvzoo_base-5.3.4/PKG-INFO
```

### Comparing `mlcvzoo_base-5.3.3/LICENSE` & `mlcvzoo_base-5.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/README.md` & `mlcvzoo_base-5.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/configuration.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_attributes.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_attributes.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_builder.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_class_mapper.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_class_mapper.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_parser.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_writer.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/bounding_box.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/bounding_box.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/box.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/box.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/class_identifier.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/class_identifier.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/classification.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/classification.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/dataset_info.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/dataset_info.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/ocr_perception.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/ocr_perception.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/segmentation.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/segmentation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/exceptions.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/interfaces.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/model.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/api/registry.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/api/registry.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/annotation_handler_config.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/annotation_handler_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/class_mapping_config.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/class_mapping_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/config_registry.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/config_registry.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/device_query.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/device_query.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/mlfow_config.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/mlfow_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/model_config.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/model_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/reduction_mapping_config.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/reduction_mapping_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/replacement_config.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/replacement_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/structs.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/structs.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/utils.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/visualization_config.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/visualization_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_handler.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_handler.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/utils.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/configuration.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/data_classes.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/metrics_computation.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/metrics_computation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/metrics_logging.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/metrics_logging.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/model_evaluation.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/structs.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/structs.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/utils.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/mlflow/mlflow_runner.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/mlflow/mlflow_runner.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/mlflow/utils.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/mlflow/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/models/model_registry.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/models/model_registry.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/models/read_from_file/configuration.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/models/read_from_file/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/models/read_from_file/model.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/models/read_from_file/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE` & `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/LICENSE.txt` & `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/perspective.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/perspective.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE` & `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/annotation_utils.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/common_utils.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/draw_utils.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/file_utils.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/gpu_util.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/gpu_util.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/implicit_path_replacements.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/implicit_path_replacements.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/versioning_utils.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/versioning_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/xml_utils.py` & `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.3/pyproject.toml` & `mlcvzoo_base-5.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mlcvzoo_base"
 description = "MLCVZoo Base Package"
-version = "5.3.3"
+version = "5.3.4"
 license = "Open Logistics Foundation License v1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `mlcvzoo_base-5.3.3/setup.py` & `mlcvzoo_base-5.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
  'tensorboardX>=2.5',
  'terminaltables>=3.1',
  'tqdm>=4.61',
  'yaml-config-builder>=8,<9']
 
 setup_kwargs = {
     'name': 'mlcvzoo-base',
-    'version': '5.3.3',
+    'version': '5.3.4',
     'description': 'MLCVZoo Base Package',
     'long_description': '# MLCVZoo Base\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_base** provides the base modules\nthat are defining the MLCVZoo API. Furthermore, it includes modules that allow to handle\nand process the data structures of the MLCVZoo, as well as providing modules for\nrunning evaluations / calculation of metrics.\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-base\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base',
```

### Comparing `mlcvzoo_base-5.3.3/PKG-INFO` & `mlcvzoo_base-5.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-base
-Version: 5.3.3
+Version: 5.3.4
 Summary: MLCVZoo Base Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base
 License: Open Logistics Foundation License v1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

