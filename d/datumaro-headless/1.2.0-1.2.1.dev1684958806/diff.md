# Comparing `tmp/datumaro-headless-1.2.0.tar.gz` & `tmp/datumaro-headless-1.2.1.dev1684958806.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-headless-1.2.0.tar", last modified: Wed May 24 20:17:04 2023, max compression
+gzip compressed data, was "datumaro-headless-1.2.1.dev1684958806.tar", last modified: Wed May 24 20:06:50 2023, max compression
```

## Comparing `datumaro-headless-1.2.0.tar` & `datumaro-headless-1.2.1.dev1684958806.tar`

### file list

```diff
@@ -1,321 +1,321 @@
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.750912 datumaro-headless-1.2.0/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)   373252 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/3rd-party.txt
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1090 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/LICENSE
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      103 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/MANIFEST.in
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      229 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/NOTICE
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5907 2023-05-24 20:17:04.750912 datumaro-headless-1.2.0/PKG-INFO
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5328 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/README.md
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.730912 datumaro-headless-1.2.0/datumaro/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1715 2023-05-24 19:59:25.000000 datumaro-headless-1.2.0/datumaro/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      178 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/__main__.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.730912 datumaro-headless-1.2.0/datumaro/capi/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3379 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/capi/pybind.cpp
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.730912 datumaro-headless-1.2.0/datumaro/cli/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       77 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5686 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/__main__.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.730912 datumaro-headless-1.2.0/datumaro/cli/commands/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1317 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5187 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/convert.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3991 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/detect_format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9154 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/diff.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10146 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/download.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9340 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/explain.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4118 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/cli/commands/explore.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9046 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/filter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3073 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/generate.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4238 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/info.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10275 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/merge.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5979 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/patch.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.730912 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      985 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/__init__.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.734912 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      124 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5227 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/add.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1957 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/create.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5906 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/export.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5892 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/import_.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1677 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/remove.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.734912 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      123 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2946 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2150 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/commit.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2758 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/info.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1132 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/log.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1412 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/status.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3116 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/stats.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8363 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/transform.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4837 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/commands/validate.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.734912 datumaro-headless-1.2.0/datumaro/cli/contexts/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      121 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/contexts/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9089 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/contexts/model.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.734912 datumaro-headless-1.2.0/datumaro/cli/contexts/project/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4501 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/contexts/project/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2553 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/contexts/source.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4097 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/contexts/util.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.734912 datumaro-headless-1.2.0/datumaro/cli/util/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3988 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/cli/util/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    13328 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/util/diff.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      391 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/util/errors.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5640 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/cli/util/project.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.734912 datumaro-headless-1.2.0/datumaro/components/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       77 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/__init__.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.734912 datumaro-headless-1.2.0/datumaro/components/abstracts/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       95 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/abstracts/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1077 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/abstracts/merger.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.734912 datumaro-headless-1.2.0/datumaro/components/algorithms/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      135 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/algorithms/__init__.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.734912 datumaro-headless-1.2.0/datumaro/components/algorithms/noisy_label_detection/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      111 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7851 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8073 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/algorithms/rise.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    29706 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/annotation.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.738912 datumaro-headless-1.2.0/datumaro/components/annotations/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      118 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/annotations/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8965 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/annotations/matcher.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5242 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/annotations/merger.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2146 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/cli_plugin.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8101 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/config.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3570 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/config_model.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2240 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/crypter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    46849 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/components/dataset.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10965 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/dataset_base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6034 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/dataset_item_storage.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10480 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/components/environment.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    17884 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/components/errors.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5209 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/components/explorer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    13568 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/components/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    19651 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/extractor_tfds.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10063 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/filter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    19613 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/components/format_detection.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      534 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/generator.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.738912 datumaro-headless-1.2.0/datumaro/components/hl_ops/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8684 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/hl_ops/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8657 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/components/importer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2901 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/launcher.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    36004 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/media.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2450 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/media_manager.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.738912 datumaro-headless-1.2.0/datumaro/components/merge/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3694 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/merge/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4103 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/merge/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    12216 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/merge/exact_merge.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    24147 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/merge/intersect_merge.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4453 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/merge/union_merge.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    23487 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/operations.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5221 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/progress_reporting.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    89332 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/components/project.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9352 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/shift_analyzer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1830 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/transformer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2105 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/components/validator.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    21450 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/components/visualizer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      164 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/errors.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      172 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/ops.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.738912 datumaro-headless-1.2.0/datumaro/plugins/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/__init__.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.738912 datumaro-headless-1.2.0/datumaro/plugins/accuracy_checker_plugin/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       77 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1148 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.738912 datumaro-headless-1.2.0/datumaro/plugins/accuracy_checker_plugin/details/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       77 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4038 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2217 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.738912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       77 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6297 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/ade20k2017.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8482 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/ade20k2020.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      232 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5963 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2351 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    15037 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1514 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2129 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/importer.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/mapper/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      232 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2607 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10224 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/mapper/media.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1625 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/mapper/utils.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/ava/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/ava/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8441 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/ava/ava.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5585 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3501 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/brats.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3659 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/brats_numpy.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    17438 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/camvid.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/celeba/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      183 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/celeba/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7512 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10476 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/celeba/celeba.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    12141 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/cifar.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    20683 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/cityscapes.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/coco/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/coco/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    19013 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/coco/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    28658 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/coco/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      477 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/coco/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6074 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/coco/importer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6397 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3128 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/common_super_resolution.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/cvat/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/cvat/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    14166 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/cvat/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    20627 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/cvat/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      214 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/cvat/format.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       72 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11047 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    15377 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      317 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1236 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro/importer.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      286 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6627 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11117 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      828 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1921 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      694 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11105 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2236 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1563 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5235 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/icdar/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/icdar/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11780 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/icdar/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6440 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/icdar/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      311 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/icdar/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1828 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/image_dir.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3950 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/image_zip.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6972 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/imagenet.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8124 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/imagenet_txt.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5752 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kinetics.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5975 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11358 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3970 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3713 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti/importer.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti_raw/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11148 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    17831 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      711 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    20175 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/labelme.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    14960 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/lfw.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.742912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mapillary_vistas/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10887 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    12550 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3712 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6396 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/market1501.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5013 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mars.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9041 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mnist.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7026 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mnist_csv.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10664 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mot.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6493 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mots.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.746912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mpii/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mpii/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      556 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mpii/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5193 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4937 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.746912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mvtec/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3937 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mvtec/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4813 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      563 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mvtec/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1873 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/mvtec/importer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1625 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    38486 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/open_images.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.746912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/sly_pointcloud/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6888 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    16260 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      420 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/sly_pointcloud/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7024 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/synthia.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.746912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/tf_detection_api/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7629 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8812 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      308 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    15332 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/vgg_face2.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6379 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/video.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.746912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/voc/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/voc/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    16609 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/voc/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    30069 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/voc/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9071 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/voc/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2897 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/voc/importer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2813 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/vott_csv.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3854 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/vott_json.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10103 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/widerface.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.746912 datumaro-headless-1.2.0/datumaro/plugins/data_formats/yolo/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/yolo/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    12397 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/yolo/base.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    12070 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/yolo/exporter.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      457 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/yolo/format.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5573 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/data_formats/yolo/importer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2869 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/explorer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    16787 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/ndr.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.746912 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9757 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/launcher.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.746912 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      411 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      744 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1697 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1288 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2629 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2864 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2631 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2700 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2632 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.746912 datumaro-headless-1.2.0/datumaro/plugins/sampler/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       72 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/sampler/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7786 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/sampler/random_sampler.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8772 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/sampler/relevancy_sampler.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1213 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/shift_analyzer.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    32124 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/splitter.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.746912 datumaro-headless-1.2.0/datumaro/plugins/synthetic_data/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      155 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/synthetic_data/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11335 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/synthetic_data/background_colors.txt
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11577 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/synthetic_data/image_generator.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6194 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/synthetic_data/utils.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.746912 datumaro-headless-1.2.0/datumaro/plugins/tiling/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      116 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/tiling/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9398 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/tiling/merge_tile.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9834 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/tiling/tile.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1141 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/plugins/tiling/util.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    41240 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/transforms.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    44261 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/plugins/validators.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      376 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/project.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.750912 datumaro-headless-1.2.0/datumaro/util/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4809 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/__init__.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8473 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/util/annotation_util.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1198 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/attrs_util.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      262 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/definitions.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      882 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/file_utils.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11657 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/image.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      968 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/image_cache.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      795 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/log_utils.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11440 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/util/mask_tools.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2062 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/datumaro/util/meta_file_util.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8479 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/os_util.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      758 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/pickle_util.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      246 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/samples.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4702 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/scope.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      616 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/telemetry_stub.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6073 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/telemetry_utils.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2579 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/datumaro/util/tf_util.py
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       23 2023-05-24 20:16:53.000000 datumaro-headless-1.2.0/datumaro/version.py
-drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:17:04.750912 datumaro-headless-1.2.0/datumaro_headless.egg-info/
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5907 2023-05-24 20:17:04.000000 datumaro-headless-1.2.0/datumaro_headless.egg-info/PKG-INFO
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11540 2023-05-24 20:17:04.000000 datumaro-headless-1.2.0/datumaro_headless.egg-info/SOURCES.txt
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        1 2023-05-24 20:17:04.000000 datumaro-headless-1.2.0/datumaro_headless.egg-info/dependency_links.txt
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       53 2023-05-24 20:17:04.000000 datumaro-headless-1.2.0/datumaro_headless.egg-info/entry_points.txt
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      773 2023-05-24 20:17:04.000000 datumaro-headless-1.2.0/datumaro_headless.egg-info/requires.txt
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        9 2023-05-24 20:17:04.000000 datumaro-headless-1.2.0/datumaro_headless.egg-info/top_level.txt
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2488 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/pyproject.toml
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      692 2023-05-24 20:00:30.000000 datumaro-headless-1.2.0/requirements-core.txt
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      266 2023-05-24 19:58:03.000000 datumaro-headless-1.2.0/requirements-default.txt
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       38 2023-05-24 20:17:04.750912 datumaro-headless-1.2.0/setup.cfg
--rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3236 2023-05-24 20:03:39.000000 datumaro-headless-1.2.0/setup.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.464894 datumaro-headless-1.2.1.dev1684958806/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)   373252 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/3rd-party.txt
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1090 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/LICENSE
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      103 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/MANIFEST.in
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      229 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/NOTICE
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5921 2023-05-24 20:06:50.464894 datumaro-headless-1.2.1.dev1684958806/PKG-INFO
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5328 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/README.md
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.444895 datumaro-headless-1.2.1.dev1684958806/datumaro/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1715 2023-05-24 19:59:25.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      178 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/__main__.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.444895 datumaro-headless-1.2.1.dev1684958806/datumaro/capi/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3379 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/capi/pybind.cpp
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.444895 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       77 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5686 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/__main__.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.444895 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1317 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5187 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/convert.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3991 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/detect_format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9154 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/diff.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10146 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/download.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9340 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/explain.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4118 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/explore.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9046 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/filter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3073 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/generate.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4238 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/info.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10275 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/merge.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5979 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/patch.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.444895 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      985 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/__init__.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.444895 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      124 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5227 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/add.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1957 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/create.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5906 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/export.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5892 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/import_.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1677 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/remove.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.444895 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      123 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2946 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2150 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2758 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/info.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1132 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/log.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1412 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/status.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3116 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/stats.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8363 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/transform.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4837 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/validate.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.444895 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/contexts/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      121 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/contexts/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9089 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/contexts/model.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.444895 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/contexts/project/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4501 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/contexts/project/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2553 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/contexts/source.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4097 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/contexts/util.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.444895 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/util/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3988 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/util/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    13328 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/util/diff.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      391 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/util/errors.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5640 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/cli/util/project.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.448895 datumaro-headless-1.2.1.dev1684958806/datumaro/components/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       77 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/__init__.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.448895 datumaro-headless-1.2.1.dev1684958806/datumaro/components/abstracts/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       95 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/abstracts/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1077 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/abstracts/merger.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.448895 datumaro-headless-1.2.1.dev1684958806/datumaro/components/algorithms/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      135 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/algorithms/__init__.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.448895 datumaro-headless-1.2.1.dev1684958806/datumaro/components/algorithms/noisy_label_detection/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      111 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7851 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8073 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/algorithms/rise.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    29706 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/annotation.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.448895 datumaro-headless-1.2.1.dev1684958806/datumaro/components/annotations/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      118 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/annotations/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8965 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/annotations/matcher.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5242 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/annotations/merger.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2146 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/cli_plugin.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8101 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/config.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3570 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/config_model.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2240 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/crypter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    46849 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/dataset.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10965 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/dataset_base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6034 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/dataset_item_storage.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10480 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/environment.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    17884 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/errors.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5209 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/explorer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    13568 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    19651 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/extractor_tfds.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10063 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/filter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    19613 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/format_detection.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      534 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/generator.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.448895 datumaro-headless-1.2.1.dev1684958806/datumaro/components/hl_ops/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8684 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/hl_ops/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8657 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/importer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2901 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/launcher.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    36004 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/media.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2450 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/media_manager.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.448895 datumaro-headless-1.2.1.dev1684958806/datumaro/components/merge/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3694 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/merge/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4103 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/merge/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    12216 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/merge/exact_merge.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    24147 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/merge/intersect_merge.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4453 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/merge/union_merge.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    23487 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/operations.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5221 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/progress_reporting.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    89332 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/project.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9352 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/shift_analyzer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1830 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/transformer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2105 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/validator.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    21450 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/components/visualizer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      164 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/errors.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      172 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/ops.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.448895 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/__init__.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.448895 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/accuracy_checker_plugin/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       77 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1148 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.448895 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       77 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4038 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2217 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.452894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       77 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6297 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/ade20k2017.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8482 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/ade20k2020.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.452894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      232 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5963 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2351 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    15037 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1514 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2129 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/importer.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.452894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/mapper/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      232 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2607 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10224 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/mapper/media.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1625 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/mapper/utils.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.452894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/ava/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/ava/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8441 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/ava/ava.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5585 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3501 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/brats.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3659 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/brats_numpy.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    17438 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/camvid.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.452894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/celeba/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      183 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7512 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10476 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    12141 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/cifar.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    20683 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/cityscapes.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.452894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/coco/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/coco/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    19013 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/coco/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    28658 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/coco/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      477 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/coco/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6074 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/coco/importer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6397 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3128 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/common_super_resolution.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.452894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/cvat/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    14166 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/cvat/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    20627 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      214 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/cvat/format.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.456894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       72 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11047 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    15377 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      317 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1236 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro/importer.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.456894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      286 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6627 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11117 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      828 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1921 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.456894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      694 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11105 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2236 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1563 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5235 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.456894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/icdar/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11780 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/icdar/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6440 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      311 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/icdar/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1828 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/image_dir.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3950 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/image_zip.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6972 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/imagenet.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8124 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5752 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kinetics.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.456894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5975 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11358 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3970 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3713 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti/importer.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.456894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti_raw/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11148 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    17831 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      711 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    20175 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/labelme.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    14960 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/lfw.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.456894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10887 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    12550 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3712 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6396 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/market1501.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5013 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mars.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9041 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mnist.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7026 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mnist_csv.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10664 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mot.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6493 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mots.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.456894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mpii/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      556 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mpii/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5193 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4937 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.456894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mvtec/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3937 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mvtec/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4813 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      563 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mvtec/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1873 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1625 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    38486 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/open_images.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.456894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6888 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    16260 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      420 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/sly_pointcloud/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7024 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/synthia.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.456894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/tf_detection_api/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7629 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8812 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      308 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    15332 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/vgg_face2.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6379 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/video.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.460894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/voc/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/voc/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    16609 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/voc/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    30069 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/voc/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9071 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/voc/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2897 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/voc/importer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2813 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/vott_csv.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3854 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/vott_json.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    10103 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/widerface.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.460894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/yolo/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    12397 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/yolo/base.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    12070 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      457 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/yolo/format.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5573 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/yolo/importer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2869 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/explorer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    16787 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/ndr.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.460894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9757 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/launcher.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.460894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      411 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      744 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1697 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1288 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2629 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2864 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2631 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2700 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2632 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.460894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/sampler/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       72 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/sampler/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     7786 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/sampler/random_sampler.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8772 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1213 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/shift_analyzer.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    32124 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/splitter.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.460894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/synthetic_data/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      155 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/synthetic_data/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11335 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11577 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/synthetic_data/image_generator.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6194 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/synthetic_data/utils.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.460894 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/tiling/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      116 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/tiling/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9398 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/tiling/merge_tile.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     9834 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/tiling/tile.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1141 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/tiling/util.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    41240 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/transforms.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    44261 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/validators.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      376 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/project.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.460894 datumaro-headless-1.2.1.dev1684958806/datumaro/util/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4809 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/__init__.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8473 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/annotation_util.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     1198 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/attrs_util.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      262 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/definitions.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      882 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/file_utils.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11657 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/image.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      968 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/image_cache.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      795 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/log_utils.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11440 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/mask_tools.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2062 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/meta_file_util.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     8479 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/os_util.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      758 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/pickle_util.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      246 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/samples.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     4702 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/scope.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      616 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/telemetry_stub.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     6073 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/telemetry_utils.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2579 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/util/tf_util.py
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       36 2023-05-24 20:06:46.000000 datumaro-headless-1.2.1.dev1684958806/datumaro/version.py
+drwxrwxr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-05-24 20:06:50.460894 datumaro-headless-1.2.1.dev1684958806/datumaro_headless.egg-info/
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     5921 2023-05-24 20:06:50.000000 datumaro-headless-1.2.1.dev1684958806/datumaro_headless.egg-info/PKG-INFO
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)    11540 2023-05-24 20:06:50.000000 datumaro-headless-1.2.1.dev1684958806/datumaro_headless.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        1 2023-05-24 20:06:50.000000 datumaro-headless-1.2.1.dev1684958806/datumaro_headless.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       53 2023-05-24 20:06:50.000000 datumaro-headless-1.2.1.dev1684958806/datumaro_headless.egg-info/entry_points.txt
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      773 2023-05-24 20:06:50.000000 datumaro-headless-1.2.1.dev1684958806/datumaro_headless.egg-info/requires.txt
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)        9 2023-05-24 20:06:50.000000 datumaro-headless-1.2.1.dev1684958806/datumaro_headless.egg-info/top_level.txt
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     2488 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/pyproject.toml
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      692 2023-05-24 20:00:30.000000 datumaro-headless-1.2.1.dev1684958806/requirements-core.txt
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)      266 2023-05-24 19:58:03.000000 datumaro-headless-1.2.1.dev1684958806/requirements-default.txt
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)       38 2023-05-24 20:06:50.464894 datumaro-headless-1.2.1.dev1684958806/setup.cfg
+-rw-rw-r--   0 jbencook  (1000) jbencook  (1000)     3236 2023-05-24 20:03:39.000000 datumaro-headless-1.2.1.dev1684958806/setup.py
```

### Comparing `datumaro-headless-1.2.0/3rd-party.txt` & `datumaro-headless-1.2.1.dev1684958806/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/LICENSE` & `datumaro-headless-1.2.1.dev1684958806/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/PKG-INFO` & `datumaro-headless-1.2.1.dev1684958806/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro-headless
-Version: 1.2.0
+Version: 1.2.1.dev1684958806
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-headless-1.2.0/README.md` & `datumaro-headless-1.2.1.dev1684958806/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/__init__.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/capi/pybind.cpp` & `datumaro-headless-1.2.1.dev1684958806/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/__main__.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/__init__.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/convert.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/detect_format.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/diff.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/download.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/explain.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/explore.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/explore.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/filter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/generate.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/info.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/merge.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/patch.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/require_project/__init__.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/stats.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/transform.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/commands/validate.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/contexts/model.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/contexts/project/__init__.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/contexts/source.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/contexts/util.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/util/__init__.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/util/diff.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/util/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/cli/util/project.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/abstracts/merger.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/algorithms/rise.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/annotation.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/annotations/matcher.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/annotations/merger.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/cli_plugin.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/config.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/config_model.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/crypter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/dataset.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/dataset_base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/dataset_base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/dataset_item_storage.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/dataset_item_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/environment.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/environment.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/errors.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/explorer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/extractor_tfds.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/filter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/format_detection.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/generator.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/hl_ops/__init__.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/importer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/launcher.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/media.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/media_manager.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/merge/__init__.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/merge/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/merge/exact_merge.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/merge/intersect_merge.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/merge/union_merge.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/operations.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/progress_reporting.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/project.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/shift_analyzer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/transformer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/validator.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/components/visualizer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/arrow/mapper/utils.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/arrow/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/brats.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/camvid.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/camvid.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/cifar.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/cifar.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/cityscapes.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/coco/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/coco/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/cvat/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/image_dir.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/image_zip.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/imagenet.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/imagenet.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/kinetics.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/labelme.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/labelme.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/lfw.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/market1501.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mars.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mnist.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mot.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mots.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/open_images.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/open_images.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/synthia.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/synthia.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/video.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/voc/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/voc/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/voc/format.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/vott_json.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/widerface.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/yolo/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/explorer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/ndr.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/sampler/random_sampler.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/shift_analyzer.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/splitter.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/synthetic_data/utils.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/tiling/merge_tile.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/tiling/tile.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/tiling/util.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/transforms.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/transforms.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/plugins/validators.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/__init__.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/annotation_util.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/attrs_util.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/file_utils.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/image.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/image.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/image_cache.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/log_utils.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/mask_tools.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/meta_file_util.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/os_util.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/pickle_util.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/scope.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/telemetry_stub.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/telemetry_utils.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro/util/tf_util.py` & `datumaro-headless-1.2.1.dev1684958806/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro_headless.egg-info/PKG-INFO` & `datumaro-headless-1.2.1.dev1684958806/datumaro_headless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro-headless
-Version: 1.2.0
+Version: 1.2.1.dev1684958806
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-headless-1.2.0/datumaro_headless.egg-info/SOURCES.txt` & `datumaro-headless-1.2.1.dev1684958806/datumaro_headless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/datumaro_headless.egg-info/requires.txt` & `datumaro-headless-1.2.1.dev1684958806/datumaro_headless.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/pyproject.toml` & `datumaro-headless-1.2.1.dev1684958806/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/requirements-core.txt` & `datumaro-headless-1.2.1.dev1684958806/requirements-core.txt`

 * *Files identical despite different names*

### Comparing `datumaro-headless-1.2.0/setup.py` & `datumaro-headless-1.2.1.dev1684958806/setup.py`

 * *Files identical despite different names*

