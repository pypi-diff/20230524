# Comparing `tmp/shaperone-0.41.4.tar.gz` & `tmp/shaperone-0.41.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaperone-0.41.4.tar", max compression
+gzip compressed data, was "shaperone-0.41.5.tar", last modified: Wed May 24 16:00:48 2023, max compression
```

## Comparing `shaperone-0.41.4.tar` & `shaperone-0.41.5.tar`

### file list

```diff
@@ -1,104 +1,123 @@
--rw-r--r--   0        0        0     1081 2023-05-19 12:16:20.410505 shaperone-0.41.4/LICENSE
--rw-r--r--   0        0        0      631 2023-05-23 11:51:38.933952 shaperone-0.41.4/README.md
--rw-r--r--   0        0        0      977 2023-05-23 11:53:23.639536 shaperone-0.41.4/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-19 12:16:22.675245 shaperone-0.41.4/shaperone/.pylintrc2
--rw-r--r--   0        0        0     3259 2023-05-23 11:53:16.428283 shaperone-0.41.4/shaperone/__init__.py
--rw-r--r--   0        0        0    32344 2023-05-23 11:20:06.489661 shaperone-0.41.4/shaperone/_explanation.py
--rw-r--r--   0        0        0     8707 2023-05-23 11:20:06.404107 shaperone-0.41.4/shaperone/_serializable.py
--rw-r--r--   0        0        0       27 2023-05-19 12:16:22.676670 shaperone-0.41.4/shaperone/actions/__init__.py
--rw-r--r--   0        0        0      210 2023-05-19 12:16:22.676909 shaperone-0.41.4/shaperone/actions/_action.py
--rw-r--r--   0        0        0     3636 2023-05-19 12:16:22.677174 shaperone-0.41.4/shaperone/actions/_optimizer.py
--rw-r--r--   0        0        0      214 2023-05-19 12:16:22.677428 shaperone-0.41.4/shaperone/benchmark/__init__.py
--rw-r--r--   0        0        0      289 2023-05-19 12:16:22.677588 shaperone-0.41.4/shaperone/benchmark/_compute.py
--rw-r--r--   0        0        0     8099 2023-05-23 11:20:06.198786 shaperone-0.41.4/shaperone/benchmark/_explanation_error.py
--rw-r--r--   0        0        0     1074 2023-05-19 12:16:22.678044 shaperone-0.41.4/shaperone/benchmark/_result.py
--rw-r--r--   0        0        0    13399 2023-05-23 11:20:06.379830 shaperone-0.41.4/shaperone/benchmark/_sequential.py
--rw-r--r--   0        0        0    14182 2023-05-23 11:20:06.525273 shaperone-0.41.4/shaperone/benchmark/experiments.py
--rw-r--r--   0        0        0     4243 2023-05-23 11:20:06.147074 shaperone-0.41.4/shaperone/benchmark/framework.py
--rw-r--r--   0        0        0    18601 2023-05-19 12:16:22.678958 shaperone-0.41.4/shaperone/benchmark/measures.py
--rw-r--r--   0        0        0     4287 2023-05-19 12:16:22.679149 shaperone-0.41.4/shaperone/benchmark/methods.py
--rw-r--r--   0        0        0    31376 2023-05-19 12:30:35.021854 shaperone-0.41.4/shaperone/benchmark/metrics.py
--rw-r--r--   0        0        0     6513 2023-05-19 12:16:22.679646 shaperone-0.41.4/shaperone/benchmark/models.py
--rw-r--r--   0        0        0    23812 2023-05-23 11:20:06.545890 shaperone-0.41.4/shaperone/benchmark/plots.py
--rw-r--r--   0        0        0    25873 2023-05-19 12:16:22.680237 shaperone-0.41.4/shaperone/cext/_cext.cc
--rw-r--r--   0        0        0     8085 2023-05-19 12:16:22.680403 shaperone-0.41.4/shaperone/cext/_cext_gpu.cc
--rw-r--r--   0        0        0    14595 2023-05-19 12:16:22.680578 shaperone-0.41.4/shaperone/cext/_cext_gpu.cu
--rw-r--r--   0        0        0    62762 2023-05-19 12:16:22.680977 shaperone-0.41.4/shaperone/cext/gpu_treeshap.h
--rw-r--r--   0        0        0    58256 2023-05-19 12:16:22.681320 shaperone-0.41.4/shaperone/cext/tree_shap.h
--rw-r--r--   0        0        0     9612 2023-05-23 11:20:06.172429 shaperone-0.41.4/shaperone/datasets.py
--rw-r--r--   0        0        0      268 2023-05-19 12:16:22.681691 shaperone-0.41.4/shaperone/explainers/__init__.py
--rw-r--r--   0        0        0     8939 2023-05-23 11:20:06.650366 shaperone-0.41.4/shaperone/explainers/_additive.py
--rw-r--r--   0        0        0     6730 2023-05-23 11:20:06.431032 shaperone-0.41.4/shaperone/explainers/_deep/__init__.py
--rw-r--r--   0        0        0    16170 2023-05-19 12:16:22.682286 shaperone-0.41.4/shaperone/explainers/_deep/deep_pytorch.py
--rw-r--r--   0        0        0    35006 2023-05-19 12:27:39.295775 shaperone-0.41.4/shaperone/explainers/_deep/deep_tf.py
--rw-r--r--   0        0        0    16264 2023-05-23 11:20:06.531908 shaperone-0.41.4/shaperone/explainers/_exact.py
--rw-r--r--   0        0        0    23234 2023-05-23 11:20:06.209921 shaperone-0.41.4/shaperone/explainers/_explainer.py
--rw-r--r--   0        0        0     9330 2023-05-19 12:16:22.683710 shaperone-0.41.4/shaperone/explainers/_gpu_tree.py
--rw-r--r--   0        0        0    27238 2023-05-23 11:20:06.613415 shaperone-0.41.4/shaperone/explainers/_gradient.py
--rw-r--r--   0        0        0    31017 2023-05-23 11:20:06.387085 shaperone-0.41.4/shaperone/explainers/_kernel.py
--rw-r--r--   0        0        0    19121 2023-05-23 11:20:06.550266 shaperone-0.41.4/shaperone/explainers/_linear.py
--rw-r--r--   0        0        0    31746 2023-05-23 11:20:06.371080 shaperone-0.41.4/shaperone/explainers/_partition.py
--rw-r--r--   0        0        0    10941 2023-05-23 11:20:06.440928 shaperone-0.41.4/shaperone/explainers/_permutation.py
--rw-r--r--   0        0        0     9255 2023-05-23 11:20:06.408027 shaperone-0.41.4/shaperone/explainers/_sampling.py
--rw-r--r--   0        0        0    93670 2023-05-23 11:20:06.346964 shaperone-0.41.4/shaperone/explainers/_tree.py
--rw-r--r--   0        0        0     5009 2023-05-23 11:20:06.218057 shaperone-0.41.4/shaperone/explainers/mimic.py
--rw-r--r--   0        0        0      163 2023-05-19 12:16:22.686920 shaperone-0.41.4/shaperone/explainers/other/__init__.py
--rw-r--r--   0        0        0      512 2023-05-19 12:16:22.687102 shaperone-0.41.4/shaperone/explainers/other/_coefficent.py
--rw-r--r--   0        0        0     2528 2023-05-23 11:20:06.229050 shaperone-0.41.4/shaperone/explainers/other/_lime.py
--rw-r--r--   0        0        0    11413 2023-05-19 12:16:22.687538 shaperone-0.41.4/shaperone/explainers/other/_maple.py
--rw-r--r--   0        0        0     3344 2023-05-23 11:20:06.541222 shaperone-0.41.4/shaperone/explainers/other/_random.py
--rw-r--r--   0        0        0     1283 2023-05-19 12:16:22.687898 shaperone-0.41.4/shaperone/explainers/other/_treegain.py
--rw-r--r--   0        0        0    20310 2023-05-23 11:20:06.591261 shaperone-0.41.4/shaperone/explainers/pytree.py
--rw-r--r--   0        0        0     2774 2023-05-19 12:16:22.688361 shaperone-0.41.4/shaperone/explainers/tf_utils.py
--rw-r--r--   0        0        0      443 2023-05-19 12:16:22.688609 shaperone-0.41.4/shaperone/links.py
--rw-r--r--   0        0        0      283 2023-05-19 12:16:22.688804 shaperone-0.41.4/shaperone/maskers/__init__.py
--rw-r--r--   0        0        0     5213 2023-05-19 12:16:22.688969 shaperone-0.41.4/shaperone/maskers/_composite.py
--rw-r--r--   0        0        0     1008 2023-05-19 12:16:22.689086 shaperone-0.41.4/shaperone/maskers/_fixed.py
--rw-r--r--   0        0        0     2416 2023-05-23 11:20:06.310200 shaperone-0.41.4/shaperone/maskers/_fixed_composite.py
--rw-r--r--   0        0        0     9543 2023-05-23 11:20:06.506190 shaperone-0.41.4/shaperone/maskers/_image.py
--rw-r--r--   0        0        0      753 2023-05-19 12:27:39.449782 shaperone-0.41.4/shaperone/maskers/_masker.py
--rw-r--r--   0        0        0     2692 2023-05-23 11:20:06.419680 shaperone-0.41.4/shaperone/maskers/_output_composite.py
--rw-r--r--   0        0        0    14131 2023-05-23 11:20:06.204183 shaperone-0.41.4/shaperone/maskers/_tabular.py
--rw-r--r--   0        0        0    21556 2023-05-23 11:20:06.400876 shaperone-0.41.4/shaperone/maskers/_text.py
--rw-r--r--   0        0        0      202 2023-05-19 12:16:22.690658 shaperone-0.41.4/shaperone/models/__init__.py
--rw-r--r--   0        0        0     1498 2023-05-23 11:20:06.485053 shaperone-0.41.4/shaperone/models/_model.py
--rw-r--r--   0        0        0    18717 2023-05-23 11:20:06.423374 shaperone-0.41.4/shaperone/models/_teacher_forcing.py
--rw-r--r--   0        0        0     9978 2023-05-23 11:20:06.537864 shaperone-0.41.4/shaperone/models/_text_generation.py
--rw-r--r--   0        0        0    10116 2023-05-23 11:20:06.266358 shaperone-0.41.4/shaperone/models/_topk_lm.py
--rw-r--r--   0        0        0     1623 2023-05-23 11:20:06.163448 shaperone-0.41.4/shaperone/models/_transformers_pipeline.py
--rw-r--r--   0        0        0      685 2023-05-19 12:16:22.692042 shaperone-0.41.4/shaperone/plots/__init__.py
--rw-r--r--   0        0        0    17309 2023-05-23 11:20:06.167759 shaperone-0.41.4/shaperone/plots/_bar.py
--rw-r--r--   0        0        0    41107 2023-05-23 11:20:06.582131 shaperone-0.41.4/shaperone/plots/_beeswarm.py
--rw-r--r--   0        0        0     9455 2023-05-19 12:16:22.693063 shaperone-0.41.4/shaperone/plots/_benchmark.py
--rw-r--r--   0        0        0    26022 2023-05-23 11:20:06.461304 shaperone-0.41.4/shaperone/plots/_decision.py
--rw-r--r--   0        0        0     2813 2023-05-19 12:16:22.693473 shaperone-0.41.4/shaperone/plots/_embedding.py
--rw-r--r--   0        0        0    19463 2023-05-23 11:20:06.137439 shaperone-0.41.4/shaperone/plots/_force.py
--rw-r--r--   0        0        0    14797 2023-05-23 11:20:06.496409 shaperone-0.41.4/shaperone/plots/_force_matplotlib.py
--rw-r--r--   0        0        0     3121 2023-05-19 12:27:39.370797 shaperone-0.41.4/shaperone/plots/_group_difference.py
--rw-r--r--   0        0        0     6502 2023-05-23 11:20:06.244976 shaperone-0.41.4/shaperone/plots/_heatmap.py
--rw-r--r--   0        0        0    25135 2023-05-23 11:20:06.364945 shaperone-0.41.4/shaperone/plots/_image.py
--rw-r--r--   0        0        0      608 2023-05-19 12:16:22.694518 shaperone-0.41.4/shaperone/plots/_labels.py
--rw-r--r--   0        0        0     2825 2023-05-19 12:16:22.694625 shaperone-0.41.4/shaperone/plots/_monitoring.py
--rw-r--r--   0        0        0     9521 2023-05-19 12:16:22.694768 shaperone-0.41.4/shaperone/plots/_partial_dependence.py
--rw-r--r--   0        0        0    33020 2023-05-23 11:20:06.153574 shaperone-0.41.4/shaperone/plots/_scatter.py
--rw-r--r--   0        0        0    59166 2023-05-23 11:20:06.501966 shaperone-0.41.4/shaperone/plots/_text.py
--rw-r--r--   0        0        0     7616 2023-05-19 12:16:22.695662 shaperone-0.41.4/shaperone/plots/_utils.py
--rw-r--r--   0        0        0    23943 2023-05-23 11:20:06.326960 shaperone-0.41.4/shaperone/plots/_violin.py
--rw-r--r--   0        0        0    26592 2023-05-23 11:20:06.468981 shaperone-0.41.4/shaperone/plots/_waterfall.py
--rw-r--r--   0        0        0      262 2023-05-19 12:16:22.696525 shaperone-0.41.4/shaperone/plots/colors/__init__.py
--rw-r--r--   0        0        0    36754 2023-05-19 12:27:39.309034 shaperone-0.41.4/shaperone/plots/colors/_colorconv.py
--rw-r--r--   0        0        0     5096 2023-05-19 12:16:22.696928 shaperone-0.41.4/shaperone/plots/colors/_colors.py
--rw-r--r--   0        0        0   370829 2023-05-19 12:16:22.704487 shaperone-0.41.4/shaperone/plots/resources/bundle.js
--rw-r--r--   0        0        0      570 2023-05-19 12:16:22.704694 shaperone-0.41.4/shaperone/plots/resources/logoSmallGray.png
--rw-r--r--   0        0        0       31 2023-05-19 12:16:22.704846 shaperone-0.41.4/shaperone/setup.cfg
--rw-r--r--   0        0        0      449 2023-05-19 12:16:22.705057 shaperone-0.41.4/shaperone/utils/__init__.py
--rw-r--r--   0        0        0     8513 2023-05-23 11:20:06.176709 shaperone-0.41.4/shaperone/utils/_clustering.py
--rw-r--r--   0        0        0      591 2023-05-19 12:16:22.705349 shaperone-0.41.4/shaperone/utils/_exceptions.py
--rw-r--r--   0        0        0    10645 2023-05-23 11:20:06.186826 shaperone-0.41.4/shaperone/utils/_general.py
--rw-r--r--   0        0        0     2576 2023-05-19 12:16:22.705705 shaperone-0.41.4/shaperone/utils/_keras.py
--rw-r--r--   0        0        0     7329 2023-05-19 12:16:22.705884 shaperone-0.41.4/shaperone/utils/_legacy.py
--rw-r--r--   0        0        0    21361 2023-05-19 12:32:42.478522 shaperone-0.41.4/shaperone/utils/_masked_model.py
--rw-r--r--   0        0        0     1227 2023-05-19 12:16:22.706555 shaperone-0.41.4/shaperone/utils/_show_progress.py
--rw-r--r--   0        0        0     5562 2023-05-23 11:20:06.428023 shaperone-0.41.4/shaperone/utils/image.py
--rw-r--r--   0        0        0     6494 2023-05-19 12:16:22.706900 shaperone-0.41.4/shaperone/utils/transformers.py
--rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 shaperone-0.41.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.730425 shaperone-0.41.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-24 16:00:33.000000 shaperone-0.41.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-24 16:00:33.000000 shaperone-0.41.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-24 16:00:48.730425 shaperone-0.41.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-05-24 16:00:33.000000 shaperone-0.41.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-24 16:00:34.000000 shaperone-0.41.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 16:00:48.730425 shaperone-0.41.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11869 2023-05-24 16:00:34.000000 shaperone-0.41.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.694424 shaperone-0.41.5/shaperone/
+-rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32344 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8707 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/_serializable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.698425 shaperone-0.41.5/shaperone/actions/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/actions/_action.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3636 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/actions/_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.702425 shaperone-0.41.5/shaperone/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/_compute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8099 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/_explanation_error.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13399 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14182 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4243 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/framework.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18601 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/measures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31376 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6513 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23812 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.706425 shaperone-0.41.5/shaperone/cext/
+-rw-r--r--   0 runner    (1001) docker     (122)    25873 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/cext/_cext.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    58256 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/cext/tree_shap.h
+-rw-r--r--   0 runner    (1001) docker     (122)     9316 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.710425 shaperone-0.41.5/shaperone/explainers/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8939 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_additive.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.710425 shaperone-0.41.5/shaperone/explainers/_deep/
+-rw-r--r--   0 runner    (1001) docker     (122)     6730 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16170 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_deep/deep_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35006 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_deep/deep_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16264 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_exact.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23234 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_gpu_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27238 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31017 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19121 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31746 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_partition.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9255 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (122)    93670 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/mimic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.714425 shaperone-0.41.5/shaperone/explainers/other/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/_coefficent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/_lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11413 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/_maple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3344 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/_random.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/_treegain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20310 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/pytree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/links.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.718425 shaperone-0.41.5/shaperone/maskers/
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5213 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_fixed_composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9543 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_masker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_output_composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21556 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_text.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.718425 shaperone-0.41.5/shaperone/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18717 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/_teacher_forcing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9978 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/_text_generation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10116 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/_topk_lm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/_transformers_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.726425 shaperone-0.41.5/shaperone/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17309 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_bar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41107 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_beeswarm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9455 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26022 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_decision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19463 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_force.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14797 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_force_matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_group_difference.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6502 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25135 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9521 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_partial_dependence.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33020 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    59166 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7616 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23943 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_violin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26592 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_waterfall.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.726425 shaperone-0.41.5/shaperone/plots/colors/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36754 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/colors/_colorconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5096 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/colors/_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.726425 shaperone-0.41.5/shaperone/plots/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)   370829 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/resources/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/resources/logoSmallGray.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.730425 shaperone-0.41.5/shaperone/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      449 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8513 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10645 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_general.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2576 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7329 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21361 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_masked_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_show_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5416 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6494 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.698425 shaperone-0.41.5/shaperone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/top_level.txt
```

### Comparing `shaperone-0.41.4/LICENSE` & `shaperone-0.41.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/README.md` & `shaperone-0.41.5/README.md`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/__init__.py` & `shaperone-0.41.5/shaperone/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # flake8: noqa
 
 import warnings
 import sys
 
-__version__ = '0.41.4'
+__version__ = '0.41.5'
 
 # check python version
 if (sys.version_info < (3, 0)):
     warnings.warn("As of version 0.29.0 shaperone only supports Python 3 (not 2)!")
 
 from ._explanation import Explanation, Cohorts
```

### Comparing `shaperone-0.41.4/shaperone/_explanation.py` & `shaperone-0.41.5/shaperone/_explanation.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/_serializable.py` & `shaperone-0.41.5/shaperone/_serializable.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/actions/_optimizer.py` & `shaperone-0.41.5/shaperone/actions/_optimizer.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/benchmark/_explanation_error.py` & `shaperone-0.41.5/shaperone/benchmark/_explanation_error.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/benchmark/_result.py` & `shaperone-0.41.5/shaperone/benchmark/_result.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/benchmark/_sequential.py` & `shaperone-0.41.5/shaperone/benchmark/_sequential.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/benchmark/experiments.py` & `shaperone-0.41.5/shaperone/benchmark/experiments.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/benchmark/framework.py` & `shaperone-0.41.5/shaperone/benchmark/framework.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/benchmark/measures.py` & `shaperone-0.41.5/shaperone/benchmark/measures.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/benchmark/methods.py` & `shaperone-0.41.5/shaperone/benchmark/methods.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/benchmark/metrics.py` & `shaperone-0.41.5/shaperone/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/benchmark/models.py` & `shaperone-0.41.5/shaperone/benchmark/models.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/benchmark/plots.py` & `shaperone-0.41.5/shaperone/benchmark/plots.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/cext/_cext.cc` & `shaperone-0.41.5/shaperone/cext/_cext.cc`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/cext/tree_shap.h` & `shaperone-0.41.5/shaperone/cext/tree_shap.h`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/datasets.py` & `shaperone-0.41.5/shaperone/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,14 @@
     """
 
     prefix = github_data_url + "imagenet50_"
     X = np.load(cache(prefix + "%sx%s.npy" % (resolution, resolution))).astype(np.float32)
     y = np.loadtxt(cache(prefix + "labels.csv"))
     return X, y
 
-def boston(display=False): # pylint: disable=unused-argument
-    """ Return the boston housing data in a nice package. """
-
-    d = sklearn.datasets.load_boston()
-    df = pd.DataFrame(data=d.data, columns=d.feature_names) # pylint: disable=E1101
-    return df, d.target # pylint: disable=E1101
-
 
 def california(display=False, n_points=None): # pylint: disable=unused-argument
     """ Return the california housing data in a nice package. """
 
     d = sklearn.datasets.fetch_california_housing()
     df = pd.DataFrame(data=d.data, columns=d.feature_names) # pylint: disable=E1101
     target = d.target
```

### Comparing `shaperone-0.41.4/shaperone/explainers/_additive.py` & `shaperone-0.41.5/shaperone/explainers/_additive.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_deep/__init__.py` & `shaperone-0.41.5/shaperone/explainers/_deep/__init__.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_deep/deep_pytorch.py` & `shaperone-0.41.5/shaperone/explainers/_deep/deep_pytorch.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_deep/deep_tf.py` & `shaperone-0.41.5/shaperone/explainers/_deep/deep_tf.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_exact.py` & `shaperone-0.41.5/shaperone/explainers/_exact.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_explainer.py` & `shaperone-0.41.5/shaperone/explainers/_explainer.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_gpu_tree.py` & `shaperone-0.41.5/shaperone/explainers/_gpu_tree.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_gradient.py` & `shaperone-0.41.5/shaperone/explainers/_gradient.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_kernel.py` & `shaperone-0.41.5/shaperone/explainers/_kernel.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_linear.py` & `shaperone-0.41.5/shaperone/explainers/_linear.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_partition.py` & `shaperone-0.41.5/shaperone/explainers/_partition.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_permutation.py` & `shaperone-0.41.5/shaperone/explainers/_permutation.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_sampling.py` & `shaperone-0.41.5/shaperone/explainers/_sampling.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/_tree.py` & `shaperone-0.41.5/shaperone/explainers/_tree.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/mimic.py` & `shaperone-0.41.5/shaperone/explainers/mimic.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/other/_coefficent.py` & `shaperone-0.41.5/shaperone/explainers/other/_coefficent.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/other/_lime.py` & `shaperone-0.41.5/shaperone/explainers/other/_lime.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/other/_maple.py` & `shaperone-0.41.5/shaperone/explainers/other/_maple.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/other/_random.py` & `shaperone-0.41.5/shaperone/explainers/other/_random.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/other/_treegain.py` & `shaperone-0.41.5/shaperone/explainers/other/_treegain.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/pytree.py` & `shaperone-0.41.5/shaperone/explainers/pytree.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/explainers/tf_utils.py` & `shaperone-0.41.5/shaperone/explainers/tf_utils.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/maskers/_composite.py` & `shaperone-0.41.5/shaperone/maskers/_composite.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/maskers/_fixed.py` & `shaperone-0.41.5/shaperone/maskers/_fixed.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/maskers/_fixed_composite.py` & `shaperone-0.41.5/shaperone/maskers/_fixed_composite.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/maskers/_image.py` & `shaperone-0.41.5/shaperone/maskers/_image.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/maskers/_masker.py` & `shaperone-0.41.5/shaperone/maskers/_masker.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/maskers/_output_composite.py` & `shaperone-0.41.5/shaperone/maskers/_output_composite.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/maskers/_tabular.py` & `shaperone-0.41.5/shaperone/maskers/_tabular.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/maskers/_text.py` & `shaperone-0.41.5/shaperone/maskers/_text.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/models/_model.py` & `shaperone-0.41.5/shaperone/models/_model.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/models/_teacher_forcing.py` & `shaperone-0.41.5/shaperone/models/_teacher_forcing.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/models/_text_generation.py` & `shaperone-0.41.5/shaperone/models/_text_generation.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/models/_topk_lm.py` & `shaperone-0.41.5/shaperone/models/_topk_lm.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/models/_transformers_pipeline.py` & `shaperone-0.41.5/shaperone/models/_transformers_pipeline.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/__init__.py` & `shaperone-0.41.5/shaperone/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_bar.py` & `shaperone-0.41.5/shaperone/plots/_bar.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_beeswarm.py` & `shaperone-0.41.5/shaperone/plots/_beeswarm.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_benchmark.py` & `shaperone-0.41.5/shaperone/plots/_benchmark.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_decision.py` & `shaperone-0.41.5/shaperone/plots/_decision.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_embedding.py` & `shaperone-0.41.5/shaperone/plots/_embedding.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_force.py` & `shaperone-0.41.5/shaperone/plots/_force.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_force_matplotlib.py` & `shaperone-0.41.5/shaperone/plots/_force_matplotlib.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_group_difference.py` & `shaperone-0.41.5/shaperone/plots/_group_difference.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_heatmap.py` & `shaperone-0.41.5/shaperone/plots/_heatmap.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_image.py` & `shaperone-0.41.5/shaperone/plots/_image.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_labels.py` & `shaperone-0.41.5/shaperone/plots/_labels.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_monitoring.py` & `shaperone-0.41.5/shaperone/plots/_monitoring.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_partial_dependence.py` & `shaperone-0.41.5/shaperone/plots/_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_scatter.py` & `shaperone-0.41.5/shaperone/plots/_scatter.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_text.py` & `shaperone-0.41.5/shaperone/plots/_text.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_utils.py` & `shaperone-0.41.5/shaperone/plots/_utils.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_violin.py` & `shaperone-0.41.5/shaperone/plots/_violin.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/_waterfall.py` & `shaperone-0.41.5/shaperone/plots/_waterfall.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/colors/_colorconv.py` & `shaperone-0.41.5/shaperone/plots/colors/_colorconv.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/colors/_colors.py` & `shaperone-0.41.5/shaperone/plots/colors/_colors.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/resources/bundle.js` & `shaperone-0.41.5/shaperone/plots/resources/bundle.js`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/plots/resources/logoSmallGray.png` & `shaperone-0.41.5/shaperone/plots/resources/logoSmallGray.png`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/utils/_clustering.py` & `shaperone-0.41.5/shaperone/utils/_clustering.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/utils/_exceptions.py` & `shaperone-0.41.5/shaperone/utils/_exceptions.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/utils/_general.py` & `shaperone-0.41.5/shaperone/utils/_general.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/utils/_keras.py` & `shaperone-0.41.5/shaperone/utils/_keras.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/utils/_legacy.py` & `shaperone-0.41.5/shaperone/utils/_legacy.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/utils/_masked_model.py` & `shaperone-0.41.5/shaperone/utils/_masked_model.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/utils/_show_progress.py` & `shaperone-0.41.5/shaperone/utils/_show_progress.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.4/shaperone/utils/image.py` & `shaperone-0.41.5/shaperone/utils/image.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-import cv2
-import json
-import matplotlib.pyplot as plt 
-import numpy as np
-import os
-import requests
-import shaperone
-from textwrap import wrap
-
-def is_empty(path):
-    """ Function to check if folder at given path exists and is not empty.
-    
-    Returns True if folder is empty or does not exist.
-    """
-    empty = False
-    if os.path.exists(path) and not os.path.isfile(path): 
-        # Checking if the directory is empty or not 
-        if not os.listdir(path): 
-            empty = True
-            print("'test_images' folder is empty. Please place images to be tested in this folder.") 
-    else: 
-        empty = True
-        print("There is no 'test_images' folder under current directory. Please create one and place images to be tested there.")
-    return empty
-
-def make_dir(path):
-    """
-    Function to create a new directory with given path or empty if it already exists.
-    """
-    if not os.path.exists(path):
-        if not os.path.isfile(path): 
-            # make directory if it does not exist
-            os.makedirs(path)
-        else:
-            print("Please give a valid folder path.")
-    else:
-        # Check if empty or not 
-        if os.listdir(path): 
-            # if exists, empty directory
-            for file in os.listdir(path):
-                os.remove(path+file)
-
-def add_sample_images(path):
-    """
-    Function to add sample images from imagenet50 SHAP data in the given folder.
-    """
-    X, _ = shaperone.datasets.imagenet50()
-    counter = 1
-    indexes_list = [25, 26, 30, 44]
-    for i, image in enumerate(X):
-        if i in indexes_list:
-            path_to_image = os.path.join(path, "{0}.jpg".format(counter))
-            save_image(image, path_to_image)
-            counter += 1
-
-def load_image(path_to_image):
-    """
-    Function to load image at given path and return numpy array of RGB float values. 
-    """
-    image = cv2.imread(path_to_image)
-    image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB) 
-    return np.array(image).astype('float')
-
-def check_valid_image(path_to_image):
-    """
-    Function to check if a file has valid image extensions and return True if it does. 
-    Note: Azure Cognitive Services only accepts below file formats.  
-    """
-    valid_extensions = ['.png', '.jpg', '.jpeg', '.gif', '.bmp', '.jfif']
-    if path_to_image.endswith((tuple(valid_extensions))):
-        return True 
-
-def save_image(array, path_to_image):
-    """
-    Function to save image(RGB values array) at given path (filename and location).
-    """
-    # saving array of RGB values as an image 
-    image = np.array(array)/255.0
-    plt.imsave(path_to_image, image)
-
-
-def resize_image(path_to_image, reshaped_dir):
-    """
-    Function to resize given image retaining original aspect ratio and save in given directory 'reshaped_dir'. 
-    Returns numpy array of resized image and path where resized file is saved. 
-    Note: 
-    Azure COGS CV has size limit of < 4MB and min size of 50x50 for images. 
-    Hence, large image files are being reshaped in code below to increase speed of SHAP explanations and run Azure COGS for image captions. 
-    If image (pixel_size, pixel_size) is greater than 500 for either of the dimensions: 
-    1 - image is resized to have max. 500 pixel size for the dimension > 500
-    2 - other dimension is resized retaining the original aspect ratio 
-    """
-    image = load_image(path_to_image)
-    
-    # checking if either of (pixel_size, pixel_size) dimension is greater than 500. 
-    reshaped_path = None
-    _, tail = os.path.split(path_to_image)
-    file_name = tail.split('.')[0]
-    max_pixels = 500
-    reshape = True
-
-    if image.shape[0] == image.shape[1] and image.shape[0] > 500:
-        new_dim = (max_pixels, max_pixels)
-    elif image.shape[0] > image.shape[1] and  image.shape[0] > 500:
-        new_dim = (max_pixels, int(image.shape[1]*max_pixels/image.shape[0]))
-    elif image.shape[1] > image.shape[0] and image.shape[1] > 500:
-        new_dim = (int(image.shape[0]*max_pixels/image.shape[1]), max_pixels)
-    else:
-        reshape = False 
-
-    # reshape image
-    if reshape:
-        # flipping axis for cv2 because cv2 uses width x height while numpy uses height x width
-        image = cv2.resize(image, dsize = (new_dim[1], new_dim[0])) 
-        reshaped_path = os.path.join(reshaped_dir, file_name + ".png")
-        print("Reshaped image size:", image.shape)
-        save_image(image, reshaped_path)
-        image = np.array(image).astype('float')
-    
-    return image, reshaped_path
-
-
-def display_grid_plot(list_of_captions, list_of_images, max_columns=4, figsize=(20,20)):
-    """
-    Function to display grid of images and their titles/captions.
-    """
-
-    # load list of images
-    masked_images = []
-    for filename in  list_of_images:
-        image = load_image(filename) 
-        masked_images.append(image.astype(int))
-
-    # display grid plot with wrapping
-    fig = plt.figure(figsize=figsize)
-    column = 0
-    for i in range(len(masked_images)):
-        column += 1
-        #  check for end of column and create a new figure
-        if column == max_columns+1:
-            fig = plt.figure(figsize=figsize)
-            column = 1
-        fig.add_subplot(1, max_columns, column)
-        plt.imshow(masked_images[i])
-        plt.axis('off')
-        if len(list_of_captions) >= len(masked_images):
+import cv2
+import json
+import matplotlib.pyplot as plt 
+import numpy as np
+import os
+import requests
+import shaperone
+from textwrap import wrap
+
+def is_empty(path):
+    """ Function to check if folder at given path exists and is not empty.
+    
+    Returns True if folder is empty or does not exist.
+    """
+    empty = False
+    if os.path.exists(path) and not os.path.isfile(path): 
+        # Checking if the directory is empty or not 
+        if not os.listdir(path): 
+            empty = True
+            print("'test_images' folder is empty. Please place images to be tested in this folder.") 
+    else: 
+        empty = True
+        print("There is no 'test_images' folder under current directory. Please create one and place images to be tested there.")
+    return empty
+
+def make_dir(path):
+    """
+    Function to create a new directory with given path or empty if it already exists.
+    """
+    if not os.path.exists(path):
+        if not os.path.isfile(path): 
+            # make directory if it does not exist
+            os.makedirs(path)
+        else:
+            print("Please give a valid folder path.")
+    else:
+        # Check if empty or not 
+        if os.listdir(path): 
+            # if exists, empty directory
+            for file in os.listdir(path):
+                os.remove(path+file)
+
+def add_sample_images(path):
+    """
+    Function to add sample images from imagenet50 SHAP data in the given folder.
+    """
+    X, _ = shaperone.datasets.imagenet50()
+    counter = 1
+    indexes_list = [25, 26, 30, 44]
+    for i, image in enumerate(X):
+        if i in indexes_list:
+            path_to_image = os.path.join(path, "{0}.jpg".format(counter))
+            save_image(image, path_to_image)
+            counter += 1
+
+def load_image(path_to_image):
+    """
+    Function to load image at given path and return numpy array of RGB float values. 
+    """
+    image = cv2.imread(path_to_image)
+    image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB) 
+    return np.array(image).astype('float')
+
+def check_valid_image(path_to_image):
+    """
+    Function to check if a file has valid image extensions and return True if it does. 
+    Note: Azure Cognitive Services only accepts below file formats.  
+    """
+    valid_extensions = ['.png', '.jpg', '.jpeg', '.gif', '.bmp', '.jfif']
+    if path_to_image.endswith((tuple(valid_extensions))):
+        return True 
+
+def save_image(array, path_to_image):
+    """
+    Function to save image(RGB values array) at given path (filename and location).
+    """
+    # saving array of RGB values as an image 
+    image = np.array(array)/255.0
+    plt.imsave(path_to_image, image)
+
+
+def resize_image(path_to_image, reshaped_dir):
+    """
+    Function to resize given image retaining original aspect ratio and save in given directory 'reshaped_dir'. 
+    Returns numpy array of resized image and path where resized file is saved. 
+    Note: 
+    Azure COGS CV has size limit of < 4MB and min size of 50x50 for images. 
+    Hence, large image files are being reshaped in code below to increase speed of SHAP explanations and run Azure COGS for image captions. 
+    If image (pixel_size, pixel_size) is greater than 500 for either of the dimensions: 
+    1 - image is resized to have max. 500 pixel size for the dimension > 500
+    2 - other dimension is resized retaining the original aspect ratio 
+    """
+    image = load_image(path_to_image)
+    
+    # checking if either of (pixel_size, pixel_size) dimension is greater than 500. 
+    reshaped_path = None
+    _, tail = os.path.split(path_to_image)
+    file_name = tail.split('.')[0]
+    max_pixels = 500
+    reshape = True
+
+    if image.shape[0] == image.shape[1] and image.shape[0] > 500:
+        new_dim = (max_pixels, max_pixels)
+    elif image.shape[0] > image.shape[1] and  image.shape[0] > 500:
+        new_dim = (max_pixels, int(image.shape[1]*max_pixels/image.shape[0]))
+    elif image.shape[1] > image.shape[0] and image.shape[1] > 500:
+        new_dim = (int(image.shape[0]*max_pixels/image.shape[1]), max_pixels)
+    else:
+        reshape = False 
+
+    # reshape image
+    if reshape:
+        # flipping axis for cv2 because cv2 uses width x height while numpy uses height x width
+        image = cv2.resize(image, dsize = (new_dim[1], new_dim[0])) 
+        reshaped_path = os.path.join(reshaped_dir, file_name + ".png")
+        print("Reshaped image size:", image.shape)
+        save_image(image, reshaped_path)
+        image = np.array(image).astype('float')
+    
+    return image, reshaped_path
+
+
+def display_grid_plot(list_of_captions, list_of_images, max_columns=4, figsize=(20,20)):
+    """
+    Function to display grid of images and their titles/captions.
+    """
+
+    # load list of images
+    masked_images = []
+    for filename in  list_of_images:
+        image = load_image(filename) 
+        masked_images.append(image.astype(int))
+
+    # display grid plot with wrapping
+    fig = plt.figure(figsize=figsize)
+    column = 0
+    for i in range(len(masked_images)):
+        column += 1
+        #  check for end of column and create a new figure
+        if column == max_columns+1:
+            fig = plt.figure(figsize=figsize)
+            column = 1
+        fig.add_subplot(1, max_columns, column)
+        plt.imshow(masked_images[i])
+        plt.axis('off')
+        if len(list_of_captions) >= len(masked_images):
             plt.title("\n".join(wrap(str(list_of_captions[i]), width = 40)))
```

### Comparing `shaperone-0.41.4/shaperone/utils/transformers.py` & `shaperone-0.41.5/shaperone/utils/transformers.py`

 * *Files identical despite different names*

