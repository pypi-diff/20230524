# Comparing `tmp/anomalib-0.5.0.tar.gz` & `tmp/anomalib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomalib-0.5.0.tar", last modified: Tue May  9 15:43:58 2023, max compression
+gzip compressed data, was "anomalib-0.5.1.tar", last modified: Wed May 24 14:43:06 2023, max compression
```

## Comparing `anomalib-0.5.0.tar` & `anomalib-0.5.1.tar`

### file list

```diff
@@ -1,279 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-09 15:43:45.000000 anomalib-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-05-09 15:43:45.000000 anomalib-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    24126 2023-05-09 15:43:58.925282 anomalib-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23624 2023-05-09 15:43:45.000000 anomalib-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-05-09 15:43:45.000000 anomalib-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/loggers.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/notebooks.txt
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/openvino.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 15:43:58.925282 anomalib-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3609 2023-05-09 15:43:45.000000 anomalib-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.901282 anomalib-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/src/anomalib/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/src/anomalib/config/
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13768 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/src/anomalib/data/
--rw-r--r--   0 runner    (1001) docker     (122)    11412 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12710 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/avenue.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/src/anomalib/data/base/
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8134 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/base/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     7327 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/base/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2540 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/base/depth.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/base/video.py
--rw-r--r--   0 runner    (1001) docker     (122)    12043 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/btech.py
--rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/folder.py
--rw-r--r--   0 runner    (1001) docker     (122)    17503 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/folder_3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/inference.py
--rw-r--r--   0 runner    (1001) docker     (122)    11831 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/mvtec.py
--rw-r--r--   0 runner    (1001) docker     (122)    12984 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/mvtec_3d.py
--rw-r--r--   0 runner    (1001) docker     (122)    14449 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/shanghaitech.py
--rw-r--r--   0 runner    (1001) docker     (122)     6941 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/task_type.py
--rw-r--r--   0 runner    (1001) docker     (122)    11770 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/ucsd_ped.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/data/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (122)     5077 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/boxes.py
--rw-r--r--   0 runner    (1001) docker     (122)    14332 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/download.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/data/utils/generators/
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6027 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/generators/perlin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8113 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/label.py
--rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/split.py
--rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     3651 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/video.py
--rw-r--r--   0 runner    (1001) docker     (122)     9615 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/visa.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/deploy/
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5674 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/export.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/deploy/inferencers/
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/inferencers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7184 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/inferencers/base_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7826 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/inferencers/openvino_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/inferencers/torch_inferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/
--rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/ai_vad/
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/ai_vad/clip/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7865 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/clip/clip.py
--rw-r--r--   0 runner    (1001) docker     (122)    17868 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/clip/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2922 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    11997 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/density.py
--rw-r--r--   0 runner    (1001) docker     (122)     9489 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/features.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/flow.py
--rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/regions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4331 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/cfa/
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    13213 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/cflow/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8299 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5230 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4179 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/components/
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/base/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/base/anomaly_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/base/dynamic_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/classification/
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/classification/kde_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/pca.py
--rw-r--r--   0 runner    (1001) docker     (122)     5337 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/random_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/feature_extractors/
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/feature_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/feature_extractors/timm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9158 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/feature_extractors/torchfx.py
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/feature_extractors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/filters/blur.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/flow/
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12649 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/flow/all_in_one_block.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/layers/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3143 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/layers/sspcab.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/sampling/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/sampling/k_center_greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/stats/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/stats/kde.py
--rw-r--r--   0 runner    (1001) docker     (122)     5603 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/stats/multi_variate_gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/csflow/
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4772 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    21233 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/dfkde/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfkde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfkde/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfkde/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfkde/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/dfm/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfm/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3024 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfm/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     6872 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfm/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/draem/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/draem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/draem/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/draem/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/draem/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    19097 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/draem/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/fastflow/
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     9915 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/ganomaly/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ganomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3070 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ganomaly/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     9292 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ganomaly/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ganomaly/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    12986 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ganomaly/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/padim/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/padim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4731 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/padim/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3049 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/padim/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4851 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/padim/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/padim/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/patchcore/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/patchcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/patchcore/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/patchcore/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/patchcore/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     7789 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/patchcore/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/reverse_distillation/
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/anomaly_map.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5832 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/bottleneck.py
--rw-r--r--   0 runner    (1001) docker     (122)    11795 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/de_resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5411 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/rkde/
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3233 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/region_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/models/stfpm/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4438 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2691 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/post_processing/
--rw-r--r--   0 runner    (1001) docker     (122)      683 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/post_processing/normalization/
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/normalization/cdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/normalization/min_max.py
--rw-r--r--   0 runner    (1001) docker     (122)     5797 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/post_process.py
--rw-r--r--   0 runner    (1001) docker     (122)    13077 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/pre_processing/pre_process.py
--rw-r--r--   0 runner    (1001) docker     (122)    15168 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/pre_processing/tiler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/pre_processing/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/pre_processing/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/pre_processing/transforms/custom.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)     8412 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6536 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/cdf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (122)     1760 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/export.py
--rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/metrics_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/min_max_normalization.py
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3607 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     7363 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/post_processing_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/tiler_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4066 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/cv/
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/cv/connected_components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/hpo/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/hpo/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/hpo/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4849 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/loggers/comet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     4201 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/loggers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     6914 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/anomaly_score_distribution.py
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/anomaly_score_threshold.py
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/aupr.py
--rw-r--r--   0 runner    (1001) docker     (122)     9080 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/aupro.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/auroc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/min_max.py
--rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/optimal_f1.py
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/pro.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/sweep/
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6456 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/sweep/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/sweep/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/sweep/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/sweep/helpers/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2325 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/sweep/helpers/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/src/anomalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    24126 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9182 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.741655 anomalib-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-24 14:42:52.000000 anomalib-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-05-24 14:42:52.000000 anomalib-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    24127 2023-05-24 14:43:06.741655 anomalib-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23625 2023-05-24 14:42:52.000000 anomalib-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-05-24 14:42:53.000000 anomalib-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.705659 anomalib-0.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/loggers.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/notebooks.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/openvino.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 14:43:06.741655 anomalib-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-05-24 14:42:53.000000 anomalib-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.701659 anomalib-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.705659 anomalib-0.5.1/src/anomalib/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.709658 anomalib-0.5.1/src/anomalib/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13768 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.709658 anomalib-0.5.1/src/anomalib/data/
+-rw-r--r--   0 runner    (1001) docker     (122)    11412 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12710 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/avenue.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/data/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8134 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/base/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7327 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/base/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2540 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/base/depth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/base/video.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12043 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/btech.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/folder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17503 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/folder_3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/inference.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11448 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/kolektor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11831 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/mvtec.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12984 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/mvtec_3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14449 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/shanghaitech.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6941 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11770 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/ucsd_ped.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5077 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/boxes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14453 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/download.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/data/utils/generators/
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6027 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/generators/perlin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8113 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/split.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3651 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/video.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9615 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/visa.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/deploy/
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5674 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/export.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/deploy/inferencers/
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/inferencers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7184 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/inferencers/base_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7903 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/inferencers/openvino_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/inferencers/torch_inferencer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/ai_vad/
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/ai_vad/clip/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7865 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/clip/clip.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17868 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/clip/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2922 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11997 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/density.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9489 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/flow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/regions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4331 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/cfa/
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13213 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/cflow/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     8299 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5230 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4179 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/components/
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/components/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/base/anomaly_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/base/dynamic_module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/components/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/classification/kde_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/pca.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5337 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/random_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/feature_extractors/
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/feature_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/feature_extractors/timm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9158 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/feature_extractors/torchfx.py
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/feature_extractors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/filters/blur.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/flow/
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12649 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/flow/all_in_one_block.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/layers/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3143 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/layers/sspcab.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/sampling/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/sampling/k_center_greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/stats/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/stats/kde.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5603 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/stats/multi_variate_gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/csflow/
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4772 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21233 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/dfkde/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfkde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfkde/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfkde/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfkde/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.725657 anomalib-0.5.1/src/anomalib/models/dfm/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfm/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3024 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfm/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6872 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfm/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.725657 anomalib-0.5.1/src/anomalib/models/draem/
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/draem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/draem/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/draem/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/draem/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19097 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/draem/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.725657 anomalib-0.5.1/src/anomalib/models/fastflow/
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9915 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.725657 anomalib-0.5.1/src/anomalib/models/ganomaly/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ganomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3070 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ganomaly/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     9292 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ganomaly/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ganomaly/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12986 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ganomaly/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.729656 anomalib-0.5.1/src/anomalib/models/padim/
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/padim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4731 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/padim/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3049 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/padim/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4851 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/padim/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/padim/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.729656 anomalib-0.5.1/src/anomalib/models/patchcore/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/patchcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/patchcore/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/patchcore/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/patchcore/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7789 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/patchcore/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.729656 anomalib-0.5.1/src/anomalib/models/reverse_distillation/
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/anomaly_map.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.729656 anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5832 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/bottleneck.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11795 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/de_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5411 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.729656 anomalib-0.5.1/src/anomalib/models/rkde/
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3233 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/region_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/models/stfpm/
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4438 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2691 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/post_processing/
+-rw-r--r--   0 runner    (1001) docker     (122)      683 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/post_processing/normalization/
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/normalization/cdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/normalization/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5797 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13077 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/pre_processing/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15168 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/pre_processing/tiler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/pre_processing/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/pre_processing/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/pre_processing/transforms/custom.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)     8412 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6536 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/cdf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1760 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/export.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/metrics_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/min_max_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7363 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/post_processing_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/tiler_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4066 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/cv/
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/cv/connected_components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/hpo/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/hpo/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/hpo/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4849 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/loggers/comet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4201 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.741655 anomalib-0.5.1/src/anomalib/utils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     6914 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/anomaly_score_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/anomaly_score_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/aupr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9080 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/aupro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/optimal_f1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/pro.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.741655 anomalib-0.5.1/src/anomalib/utils/sweep/
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6456 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/sweep/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.741655 anomalib-0.5.1/src/anomalib/utils/sweep/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/sweep/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/sweep/helpers/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2320 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/sweep/helpers/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.709658 anomalib-0.5.1/src/anomalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    24127 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9212 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/top_level.txt
```

### Comparing `anomalib-0.5.0/LICENSE` & `anomalib-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/PKG-INFO` & `anomalib-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomalib
-Version: 0.5.0
+Version: 0.5.1
 Summary: anomalib - Anomaly Detection Library
 Home-page: 
 Author: Intel OpenVINO
 Author-email: help@openvino.intel.com
 License: Copyright (c) Intel - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the "License")See LICENSE file for more details.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -75,15 +75,15 @@
 ```
 
 ## Local Install
 
 It is highly recommended to use virtual environment when installing anomalib. For instance, with [anaconda](https://www.anaconda.com/products/individual), `anomalib` could be installed as,
 
 ```bash
-yes | conda create -n anomalib_env python=3.8
+yes | conda create -n anomalib_env python=3.10
 conda activate anomalib_env
 git clone https://github.com/openvinotoolkit/anomalib.git
 cd anomalib
 pip install -e .
 ```
 
 # Training
```

### Comparing `anomalib-0.5.0/README.md` & `anomalib-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 ```
 
 ## Local Install
 
 It is highly recommended to use virtual environment when installing anomalib. For instance, with [anaconda](https://www.anaconda.com/products/individual), `anomalib` could be installed as,
 
 ```bash
-yes | conda create -n anomalib_env python=3.8
+yes | conda create -n anomalib_env python=3.10
 conda activate anomalib_env
 git clone https://github.com/openvinotoolkit/anomalib.git
 cd anomalib
 pip install -e .
 ```
 
 # Training
```

### Comparing `anomalib-0.5.0/pyproject.toml` & `anomalib-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 # MYPY CONFIGURATION.                                                         #
 [tool.mypy]
 ignore_missing_imports = true
 show_error_codes = true
 
 
 [[tool.mypy.overrides]]
-module = "torch.*"
+module = ["torch.*", "wandb.*"]
 follow_imports = "skip"
 follow_imports_for_stubs = true
 
 
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 # PYTEST CONFIGURATION                                                        #
 [tool.pytest.ini_options]
```

### Comparing `anomalib-0.5.0/setup.py` & `anomalib-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,10 +103,11 @@
     'Licensed under the Apache License, Version 2.0 (the "License")'
     "See LICENSE file for more details.",
     python_requires=">=3.7",
     package_dir={"": "src"},
     packages=find_packages(where="src", include=["anomalib", "anomalib.*"]),
     install_requires=INSTALL_REQUIRES,
     extras_require=EXTRAS_REQUIRE,
+    include_package_data=True,
     package_data={"": ["config.yaml"]},
     entry_points={"console_scripts": ["anomalib=anomalib.utils.cli.cli:main"]},
 )
```

### Comparing `anomalib-0.5.0/src/anomalib/config/config.py` & `anomalib-0.5.1/src/anomalib/config/config.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/__init__.py` & `anomalib-0.5.1/src/anomalib/data/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/avenue.py` & `anomalib-0.5.1/src/anomalib/data/avenue.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/base/datamodule.py` & `anomalib-0.5.1/src/anomalib/data/base/datamodule.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/base/dataset.py` & `anomalib-0.5.1/src/anomalib/data/base/dataset.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/base/depth.py` & `anomalib-0.5.1/src/anomalib/data/base/depth.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/base/video.py` & `anomalib-0.5.1/src/anomalib/data/base/video.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/btech.py` & `anomalib-0.5.1/src/anomalib/data/btech.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/folder.py` & `anomalib-0.5.1/src/anomalib/data/folder.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/folder_3d.py` & `anomalib-0.5.1/src/anomalib/data/folder_3d.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/inference.py` & `anomalib-0.5.1/src/anomalib/data/inference.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/mvtec.py` & `anomalib-0.5.1/src/anomalib/data/mvtec.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/mvtec_3d.py` & `anomalib-0.5.1/src/anomalib/data/mvtec_3d.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/shanghaitech.py` & `anomalib-0.5.1/src/anomalib/data/shanghaitech.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/synthetic.py` & `anomalib-0.5.1/src/anomalib/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/ucsd_ped.py` & `anomalib-0.5.1/src/anomalib/data/ucsd_ped.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/utils/__init__.py` & `anomalib-0.5.1/src/anomalib/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/utils/augmenter.py` & `anomalib-0.5.1/src/anomalib/data/utils/augmenter.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/utils/boxes.py` & `anomalib-0.5.1/src/anomalib/data/utils/boxes.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/utils/download.py` & `anomalib-0.5.1/src/anomalib/data/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 @dataclass
 class DownloadInfo:
     """Info needed to download a dataset from a url."""
 
     name: str
     url: str
     hash: str
+    filename: str | None = None
 
 
 class DownloadProgressBar(tqdm):
     """Create progress bar for urlretrieve. Subclasses `tqdm`.
 
     For information about the parameters in constructor, refer to `tqdm`'s documentation.
 
@@ -223,15 +224,19 @@
     Args:
         root (Path): Root directory where the dataset will be stored.
         info (DownloadInfo): Info needed to download the dataset.
     """
     root.mkdir(parents=True, exist_ok=True)
 
     # save the compressed file in the specified root directory, using the same file name as on the server
-    downloaded_file_path = root / info.url.split("/")[-1]
+    if info.filename:
+        downloaded_file_path = root / info.filename
+    else:
+        downloaded_file_path = root / info.url.split("/")[-1]
+
     if downloaded_file_path.exists():
         logger.info("Existing dataset archive found. Skipping download stage.")
     else:
         logger.info("Downloading the %s dataset.", info.name)
         with DownloadProgressBar(unit="B", unit_scale=True, miniters=1, desc=info.name) as progress_bar:
             urlretrieve(  # nosec - suppress bandit warning (urls are hardcoded)
                 url=f"{info.url}",
```

### Comparing `anomalib-0.5.0/src/anomalib/data/utils/generators/perlin.py` & `anomalib-0.5.1/src/anomalib/data/utils/generators/perlin.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/utils/image.py` & `anomalib-0.5.1/src/anomalib/data/utils/image.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/utils/path.py` & `anomalib-0.5.1/src/anomalib/data/utils/path.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/utils/split.py` & `anomalib-0.5.1/src/anomalib/data/utils/split.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/utils/transform.py` & `anomalib-0.5.1/src/anomalib/data/utils/transform.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/utils/video.py` & `anomalib-0.5.1/src/anomalib/data/utils/video.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/data/visa.py` & `anomalib-0.5.1/src/anomalib/data/visa.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/deploy/export.py` & `anomalib-0.5.1/src/anomalib/deploy/export.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/deploy/inferencers/base_inferencer.py` & `anomalib-0.5.1/src/anomalib/deploy/inferencers/base_inferencer.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/deploy/inferencers/openvino_inferencer.py` & `anomalib-0.5.1/src/anomalib/deploy/inferencers/openvino_inferencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,39 +15,38 @@
 from omegaconf import DictConfig
 
 from anomalib.data import TaskType
 
 from .base_inferencer import Inferencer
 
 if find_spec("openvino") is not None:
-    from openvino.inference_engine import (  # type: ignore  # pylint: disable=no-name-in-module
-        IECore,
-    )
+    from openvino.inference_engine import IECore  # type: ignore  # pylint: disable=no-name-in-module
 
 
 class OpenVINOInferencer(Inferencer):
     """OpenVINO implementation for the inference.
 
     Args:
         path (str | Path): Path to the openvino onnx, xml or bin file.
-        metadata_path (str | Path, optional): Path to metadata file. Defaults to None.
+        metadata (str | Path | dict, optional): Path to metadata file or a dict object defining the
+            metadata. Defaults to None.
         device (str | None, optional): Device to run the inference on. Defaults to "CPU".
         task (TaskType | None, optional): Task type. Defaults to None.
     """
 
     def __init__(
         self,
         path: str | Path | tuple[bytes, bytes],
-        metadata_path: str | Path | None = None,
+        metadata: str | Path | dict | None = None,
         device: str | None = "CPU",
         task: str | None = None,
     ) -> None:
         self.device = device
         self.input_blob, self.output_blob, self.network = self.load_model(path)
-        self.metadata = super()._load_metadata(metadata_path)
+        self.metadata = metadata if isinstance(metadata, dict) else super()._load_metadata(metadata)
         self.task = TaskType(task) if task else TaskType(self.metadata["task"])
 
     def load_model(self, path: str | Path | tuple[bytes, bytes]):
         """Load the OpenVINO model.
 
         Args:
             path (str | Path | tuple[bytes, bytes]): Path to the onnx or xml and bin files
```

### Comparing `anomalib-0.5.0/src/anomalib/deploy/inferencers/torch_inferencer.py` & `anomalib-0.5.1/src/anomalib/deploy/inferencers/torch_inferencer.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/__init__.py` & `anomalib-0.5.1/src/anomalib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ai_vad/clip/clip.py` & `anomalib-0.5.1/src/anomalib/models/ai_vad/clip/clip.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ai_vad/clip/model.py` & `anomalib-0.5.1/src/anomalib/models/ai_vad/clip/model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ai_vad/config.yaml` & `anomalib-0.5.1/src/anomalib/models/ai_vad/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ai_vad/density.py` & `anomalib-0.5.1/src/anomalib/models/ai_vad/density.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ai_vad/features.py` & `anomalib-0.5.1/src/anomalib/models/ai_vad/features.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ai_vad/flow.py` & `anomalib-0.5.1/src/anomalib/models/ai_vad/flow.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ai_vad/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/ai_vad/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ai_vad/regions.py` & `anomalib-0.5.1/src/anomalib/models/ai_vad/regions.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ai_vad/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/ai_vad/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/cfa/anomaly_map.py` & `anomalib-0.5.1/src/anomalib/models/cfa/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/cfa/config.yaml` & `anomalib-0.5.1/src/anomalib/models/cfa/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/cfa/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/cfa/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/cfa/loss.py` & `anomalib-0.5.1/src/anomalib/models/cfa/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/cfa/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/cfa/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/cflow/anomaly_map.py` & `anomalib-0.5.1/src/anomalib/models/cflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/cflow/config.yaml` & `anomalib-0.5.1/src/anomalib/models/cflow/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/cflow/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/cflow/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/cflow/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/cflow/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/cflow/utils.py` & `anomalib-0.5.1/src/anomalib/models/cflow/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/__init__.py` & `anomalib-0.5.1/src/anomalib/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/base/anomaly_module.py` & `anomalib-0.5.1/src/anomalib/models/components/base/anomaly_module.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/base/dynamic_module.py` & `anomalib-0.5.1/src/anomalib/models/components/base/dynamic_module.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/classification/kde_classifier.py` & `anomalib-0.5.1/src/anomalib/models/components/classification/kde_classifier.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/pca.py` & `anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/pca.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/random_projection.py` & `anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/random_projection.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/feature_extractors/timm.py` & `anomalib-0.5.1/src/anomalib/models/components/feature_extractors/timm.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/feature_extractors/torchfx.py` & `anomalib-0.5.1/src/anomalib/models/components/feature_extractors/torchfx.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/feature_extractors/utils.py` & `anomalib-0.5.1/src/anomalib/models/components/feature_extractors/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/filters/blur.py` & `anomalib-0.5.1/src/anomalib/models/components/filters/blur.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/flow/all_in_one_block.py` & `anomalib-0.5.1/src/anomalib/models/components/flow/all_in_one_block.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/layers/sspcab.py` & `anomalib-0.5.1/src/anomalib/models/components/layers/sspcab.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/sampling/k_center_greedy.py` & `anomalib-0.5.1/src/anomalib/models/components/sampling/k_center_greedy.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/stats/kde.py` & `anomalib-0.5.1/src/anomalib/models/components/stats/kde.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/components/stats/multi_variate_gaussian.py` & `anomalib-0.5.1/src/anomalib/models/components/stats/multi_variate_gaussian.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/csflow/anomaly_map.py` & `anomalib-0.5.1/src/anomalib/models/csflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/csflow/config.yaml` & `anomalib-0.5.1/src/anomalib/models/csflow/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/csflow/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/csflow/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/csflow/loss.py` & `anomalib-0.5.1/src/anomalib/models/csflow/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/csflow/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/csflow/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/dfkde/config.yaml` & `anomalib-0.5.1/src/anomalib/models/dfkde/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/dfkde/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/dfkde/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/dfkde/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/dfkde/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/dfm/config.yaml` & `anomalib-0.5.1/src/anomalib/models/dfm/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/dfm/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/dfm/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/dfm/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/dfm/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/draem/config.yaml` & `anomalib-0.5.1/src/anomalib/models/draem/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/draem/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/draem/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/draem/loss.py` & `anomalib-0.5.1/src/anomalib/models/draem/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/draem/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/draem/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/fastflow/anomaly_map.py` & `anomalib-0.5.1/src/anomalib/models/fastflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/fastflow/config.yaml` & `anomalib-0.5.1/src/anomalib/models/fastflow/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/fastflow/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/fastflow/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/fastflow/loss.py` & `anomalib-0.5.1/src/anomalib/models/fastflow/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/fastflow/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/fastflow/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ganomaly/config.yaml` & `anomalib-0.5.1/src/anomalib/models/ganomaly/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ganomaly/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/ganomaly/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ganomaly/loss.py` & `anomalib-0.5.1/src/anomalib/models/ganomaly/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/ganomaly/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/ganomaly/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/padim/anomaly_map.py` & `anomalib-0.5.1/src/anomalib/models/padim/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/padim/config.yaml` & `anomalib-0.5.1/src/anomalib/models/padim/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/padim/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/padim/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/padim/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/padim/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/patchcore/anomaly_map.py` & `anomalib-0.5.1/src/anomalib/models/patchcore/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/patchcore/config.yaml` & `anomalib-0.5.1/src/anomalib/models/patchcore/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/patchcore/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/patchcore/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/patchcore/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/patchcore/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/reverse_distillation/anomaly_map.py` & `anomalib-0.5.1/src/anomalib/models/reverse_distillation/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/__init__.py` & `anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/bottleneck.py` & `anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/bottleneck.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/de_resnet.py` & `anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/de_resnet.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/reverse_distillation/config.yaml` & `anomalib-0.5.1/src/anomalib/models/reverse_distillation/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/reverse_distillation/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/reverse_distillation/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/reverse_distillation/loss.py` & `anomalib-0.5.1/src/anomalib/models/reverse_distillation/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/reverse_distillation/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/reverse_distillation/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/rkde/config.yaml` & `anomalib-0.5.1/src/anomalib/models/rkde/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/rkde/feature_extractor.py` & `anomalib-0.5.1/src/anomalib/models/rkde/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/rkde/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/rkde/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/rkde/region_extractor.py` & `anomalib-0.5.1/src/anomalib/models/rkde/region_extractor.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/rkde/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/rkde/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/stfpm/anomaly_map.py` & `anomalib-0.5.1/src/anomalib/models/stfpm/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/stfpm/config.yaml` & `anomalib-0.5.1/src/anomalib/models/stfpm/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/stfpm/lightning_model.py` & `anomalib-0.5.1/src/anomalib/models/stfpm/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/stfpm/loss.py` & `anomalib-0.5.1/src/anomalib/models/stfpm/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/models/stfpm/torch_model.py` & `anomalib-0.5.1/src/anomalib/models/stfpm/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/post_processing/__init__.py` & `anomalib-0.5.1/src/anomalib/post_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/post_processing/normalization/cdf.py` & `anomalib-0.5.1/src/anomalib/post_processing/normalization/cdf.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/post_processing/normalization/min_max.py` & `anomalib-0.5.1/src/anomalib/post_processing/normalization/min_max.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/post_processing/post_process.py` & `anomalib-0.5.1/src/anomalib/post_processing/post_process.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/post_processing/visualizer.py` & `anomalib-0.5.1/src/anomalib/post_processing/visualizer.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/pre_processing/pre_process.py` & `anomalib-0.5.1/src/anomalib/pre_processing/pre_process.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/pre_processing/tiler.py` & `anomalib-0.5.1/src/anomalib/pre_processing/tiler.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/pre_processing/transforms/custom.py` & `anomalib-0.5.1/src/anomalib/pre_processing/transforms/custom.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/__init__.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/cdf_normalization.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/cdf_normalization.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/export.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/export.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/graph.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/graph.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/metrics_configuration.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/metrics_configuration.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/min_max_normalization.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/min_max_normalization.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/model_loader.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/model_loader.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/callback.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,18 @@
 
         # Get validate subset to initialize quantization,
         # because train subset does not contain anomalous images.
         init_loader = InitLoader(trainer.datamodule.val_dataloader())  # type: ignore
         config = register_default_init_args(self.config, init_loader)
 
         self.nncf_ctrl, pl_module.model = wrap_nncf_model(
-            model=pl_module.model, config=config, dataloader=trainer.datamodule.train_dataloader()  # type: ignore
+            model=pl_module.model,
+            config=config,
+            dataloader=trainer.datamodule.train_dataloader(),  # type: ignore
+            init_state_dict=None,  # type: ignore
         )
 
     def on_train_batch_start(
         self, trainer: pl.Trainer, pl_module: pl.LightningModule, batch: Any, batch_idx: int, unused: int = 0
     ) -> None:
         """Call when the train batch begins.
```

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/utils.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/post_processing_configuration.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/post_processing_configuration.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/tiler_configuration.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/tiler_configuration.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/timer.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/timer.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_base.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_base.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_image.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_image.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_metric.py` & `anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_metric.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/cli/cli.py` & `anomalib-0.5.1/src/anomalib/utils/cli/cli.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/cv/connected_components.py` & `anomalib-0.5.1/src/anomalib/utils/cv/connected_components.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/hpo/config.py` & `anomalib-0.5.1/src/anomalib/utils/hpo/config.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/hpo/runners.py` & `anomalib-0.5.1/src/anomalib/utils/hpo/runners.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/loggers/__init__.py` & `anomalib-0.5.1/src/anomalib/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/loggers/base.py` & `anomalib-0.5.1/src/anomalib/utils/loggers/base.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/loggers/comet.py` & `anomalib-0.5.1/src/anomalib/utils/loggers/comet.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/loggers/tensorboard.py` & `anomalib-0.5.1/src/anomalib/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/loggers/wandb.py` & `anomalib-0.5.1/src/anomalib/utils/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/metrics/__init__.py` & `anomalib-0.5.1/src/anomalib/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/metrics/anomaly_score_distribution.py` & `anomalib-0.5.1/src/anomalib/utils/metrics/anomaly_score_distribution.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/metrics/anomaly_score_threshold.py` & `anomalib-0.5.1/src/anomalib/utils/metrics/anomaly_score_threshold.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/metrics/aupr.py` & `anomalib-0.5.1/src/anomalib/utils/metrics/aupr.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/metrics/aupro.py` & `anomalib-0.5.1/src/anomalib/utils/metrics/aupro.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/metrics/auroc.py` & `anomalib-0.5.1/src/anomalib/utils/metrics/auroc.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/metrics/collection.py` & `anomalib-0.5.1/src/anomalib/utils/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/metrics/min_max.py` & `anomalib-0.5.1/src/anomalib/utils/metrics/min_max.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/metrics/optimal_f1.py` & `anomalib-0.5.1/src/anomalib/utils/metrics/optimal_f1.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/metrics/plotting_utils.py` & `anomalib-0.5.1/src/anomalib/utils/metrics/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/metrics/pro.py` & `anomalib-0.5.1/src/anomalib/utils/metrics/pro.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/sweep/config.py` & `anomalib-0.5.1/src/anomalib/utils/sweep/config.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/sweep/helpers/callbacks.py` & `anomalib-0.5.1/src/anomalib/utils/sweep/helpers/callbacks.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.0/src/anomalib/utils/sweep/helpers/inference.py` & `anomalib-0.5.1/src/anomalib/utils/sweep/helpers/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     Returns:
         float: Inference throughput
     """
     model_path = Path(model_path)
 
     inferencer = OpenVINOInferencer(
         path=model_path / "weights" / "openvino" / "model.xml",
-        metadata_path=model_path / "weights" / "openvino" / "metadata.json",
+        metadata=model_path / "weights" / "openvino" / "metadata.json",
     )
     start_time = time.time()
     for image_path in test_dataset.samples.image_path:
         inferencer.predict(image_path)
 
     # get throughput
     inference_time = time.time() - start_time
```

### Comparing `anomalib-0.5.0/src/anomalib.egg-info/PKG-INFO` & `anomalib-0.5.1/src/anomalib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomalib
-Version: 0.5.0
+Version: 0.5.1
 Summary: anomalib - Anomaly Detection Library
 Home-page: 
 Author: Intel OpenVINO
 Author-email: help@openvino.intel.com
 License: Copyright (c) Intel - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the "License")See LICENSE file for more details.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -75,15 +75,15 @@
 ```
 
 ## Local Install
 
 It is highly recommended to use virtual environment when installing anomalib. For instance, with [anaconda](https://www.anaconda.com/products/individual), `anomalib` could be installed as,
 
 ```bash
-yes | conda create -n anomalib_env python=3.8
+yes | conda create -n anomalib_env python=3.10
 conda activate anomalib_env
 git clone https://github.com/openvinotoolkit/anomalib.git
 cd anomalib
 pip install -e .
 ```
 
 # Training
```

### Comparing `anomalib-0.5.0/src/anomalib.egg-info/SOURCES.txt` & `anomalib-0.5.1/src/anomalib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 src/anomalib/config/config.py
 src/anomalib/data/__init__.py
 src/anomalib/data/avenue.py
 src/anomalib/data/btech.py
 src/anomalib/data/folder.py
 src/anomalib/data/folder_3d.py
 src/anomalib/data/inference.py
+src/anomalib/data/kolektor.py
 src/anomalib/data/mvtec.py
 src/anomalib/data/mvtec_3d.py
 src/anomalib/data/shanghaitech.py
 src/anomalib/data/synthetic.py
 src/anomalib/data/task_type.py
 src/anomalib/data/ucsd_ped.py
 src/anomalib/data/visa.py
```

### Comparing `anomalib-0.5.0/src/anomalib.egg-info/requires.txt` & `anomalib-0.5.1/src/anomalib.egg-info/requires.txt`

 * *Files identical despite different names*

