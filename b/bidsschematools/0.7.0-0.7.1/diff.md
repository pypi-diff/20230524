# Comparing `tmp/bidsschematools-0.7.0.tar.gz` & `tmp/bidsschematools-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bidsschematools-0.7.0.tar", last modified: Thu May 18 19:49:22 2023, max compression
+gzip compressed data, was "bidsschematools-0.7.1.tar", last modified: Wed May 24 20:38:03 2023, max compression
```

## Comparing `bidsschematools-0.7.0.tar` & `bidsschematools-0.7.1.tar`

### file list

```diff
@@ -1,1735 +1,1736 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.746920 bidsschematools-0.7.0/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1085 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)     1709 2023-05-18 19:49:22.746920 bidsschematools-0.7.0/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      854 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/
--rw-rw-r--   0 chris     (1000) chris     (1000)      505 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      859 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/__main__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3493 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/conftest.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/data/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/data/schema/
--rw-rw-r--   0 chris     (1000) chris     (1000)       10 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/BIDS_VERSION
--rw-rw-r--   0 chris     (1000) chris     (1000)        6 2023-05-18 19:48:46.000000 bidsschematools-0.7.0/bidsschematools/data/schema/SCHEMA_VERSION
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/data/schema/meta/
--rw-rw-r--   0 chris     (1000) chris     (1000)    11408 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/meta/context.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     3173 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/meta/expression_tests.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      239 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/data/schema/meta/versions.yaml
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.630920 bidsschematools-0.7.0/bidsschematools/data/schema/objects/
--rw-rw-r--   0 chris     (1000) chris     (1000)    25092 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/data/schema/objects/columns.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     7893 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/objects/common_principles.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1779 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/objects/datatypes.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)    17197 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/objects/entities.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)    11348 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/objects/extensions.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     7250 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/objects/files.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     4854 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/data/schema/objects/formats.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)   124077 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/data/schema/objects/metadata.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      949 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/objects/modalities.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)    28200 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/objects/suffixes.yaml
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.630920 bidsschematools-0.7.0/bidsschematools/data/schema/rules/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.630920 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1052 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/anat.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)    13313 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/asl.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      548 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/common_derivatives.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1817 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/dataset.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1502 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/dwi.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      895 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/events.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1389 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/fmap.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     4190 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/func.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      628 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/general.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1517 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/hints.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1315 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/micr.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     3514 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/mri.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1302 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/nifti.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     2327 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/nirs.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      915 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/privacy.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1282 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/references.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      334 2023-03-17 18:18:07.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/common_principles.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1345 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/dataset_metadata.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      450 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/entities.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     6903 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/errors.yaml
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.618920 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.630920 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/common/
--rw-rw-r--   0 chris     (1000) chris     (1000)      651 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/common/core.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      567 2023-03-17 18:18:07.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/common/tables.yaml
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.630920 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/deriv/
--rw-rw-r--   0 chris     (1000) chris     (1000)     4800 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/deriv/imaging.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     5277 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/deriv/preprocessed_data.yaml
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.630920 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/
--rw-rw-r--   0 chris     (1000) chris     (1000)     3301 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/anat.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      242 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/beh.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1467 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/channels.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      579 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/dwi.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      278 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/eeg.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     2243 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/fmap.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      695 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/func.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      294 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/ieeg.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1219 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/meg.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      478 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/micr.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      242 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/motion.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      215 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/nirs.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      750 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/perf.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      507 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/pet.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      432 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/photo.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     2301 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/task.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      375 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/modalities.yaml
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.634920 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1044 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/anat.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     6566 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/asl.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/beh.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      607 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/continuous.yaml
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.634920 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/derivatives/
--rw-rw-r--   0 chris     (1000) chris     (1000)     2625 2023-05-18 19:19:43.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/derivatives/common_derivatives.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      438 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/dwi.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     5095 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/eeg.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1324 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/entity_rules.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/events.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1827 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/fmap.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     2220 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/func.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     4492 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/ieeg.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     8162 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/meg.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     2785 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/micr.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     2466 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/motion.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)    10087 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/mri.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     5384 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/nirs.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     9017 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/pet.yaml
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.634920 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.634920 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/derivatives/
--rw-rw-r--   0 chris     (1000) chris     (1000)      306 2023-03-17 18:18:07.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/derivatives/common_derivatives.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      993 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/eeg.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1853 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/ieeg.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      567 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/meg.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1423 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/modality_agnostic.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      602 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/motion.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1661 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/nirs.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      154 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/perf.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1678 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/pet.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      168 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/physio.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)      306 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/task.yaml
--rw-rw-r--   0 chris     (1000) chris     (1000)     6572 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/expressions.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.634920 bidsschematools-0.7.0/bidsschematools/render/
--rw-rw-r--   0 chris     (1000) chris     (1000)      781 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/render/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    20849 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/render/tables.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    18185 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/render/text.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12036 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/render/utils.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7256 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/rules.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7484 2023-05-02 14:07:12.000000 bidsschematools-0.7.0/bidsschematools/schema.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.634920 bidsschematools-0.7.0/bidsschematools/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.634920 bidsschematools-0.7.0/bidsschematools/tests/data/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/data/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.634920 bidsschematools-0.7.0/bidsschematools/tests/data/__pycache__/
--rw-rw-r--   0 chris     (1000) chris     (1000)      188 2023-05-18 19:49:00.000000 bidsschematools-0.7.0/bidsschematools/tests/data/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.634920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/
--rw-rw-r--   0 chris     (1000) chris     (1000)     2217 2023-05-18 19:49:12.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/CONTRIBUTING.md
--rw-rw-r--   0 chris     (1000) chris     (1000)      827 2023-05-18 19:49:12.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.634920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/
--rw-rw-r--   0 chris     (1000) chris     (1000)      295 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/README
--rw-rw-r--   0 chris     (1000) chris     (1000)      488 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/dataset_description.json
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.618920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.634920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/
--rw-rw-r--   0 chris     (1000) chris     (1000)      500 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/sub-Sub1_T1w.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/sub-Sub1_T1w.nii.gz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.638920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1301 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)      152 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_aslcontext.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)   411101 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg
--rw-rw-r--   0 chris     (1000) chris     (1000)   411101 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_headshape.jpg
--rw-rw-r--   0 chris     (1000) chris     (1000)      735 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.nii.gz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.638920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/
--rw-rw-r--   0 chris     (1000) chris     (1000)      176 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/README
--rw-rw-r--   0 chris     (1000) chris     (1000)      832 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/dataset_description.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      162 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/participants.json
--rw-rw-r--   0 chris     (1000) chris     (1000)       32 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/participants.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.622920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.622920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.638920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/
--rwxrwxr-x   0 chris     (1000) chris     (1000)   118231 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii
--rwxrwxr-x   0 chris     (1000) chris     (1000)     1190 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-02_ses-01_T1w.json
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.638920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/
--rwxrwxr-x   0 chris     (1000) chris     (1000)     1941 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.json
--rw-rw-r--   0 chris     (1000) chris     (1000)    84350 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz
--rwxrwxr-x   0 chris     (1000) chris     (1000)      413 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.json
--rw-rw-r--   0 chris     (1000) chris     (1000)    15131 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.tsv
--rwxrwxr-x   0 chris     (1000) chris     (1000)     1061 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      509 2023-05-18 19:49:13.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.638920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/
--rw-rw-r--   0 chris     (1000) chris     (1000)     2928 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/CONTRIBUTING.md
--rw-rw-r--   0 chris     (1000) chris     (1000)    25620 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.638920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/
--rw-rw-r--   0 chris     (1000) chris     (1000)      232 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/README
--rw-rw-r--   0 chris     (1000) chris     (1000)      488 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/dataset_description.json
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.622920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.638920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/
--rw-rw-r--   0 chris     (1000) chris     (1000)      500 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/sub-Sub1_T1w.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/sub-Sub1_T1w.nii.gz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.638920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1301 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)      152 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_aslcontext.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)   411101 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg
--rw-rw-r--   0 chris     (1000) chris     (1000)      735 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)       23 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/bidsconfig.json
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.638920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/
--rw-rw-r--   0 chris     (1000) chris     (1000)      235 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/CHANGES
--rw-rw-r--   0 chris     (1000) chris     (1000)     2697 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/README
--rw-rw-r--   0 chris     (1000) chris     (1000)      195 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/acq-epi_T1w.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1554 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/dataset_description.json
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.622920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.622920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.622920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.622920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.638920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/brain.surf
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-5120-5120-5120-bem-sol.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-5120-5120-5120-bem.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-fiducials.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-head-dense.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-head-medium.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-head.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-ico-5-src.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-inner_skull-bem.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-trans.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-vol-5-src.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/inner_skull.surf
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/outer_skin.surf
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/outer_skull.surf
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.654920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/Yeo_Brainmap_fsaverage_README
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA1.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA1_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA1_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA2.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA2_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA2_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3a.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3a_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3a_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3b.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3b_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3b_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA44.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA44_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA44_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA45.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA45_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA45_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4a.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4a_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4a_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4p.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4p_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4p_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA6.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA6_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA6_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.HCPMMP1.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.HCPMMP1_combined.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.MT.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.MT_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.MT_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Medial_wall.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.PALS_B12.labels.gii
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.PALS_B12_Brodmann.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.PALS_B12_Lobes.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.PALS_B12_OrbitoFrontal.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.PALS_B12_Visuotopic.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V1.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V1_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V1_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V2.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V2_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V2_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo2011_17NetworksConfidence_N1000.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo2011_17Networks_N1000.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo2011_7NetworksConfidence_N1000.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo2011_7Networks_N1000.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_10Comp_PrActGivenComp.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_10to14Comp_Flexibility.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_10to14Comp_Specialization.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_10to14Comp_SpecializationROI.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_10to14Comp_TopSpecializationComp.csv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_11Comp_PrActGivenComp.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_12Comp_PrActGivenComp.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_13Comp_PrActGivenComp.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_14Comp_PrActGivenComp.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.aparc.a2005s.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.aparc.a2009s.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.aparc.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.aparc.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.aparc_sub.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.cortex.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.entorhinal.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.entorhinal_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.entorhinal_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.ifc.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.ipc.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.ips.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.lateraltemporal.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.medialpfc.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.mtl.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.retrosplenial.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.tp.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.perirhinal_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.perirhinal_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA1.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA1_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA1_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA2.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA2_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA2_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3a.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3a_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3a_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3b.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3b_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3b_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA44.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA44_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA44_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA45.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA45_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA45_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4a.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4a_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4a_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4p.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4p_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4p_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA6.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA6_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA6_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.HCPMMP1.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.HCPMMP1_combined.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.MT.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.MT_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.MT_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Medial_wall.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.PALS_B12.labels.gii
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.PALS_B12_Brodmann.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.PALS_B12_Lobes.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.PALS_B12_OrbitoFrontal.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.PALS_B12_Visuotopic.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V1.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V1_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V1_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V2.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V2_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V2_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo2011_17NetworksConfidence_N1000.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo2011_17Networks_N1000.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo2011_7NetworksConfidence_N1000.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo2011_7Networks_N1000.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_10Comp_PrActGivenComp.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_10to14Comp_Flexibility.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_10to14Comp_Specialization.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_10to14Comp_SpecializationROI.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_10to14Comp_TopSpecializationComp.csv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_11Comp_PrActGivenComp.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_12Comp_PrActGivenComp.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_13Comp_PrActGivenComp.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_14Comp_PrActGivenComp.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.aparc.a2005s.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.aparc.a2009s.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.aparc.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.aparc.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.aparc_sub.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.cortex.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.entorhinal.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.entorhinal_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.entorhinal_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.ifc.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.ipc.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.ips.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.lateraltemporal.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.medialpfc.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.mtl.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.retrosplenial.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.tp.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.perirhinal_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.perirhinal_exvivo.thresh.label
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.654920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/T1.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/aparc+aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/aparc.a2005s+aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/aparc.a2009s+aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/brain.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/brainmask.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/lh.ribbon.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/mni305.cor.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/orig.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/p.aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/rh.ribbon.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/ribbon.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/seghead.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/subcort.mask.1mm.README
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/subcort.mask.1mm.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/subcort.prob.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/subcort.prob.mgz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.658920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/transforms/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/transforms/reg.mni152.2mm.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/transforms/talairach.xfm
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.658920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/README
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/T1.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/brain.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/brainmask.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/mni305.cor.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/orig.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/reg.2mm.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/reg.2mm.mni152.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/subcort.mask.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/subcort.prob.mgz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.658920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/build-stamp.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/csurfdir
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/cvs_log_pre_31May2011.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/make_average_surface.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/make_average_volume.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/mkheadsurf.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/mris_inflate.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/mris_inflate_lh.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/mris_inflate_rh.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all-status.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.cmd
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.done
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.env
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.env.bak
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.local-copy
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/surfreg.fsaverage_sym.lh.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/surfreg.fsaverage_sym.rh.log
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.662920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.area
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.area.seghead
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.avg_curv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.avg_sulc
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.avg_thickness
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.cortex.patch.3d
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.cortex.patch.flat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.curv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.curv.seghead
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.fsaverage_sym.sphere.reg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.inflated
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.inflated.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.inflated.K
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.inflated_avg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.inflated_pre
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.orig
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.orig.avg.area.mgh
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.orig_avg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.pial
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.pial.avg.area.mgh
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.pial_avg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.pial_semi_inflated
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.seghead
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.seghead.inflated
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.smoothwm
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sphere
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sphere.left_right
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sphere.reg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sphere.reg.avg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sulc
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sulc.seghead
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.thickness
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.white
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.white.avg.area.mgh
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.white_avg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.white_avg.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.white_avg.K
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/mris_preproc.surface.lh.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/mris_preproc.surface.rh.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.area
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.avg_curv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.avg_sulc
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.avg_thickness
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.cortex.patch.3d
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.cortex.patch.flat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.curv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.fsaverage_sym.sphere.reg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.inflated
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.inflated.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.inflated.K
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.inflated_avg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.inflated_pre
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.orig
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.orig.avg.area.mgh
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.orig_avg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.pial
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.pial.avg.area.mgh
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.pial_avg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.pial_semi_inflated
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.smoothwm
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.sphere
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.sphere.left_right
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.sphere.reg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.sphere.reg.avg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.sulc
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.thickness
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.white
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.white.avg.area.mgh
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.white_avg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.white_avg.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.white_avg.K
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.662920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.662920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/lh.aparc.a2009s.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/lh.aparc.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/lh.cortex.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/rh.aparc.a2009s.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/rh.aparc.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/rh.cortex.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/lrrev.pure.register.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/lrrev.register.dat
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.662920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/T1.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/aparc+aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/brain.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/brainmask.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/mri_nu_correct.mni.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/orig.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/orig_nu.mgz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.662920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/transforms/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/transforms/talairach.auto.xfm
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/transforms/talairach.xfm
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/transforms/talairach_avi.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/transforms/talsrcimg_to_711-2C_as_mni_average_305_t4_vox2vox.txt
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.662920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/build-stamp.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/lastcall.build-stamp.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/patchdir.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all-status.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all.cmd
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all.done
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all.env
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all.local-copy
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/surfreg.fsaverage_sym.lh.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/surfreg.fsaverage_sym.rh.log
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.666920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.area
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.curv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.fsaverage_sym.sphere.reg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.inflated
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.inflated.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.inflated.K
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.orig
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.pial
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.smoothwm
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.sphere
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.sulc
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.thickness
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.white
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.area
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.curv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.fsaverage_sym.sphere.reg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.inflated
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.inflated.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.inflated.K
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.orig
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.pial
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.smoothwm
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.sphere
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.sulc
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.thickness
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.white
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.666920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/touch/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/touch/talairach.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/xhemireg.lh.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/xhemireg.rh.log
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.666920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/morph-maps/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/morph-maps/fsaverage-sub-01-morph.fif
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.622920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.666920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.666920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/inner_skull.surf
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/inner_skull.tri
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/outer_skin.surf
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/outer_skin.tri
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/outer_skull.surf
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/outer_skull.tri
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/inner_skull.surf
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/outer_skin.surf
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/outer_skull.surf
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.670920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/BA_exvivo.ctab
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/BA_exvivo.thresh.ctab
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/aparc.annot.DKTatlas.ctab
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/aparc.annot.a2009s.ctab
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/aparc.annot.ctab
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA1_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA1_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA2_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA2_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA3a_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA3a_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA3b_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA3b_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA44_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA44_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA45_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA45_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA4a_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA4a_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA4p_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA4p_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA6_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA6_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA_exvivo.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA_exvivo.thresh.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.MT_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.MT_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.V1_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.V1_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.V2_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.V2_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.aparc.DKTatlas.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.aparc.a2009s.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.aparc.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.cortex.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.entorhinal_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.entorhinal_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.perirhinal_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.perirhinal_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA1_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA1_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA2_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA2_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA3a_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA3a_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA3b_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA3b_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA44_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA44_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA45_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA45_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA4a_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA4a_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA4p_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA4p_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA6_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA6_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA_exvivo.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA_exvivo.thresh.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.MT_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.MT_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.V1_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.V1_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.V2_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.V2_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.aparc.DKTatlas.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.aparc.a2009s.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.aparc.annot
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.cortex.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.entorhinal_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.entorhinal_exvivo.thresh.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.perirhinal_exvivo.label
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.perirhinal_exvivo.thresh.label
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.674920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.694920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-.info
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-001
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-002
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-003
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-004
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-005
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-006
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-007
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-008
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-009
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-010
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-011
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-012
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-013
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-014
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-015
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-016
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-017
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-018
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-019
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-020
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-021
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-022
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-023
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-024
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-025
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-026
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-027
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-028
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-029
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-030
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-031
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-032
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-033
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-034
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-035
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-036
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-037
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-038
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-039
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-040
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-041
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-042
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-043
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-044
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-045
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-046
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-047
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-048
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-049
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-050
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-051
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-052
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-053
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-054
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-055
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-056
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-057
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-058
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-059
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-060
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-061
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-062
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-063
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-064
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-065
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-066
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-067
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-068
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-069
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-070
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-071
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-072
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-073
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-074
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-075
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-076
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-077
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-078
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-079
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-080
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-081
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-082
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-083
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-084
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-085
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-086
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-087
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-088
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-089
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-090
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-091
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-092
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-093
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-094
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-095
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-096
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-097
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-098
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-099
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-100
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-101
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-102
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-103
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-104
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-105
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-106
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-107
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-108
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-109
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-110
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-111
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-112
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-113
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-114
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-115
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-116
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-117
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-118
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-119
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-120
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-121
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-122
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-123
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-124
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-125
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-126
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-127
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-128
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-129
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-130
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-131
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-132
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-133
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-134
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-135
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-136
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-137
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-138
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-139
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-140
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-141
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-142
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-143
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-144
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-145
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-146
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-147
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-148
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-149
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-150
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-151
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-152
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-153
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-154
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-155
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-156
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-157
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-158
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-159
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-160
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-161
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-162
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-163
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-164
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-165
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-166
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-167
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-168
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-169
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-170
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-171
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-172
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-173
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-174
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-175
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-176
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-177
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-178
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-179
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-180
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-181
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-182
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-183
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-184
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-185
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-186
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-187
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-188
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-189
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-190
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-191
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-192
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-193
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-194
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-195
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-196
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-197
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-198
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-199
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-200
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-201
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-202
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-203
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-204
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-205
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-206
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-207
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-208
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-209
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-210
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-211
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-212
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-213
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-214
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-215
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-216
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-217
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-218
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-219
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-220
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-221
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-222
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-223
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-224
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-225
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-226
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-227
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-228
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-229
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-230
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-231
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-232
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-233
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-234
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-235
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-236
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-237
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-238
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-239
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-240
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-241
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-242
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-243
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-244
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-245
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-246
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-247
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-248
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-249
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-250
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-251
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-252
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-253
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-254
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-255
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-256
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aparc+aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aparc.DKTatlas+aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aparc.a2009s+aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.auto.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.auto_noCCseg.label_intensities.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.auto_noCCseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.presurf.hypos.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.presurf.mgz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.710920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-.info
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-001
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-002
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-003
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-004
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-005
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-006
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-007
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-008
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-009
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-010
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-011
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-012
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-013
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-014
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-015
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-016
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-017
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-018
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-019
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-020
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-021
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-022
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-023
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-024
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-025
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-026
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-027
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-028
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-029
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-030
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-031
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-032
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-033
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-034
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-035
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-036
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-037
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-038
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-039
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-040
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-041
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-042
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-043
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-044
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-045
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-046
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-047
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-048
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-049
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-050
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-051
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-052
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-053
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-054
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-055
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-056
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-057
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-058
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-059
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-060
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-061
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-062
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-063
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-064
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-065
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-066
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-067
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-068
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-069
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-070
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-071
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-072
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-073
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-074
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-075
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-076
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-077
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-078
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-079
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-080
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-081
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-082
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-083
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-084
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-085
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-086
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-087
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-088
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-089
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-090
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-091
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-092
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-093
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-094
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-095
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-096
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-097
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-098
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-099
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-100
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-101
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-102
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-103
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-104
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-105
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-106
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-107
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-108
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-109
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-110
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-111
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-112
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-113
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-114
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-115
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-116
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-117
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-118
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-119
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-120
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-121
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-122
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-123
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-124
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-125
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-126
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-127
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-128
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-129
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-130
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-131
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-132
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-133
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-134
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-135
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-136
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-137
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-138
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-139
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-140
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-141
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-142
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-143
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-144
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-145
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-146
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-147
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-148
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-149
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-150
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-151
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-152
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-153
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-154
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-155
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-156
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-157
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-158
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-159
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-160
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-161
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-162
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-163
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-164
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-165
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-166
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-167
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-168
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-169
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-170
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-171
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-172
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-173
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-174
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-175
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-176
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-177
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-178
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-179
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-180
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-181
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-182
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-183
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-184
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-185
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-186
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-187
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-188
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-189
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-190
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-191
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-192
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-193
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-194
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-195
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-196
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-197
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-198
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-199
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-200
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-201
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-202
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-203
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-204
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-205
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-206
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-207
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-208
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-209
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-210
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-211
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-212
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-213
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-214
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-215
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-216
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-217
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-218
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-219
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-220
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-221
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-222
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-223
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-224
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-225
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-226
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-227
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-228
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-229
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-230
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-231
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-232
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-233
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-234
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-235
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-236
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-237
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-238
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-239
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-240
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-241
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-242
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-243
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-244
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-245
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-246
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-247
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-248
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-249
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-250
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-251
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-252
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-253
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-254
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-255
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-256
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain.finalsurfs.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brainmask.auto.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brainmask.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/ctrl_pts.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/filled.mgz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.710920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/mef05.mgz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.710920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/flash5.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/flash5_reg.mgz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.722920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/initxfm.fslmat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/invol.fsl_rigid_register.nii
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/outvol.fsl_rigid_register.fslmat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/outvol.fsl_rigid_register.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/refvol.fsl_rigid_register.nii
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.722920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/initxfm.fslmat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/invol.fsl_rigid_register.nii
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/outvol.fsl_rigid_register.fslmat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/outvol.fsl_rigid_register.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/refvol.fsl_rigid_register.nii
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.722920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/initxfm.fslmat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/invol.fsl_rigid_register.nii
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/outvol.fsl_rigid_register.fslmat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/outvol.fsl_rigid_register.nii
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/outvol.fsl_rigid_register.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/refvol.fsl_rigid_register.nii
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.722920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/initxfm.fslmat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/invol.fsl_rigid_register.nii
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/outvol.fsl_rigid_register.fslmat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/outvol.fsl_rigid_register.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/refvol.fsl_rigid_register.nii
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/lh.ribbon.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/mri_nu_correct.mni.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/mri_nu_correct.mni.log.bak
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/norm.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/nu.mgz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.722920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/orig/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/orig/001.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/orig.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/orig_nu.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/rawavg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/rh.ribbon.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/ribbon.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/segment.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/talairach.label_intensities.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/talairach.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/talairach_with_skull.log
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.722920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/cc_up.lta
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach.auto.xfm
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach.auto.xfm.lta
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach.lta
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach.m3z
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach.xfm
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach_avi.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach_avi_QA.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach_with_skull.lta
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talsrcimg_to_3T18yoSchwartzReactN32_as_orig_t4_vox2vox.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/wm.asegedit.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/wm.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/wm.seg.mgz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/wmparc.mgz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.722920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/build-stamp.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/lastcall.build-stamp.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/patchdir.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/pctsurfcon.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/pctsurfcon.log.old
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/ponscc.cut.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/recon-all-status.log
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/recon-all.cmd
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/recon-all.done
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/recon-all.env
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/recon-all.log
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.726920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/aseg.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.BA_exvivo.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.BA_exvivo.thresh.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.aparc.DKTatlas.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.aparc.a2009s.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.aparc.pial.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.aparc.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.curv.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.w-g.pct.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.BA_exvivo.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.BA_exvivo.thresh.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.aparc.DKTatlas.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.aparc.a2009s.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.aparc.pial.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.aparc.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.curv.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.w-g.pct.stats
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/wmparc.stats
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.730920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.area
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.area.mid
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.area.pial
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.avg_curv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.curv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.curv.pial
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.defect_borders
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.defect_chull
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.defect_labels
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.inflated
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.inflated.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.inflated.K
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.inflated.nofix
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.jacobian_white
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.orig
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.orig.nofix
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.pial
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.qsphere.nofix
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.BE.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.C.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.FI.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.H.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.K.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.K1.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.K2.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.S.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.nofix
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.sphere
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.sphere.reg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.sulc
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.thickness
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.volume
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.w-g.pct.mgh
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white.K
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white.preaparc
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white.preaparc.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white.preaparc.K
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.area
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.area.mid
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.area.pial
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.avg_curv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.curv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.curv.pial
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.defect_borders
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.defect_chull
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.defect_labels
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.inflated
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.inflated.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.inflated.K
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.inflated.nofix
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.jacobian_white
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.orig
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.orig.nofix
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.pial
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.qsphere.nofix
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.BE.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.C.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.FI.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.H.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.K.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.K1.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.K2.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.S.crv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.nofix
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.sphere
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.sphere.reg
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.sulc
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.thickness
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.volume
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.w-g.pct.mgh
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white.K
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white.preaparc
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white.preaparc.H
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white.preaparc.K
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/aparc.DKTatlas2aseg.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/aparc.a2009s2aseg.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/apas2aseg.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/asegmerge.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/ca_label.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/ca_normalize.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/ca_register.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/conform.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/cortical_ribbon.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/em_register.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/fill.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/inorm1.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/inorm2.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.aparc.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.aparc2.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.aparcstats.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.aparcstats2.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.aparcstats3.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.avgcurv.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.curvstats.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.final_surfaces.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.inflate.H.K.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.inflate1.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.inflate2.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.jacobian_white.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.pctsurfcon.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.pial_surface.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.qsphere.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.smoothwm1.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.smoothwm2.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.sphmorph.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.sphreg.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.surfvolume.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.tessellate.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.topofix.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.white.H.K.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.white_surface.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/nu.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/relabelhypos.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.aparc.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.aparc2.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.aparcstats.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.aparcstats2.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.aparcstats3.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.avgcurv.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.curvstats.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.final_surfaces.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.inflate.H.K.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.inflate1.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.inflate2.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.jacobian_white.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.pctsurfcon.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.pial_surface.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.qsphere.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.smoothwm1.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.smoothwm2.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.sphmorph.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.sphreg.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.surfvolume.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.tessellate.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.topofix.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.white.H.K.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.white_surface.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mri_ca_register.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mri_em_register.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mri_em_register.skull.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mri_watershed.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_fix_topology.lh.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_fix_topology.rh.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_inflate.lh.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_inflate.rh.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_register.lh.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_register.rh.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_sphere.lh.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_sphere.rh.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/segstats.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/skull.lta.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/skull_strip.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/talairach.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/wmaparc.stats.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/wmaparc.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/wmsegment.touch
--rw-rw-r--   0 chris     (1000) chris     (1000)      553 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/participants.json
--rw-rw-r--   0 chris     (1000) chris     (1000)       75 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/participants.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/
--rw-rw-r--   0 chris     (1000) chris     (1000)      414 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/sub-01_FLASH.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/sub-01_FLASH.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)      413 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/sub-01_T1w.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/sub-01_T1w.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)      414 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/sub-01_THISSUFFIXISNOTVALID.json
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/
--rw-rw-r--   0 chris     (1000) chris     (1000)    40098 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_acq-calibration_meg.dat
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_acq-crosstalk_meg.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)     1160 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_coordsystem.json
--rw-rw-r--   0 chris     (1000) chris     (1000)    39420 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)    13969 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_meg.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)      560 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_meg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)       91 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/sub-01_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.622920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/
--rw-rw-r--   0 chris     (1000) chris     (1000)    33325 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/sub-emptyroom_ses-19210819_task-noise_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/sub-emptyroom_ses-19210819_task-noise_meg.fif
--rw-rw-r--   0 chris     (1000) chris     (1000)      553 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/sub-emptyroom_ses-19210819_task-noise_meg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)       98 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/sub-emptyroom_ses-19210819_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/README
--rw-rw-r--   0 chris     (1000) chris     (1000)      258 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/dataset_description.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      247 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/participants.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      400 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/participants.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      441 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1186 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/sub-cbm001_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      933 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/sub-cbm002_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      441 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      967 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/sub-cbm003_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      984 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/sub-cbm004_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.734920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      984 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/sub-cbm005_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1584 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/sub-cbm006_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1464 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/sub-cbm007_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1074 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/sub-cbm008_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      469 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1370 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/sub-cbm009_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      441 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      975 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/sub-cbm010_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      441 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      962 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/sub-cbm011_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      876 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/sub-cbm012_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1250 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/sub-cbm013_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1096 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/sub-cbm014_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1468 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/sub-cbm015_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1155 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/sub-cbm016_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     2094 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/sub-cbm017_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1060 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/sub-cbm018_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      441 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1027 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/sub-cbm019_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1990 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_channels.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_eeg.edf
--rw-rw-r--   0 chris     (1000) chris     (1000)      442 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_eeg.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     1064 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_events.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/sub-cbm020_scans.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/
--rw-rw-r--   0 chris     (1000) chris     (1000)       90 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/dataset_description.json
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/
--rw-rw-r--   0 chris     (1000) chris     (1000)       73 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T1w.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T1w.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)       73 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T2w.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T2w.nii.gz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.738921 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_magnitude1.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_magnitude2.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)       95 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_phasediff.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_phasediff.nii.gz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/
--rw-rw-r--   0 chris     (1000) chris     (1000)      210 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/README
--rw-rw-r--   0 chris     (1000) chris     (1000)      157 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/dataset_description.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      651 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.json
--rw-rw-r--   0 chris     (1000) chris     (1000)       98 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)      330 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/samples.json
--rw-rw-r--   0 chris     (1000) chris     (1000)       60 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/samples.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/
--rw-rw-r--   0 chris     (1000) chris     (1000)      373 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SEM.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SEM.png
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/0/
--rw-rw-r--   0 chris     (1000) chris     (1000)      128 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/0/0
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/
--rw-rw-r--   0 chris     (1000) chris     (1000)      373 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/sub-01_ses-02_sample-A_SEM.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/sub-01_ses-02_sample-A_SEM.png
--rw-rw-r--   0 chris     (1000) chris     (1000)      156 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/sub-01_sessions.json
--rw-rw-r--   0 chris     (1000) chris     (1000)       74 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/sub-01_sessions.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/
--rw-rw-r--   0 chris     (1000) chris     (1000)      616 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/README
--rw-rw-r--   0 chris     (1000) chris     (1000)      158 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/dataset_description.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      388 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/participants.json
--rw-rw-r--   0 chris     (1000) chris     (1000)       54 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/participants.tsv
--rw-rw-r--   0 chris     (1000) chris     (1000)      330 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/samples.json
--rw-rw-r--   0 chris     (1000) chris     (1000)       83 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/samples.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/
--rw-rw-r--   0 chris     (1000) chris     (1000)      387 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_photo.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_photo.png
--rw-rw-r--   0 chris     (1000) chris     (1000)      635 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     2668 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.ome.tif
--rw-rw-r--   0 chris     (1000) chris     (1000)      637 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     2668 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.ome.tif
--rw-rw-r--   0 chris     (1000) chris     (1000)      636 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     2668 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.ome.tif
--rw-rw-r--   0 chris     (1000) chris     (1000)      635 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     2668 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.ome.tif
--rw-rw-r--   0 chris     (1000) chris     (1000)      387 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_photo.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_photo.png
--rw-rw-r--   0 chris     (1000) chris     (1000)      635 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     2668 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.ome.tif
--rw-rw-r--   0 chris     (1000) chris     (1000)      637 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     2668 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.ome.tif
--rw-rw-r--   0 chris     (1000) chris     (1000)      635 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     2668 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.ome.tif
--rw-rw-r--   0 chris     (1000) chris     (1000)      635 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.json
--rw-rw-r--   0 chris     (1000) chris     (1000)     2668 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.ome.tif
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/
--rwxrwxr-x   0 chris     (1000) chris     (1000)      390 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/README
--rw-rw-r--   0 chris     (1000) chris     (1000)      552 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/dataset_description.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      156 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/participants.json
--rw-rw-r--   0 chris     (1000) chris     (1000)       28 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/participants.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/anat/
--rwxrwxr-x   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/
--rwxrwxr-x   0 chris     (1000) chris     (1000)     1804 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.json
--rwxrwxr-x   0 chris     (1000) chris     (1000)   112710 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz
--rwxrwxr-x   0 chris     (1000) chris     (1000)      774 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json
--rwxrwxr-x   0 chris     (1000) chris     (1000)      771 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/README
--rw-rw-r--   0 chris     (1000) chris     (1000)      255 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/dataset_description.json
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/
--rw-rw-r--   0 chris     (1000) chris     (1000)      275 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-anat_TB1TFL.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-anat_TB1TFL.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)      275 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-famp_TB1TFL.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-famp_TB1TFL.nii.gz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/README
--rw-rw-r--   0 chris     (1000) chris     (1000)      163 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/VFA.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      532 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/dataset_description.json
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/README
--rw-rw-r--   0 chris     (1000) chris     (1000)      346 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/dataset_description.json
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/
--rw-rw-r--   0 chris     (1000) chris     (1000)      602 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)      602 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.nii.gz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.742920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/
--rw-rw-r--   0 chris     (1000) chris     (1000)      657 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.nii.gz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.746920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/
--rw-rw-r--   0 chris     (1000) chris     (1000)       53 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-1_VFA.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-1_VFA.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)       54 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-2_VFA.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-2_VFA.nii.gz
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.746920 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/
--rw-rw-r--   0 chris     (1000) chris     (1000)      432 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr1_TB1AFI.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr1_TB1AFI.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)      430 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr2_TB1AFI.json
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr2_TB1AFI.nii.gz
--rw-rw-r--   0 chris     (1000) chris     (1000)      784 2023-05-18 19:49:11.000000 bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/run_tests.sh
--rw-rw-r--   0 chris     (1000) chris     (1000)      487 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/data/broken_dataset_description.json
--rw-rw-r--   0 chris     (1000) chris     (1000)      710 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/data/expected_bids_validator_xs_write.log
--rw-rw-r--   0 chris     (1000) chris     (1000)     2652 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/test_expressions.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1778 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/test_make_testdata.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5353 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/test_render_tables.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4838 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/test_render_text.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1100 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/test_render_utils.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3431 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/test_rules.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10543 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/test_schema.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8864 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/tests/test_validator.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.746920 bidsschematools-0.7.0/bidsschematools/types/
--rw-rw-r--   0 chris     (1000) chris     (1000)       33 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/types/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7439 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/types/namespace.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1208 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/bidsschematools/utils.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    24956 2023-05-11 19:35:39.000000 bidsschematools-0.7.0/bidsschematools/validator.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 19:49:22.626920 bidsschematools-0.7.0/bidsschematools.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1709 2023-05-18 19:49:22.000000 bidsschematools-0.7.0/bidsschematools.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)   164567 2023-05-18 19:49:22.000000 bidsschematools-0.7.0/bidsschematools.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:22.000000 bidsschematools-0.7.0/bidsschematools.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       53 2023-05-18 19:49:22.000000 bidsschematools-0.7.0/bidsschematools.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 19:49:22.000000 bidsschematools-0.7.0/bidsschematools.egg-info/not-zip-safe
--rw-rw-r--   0 chris     (1000) chris     (1000)      400 2023-05-18 19:49:22.000000 bidsschematools-0.7.0/bidsschematools.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       16 2023-05-18 19:49:22.000000 bidsschematools-0.7.0/bidsschematools.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      614 2023-03-16 13:21:32.000000 bidsschematools-0.7.0/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1602 2023-05-18 19:49:22.746920 bidsschematools-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.477204 bidsschematools-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-24 20:38:03.477204 bidsschematools-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.253205 bidsschematools-0.7.1/bidsschematools/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.253205 bidsschematools-0.7.1/bidsschematools/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.253205 bidsschematools-0.7.1/bidsschematools/data/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/BIDS_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/SCHEMA_VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.253205 bidsschematools-0.7.1/bidsschematools/data/schema/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/meta/context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/meta/expression_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/meta/versions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.257205 bidsschematools-0.7.1/bidsschematools/data/schema/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)    25092 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/objects/columns.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/objects/common_principles.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/objects/datatypes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17197 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/objects/entities.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/objects/extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/objects/files.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/objects/formats.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   124075 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/objects/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/objects/modalities.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    28199 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/objects/suffixes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.257205 bidsschematools-0.7.1/bidsschematools/data/schema/rules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.257205 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/anat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/asl.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/common_derivatives.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/dataset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/dwi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/events.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/fmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/func.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/hints.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/micr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/mri.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/nifti.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/nirs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/privacy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/references.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/common_principles.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/dataset_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/entities.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/errors.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.241206 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.257205 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/common/core.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/common/tables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.257205 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/deriv/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/deriv/imaging.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/deriv/preprocessed_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.261205 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/anat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/beh.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/channels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/dwi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/eeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/fmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/func.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/ieeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/meg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/micr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/motion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/nirs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/perf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/pet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/photo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/task.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/modalities.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.261205 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/anat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/asl.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/beh.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/continuous.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.261205 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/derivatives/common_derivatives.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/dwi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/eeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/entity_rules.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/events.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/fmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/func.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/ieeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/meg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/micr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/motion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/mri.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/nirs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/pet.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.265205 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.265205 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/derivatives/common_derivatives.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/eeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/ieeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/meg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/modality_agnostic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/motion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/nirs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/perf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/pet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/physio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/task.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.265205 bidsschematools-0.7.1/bidsschematools/render/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20849 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/render/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18185 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/render/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/render/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.265205 bidsschematools-0.7.1/bidsschematools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.265205 bidsschematools-0.7.1/bidsschematools/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.265205 bidsschematools-0.7.1/bidsschematools/tests/data/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-24 20:37:54.000000 bidsschematools-0.7.1/bidsschematools/tests/data/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.265205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.265205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/README
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.241206 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.265205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/sub-Sub1_T1w.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/sub-Sub1_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.269205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_aslcontext.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   411101 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   411101 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_headshape.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.269205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/README
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/participants.json
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/participants.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.241206 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.241206 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.269205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   118231 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1190 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-02_ses-01_T1w.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.269205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1941 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.json
+-rw-r--r--   0 runner    (1001) docker     (123)    84350 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)      413 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.tsv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1061 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-24 20:37:56.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.269205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25620 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.273205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/README
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.245205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.273205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/sub-Sub1_T1w.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/sub-Sub1_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.273205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_aslcontext.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   411101 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/bidsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.273205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/.bidsignore
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/README
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/acq-epi_T1w.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.245205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.245205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.245205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.245205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.277205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/brain.surf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-5120-5120-5120-bem-sol.fif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-5120-5120-5120-bem.fif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-fiducials.fif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-head-dense.fif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-head-medium.fif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-head.fif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-ico-5-src.fif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-inner_skull-bem.fif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-trans.fif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/fsaverage-vol-5-src.fif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/inner_skull.surf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/outer_skin.surf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/outer_skull.surf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.293205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/Yeo_Brainmap_fsaverage_README
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA1.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA1_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA1_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA2.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA2_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA2_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3a.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3a_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3a_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3b.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3b_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA3b_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA44.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA44_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA44_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA45.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA45_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA45_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4a.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4a_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4a_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4p.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4p_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA4p_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA6.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA6_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.BA6_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.HCPMMP1.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.HCPMMP1_combined.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.MT.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.MT_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.MT_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Medial_wall.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.PALS_B12.labels.gii
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.PALS_B12_Brodmann.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.PALS_B12_Lobes.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.PALS_B12_OrbitoFrontal.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.PALS_B12_Visuotopic.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V1.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V1_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V1_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V2.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V2_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.V2_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo2011_17NetworksConfidence_N1000.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo2011_17Networks_N1000.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo2011_7NetworksConfidence_N1000.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo2011_7Networks_N1000.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_10Comp_PrActGivenComp.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_10to14Comp_Flexibility.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_10to14Comp_Specialization.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_10to14Comp_SpecializationROI.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_10to14Comp_TopSpecializationComp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_11Comp_PrActGivenComp.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_12Comp_PrActGivenComp.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_13Comp_PrActGivenComp.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.Yeo_Brainmap_14Comp_PrActGivenComp.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.aparc.a2005s.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.aparc.a2009s.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.aparc.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.aparc.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.aparc_sub.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.cortex.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.entorhinal.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.entorhinal_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.entorhinal_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.ifc.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.ipc.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.ips.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.lateraltemporal.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.medialpfc.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.mtl.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.retrosplenial.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.oasis.chubs.tp.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.perirhinal_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/lh.perirhinal_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA1.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA1_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA1_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA2.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA2_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA2_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3a.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3a_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3a_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3b.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3b_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA3b_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA44.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA44_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA44_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA45.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA45_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA45_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4a.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4a_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4a_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4p.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4p_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA4p_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA6.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA6_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.BA6_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.HCPMMP1.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.HCPMMP1_combined.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.MT.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.MT_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.MT_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Medial_wall.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.PALS_B12.labels.gii
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.PALS_B12_Brodmann.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.PALS_B12_Lobes.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.PALS_B12_OrbitoFrontal.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.PALS_B12_Visuotopic.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V1.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V1_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V1_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V2.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V2_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.V2_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo2011_17NetworksConfidence_N1000.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo2011_17Networks_N1000.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo2011_7NetworksConfidence_N1000.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo2011_7Networks_N1000.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_10Comp_PrActGivenComp.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_10to14Comp_Flexibility.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_10to14Comp_Specialization.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_10to14Comp_SpecializationROI.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_10to14Comp_TopSpecializationComp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_11Comp_PrActGivenComp.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_12Comp_PrActGivenComp.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_13Comp_PrActGivenComp.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.Yeo_Brainmap_14Comp_PrActGivenComp.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.aparc.a2005s.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.aparc.a2009s.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.aparc.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.aparc.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.aparc_sub.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.cortex.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.entorhinal.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.entorhinal_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.entorhinal_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.ifc.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.ipc.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.ips.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.lateraltemporal.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.medialpfc.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.mtl.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.retrosplenial.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.oasis.chubs.tp.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.perirhinal_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/label/rh.perirhinal_exvivo.thresh.label
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.297205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/T1.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/aparc+aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/aparc.a2005s+aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/aparc.a2009s+aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/brain.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/brainmask.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/lh.ribbon.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/mni305.cor.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/orig.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/p.aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/rh.ribbon.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/ribbon.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/seghead.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/subcort.mask.1mm.README
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/subcort.mask.1mm.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/subcort.prob.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/subcort.prob.mgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.297205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/transforms/reg.mni152.2mm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri/transforms/talairach.xfm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.297205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/README
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/T1.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/brain.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/brainmask.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/mni305.cor.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/orig.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/reg.2mm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/reg.2mm.mni152.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/subcort.mask.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/mri.2mm/subcort.prob.mgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.301205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/build-stamp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/csurfdir
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/cvs_log_pre_31May2011.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/make_average_surface.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/make_average_volume.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/mkheadsurf.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/mris_inflate.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/mris_inflate_lh.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/mris_inflate_rh.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all-status.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.done
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.env
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.env.bak
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.local-copy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/recon-all.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/surfreg.fsaverage_sym.lh.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/scripts/surfreg.fsaverage_sym.rh.log
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.309205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.area
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.area.seghead
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.avg_curv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.avg_sulc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.avg_thickness
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.cortex.patch.3d
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.cortex.patch.flat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.curv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.curv.seghead
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.fsaverage_sym.sphere.reg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.inflated
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.inflated.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.inflated.K
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.inflated_avg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.inflated_pre
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.orig
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.orig.avg.area.mgh
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.orig_avg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.pial
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.pial.avg.area.mgh
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.pial_avg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.pial_semi_inflated
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.seghead
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.seghead.inflated
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.smoothwm
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sphere
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sphere.left_right
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sphere.reg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sphere.reg.avg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sulc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.sulc.seghead
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.thickness
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.white
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.white.avg.area.mgh
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.white_avg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.white_avg.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/lh.white_avg.K
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/mris_preproc.surface.lh.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/mris_preproc.surface.rh.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.area
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.avg_curv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.avg_sulc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.avg_thickness
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.cortex.patch.3d
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.cortex.patch.flat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.curv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.fsaverage_sym.sphere.reg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.inflated
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.inflated.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.inflated.K
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.inflated_avg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.inflated_pre
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.orig
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.orig.avg.area.mgh
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.orig_avg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.pial
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.pial.avg.area.mgh
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.pial_avg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.pial_semi_inflated
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.smoothwm
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.sphere
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.sphere.left_right
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.sphere.reg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.sphere.reg.avg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.sulc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.thickness
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.white
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.white.avg.area.mgh
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.white_avg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.white_avg.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/surf/rh.white_avg.K
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.309205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.309205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/lh.aparc.a2009s.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/lh.aparc.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/lh.cortex.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/rh.aparc.a2009s.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/rh.aparc.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/label/rh.cortex.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/lrrev.pure.register.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/lrrev.register.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.309205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/T1.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/aparc+aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/brain.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/brainmask.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/mri_nu_correct.mni.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/orig.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/orig_nu.mgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.309205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/transforms/talairach.auto.xfm
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/transforms/talairach.xfm
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/transforms/talairach_avi.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/mri/transforms/talsrcimg_to_711-2C_as_mni_average_305_t4_vox2vox.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.309205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/build-stamp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/lastcall.build-stamp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/patchdir.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all-status.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all.done
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all.env
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all.local-copy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/recon-all.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/surfreg.fsaverage_sym.lh.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/scripts/surfreg.fsaverage_sym.rh.log
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.313205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.area
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.curv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.fsaverage_sym.sphere.reg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.inflated
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.inflated.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.inflated.K
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.orig
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.pial
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.smoothwm
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.sphere
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.sulc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.thickness
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/lh.white
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.area
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.curv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.fsaverage_sym.sphere.reg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.inflated
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.inflated.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.inflated.K
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.orig
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.pial
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.smoothwm
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.sphere
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.sulc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.thickness
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/surf/rh.white
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.313205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/touch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/touch/talairach.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/xhemireg.lh.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/xhemi/xhemireg.rh.log
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.313205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/morph-maps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/morph-maps/fsaverage-sub-01-morph.fif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.245205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.313205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.317205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/inner_skull.surf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/inner_skull.tri
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/outer_skin.surf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/outer_skin.tri
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/outer_skull.surf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/flash/outer_skull.tri
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/inner_skull.surf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/outer_skin.surf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/bem/outer_skull.surf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.325205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/BA_exvivo.ctab
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/BA_exvivo.thresh.ctab
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/aparc.annot.DKTatlas.ctab
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/aparc.annot.a2009s.ctab
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/aparc.annot.ctab
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA1_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA1_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA2_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA2_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA3a_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA3a_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA3b_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA3b_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA44_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA44_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA45_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA45_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA4a_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA4a_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA4p_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA4p_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA6_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA6_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA_exvivo.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.BA_exvivo.thresh.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.MT_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.MT_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.V1_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.V1_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.V2_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.V2_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.aparc.DKTatlas.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.aparc.a2009s.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.aparc.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.cortex.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.entorhinal_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.entorhinal_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.perirhinal_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/lh.perirhinal_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA1_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA1_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA2_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA2_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA3a_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA3a_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA3b_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA3b_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA44_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA44_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA45_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA45_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA4a_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA4a_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA4p_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA4p_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA6_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA6_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA_exvivo.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.BA_exvivo.thresh.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.MT_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.MT_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.V1_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.V1_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.V2_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.V2_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.aparc.DKTatlas.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.aparc.a2009s.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.aparc.annot
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.cortex.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.entorhinal_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.entorhinal_exvivo.thresh.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.perirhinal_exvivo.label
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/label/rh.perirhinal_exvivo.thresh.label
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.329205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.357205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-.info
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-001
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-002
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-003
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-004
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-005
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-006
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-007
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-008
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-009
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-010
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-011
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-012
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-013
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-014
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-015
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-016
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-017
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-018
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-019
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-020
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-021
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-022
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-023
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-024
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-025
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-026
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-027
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-028
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-029
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-030
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-031
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-032
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-033
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-034
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-035
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-036
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-037
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-038
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-039
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-040
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-041
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-042
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-043
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-044
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-045
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-046
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-047
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-048
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-049
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-050
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-051
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-052
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-053
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-054
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-055
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-056
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-057
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-058
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-059
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-060
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-061
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-062
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-063
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-064
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-065
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-066
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-067
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-068
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-069
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-070
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-071
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-072
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-073
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-074
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-075
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-076
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-077
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-078
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-079
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-080
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-081
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-082
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-083
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-084
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-085
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-086
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-087
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-088
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-089
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-090
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-091
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-092
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-093
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-094
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-095
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-096
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-097
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-098
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-099
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-100
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-101
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-102
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-103
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-104
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-105
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-106
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-107
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-108
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-109
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-110
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-111
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-112
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-113
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-114
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-115
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-116
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-117
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-118
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-119
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-120
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-121
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-122
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-123
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-124
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-125
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-126
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-127
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-128
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-129
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-130
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-131
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-132
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-133
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-134
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-135
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-136
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-137
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-138
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-139
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-140
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-141
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-142
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-143
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-144
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-145
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-146
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-147
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-148
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-149
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-150
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-151
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-152
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-153
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-154
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-155
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-156
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-157
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-158
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-159
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-160
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-161
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-162
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-163
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-164
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-165
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-166
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-167
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-168
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-169
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-170
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-171
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-172
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-173
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-174
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-175
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-176
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-177
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-178
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-179
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-180
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-181
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-182
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-183
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-184
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-185
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-186
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-187
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-188
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-189
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-190
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-191
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-192
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-193
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-194
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-195
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-196
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-197
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-198
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-199
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-200
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-201
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-202
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-203
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-204
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-205
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-206
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-207
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-208
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-209
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-210
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-211
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-212
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-213
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-214
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-215
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-216
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-217
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-218
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-219
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-220
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-221
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-222
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-223
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-224
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-225
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-226
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-227
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-228
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-229
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-230
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-231
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-232
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-233
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-234
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-235
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-236
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-237
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-238
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-239
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-240
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-241
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-242
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-243
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-244
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-245
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-246
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-247
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-248
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-249
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-250
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-251
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-252
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-253
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-254
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-255
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1/COR-256
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/T1.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aparc+aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aparc.DKTatlas+aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aparc.a2009s+aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.auto.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.auto_noCCseg.label_intensities.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.auto_noCCseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.presurf.hypos.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/aseg.presurf.mgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.385205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-.info
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-001
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-002
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-003
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-004
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-005
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-006
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-007
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-008
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-009
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-010
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-011
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-012
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-013
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-014
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-015
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-016
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-017
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-018
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-019
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-020
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-021
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-022
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-023
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-024
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-025
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-026
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-027
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-028
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-029
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-030
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-031
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-032
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-033
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-034
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-035
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-036
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-037
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-038
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-039
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-040
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-041
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-042
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-043
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-044
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-045
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-046
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-047
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-048
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-049
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-050
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-051
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-052
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-053
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-054
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-055
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-056
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-057
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-058
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-059
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-060
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-061
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-062
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-063
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-064
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-065
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-066
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-067
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-068
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-069
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-070
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-071
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-072
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-073
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-074
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-075
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-076
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-077
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-078
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-079
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-080
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-081
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-082
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-083
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-084
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-085
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-086
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-087
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-088
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-089
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-090
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-091
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-092
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-093
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-094
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-095
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-096
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-097
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-098
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-099
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-100
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-101
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-102
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-103
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-104
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-105
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-106
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-107
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-108
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-109
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-110
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-111
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-112
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-113
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-114
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-115
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-116
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-117
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-118
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-119
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-120
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-121
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-122
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-123
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-124
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-125
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-126
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-127
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-128
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-129
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-130
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-131
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-132
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-133
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-134
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-135
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-136
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-137
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-138
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-139
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-140
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-141
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-142
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-143
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-144
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-145
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-146
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-147
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-148
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-149
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-150
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-151
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-152
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-153
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-154
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-155
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-156
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-157
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-158
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-159
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-160
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-161
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-162
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-163
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-164
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-165
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-166
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-167
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-168
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-169
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-170
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-171
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-172
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-173
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-174
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-175
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-176
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-177
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-178
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-179
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-180
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-181
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-182
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-183
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-184
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-185
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-186
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-187
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-188
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-189
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-190
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-191
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-192
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-193
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-194
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-195
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-196
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-197
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-198
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-199
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-200
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-201
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-202
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-203
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-204
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-205
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-206
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-207
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-208
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-209
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-210
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-211
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-212
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-213
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-214
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-215
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-216
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-217
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-218
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-219
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-220
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-221
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-222
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-223
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-224
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-225
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-226
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-227
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-228
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-229
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-230
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-231
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-232
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-233
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-234
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-235
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-236
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-237
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-238
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-239
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-240
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-241
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-242
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-243
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-244
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-245
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-246
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-247
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-248
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-249
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-250
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-251
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-252
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-253
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-254
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-255
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain/COR-256
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain.finalsurfs.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brain.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brainmask.auto.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/brainmask.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/ctrl_pts.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/filled.mgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.385205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/mef05.mgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.385205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/flash5.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/flash5_reg.mgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.385205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/initxfm.fslmat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/invol.fsl_rigid_register.nii
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/outvol.fsl_rigid_register.fslmat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/outvol.fsl_rigid_register.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.10366/refvol.fsl_rigid_register.nii
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.389205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/initxfm.fslmat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/invol.fsl_rigid_register.nii
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/outvol.fsl_rigid_register.fslmat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/outvol.fsl_rigid_register.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.14439/refvol.fsl_rigid_register.nii
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.389205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/initxfm.fslmat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/invol.fsl_rigid_register.nii
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/outvol.fsl_rigid_register.fslmat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/outvol.fsl_rigid_register.nii
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/outvol.fsl_rigid_register.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.15197/refvol.fsl_rigid_register.nii
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.389205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/initxfm.fslmat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/invol.fsl_rigid_register.nii
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/outvol.fsl_rigid_register.fslmat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/outvol.fsl_rigid_register.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/flash/parameter_maps/fsl_rigid_register.9149/refvol.fsl_rigid_register.nii
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/lh.ribbon.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/mri_nu_correct.mni.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/mri_nu_correct.mni.log.bak
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/norm.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/nu.mgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.389205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/orig/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/orig/001.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/orig.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/orig_nu.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/rawavg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/rh.ribbon.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/ribbon.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/segment.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/talairach.label_intensities.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/talairach.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/talairach_with_skull.log
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.389205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/cc_up.lta
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach.auto.xfm
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach.auto.xfm.lta
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach.lta
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach.m3z
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach.xfm
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach_avi.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach_avi_QA.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talairach_with_skull.lta
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/transforms/talsrcimg_to_3T18yoSchwartzReactN32_as_orig_t4_vox2vox.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/wm.asegedit.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/wm.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/wm.seg.mgz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/mri/wmparc.mgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.389205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/build-stamp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/lastcall.build-stamp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/patchdir.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/pctsurfcon.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/pctsurfcon.log.old
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/ponscc.cut.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/recon-all-status.log
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/recon-all.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/recon-all.done
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/recon-all.env
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/scripts/recon-all.log
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.393205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/aseg.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.BA_exvivo.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.BA_exvivo.thresh.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.aparc.DKTatlas.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.aparc.a2009s.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.aparc.pial.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.aparc.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.curv.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/lh.w-g.pct.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.BA_exvivo.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.BA_exvivo.thresh.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.aparc.DKTatlas.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.aparc.a2009s.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.aparc.pial.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.aparc.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.curv.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/rh.w-g.pct.stats
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/stats/wmparc.stats
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.401205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.area
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.area.mid
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.area.pial
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.avg_curv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.curv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.curv.pial
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.defect_borders
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.defect_chull
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.defect_labels
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.inflated
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.inflated.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.inflated.K
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.inflated.nofix
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.jacobian_white
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.orig
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.orig.nofix
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.pial
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.qsphere.nofix
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.BE.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.C.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.FI.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.H.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.K.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.K1.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.K2.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.S.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.smoothwm.nofix
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.sphere
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.sphere.reg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.sulc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.thickness
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.volume
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.w-g.pct.mgh
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white.K
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white.preaparc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white.preaparc.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/lh.white.preaparc.K
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.area
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.area.mid
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.area.pial
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.avg_curv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.curv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.curv.pial
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.defect_borders
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.defect_chull
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.defect_labels
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.inflated
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.inflated.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.inflated.K
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.inflated.nofix
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.jacobian_white
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.orig
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.orig.nofix
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.pial
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.qsphere.nofix
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.BE.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.C.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.FI.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.H.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.K.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.K1.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.K2.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.S.crv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.smoothwm.nofix
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.sphere
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.sphere.reg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.sulc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.thickness
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.volume
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.w-g.pct.mgh
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white.K
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white.preaparc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white.preaparc.H
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/surf/rh.white.preaparc.K
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.409205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/aparc.DKTatlas2aseg.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/aparc.a2009s2aseg.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/apas2aseg.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/asegmerge.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/ca_label.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/ca_normalize.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/ca_register.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/conform.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/cortical_ribbon.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/em_register.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/fill.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/inorm1.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/inorm2.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.aparc.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.aparc2.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.aparcstats.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.aparcstats2.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.aparcstats3.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.avgcurv.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.curvstats.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.final_surfaces.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.inflate.H.K.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.inflate1.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.inflate2.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.jacobian_white.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.pctsurfcon.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.pial_surface.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.qsphere.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.smoothwm1.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.smoothwm2.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.sphmorph.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.sphreg.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.surfvolume.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.tessellate.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.topofix.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.white.H.K.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/lh.white_surface.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/nu.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/relabelhypos.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.aparc.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.aparc2.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.aparcstats.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.aparcstats2.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.aparcstats3.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.avgcurv.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.curvstats.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.final_surfaces.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.inflate.H.K.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.inflate1.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.inflate2.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.jacobian_white.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.pctsurfcon.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.pial_surface.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.qsphere.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.smoothwm1.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.smoothwm2.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.sphmorph.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.sphreg.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.surfvolume.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.tessellate.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.topofix.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.white.H.K.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rh.white_surface.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mri_ca_register.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mri_em_register.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mri_em_register.skull.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mri_watershed.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_fix_topology.lh.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_fix_topology.rh.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_inflate.lh.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_inflate.rh.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_register.lh.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_register.rh.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_sphere.lh.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/rusage.mris_sphere.rh.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/segstats.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/skull.lta.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/skull_strip.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/talairach.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/wmaparc.stats.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/wmaparc.touch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/sub-01/touch/wmsegment.touch
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/participants.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/participants.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.409205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.409205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/sub-01_FLASH.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/sub-01_FLASH.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/sub-01_T1w.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/sub-01_T1w.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/anat/sub-01_THISSUFFIXISNOTVALID.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.409205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/
+-rw-r--r--   0 runner    (1001) docker     (123)    40098 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_acq-calibration_meg.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_acq-crosstalk_meg.fif
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_coordsystem.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39420 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_meg.fif
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_meg.json
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/sub-01_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.245205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.409205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.409205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/
+-rw-r--r--   0 runner    (1001) docker     (123)    33325 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/sub-emptyroom_ses-19210819_task-noise_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/sub-emptyroom_ses-19210819_task-noise_meg.fif
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/sub-emptyroom_ses-19210819_task-noise_meg.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/sub-emptyroom_ses-19210819_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.409205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/README
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/participants.json
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/participants.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.409205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.409205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/sub-cbm001_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.409205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.409205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/sub-cbm002_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/sub-cbm003_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/sub-cbm004_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/sub-cbm005_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/sub-cbm006_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/sub-cbm007_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/sub-cbm008_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/sub-cbm009_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.413205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/sub-cbm010_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.417205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.417205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/sub-cbm011_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.417205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.417205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/sub-cbm012_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.417205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.417205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/sub-cbm013_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.417205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.453204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/sub-cbm014_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.453204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.453204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/sub-cbm015_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.453204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.453204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/sub-cbm016_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.453204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.453204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/sub-cbm017_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.457204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.457204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/sub-cbm018_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.457204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.457204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/sub-cbm019_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.457204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.457204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/sub-cbm020_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.457204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.461205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T1w.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T1w.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T2w.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T2w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.461205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_magnitude1.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_magnitude2.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_phasediff.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_phasediff.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.461205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/README
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/samples.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.461205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.461205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SEM.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SEM.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.465205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/0/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.465205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/sub-01_ses-02_sample-A_SEM.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/sub-01_ses-02_sample-A_SEM.png
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/sub-01_sessions.json
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/sub-01_sessions.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.465205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/README
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/participants.json
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/participants.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/samples.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.473204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_photo.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_photo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_photo.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_photo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.ome.tif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.473204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/README
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/participants.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/participants.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.473204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/anat/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.473204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)   112710 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      771 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.473204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/README
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.473204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-anat_TB1TFL.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-anat_TB1TFL.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-famp_TB1TFL.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-famp_TB1TFL.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.473204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/README
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/VFA.json
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.473204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/README
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.473204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.477204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.249205 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.477204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-1_VFA.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-1_VFA.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-2_VFA.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-2_VFA.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.477204 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr1_TB1AFI.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr1_TB1AFI.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr2_TB1AFI.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr2_TB1AFI.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-24 20:37:55.000000 bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/run_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/data/broken_dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/data/expected_bids_validator_xs_write.log
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/test_make_testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/test_render_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/test_render_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/test_render_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.477204 bidsschematools-0.7.1/bidsschematools/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/types/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24956 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/bidsschematools/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:38:03.253205 bidsschematools-0.7.1/bidsschematools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-24 20:38:03.000000 bidsschematools-0.7.1/bidsschematools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   164629 2023-05-24 20:38:03.000000 bidsschematools-0.7.1/bidsschematools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:38:03.000000 bidsschematools-0.7.1/bidsschematools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 20:38:03.000000 bidsschematools-0.7.1/bidsschematools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:38:02.000000 bidsschematools-0.7.1/bidsschematools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-24 20:38:03.000000 bidsschematools-0.7.1/bidsschematools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 20:38:03.000000 bidsschematools-0.7.1/bidsschematools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-24 20:37:29.000000 bidsschematools-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-24 20:38:03.477204 bidsschematools-0.7.1/setup.cfg
```

### Comparing `bidsschematools-0.7.0/LICENSE` & `bidsschematools-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/PKG-INFO` & `bidsschematools-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: bidsschematools
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python tools for working with the BIDS schema.
 Home-page: https://github.com/bids-standard/bids-specification
 Author: bids-standard developers
 Author-email: bids.maintenance@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: doc
 Provides-Extra: render
 Provides-Extra: expressions
 Provides-Extra: tests
 Provides-Extra: all
```

### Comparing `bidsschematools-0.7.0/README.md` & `bidsschematools-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/__main__.py` & `bidsschematools-0.7.1/bidsschematools/__main__.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/conftest.py` & `bidsschematools-0.7.1/bidsschematools/conftest.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/meta/context.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/meta/context.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/meta/expression_tests.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/meta/expression_tests.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/objects/columns.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/objects/columns.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/objects/common_principles.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/objects/common_principles.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/objects/datatypes.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/objects/datatypes.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/objects/entities.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/objects/entities.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/objects/extensions.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/objects/extensions.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/objects/files.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/objects/files.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     at its root directory.
     BIDS does not make any recommendations with regards to the
     [Markdown flavor](https://www.markdownguide.org/extended-syntax/#lightweight-markup-languages)
     and does not validate the syntax of Markdown and reStructuredText.
     The `README` file SHOULD be structured such that its contents can be easily understood
     even if the used format is not rendered.
     A guideline for creating a good `README` file can be found in the
-    [bids-starter-kit](https://github.com/bids-standard/bids-starter-kit/blob/master/templates/README).
+    [bids-starter-kit](https://github.com/bids-standard/bids-starter-kit/tree/main/templates/).
 dataset_description:
   display_name: Dataset Description
   file_type: regular
   description: |
     The file `dataset_description.json` is a JSON file describing the dataset.
 genetic_info:
   display_name: Genetic Information
```

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/objects/formats.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/objects/formats.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/objects/metadata.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/objects/metadata.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1609,15 +1609,15 @@
   display_name: Labeling Location Description
   description: |
     Description of the location of the labeling plane (`"CASL"` or `"PCASL"`) or
     the labeling slab (`"PASL"`) that cannot be captured by fields
     `LabelingOrientation` or `LabelingDistance`.
     May include a link to an anonymized screenshot of the planning of the
     labeling slab/plane with respect to the imaging slab or slices
-    `*_asllabeling.jpg`.
+    `*_asllabeling.*`.
     Based on DICOM macro C.8.13.5.14.
   type: string
 LabelingOrientation:
   name: LabelingOrientation
   display_name: Labeling Orientation
   description: |
     Orientation of the labeling plane (`(P)CASL`) or slab (`PASL`).
```

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/objects/modalities.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/objects/modalities.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/objects/suffixes.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/objects/suffixes.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -503,17 +503,17 @@
   display_name: Arterial Spin Labeling Context
   description: |
     A TSV file defining the image types for volumes in an associated ASL file.
 asllabeling:
   value: asllabeling
   display_name: ASL Labeling Screenshot
   description: |
-    An anonymized screenshot of the planning of the labeling slab/plane with
-    respect to the imaging slab or slices `*_asllabeling.jpg`.
-    Based on DICOM macro C.8.13.5.14.
+    An anonymized screenshot of the planning of the labeling slab/plane
+    with respect to the imaging slab or slices.
+    This screenshot is based on DICOM macro C.8.13.5.14.
 beh:
   value: beh
   display_name: Behavioral recording
   description: |
     Behavioral recordings from tasks.
     These files are similar to events files, but do not include the `"onset"` and
     `"duration"` columns that are mandatory for events files.
```

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/anat.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/anat.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/asl.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/asl.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/common_derivatives.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/common_derivatives.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/dataset.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/dataset.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/dwi.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/dwi.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/events.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/events.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/fmap.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/fmap.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/func.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/func.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/general.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/general.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/hints.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/hints.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/micr.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/micr.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/mri.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/mri.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/nifti.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/nifti.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/nirs.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/nirs.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/privacy.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/privacy.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/checks/references.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/checks/references.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/dataset_metadata.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/dataset_metadata.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/errors.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/errors.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/common/core.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/common/core.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/common/tables.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/common/tables.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/deriv/imaging.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/deriv/imaging.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/deriv/preprocessed_data.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/deriv/preprocessed_data.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/anat.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/anat.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/channels.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/channels.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/dwi.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/dwi.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/fmap.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/fmap.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/func.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/func.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/meg.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/meg.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/perf.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/perf.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     run: optional
 
 aslcontext:
   suffixes:
     - aslcontext
   extensions:
     - .tsv
-    - .json
   datatypes:
     - perf
   entities:
     subject: required
     session: optional
     acquisition: optional
     reconstruction: optional
@@ -34,14 +33,16 @@
     run: optional
 
 asllabeling:
   suffixes:
     - asllabeling
   extensions:
     - .jpg
+    - .png
+    - .tif
   datatypes:
     - perf
   entities:
     subject: required
     session: optional
     acquisition: optional
     reconstruction: optional
```

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/files/raw/task.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/files/raw/task.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/anat.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/anat.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/asl.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/asl.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/beh.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/beh.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/continuous.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/continuous.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/derivatives/common_derivatives.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/derivatives/common_derivatives.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/eeg.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/eeg.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/entity_rules.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/entity_rules.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/fmap.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/fmap.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/func.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/func.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/ieeg.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/ieeg.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/meg.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/meg.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/micr.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/micr.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/motion.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/motion.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/mri.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/mri.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/nirs.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/nirs.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/sidecars/pet.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/sidecars/pet.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/eeg.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/eeg.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/ieeg.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/ieeg.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/meg.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/meg.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/modality_agnostic.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/modality_agnostic.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/motion.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/motion.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/nirs.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/nirs.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/data/schema/rules/tabular_data/pet.yaml` & `bidsschematools-0.7.1/bidsschematools/data/schema/rules/tabular_data/pet.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/expressions.py` & `bidsschematools-0.7.1/bidsschematools/expressions.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/render/__init__.py` & `bidsschematools-0.7.1/bidsschematools/render/__init__.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/render/tables.py` & `bidsschematools-0.7.1/bidsschematools/render/tables.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/render/text.py` & `bidsschematools-0.7.1/bidsschematools/render/text.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/render/utils.py` & `bidsschematools-0.7.1/bidsschematools/render/utils.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/rules.py` & `bidsschematools-0.7.1/bidsschematools/rules.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/schema.py` & `bidsschematools-0.7.1/bidsschematools/schema.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/CONTRIBUTING.md` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/README.md` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/README.md`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_headshape.jpg` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_headshape.jpg`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/dataset_description.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/dataset_description.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-02_ses-01_T1w.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-02_ses-01_T1w.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/CONTRIBUTING.md` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/README.md` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/README.md`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/README` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/README`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/dataset_description.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/dataset_description.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/participants.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/participants.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_acq-calibration_meg.dat` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_acq-calibration_meg.dat`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_coordsystem.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_coordsystem.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_meg.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-01/meg/sub-01_task-audiovisual_run-01_meg.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/sub-emptyroom_ses-19210819_task-noise_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/sub-emptyroom_ses-19210819_task-noise_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/sub-emptyroom_ses-19210819_task-noise_meg.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/ds000248/sub-emptyroom/ses-19210819/meg/sub-emptyroom_ses-19210819_task-noise_meg.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_channels.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_events.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/README` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/README`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.ome.tif` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.ome.tif` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.ome.tif` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.ome.tif` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.ome.tif` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.ome.tif` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.ome.tif` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.ome.tif` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/dataset_description.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/dataset_description.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/dataset_description.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/dataset_description.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.json` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/bids-examples/run_tests.sh` & `bidsschematools-0.7.1/bidsschematools/tests/data/bids-examples/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/data/expected_bids_validator_xs_write.log` & `bidsschematools-0.7.1/bidsschematools/tests/data/expected_bids_validator_xs_write.log`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/test_expressions.py` & `bidsschematools-0.7.1/bidsschematools/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/test_make_testdata.py` & `bidsschematools-0.7.1/bidsschematools/tests/test_make_testdata.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     -----
     * Due to intricacies arising from:
         (1) fixtures not working outside of pytest
         (2) implicit teardown leveraging tempdata removal (while held open by yield)
         (3) wrappers evaluating the yield statement
         (4) the desire to not download testdata twice for archive creation
         testdata archive creation is now inconspicuously posing as a test.
-    * Archives will be generated under `/tmp/bidsschematools-testdata-SCHEMA_VERSION.tar.gz`
     """
 
     testdata_dir = files("bidsschematools.tests.data")
     ignore_git = shutil.ignore_patterns(".git*")
     shutil.copytree(bids_examples, testdata_dir / "bids-examples", ignore=ignore_git)
     shutil.copytree(bids_error_examples, testdata_dir / "bids-error-examples", ignore=ignore_git)
```

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/test_render_tables.py` & `bidsschematools-0.7.1/bidsschematools/tests/test_render_tables.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/test_render_text.py` & `bidsschematools-0.7.1/bidsschematools/tests/test_render_text.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/test_render_utils.py` & `bidsschematools-0.7.1/bidsschematools/tests/test_render_utils.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/test_rules.py` & `bidsschematools-0.7.1/bidsschematools/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/test_schema.py` & `bidsschematools-0.7.1/bidsschematools/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/tests/test_validator.py` & `bidsschematools-0.7.1/bidsschematools/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/types/namespace.py` & `bidsschematools-0.7.1/bidsschematools/types/namespace.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/utils.py` & `bidsschematools-0.7.1/bidsschematools/utils.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools/validator.py` & `bidsschematools-0.7.1/bidsschematools/validator.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/bidsschematools.egg-info/PKG-INFO` & `bidsschematools-0.7.1/bidsschematools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: bidsschematools
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python tools for working with the BIDS schema.
 Home-page: https://github.com/bids-standard/bids-specification
 Author: bids-standard developers
 Author-email: bids.maintenance@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: doc
 Provides-Extra: render
 Provides-Extra: expressions
 Provides-Extra: tests
 Provides-Extra: all
```

### Comparing `bidsschematools-0.7.0/bidsschematools.egg-info/SOURCES.txt` & `bidsschematools-0.7.1/bidsschematools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 bidsschematools/tests/test_render_utils.py
 bidsschematools/tests/test_rules.py
 bidsschematools/tests/test_schema.py
 bidsschematools/tests/test_validator.py
 bidsschematools/tests/data/__init__.py
 bidsschematools/tests/data/broken_dataset_description.json
 bidsschematools/tests/data/expected_bids_validator_xs_write.log
-bidsschematools/tests/data/__pycache__/__init__.cpython-310.pyc
+bidsschematools/tests/data/__pycache__/__init__.cpython-311.pyc
 bidsschematools/tests/data/bids-error-examples/CONTRIBUTING.md
 bidsschematools/tests/data/bids-error-examples/README.md
 bidsschematools/tests/data/bids-error-examples/invalid_asl003/README
 bidsschematools/tests/data/bids-error-examples/invalid_asl003/dataset_description.json
 bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/sub-Sub1_T1w.json
 bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/sub-Sub1_T1w.nii.gz
 bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.json
@@ -155,14 +155,15 @@
 bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/sub-Sub1_T1w.nii.gz
 bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.json
 bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.nii.gz
 bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_aslcontext.tsv
 bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg
 bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.json
 bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.nii.gz
+bidsschematools/tests/data/bids-examples/ds000248/.bidsignore
 bidsschematools/tests/data/bids-examples/ds000248/CHANGES
 bidsschematools/tests/data/bids-examples/ds000248/README
 bidsschematools/tests/data/bids-examples/ds000248/acq-epi_T1w.json
 bidsschematools/tests/data/bids-examples/ds000248/dataset_description.json
 bidsschematools/tests/data/bids-examples/ds000248/participants.json
 bidsschematools/tests/data/bids-examples/ds000248/participants.tsv
 bidsschematools/tests/data/bids-examples/ds000248/derivatives/freesurfer/subjects/fsaverage/bem/brain.surf
```

### Comparing `bidsschematools-0.7.0/pyproject.toml` & `bidsschematools-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.7.0/setup.cfg` & `bidsschematools-0.7.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Information Analysis
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 python_requires = >=3.8
 install_requires = 
 	click
 	pyyaml
 	importlib_resources; python_version < "3.9"
@@ -53,14 +54,15 @@
 
 [options.package_data]
 bidsschematools = 
 	data/schema/BIDS_VERSION
 	data/schema/SCHEMA_VERSION
 	data/schema/**/*.yaml
 	tests/data/**/*
+	tests/data/**/.bidsignore
 
 [options.entry_points]
 console_scripts = 
 	bst=bidsschematools.__main__:cli
 
 [flake8]
 max-line-length = 99
```

