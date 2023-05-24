# Comparing `tmp/alphapulldown-0.30.5.tar.gz` & `tmp/alphapulldown-0.30.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphapulldown-0.30.5.tar", last modified: Mon May  8 11:31:44 2023, max compression
+gzip compressed data, was "alphapulldown-0.30.6.tar", last modified: Wed May 24 14:18:11 2023, max compression
```

## Comparing `alphapulldown-0.30.5.tar` & `alphapulldown-0.30.6.tar`

### file list

```diff
@@ -1,231 +1,177 @@
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:43.000000 alphapulldown-0.30.5/
--rw-r--r--   0    24600      721    35149 2022-08-09 10:02:13.000000 alphapulldown-0.30.5/LICENSE
--rw-r--r--   0    24600      721       70 2023-04-18 11:12:17.000000 alphapulldown-0.30.5/MANIFEST.in
--rw-r--r--   0    24600      721      428 2023-05-08 11:31:43.000000 alphapulldown-0.30.5/PKG-INFO
--rw-r--r--   0    24600      721     5265 2023-05-08 11:10:52.000000 alphapulldown-0.30.5/README.md
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:16.000000 alphapulldown-0.30.5/alphafold/
--rw-r--r--   0    24600      721      663 2023-04-19 11:33:22.000000 alphapulldown-0.30.5/alphafold/__init__.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:16.000000 alphapulldown-0.30.5/alphafold/alphafold/
--rw-r--r--   0    24600      721      663 2023-04-18 13:00:43.000000 alphapulldown-0.30.5/alphafold/alphafold/__init__.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:19.000000 alphapulldown-0.30.5/alphafold/alphafold/common/
--rw-r--r--   0    24600      721      655 2023-04-18 13:00:43.000000 alphapulldown-0.30.5/alphafold/alphafold/common/__init__.py
--rw-r--r--   0    24600      721     6066 2023-04-18 13:00:44.000000 alphapulldown-0.30.5/alphafold/alphafold/common/confidence.py
--rw-r--r--   0    24600      721     9959 2023-04-18 13:00:44.000000 alphapulldown-0.30.5/alphafold/alphafold/common/protein.py
--rw-r--r--   0    24600      721     4594 2023-04-18 13:00:44.000000 alphapulldown-0.30.5/alphafold/alphafold/common/protein_test.py
--rw-r--r--   0    24600      721    34974 2023-04-18 13:00:44.000000 alphapulldown-0.30.5/alphafold/alphafold/common/residue_constants.py
--rw-r--r--   0    24600      721     9256 2023-04-18 13:00:44.000000 alphapulldown-0.30.5/alphafold/alphafold/common/residue_constants_test.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:22.000000 alphapulldown-0.30.5/alphafold/alphafold/data/
--rw-r--r--   0    24600      721      634 2023-04-18 13:00:45.000000 alphapulldown-0.30.5/alphafold/alphafold/data/__init__.py
--rw-r--r--   0    24600      721     8575 2023-04-18 13:00:46.000000 alphapulldown-0.30.5/alphafold/alphafold/data/feature_processing.py
--rw-r--r--   0    24600      721    14182 2023-04-18 13:00:46.000000 alphapulldown-0.30.5/alphafold/alphafold/data/mmcif_parsing.py
--rw-r--r--   0    24600      721     3229 2023-04-18 13:11:35.000000 alphapulldown-0.30.5/alphafold/alphafold/data/msa_identifiers.py
--rw-r--r--   0    24600      721    17220 2023-04-18 13:00:46.000000 alphapulldown-0.30.5/alphafold/alphafold/data/msa_pairing.py
--rw-r--r--   0    24600      721    21397 2023-04-18 13:00:46.000000 alphapulldown-0.30.5/alphafold/alphafold/data/parsers.py
--rw-r--r--   0    24600      721    10419 2023-04-18 13:00:46.000000 alphapulldown-0.30.5/alphafold/alphafold/data/pipeline.py
--rw-r--r--   0    24600      721    11126 2023-04-18 13:00:47.000000 alphapulldown-0.30.5/alphafold/alphafold/data/pipeline_multimer.py
--rw-r--r--   0    24600      721    40677 2023-04-18 13:00:47.000000 alphapulldown-0.30.5/alphafold/alphafold/data/templates.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:26.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/
--rw-r--r--   0    24600      721      639 2023-04-18 13:00:47.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/__init__.py
--rw-r--r--   0    24600      721     5504 2023-04-18 13:00:47.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/hhblits.py
--rw-r--r--   0    24600      721     3601 2023-04-18 13:00:47.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/hhsearch.py
--rw-r--r--   0    24600      721     4576 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/hmmbuild.py
--rw-r--r--   0    24600      721     4556 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/hmmsearch.py
--rw-r--r--   0    24600      721     8386 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/jackhmmer.py
--rw-r--r--   0    24600      721     3387 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/kalign.py
--rw-r--r--   0    24600      721     1223 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/utils.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:42.000000 alphapulldown-0.30.5/alphafold/alphafold/model/
--rw-r--r--   0    24600      721      617 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/model/__init__.py
--rw-r--r--   0    24600      721    47028 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/all_atom.py
--rw-r--r--   0    24600      721    40145 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/all_atom_multimer.py
--rw-r--r--   0    24600      721     4706 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/all_atom_test.py
--rw-r--r--   0    24600      721     5957 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/common_modules.py
--rw-r--r--   0    24600      721    26814 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/config.py
--rw-r--r--   0    24600      721     1097 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/data.py
--rw-r--r--   0    24600      721     3692 2023-04-18 13:00:50.000000 alphapulldown-0.30.5/alphafold/alphafold/model/features.py
--rw-r--r--   0    24600      721    37264 2023-04-18 13:00:50.000000 alphapulldown-0.30.5/alphafold/alphafold/model/folding.py
--rw-r--r--   0    24600      721    42498 2023-04-18 13:00:50.000000 alphapulldown-0.30.5/alphafold/alphafold/model/folding_multimer.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:46.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/
--rw-r--r--   0    24600      721     1172 2023-04-18 13:00:50.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/__init__.py
--rw-r--r--   0    24600      721     4148 2023-04-18 13:00:50.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/rigid_matrix_vector.py
--rw-r--r--   0    24600      721     5751 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/rotation_matrix.py
--rw-r--r--   0    24600      721     7745 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/struct_of_array.py
--rw-r--r--   0    24600      721     4166 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/test_utils.py
--rw-r--r--   0    24600      721      853 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/utils.py
--rw-r--r--   0    24600      721     6896 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/vector.py
--rw-r--r--   0    24600      721     9134 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/layer_stack.py
--rw-r--r--   0    24600      721    10315 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/layer_stack_test.py
--rw-r--r--   0    24600      721     3505 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/lddt.py
--rw-r--r--   0    24600      721     2384 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/lddt_test.py
--rw-r--r--   0    24600      721     7963 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/mapping.py
--rw-r--r--   0    24600      721     6613 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/model.py
--rw-r--r--   0    24600      721    74120 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/modules.py
--rw-r--r--   0    24600      721    42228 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/modules_multimer.py
--rw-r--r--   0    24600      721     1978 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/prng.py
--rw-r--r--   0    24600      721     1250 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/prng_test.py
--rw-r--r--   0    24600      721    17388 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/quat_affine.py
--rw-r--r--   0    24600      721     5038 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/quat_affine_test.py
--rw-r--r--   0    24600      721    10935 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/r3.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/
--rw-r--r--   0    24600      721      633 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/__init__.py
--rw-r--r--   0    24600      721    21428 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/data_transforms.py
--rw-r--r--   0    24600      721     5357 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/input_pipeline.py
--rw-r--r--   0    24600      721     5051 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/protein_features.py
--rw-r--r--   0    24600      721     1822 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/protein_features_test.py
--rw-r--r--   0    24600      721     6344 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/proteins_dataset.py
--rw-r--r--   0    24600      721     1415 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_helpers.py
--rw-r--r--   0    24600      721     1318 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_helpers_test.py
--rw-r--r--   0    24600      721      812 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_placeholders.py
--rw-r--r--   0    24600      721     1276 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/utils.py
--rw-r--r--   0    24600      721     5328 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/model/utils.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:51.000000 alphapulldown-0.30.5/alphafold/alphafold/notebooks/
--rw-r--r--   0    24600      721      626 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/notebooks/__init__.py
--rw-r--r--   0    24600      721     7520 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/notebooks/notebook_utils.py
--rw-r--r--   0    24600      721     9571 2023-04-18 13:00:56.000000 alphapulldown-0.30.5/alphafold/alphafold/notebooks/notebook_utils_test.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:54.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/
--rw-r--r--   0    24600      721      618 2023-04-18 13:00:56.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/__init__.py
--rw-r--r--   0    24600      721    19061 2023-04-18 13:00:56.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/amber_minimize.py
--rw-r--r--   0    24600      721     4348 2023-04-18 13:00:56.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/amber_minimize_test.py
--rw-r--r--   0    24600      721     4832 2023-04-18 13:00:57.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/cleanup.py
--rw-r--r--   0    24600      721     6170 2023-04-18 13:00:57.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/cleanup_test.py
--rw-r--r--   0    24600      721     3288 2023-04-18 13:00:57.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/relax.py
--rw-r--r--   0    24600      721     3827 2023-04-18 13:00:57.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/relax_test.py
--rw-r--r--   0    24600      721     2501 2023-04-18 13:00:58.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/utils.py
--rw-r--r--   0    24600      721     1996 2023-04-18 13:00:59.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/utils_test.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:56.000000 alphapulldown-0.30.5/alphafold/common/
--rw-r--r--   0    24600      721      655 2023-04-19 11:33:22.000000 alphapulldown-0.30.5/alphafold/common/__init__.py
--rw-r--r--   0    24600      721     6066 2023-04-19 11:33:23.000000 alphapulldown-0.30.5/alphafold/common/confidence.py
--rw-r--r--   0    24600      721     9959 2023-04-19 11:33:23.000000 alphapulldown-0.30.5/alphafold/common/protein.py
--rw-r--r--   0    24600      721     4594 2023-04-19 11:33:23.000000 alphapulldown-0.30.5/alphafold/common/protein_test.py
--rw-r--r--   0    24600      721    34974 2023-04-19 11:33:24.000000 alphapulldown-0.30.5/alphafold/common/residue_constants.py
--rw-r--r--   0    24600      721     9256 2023-04-19 11:33:24.000000 alphapulldown-0.30.5/alphafold/common/residue_constants_test.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:59.000000 alphapulldown-0.30.5/alphafold/data/
--rw-r--r--   0    24600      721      634 2023-04-19 11:33:26.000000 alphapulldown-0.30.5/alphafold/data/__init__.py
--rw-r--r--   0    24600      721     8575 2023-04-19 11:33:26.000000 alphapulldown-0.30.5/alphafold/data/feature_processing.py
--rw-r--r--   0    24600      721    14182 2023-04-19 11:33:26.000000 alphapulldown-0.30.5/alphafold/data/mmcif_parsing.py
--rw-r--r--   0    24600      721     2966 2023-04-19 11:33:27.000000 alphapulldown-0.30.5/alphafold/data/msa_identifiers.py
--rw-r--r--   0    24600      721    17220 2023-04-19 11:33:27.000000 alphapulldown-0.30.5/alphafold/data/msa_pairing.py
--rw-r--r--   0    24600      721    21397 2023-04-19 11:33:28.000000 alphapulldown-0.30.5/alphafold/data/parsers.py
--rw-r--r--   0    24600      721    10419 2023-04-19 11:33:28.000000 alphapulldown-0.30.5/alphafold/data/pipeline.py
--rw-r--r--   0    24600      721    11126 2023-04-19 11:33:28.000000 alphapulldown-0.30.5/alphafold/data/pipeline_multimer.py
--rw-r--r--   0    24600      721    40677 2023-04-19 11:33:29.000000 alphapulldown-0.30.5/alphafold/data/templates.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:03.000000 alphapulldown-0.30.5/alphafold/data/tools/
--rw-r--r--   0    24600      721      639 2023-04-19 11:33:29.000000 alphapulldown-0.30.5/alphafold/data/tools/__init__.py
--rw-r--r--   0    24600      721     5504 2023-04-19 11:33:29.000000 alphapulldown-0.30.5/alphafold/data/tools/hhblits.py
--rw-r--r--   0    24600      721     3601 2023-04-19 11:33:30.000000 alphapulldown-0.30.5/alphafold/data/tools/hhsearch.py
--rw-r--r--   0    24600      721     4576 2023-04-19 11:33:30.000000 alphapulldown-0.30.5/alphafold/data/tools/hmmbuild.py
--rw-r--r--   0    24600      721     4556 2023-04-19 11:33:31.000000 alphapulldown-0.30.5/alphafold/data/tools/hmmsearch.py
--rw-r--r--   0    24600      721     8386 2023-04-19 11:33:31.000000 alphapulldown-0.30.5/alphafold/data/tools/jackhmmer.py
--rw-r--r--   0    24600      721     3387 2023-04-19 11:33:31.000000 alphapulldown-0.30.5/alphafold/data/tools/kalign.py
--rw-r--r--   0    24600      721     1223 2023-04-19 11:33:31.000000 alphapulldown-0.30.5/alphafold/data/tools/utils.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:14.000000 alphapulldown-0.30.5/alphafold/model/
--rw-r--r--   0    24600      721      617 2023-04-19 11:33:32.000000 alphapulldown-0.30.5/alphafold/model/__init__.py
--rw-r--r--   0    24600      721    47028 2023-04-19 11:33:32.000000 alphapulldown-0.30.5/alphafold/model/all_atom.py
--rw-r--r--   0    24600      721    40145 2023-04-19 11:33:33.000000 alphapulldown-0.30.5/alphafold/model/all_atom_multimer.py
--rw-r--r--   0    24600      721     4706 2023-04-19 11:33:33.000000 alphapulldown-0.30.5/alphafold/model/all_atom_test.py
--rw-r--r--   0    24600      721     5957 2023-04-19 11:33:33.000000 alphapulldown-0.30.5/alphafold/model/common_modules.py
--rw-r--r--   0    24600      721    26814 2023-04-19 11:33:34.000000 alphapulldown-0.30.5/alphafold/model/config.py
--rw-r--r--   0    24600      721     1097 2023-04-19 11:33:34.000000 alphapulldown-0.30.5/alphafold/model/data.py
--rw-r--r--   0    24600      721     3692 2023-04-19 11:33:34.000000 alphapulldown-0.30.5/alphafold/model/features.py
--rw-r--r--   0    24600      721    37264 2023-04-19 11:33:35.000000 alphapulldown-0.30.5/alphafold/model/folding.py
--rw-r--r--   0    24600      721    42498 2023-04-19 11:33:35.000000 alphapulldown-0.30.5/alphafold/model/folding_multimer.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:17.000000 alphapulldown-0.30.5/alphafold/model/geometry/
--rw-r--r--   0    24600      721     1172 2023-04-19 11:33:36.000000 alphapulldown-0.30.5/alphafold/model/geometry/__init__.py
--rw-r--r--   0    24600      721     4148 2023-04-19 11:33:36.000000 alphapulldown-0.30.5/alphafold/model/geometry/rigid_matrix_vector.py
--rw-r--r--   0    24600      721     5751 2023-04-19 11:33:37.000000 alphapulldown-0.30.5/alphafold/model/geometry/rotation_matrix.py
--rw-r--r--   0    24600      721     7745 2023-04-19 11:33:37.000000 alphapulldown-0.30.5/alphafold/model/geometry/struct_of_array.py
--rw-r--r--   0    24600      721     4166 2023-04-19 11:33:37.000000 alphapulldown-0.30.5/alphafold/model/geometry/test_utils.py
--rw-r--r--   0    24600      721      853 2023-04-19 11:33:38.000000 alphapulldown-0.30.5/alphafold/model/geometry/utils.py
--rw-r--r--   0    24600      721     6896 2023-04-19 11:33:38.000000 alphapulldown-0.30.5/alphafold/model/geometry/vector.py
--rw-r--r--   0    24600      721     9134 2023-04-19 11:33:38.000000 alphapulldown-0.30.5/alphafold/model/layer_stack.py
--rw-r--r--   0    24600      721    10315 2023-04-19 11:33:39.000000 alphapulldown-0.30.5/alphafold/model/layer_stack_test.py
--rw-r--r--   0    24600      721     3505 2023-04-19 11:33:39.000000 alphapulldown-0.30.5/alphafold/model/lddt.py
--rw-r--r--   0    24600      721     2384 2023-04-19 11:33:39.000000 alphapulldown-0.30.5/alphafold/model/lddt_test.py
--rw-r--r--   0    24600      721     7963 2023-04-19 11:33:40.000000 alphapulldown-0.30.5/alphafold/model/mapping.py
--rw-r--r--   0    24600      721     6613 2023-04-19 11:33:40.000000 alphapulldown-0.30.5/alphafold/model/model.py
--rw-r--r--   0    24600      721    74120 2023-04-19 11:33:40.000000 alphapulldown-0.30.5/alphafold/model/modules.py
--rw-r--r--   0    24600      721    42228 2023-04-19 11:33:41.000000 alphapulldown-0.30.5/alphafold/model/modules_multimer.py
--rw-r--r--   0    24600      721     1978 2023-04-19 11:33:41.000000 alphapulldown-0.30.5/alphafold/model/prng.py
--rw-r--r--   0    24600      721     1250 2023-04-19 11:33:41.000000 alphapulldown-0.30.5/alphafold/model/prng_test.py
--rw-r--r--   0    24600      721    17388 2023-04-19 11:33:42.000000 alphapulldown-0.30.5/alphafold/model/quat_affine.py
--rw-r--r--   0    24600      721     5038 2023-04-19 11:33:42.000000 alphapulldown-0.30.5/alphafold/model/quat_affine_test.py
--rw-r--r--   0    24600      721    10935 2023-04-19 11:33:42.000000 alphapulldown-0.30.5/alphafold/model/r3.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:21.000000 alphapulldown-0.30.5/alphafold/model/tf/
--rw-r--r--   0    24600      721      633 2023-04-19 11:33:43.000000 alphapulldown-0.30.5/alphafold/model/tf/__init__.py
--rw-r--r--   0    24600      721    21428 2023-04-19 11:33:43.000000 alphapulldown-0.30.5/alphafold/model/tf/data_transforms.py
--rw-r--r--   0    24600      721     5357 2023-04-19 11:33:44.000000 alphapulldown-0.30.5/alphafold/model/tf/input_pipeline.py
--rw-r--r--   0    24600      721     5051 2023-04-19 11:33:44.000000 alphapulldown-0.30.5/alphafold/model/tf/protein_features.py
--rw-r--r--   0    24600      721     1822 2023-04-19 11:33:44.000000 alphapulldown-0.30.5/alphafold/model/tf/protein_features_test.py
--rw-r--r--   0    24600      721     6344 2023-04-19 11:33:45.000000 alphapulldown-0.30.5/alphafold/model/tf/proteins_dataset.py
--rw-r--r--   0    24600      721     1415 2023-04-19 11:33:45.000000 alphapulldown-0.30.5/alphafold/model/tf/shape_helpers.py
--rw-r--r--   0    24600      721     1318 2023-04-19 11:33:45.000000 alphapulldown-0.30.5/alphafold/model/tf/shape_helpers_test.py
--rw-r--r--   0    24600      721      812 2023-04-19 11:33:46.000000 alphapulldown-0.30.5/alphafold/model/tf/shape_placeholders.py
--rw-r--r--   0    24600      721     1276 2023-04-19 11:33:46.000000 alphapulldown-0.30.5/alphafold/model/tf/utils.py
--rw-r--r--   0    24600      721     5328 2023-04-19 11:33:46.000000 alphapulldown-0.30.5/alphafold/model/utils.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:22.000000 alphapulldown-0.30.5/alphafold/notebooks/
--rw-r--r--   0    24600      721      626 2023-04-19 11:33:46.000000 alphapulldown-0.30.5/alphafold/notebooks/__init__.py
--rw-r--r--   0    24600      721     7520 2023-04-19 11:33:47.000000 alphapulldown-0.30.5/alphafold/notebooks/notebook_utils.py
--rw-r--r--   0    24600      721     9571 2023-04-19 11:33:47.000000 alphapulldown-0.30.5/alphafold/notebooks/notebook_utils_test.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:25.000000 alphapulldown-0.30.5/alphafold/relax/
--rw-r--r--   0    24600      721      618 2023-04-19 11:33:48.000000 alphapulldown-0.30.5/alphafold/relax/__init__.py
--rw-r--r--   0    24600      721    19061 2023-04-19 11:33:48.000000 alphapulldown-0.30.5/alphafold/relax/amber_minimize.py
--rw-r--r--   0    24600      721     4348 2023-04-19 11:33:48.000000 alphapulldown-0.30.5/alphafold/relax/amber_minimize_test.py
--rw-r--r--   0    24600      721     4832 2023-04-19 11:33:49.000000 alphapulldown-0.30.5/alphafold/relax/cleanup.py
--rw-r--r--   0    24600      721     6170 2023-04-19 11:33:49.000000 alphapulldown-0.30.5/alphafold/relax/cleanup_test.py
--rw-r--r--   0    24600      721     3288 2023-04-19 11:33:49.000000 alphapulldown-0.30.5/alphafold/relax/relax.py
--rw-r--r--   0    24600      721     3827 2023-04-19 11:33:50.000000 alphapulldown-0.30.5/alphafold/relax/relax_test.py
--rw-r--r--   0    24600      721     2501 2023-04-19 11:33:52.000000 alphapulldown-0.30.5/alphafold/relax/utils.py
--rw-r--r--   0    24600      721     1996 2023-04-19 11:33:52.000000 alphapulldown-0.30.5/alphafold/relax/utils_test.py
--rw-r--r--   0    24600      721    19606 2023-04-19 11:33:53.000000 alphapulldown-0.30.5/alphafold/run_alphafold.py
--rw-r--r--   0    24600      721     3814 2023-04-18 13:01:10.000000 alphapulldown-0.30.5/alphafold/run_alphafold_test.py
--rw-r--r--   0    24600      721     2064 2023-04-18 13:01:11.000000 alphapulldown-0.30.5/alphafold/setup.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:29.000000 alphapulldown-0.30.5/alphapulldown/
--rw-r--r--   0    24600      721        0 2023-01-27 13:02:50.000000 alphapulldown-0.30.5/alphapulldown/__init__.py
--rw-r--r--   0    24600      721     3944 2023-03-14 16:09:43.000000 alphapulldown-0.30.5/alphapulldown/colab_batch_no_prediction.py
--rwxr-xr-x   0    24600      721    10571 2023-04-19 11:33:53.000000 alphapulldown-0.30.5/alphapulldown/create_individual_features.py
--rw-r--r--   0    24600      721    22205 2023-04-19 11:33:53.000000 alphapulldown-0.30.5/alphapulldown/objects.py
--rw-r--r--   0    24600      721     1822 2023-03-14 16:09:43.000000 alphapulldown-0.30.5/alphapulldown/plot_pae.py
--rw-r--r--   0    24600      721     8878 2023-04-18 11:12:23.000000 alphapulldown-0.30.5/alphapulldown/predict_structure.py
--rwxr-xr-x   0    24600      721     1166 2023-03-14 16:09:44.000000 alphapulldown-0.30.5/alphapulldown/prepare_seq_names.py
--rwxr-xr-x   0    24600      721     1261 2023-03-14 16:09:44.000000 alphapulldown-0.30.5/alphapulldown/rename_colab_search_a3m.py
--rw-r--r--   0    24600      721    11611 2023-04-18 11:12:24.000000 alphapulldown-0.30.5/alphapulldown/run_multimer_jobs.py
--rw-r--r--   0    24600      721       63 2023-03-14 16:09:45.000000 alphapulldown-0.30.5/alphapulldown/test_global.py
--rw-r--r--   0    24600      721    11544 2023-05-08 11:10:53.000000 alphapulldown-0.30.5/alphapulldown/utils.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:31.000000 alphapulldown-0.30.5/alphapulldown.egg-info/
--rw-r--r--   0    24600      721      428 2023-05-08 11:30:07.000000 alphapulldown-0.30.5/alphapulldown.egg-info/PKG-INFO
--rw-r--r--   0    24600      721     7553 2023-05-08 11:30:08.000000 alphapulldown-0.30.5/alphapulldown.egg-info/SOURCES.txt
--rw-r--r--   0    24600      721        1 2023-05-08 11:30:07.000000 alphapulldown-0.30.5/alphapulldown.egg-info/dependency_links.txt
--rw-r--r--   0    24600      721      262 2023-05-08 11:30:07.000000 alphapulldown-0.30.5/alphapulldown.egg-info/requires.txt
--rw-r--r--   0    24600      721       52 2023-05-08 11:30:08.000000 alphapulldown-0.30.5/alphapulldown.egg-info/top_level.txt
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:33.000000 alphapulldown-0.30.5/analysis_pipeline/
--rw-r--r--   0    24600      721        0 2023-04-18 11:12:25.000000 alphapulldown-0.30.5/analysis_pipeline/__init__.py
--rw-r--r--   0    24600      721     7268 2023-04-18 11:12:25.000000 alphapulldown-0.30.5/analysis_pipeline/af2_3dmol.py
--rw-r--r--   0    24600      721     4967 2023-04-18 11:12:25.000000 alphapulldown-0.30.5/analysis_pipeline/calculate_mpdockq.py
--rw-r--r--   0    24600      721     5510 2023-04-18 11:12:26.000000 alphapulldown-0.30.5/analysis_pipeline/create_notebook.py
--rw-r--r--   0    24600      721     6253 2023-04-18 11:12:26.000000 alphapulldown-0.30.5/analysis_pipeline/get_good_inter_pae.py
--rw-r--r--   0    24600      721      962 2023-04-18 11:12:26.000000 alphapulldown-0.30.5/analysis_pipeline/utils.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:40.000000 alphapulldown-0.30.5/colabfold/
--rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/__init__.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:41.000000 alphapulldown-0.30.5/colabfold/alphafold/
--rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/alphafold/__init__.py
--rw-r--r--   0    24600      721     5923 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/alphafold/models.py
--rw-r--r--   0    24600      721     1565 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/alphafold/msa.py
--rw-r--r--   0    24600      721    65347 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/batch.py
--rw-r--r--   0    24600      721     5988 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/citations.py
--rw-r--r--   0    24600      721    24980 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/colabfold.py
--rw-r--r--   0    24600      721    32656 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/colabfold_alphafold.py
--rw-r--r--   0    24600      721     1982 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/download.py
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:42.000000 alphapulldown-0.30.5/colabfold/mmseqs/
--rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/mmseqs/__init__.py
--rw-r--r--   0    24600      721     1933 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/mmseqs/merge_and_split_msas.py
--rw-r--r--   0    24600      721    18799 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/mmseqs/search.py
--rw-r--r--   0    24600      721     1429 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/mmseqs/split_msas.py
--rw-r--r--   0    24600      721     2120 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/pdb.py
--rw-r--r--   0    24600      721     3419 2023-04-06 09:21:35.000000 alphapulldown-0.30.5/colabfold/plot.py
--rw-r--r--   0    24600      721     9954 2023-04-06 09:21:35.000000 alphapulldown-0.30.5/colabfold/utils.py
--rw-r--r--   0    24600      721      140 2023-04-05 11:02:03.000000 alphapulldown-0.30.5/pyproject.toml
--rw-r--r--   0    24600      721     1164 2023-05-08 11:31:44.000000 alphapulldown-0.30.5/setup.cfg
--rwxr-xr-x   0    24600      721       67 2023-04-18 11:12:27.000000 alphapulldown-0.30.5/setup.py
--rw-r--r--   0    24600      721     9119 2023-04-18 11:12:28.000000 alphapulldown-0.30.5/stereo_chemical_props.txt
-drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:43.000000 alphapulldown-0.30.5/test/
--rw-r--r--   0    24600      721     4546 2023-04-19 11:33:54.000000 alphapulldown-0.30.5/test/test_create_objects.py
--rwxr-xr-x   0    24600      721    11179 2023-05-08 11:07:26.000000 alphapulldown-0.30.5/test/test_predict_structure.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:10.000000 alphapulldown-0.30.6/
+-rw-r--r--   0    24600      721    35149 2022-08-09 10:02:13.000000 alphapulldown-0.30.6/LICENSE
+-rw-r--r--   0    24600      721       70 2023-04-18 11:12:17.000000 alphapulldown-0.30.6/MANIFEST.in
+-rw-r--r--   0    24600      721      428 2023-05-24 14:18:10.000000 alphapulldown-0.30.6/PKG-INFO
+-rw-r--r--   0    24600      721     5483 2023-05-24 13:23:45.000000 alphapulldown-0.30.6/README.md
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:17.000000 alphapulldown-0.30.6/alphafold/
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:18.000000 alphapulldown-0.30.6/alphafold/alphafold/
+-rw-r--r--   0    24600      721      663 2023-05-16 14:00:32.000000 alphapulldown-0.30.6/alphafold/alphafold/__init__.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:20.000000 alphapulldown-0.30.6/alphafold/alphafold/common/
+-rw-r--r--   0    24600      721      655 2023-05-16 14:00:32.000000 alphapulldown-0.30.6/alphafold/alphafold/common/__init__.py
+-rw-r--r--   0    24600      721     6066 2023-05-16 14:00:33.000000 alphapulldown-0.30.6/alphafold/alphafold/common/confidence.py
+-rw-r--r--   0    24600      721     9959 2023-05-16 14:00:33.000000 alphapulldown-0.30.6/alphafold/alphafold/common/protein.py
+-rw-r--r--   0    24600      721     4594 2023-05-16 14:00:33.000000 alphapulldown-0.30.6/alphafold/alphafold/common/protein_test.py
+-rw-r--r--   0    24600      721    34974 2023-05-16 14:00:33.000000 alphapulldown-0.30.6/alphafold/alphafold/common/residue_constants.py
+-rw-r--r--   0    24600      721     9256 2023-05-16 14:00:33.000000 alphapulldown-0.30.6/alphafold/alphafold/common/residue_constants_test.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:23.000000 alphapulldown-0.30.6/alphafold/alphafold/data/
+-rw-r--r--   0    24600      721      634 2023-05-16 14:00:34.000000 alphapulldown-0.30.6/alphafold/alphafold/data/__init__.py
+-rw-r--r--   0    24600      721     8575 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/feature_processing.py
+-rw-r--r--   0    24600      721    14182 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/mmcif_parsing.py
+-rw-r--r--   0    24600      721     3229 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/msa_identifiers.py
+-rw-r--r--   0    24600      721    17220 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/msa_pairing.py
+-rw-r--r--   0    24600      721    21397 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/parsers.py
+-rw-r--r--   0    24600      721    10419 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/pipeline.py
+-rw-r--r--   0    24600      721    11126 2023-05-16 14:00:36.000000 alphapulldown-0.30.6/alphafold/alphafold/data/pipeline_multimer.py
+-rw-r--r--   0    24600      721    40677 2023-05-16 14:00:36.000000 alphapulldown-0.30.6/alphafold/alphafold/data/templates.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:26.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/
+-rw-r--r--   0    24600      721      639 2023-05-16 14:00:36.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/__init__.py
+-rw-r--r--   0    24600      721     5504 2023-05-16 14:00:36.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/hhblits.py
+-rw-r--r--   0    24600      721     3601 2023-05-16 14:00:36.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/hhsearch.py
+-rw-r--r--   0    24600      721     4576 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/hmmbuild.py
+-rw-r--r--   0    24600      721     4556 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/hmmsearch.py
+-rw-r--r--   0    24600      721     8386 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/jackhmmer.py
+-rw-r--r--   0    24600      721     3387 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/kalign.py
+-rw-r--r--   0    24600      721     1223 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/utils.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:35.000000 alphapulldown-0.30.6/alphafold/alphafold/model/
+-rw-r--r--   0    24600      721      617 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/model/__init__.py
+-rw-r--r--   0    24600      721    47028 2023-05-16 14:00:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/all_atom.py
+-rw-r--r--   0    24600      721    40145 2023-05-16 14:00:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/all_atom_multimer.py
+-rw-r--r--   0    24600      721     4706 2023-05-16 14:00:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/all_atom_test.py
+-rw-r--r--   0    24600      721     5957 2023-05-16 14:00:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/common_modules.py
+-rw-r--r--   0    24600      721    26814 2023-05-16 14:00:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/config.py
+-rw-r--r--   0    24600      721     1097 2023-05-16 14:00:39.000000 alphapulldown-0.30.6/alphafold/alphafold/model/data.py
+-rw-r--r--   0    24600      721     3692 2023-05-16 14:00:39.000000 alphapulldown-0.30.6/alphafold/alphafold/model/features.py
+-rw-r--r--   0    24600      721    37264 2023-05-16 14:00:39.000000 alphapulldown-0.30.6/alphafold/alphafold/model/folding.py
+-rw-r--r--   0    24600      721    42498 2023-05-16 14:00:39.000000 alphapulldown-0.30.6/alphafold/alphafold/model/folding_multimer.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/
+-rw-r--r--   0    24600      721     1172 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/__init__.py
+-rw-r--r--   0    24600      721     4148 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/rigid_matrix_vector.py
+-rw-r--r--   0    24600      721     5751 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/rotation_matrix.py
+-rw-r--r--   0    24600      721     7745 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/struct_of_array.py
+-rw-r--r--   0    24600      721     4166 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/test_utils.py
+-rw-r--r--   0    24600      721      853 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/utils.py
+-rw-r--r--   0    24600      721     6896 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/vector.py
+-rw-r--r--   0    24600      721     9134 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/layer_stack.py
+-rw-r--r--   0    24600      721    10315 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/layer_stack_test.py
+-rw-r--r--   0    24600      721     3505 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/lddt.py
+-rw-r--r--   0    24600      721     2384 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/lddt_test.py
+-rw-r--r--   0    24600      721     7963 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/mapping.py
+-rw-r--r--   0    24600      721     6613 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/model.py
+-rw-r--r--   0    24600      721    74120 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/modules.py
+-rw-r--r--   0    24600      721    42228 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/modules_multimer.py
+-rw-r--r--   0    24600      721     1978 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/prng.py
+-rw-r--r--   0    24600      721     1250 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/prng_test.py
+-rw-r--r--   0    24600      721    17388 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/quat_affine.py
+-rw-r--r--   0    24600      721     5038 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/quat_affine_test.py
+-rw-r--r--   0    24600      721    10935 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/r3.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/
+-rw-r--r--   0    24600      721      633 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/__init__.py
+-rw-r--r--   0    24600      721    21428 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/data_transforms.py
+-rw-r--r--   0    24600      721     5357 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/input_pipeline.py
+-rw-r--r--   0    24600      721     5051 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/protein_features.py
+-rw-r--r--   0    24600      721     1822 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/protein_features_test.py
+-rw-r--r--   0    24600      721     6344 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/proteins_dataset.py
+-rw-r--r--   0    24600      721     1415 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_helpers.py
+-rw-r--r--   0    24600      721     1318 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_helpers_test.py
+-rw-r--r--   0    24600      721      812 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_placeholders.py
+-rw-r--r--   0    24600      721     1276 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/utils.py
+-rw-r--r--   0    24600      721     5328 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/utils.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:43.000000 alphapulldown-0.30.6/alphafold/alphafold/notebooks/
+-rw-r--r--   0    24600      721      626 2023-05-16 14:00:45.000000 alphapulldown-0.30.6/alphafold/alphafold/notebooks/__init__.py
+-rw-r--r--   0    24600      721     7520 2023-05-16 14:00:45.000000 alphapulldown-0.30.6/alphafold/alphafold/notebooks/notebook_utils.py
+-rw-r--r--   0    24600      721     9571 2023-05-16 14:00:45.000000 alphapulldown-0.30.6/alphafold/alphafold/notebooks/notebook_utils_test.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/
+-rw-r--r--   0    24600      721      618 2023-05-16 14:00:45.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/__init__.py
+-rw-r--r--   0    24600      721    19061 2023-05-16 14:00:45.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/amber_minimize.py
+-rw-r--r--   0    24600      721     4348 2023-05-16 14:00:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/amber_minimize_test.py
+-rw-r--r--   0    24600      721     4832 2023-05-16 14:00:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/cleanup.py
+-rw-r--r--   0    24600      721     6170 2023-05-16 14:00:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/cleanup_test.py
+-rw-r--r--   0    24600      721     3288 2023-05-16 14:00:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/relax.py
+-rw-r--r--   0    24600      721     3827 2023-05-16 14:00:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/relax_test.py
+-rw-r--r--   0    24600      721     2501 2023-05-16 14:00:48.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/utils.py
+-rw-r--r--   0    24600      721     1996 2023-05-16 14:00:48.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/utils_test.py
+-rw-r--r--   0    24600      721    19606 2023-05-19 10:39:58.000000 alphapulldown-0.30.6/alphafold/run_alphafold.py
+-rw-r--r--   0    24600      721     3814 2023-05-16 14:00:59.000000 alphapulldown-0.30.6/alphafold/run_alphafold_test.py
+-rw-r--r--   0    24600      721     2064 2023-05-16 14:01:01.000000 alphapulldown-0.30.6/alphafold/setup.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:49.000000 alphapulldown-0.30.6/alphapulldown/
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:12.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:55.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/
+-rw-r--r--   0    24600      721        0 2023-05-16 09:15:18.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/__init__.py
+-rw-r--r--   0    24600      721    65347 2023-05-16 11:20:06.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/batch.py
+-rw-r--r--   0    24600      721     5988 2023-05-16 11:20:07.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/citations.py
+-rw-r--r--   0    24600      721    24980 2023-05-16 11:20:07.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/colabfold.py
+-rw-r--r--   0    24600      721    32656 2023-05-16 11:20:07.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/colabfold_alphafold.py
+-rw-r--r--   0    24600      721     1982 2023-05-16 11:20:07.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/download.py
+-rw-r--r--   0    24600      721     2120 2023-05-16 09:15:21.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/pdb.py
+-rw-r--r--   0    24600      721     3419 2023-05-16 11:20:07.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/plot.py
+-rw-r--r--   0    24600      721     9954 2023-05-16 11:20:08.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/utils.py
+-rw-r--r--   0    24600      721        0 2023-01-27 13:02:50.000000 alphapulldown-0.30.6/alphapulldown/__init__.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:57.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/
+-rw-r--r--   0    24600      721     7268 2023-03-14 10:54:09.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_3dmol.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:57.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:58.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/
+-rw-r--r--   0    24600      721        0 2023-05-16 12:08:43.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/__init__.py
+-rw-r--r--   0    24600      721     3745 2023-05-16 11:50:17.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/__main__.py
+-rw-r--r--   0    24600      721    15555 2023-05-16 11:50:17.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/plotter.py
+-rw-r--r--   0    24600      721       21 2023-05-16 11:50:18.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/version.py
+-rw-r--r--   0    24600      721      851 2023-05-16 11:51:00.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/setup.py
+-rw-rw-r--   0    24600      721     6028 2023-01-27 13:24:19.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/calculate_mpdockq.py
+-rw-r--r--   0    24600      721     5510 2023-01-27 13:03:03.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/create_notebook.py
+-rw-r--r--   0    24600      721     6520 2023-01-27 13:24:19.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/get_good_inter_pae.py
+-rw-r--r--   0    24600      721      962 2023-01-27 13:03:03.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/utils.py
+-rwxr-xr-x   0    24600      721    10571 2023-04-19 11:33:53.000000 alphapulldown-0.30.6/alphapulldown/create_individual_features.py
+-rw-r--r--   0    24600      721    22205 2023-04-19 11:33:53.000000 alphapulldown-0.30.6/alphapulldown/objects.py
+-rw-r--r--   0    24600      721     1822 2023-03-14 16:09:43.000000 alphapulldown-0.30.6/alphapulldown/plot_pae.py
+-rw-r--r--   0    24600      721     8878 2023-04-18 11:12:23.000000 alphapulldown-0.30.6/alphapulldown/predict_structure.py
+-rwxr-xr-x   0    24600      721     1166 2023-03-14 16:09:44.000000 alphapulldown-0.30.6/alphapulldown/prepare_seq_names.py
+-rwxr-xr-x   0    24600      721     1261 2023-03-14 16:09:44.000000 alphapulldown-0.30.6/alphapulldown/rename_colab_search_a3m.py
+-rw-r--r--   0    24600      721    11611 2023-05-24 13:19:32.000000 alphapulldown-0.30.6/alphapulldown/run_multimer_jobs.py
+-rw-r--r--   0    24600      721    11546 2023-05-24 14:16:37.000000 alphapulldown-0.30.6/alphapulldown/utils.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:09.000000 alphapulldown-0.30.6/alphapulldown.egg-info/
+-rw-r--r--   0    24600      721     4096 2023-05-19 09:47:48.000000 alphapulldown-0.30.6/alphapulldown.egg-info/._PKG-INFO
+-rw-r--r--   0    24600      721     4096 2023-05-19 09:47:58.000000 alphapulldown-0.30.6/alphapulldown.egg-info/._SOURCES.txt
+-rw-r--r--   0    24600      721     4096 2023-05-19 09:47:49.000000 alphapulldown-0.30.6/alphapulldown.egg-info/._dependency_links.txt
+-rw-r--r--   0    24600      721     4096 2023-05-19 09:47:50.000000 alphapulldown-0.30.6/alphapulldown.egg-info/._requires.txt
+-rw-r--r--   0    24600      721     4096 2023-05-19 09:47:50.000000 alphapulldown-0.30.6/alphapulldown.egg-info/._top_level.txt
+-rw-r--r--   0    24600      721      428 2023-05-24 14:17:09.000000 alphapulldown-0.30.6/alphapulldown.egg-info/PKG-INFO
+-rw-r--r--   0    24600      721     6248 2023-05-24 14:17:10.000000 alphapulldown-0.30.6/alphapulldown.egg-info/SOURCES.txt
+-rw-r--r--   0    24600      721        1 2023-05-24 14:17:09.000000 alphapulldown-0.30.6/alphapulldown.egg-info/dependency_links.txt
+-rw-r--r--   0    24600      721      262 2023-05-24 14:17:10.000000 alphapulldown-0.30.6/alphapulldown.egg-info/requires.txt
+-rw-r--r--   0    24600      721       61 2023-05-24 14:17:10.000000 alphapulldown-0.30.6/alphapulldown.egg-info/top_level.txt
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:02.000000 alphapulldown-0.30.6/colabfold/
+-rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/__init__.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:03.000000 alphapulldown-0.30.6/colabfold/alphafold/
+-rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/alphafold/__init__.py
+-rw-r--r--   0    24600      721     5923 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/alphafold/models.py
+-rw-r--r--   0    24600      721     1565 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/alphafold/msa.py
+-rw-r--r--   0    24600      721    65347 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/batch.py
+-rw-r--r--   0    24600      721     5988 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/citations.py
+-rw-r--r--   0    24600      721    24980 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/colabfold.py
+-rw-r--r--   0    24600      721    32656 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/colabfold_alphafold.py
+-rw-r--r--   0    24600      721     1982 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/download.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:04.000000 alphapulldown-0.30.6/colabfold/mmseqs/
+-rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/mmseqs/__init__.py
+-rw-r--r--   0    24600      721     1933 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/mmseqs/merge_and_split_msas.py
+-rw-r--r--   0    24600      721    18799 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/mmseqs/search.py
+-rw-r--r--   0    24600      721     1429 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/mmseqs/split_msas.py
+-rw-r--r--   0    24600      721     2120 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/pdb.py
+-rw-r--r--   0    24600      721     3419 2023-04-06 09:21:35.000000 alphapulldown-0.30.6/colabfold/plot.py
+-rw-r--r--   0    24600      721     9954 2023-04-06 09:21:35.000000 alphapulldown-0.30.6/colabfold/utils.py
+-rw-r--r--   0    24600      721      140 2023-04-05 11:02:03.000000 alphapulldown-0.30.6/pyproject.toml
+-rw-r--r--   0    24600      721     1470 2023-05-24 14:18:10.000000 alphapulldown-0.30.6/setup.cfg
+-rwxr-xr-x   0    24600      721       67 2023-04-18 11:12:27.000000 alphapulldown-0.30.6/setup.py
+-rw-r--r--   0    24600      721     9119 2023-04-18 11:12:28.000000 alphapulldown-0.30.6/stereo_chemical_props.txt
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:10.000000 alphapulldown-0.30.6/test/
+-rw-r--r--   0    24600      721     4546 2023-04-19 11:33:54.000000 alphapulldown-0.30.6/test/test_create_objects.py
+-rwxr-xr-x   0    24600      721    12809 2023-05-19 10:38:44.000000 alphapulldown-0.30.6/test/test_predict_structure.py
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:13.000000 alphapulldown-0.30.6/unifold/
+drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:07.000000 alphapulldown-0.30.6/unifold/unifold/
+-rw-r--r--   0    24600      721       72 2023-05-19 11:17:04.000000 alphapulldown-0.30.6/unifold/unifold/__init__.py
+-rw-r--r--   0    24600      721    25459 2023-05-24 12:02:28.000000 alphapulldown-0.30.6/unifold/unifold/config.py
+-rw-r--r--   0    24600      721    21165 2023-05-24 12:02:54.000000 alphapulldown-0.30.6/unifold/unifold/dataset.py
+-rw-r--r--   0    24600      721    10412 2023-05-19 11:17:20.000000 alphapulldown-0.30.6/unifold/unifold/homo_search.py
+-rw-r--r--   0    24600      721    16351 2023-05-24 12:02:55.000000 alphapulldown-0.30.6/unifold/unifold/inference.py
+-rw-r--r--   0    24600      721     7587 2023-05-19 11:17:22.000000 alphapulldown-0.30.6/unifold/unifold/inference_symmetry.py
+-rw-r--r--   0    24600      721     9457 2023-05-19 11:17:23.000000 alphapulldown-0.30.6/unifold/unifold/loss.py
+-rw-r--r--   0    24600      721     1453 2023-05-19 11:17:30.000000 alphapulldown-0.30.6/unifold/unifold/model.py
+-rw-r--r--   0    24600      721     2445 2023-05-19 11:18:12.000000 alphapulldown-0.30.6/unifold/unifold/task.py
```

### Comparing `alphapulldown-0.30.5/LICENSE` & `alphapulldown-0.30.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/README.md` & `alphapulldown-0.30.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,26 +35,34 @@
         uniclust30_2018_08/
             # 13 files.
     uniprot/                               # ~ 98.3 GB (download: 49 GB)
         uniprot.fasta
     uniref90/                              # ~ 58 GB (download: 29.7 GB)
         uniref90.fasta
  ```
+## (For developers) Installation locally
+```bash
+git clone --recurse-submodules git@github.com:KosinskiLab/AlphaPulldown.git
+cd AlphaPulldown 
+git submodule init
+git submodule update 
+pip install .
+```
 
-## Installation 
+## (For users) pip installation 
 
 **Firstly**, install [Anaconda](https://www.anaconda.com/) and create AlphaPulldown environment, gathering necessary dependencies 
 ```bash
 conda create -n AlphaPulldown -c omnia -c bioconda -c conda-forge python==3.8 openmm=7.5.1 pdbfixer=1.6 kalign2=2.04 cctbx-base
 ```
 
 **Secondly**, activate the AlphaPulldown environment and install AlphaPulldown
 ```bash
 source activate AlphaPulldown
-python3 -m pip install alphapulldown==0.30.1
+python3 -m pip install alphapulldown==0.30.5
 pip install -q "jax[cuda]==0.3.25" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 **Optionally**, if you do not have these software yet on your system, install [HMMER](http://hmmer.org/documentation.html), [HH-suite](https://github.com/soedinglab/hh-suite) from Anaconda
 ```bash
 source activate AlphaPulldown
 conda install -c bioconda hmmer hhsuite
```

### Comparing `alphapulldown-0.30.5/alphafold/__init__.py` & `alphapulldown-0.30.6/alphafold/alphafold/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/__init__.py` & `alphapulldown-0.30.6/alphafold/alphafold/notebooks/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""An implementation of the inference pipeline of AlphaFold v2.0."""
+"""AlphaFold Colab notebook."""
```

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/common/__init__.py` & `alphapulldown-0.30.6/alphafold/alphafold/common/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/common/confidence.py` & `alphapulldown-0.30.6/alphafold/alphafold/common/confidence.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/common/protein.py` & `alphapulldown-0.30.6/alphafold/alphafold/common/protein.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/common/protein_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/common/protein_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/common/residue_constants.py` & `alphapulldown-0.30.6/alphafold/alphafold/common/residue_constants.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/common/residue_constants_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/common/residue_constants_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/__init__.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/feature_processing.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/feature_processing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/mmcif_parsing.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/mmcif_parsing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/msa_identifiers.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/msa_identifiers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/msa_pairing.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/msa_pairing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/parsers.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/parsers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/pipeline.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/pipeline_multimer.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/pipeline_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/templates.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/templates.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/tools/__init__.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/tools/hhblits.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/tools/hhblits.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/tools/hhsearch.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/tools/hhsearch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/tools/hmmbuild.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/tools/hmmbuild.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/tools/hmmsearch.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/tools/hmmsearch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/tools/jackhmmer.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/tools/jackhmmer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/tools/kalign.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/tools/kalign.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/data/tools/utils.py` & `alphapulldown-0.30.6/alphafold/alphafold/data/tools/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/__init__.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/all_atom.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/all_atom.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/all_atom_multimer.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/all_atom_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/all_atom_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/all_atom_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/common_modules.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/common_modules.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/config.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/config.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/data.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/data.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/features.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/folding.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/folding.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/folding_multimer.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/folding_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/__init__.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/rigid_matrix_vector.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/rigid_matrix_vector.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/rotation_matrix.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/struct_of_array.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/struct_of_array.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/test_utils.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/test_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/utils.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/vector.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/layer_stack.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/layer_stack.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/layer_stack_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/layer_stack_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/lddt.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/lddt.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/lddt_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/lddt_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/mapping.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/mapping.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/model.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/model.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/modules.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/modules.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/modules_multimer.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/modules_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/prng.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/prng.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/prng_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/prng_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/quat_affine.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/quat_affine.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/quat_affine_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/quat_affine_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/r3.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/r3.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/tf/__init__.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/tf/data_transforms.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/tf/data_transforms.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/tf/input_pipeline.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/tf/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/tf/protein_features.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/tf/protein_features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/tf/protein_features_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/tf/protein_features_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/tf/proteins_dataset.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/tf/proteins_dataset.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_helpers.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_helpers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_helpers_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_helpers_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_placeholders.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_placeholders.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/tf/utils.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/tf/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/model/utils.py` & `alphapulldown-0.30.6/alphafold/alphafold/model/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/notebooks/__init__.py` & `alphapulldown-0.30.6/alphafold/alphafold/relax/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""AlphaFold Colab notebook."""
+"""Amber relaxation."""
```

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/notebooks/notebook_utils.py` & `alphapulldown-0.30.6/alphafold/alphafold/notebooks/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/notebooks/notebook_utils_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/notebooks/notebook_utils_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/relax/amber_minimize.py` & `alphapulldown-0.30.6/alphafold/alphafold/relax/amber_minimize.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/relax/amber_minimize_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/relax/amber_minimize_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/relax/cleanup.py` & `alphapulldown-0.30.6/alphafold/alphafold/relax/cleanup.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/relax/cleanup_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/relax/cleanup_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/relax/relax.py` & `alphapulldown-0.30.6/alphafold/alphafold/relax/relax.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/relax/relax_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/relax/relax_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/relax/utils.py` & `alphapulldown-0.30.6/alphafold/alphafold/relax/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/alphafold/relax/utils_test.py` & `alphapulldown-0.30.6/alphafold/alphafold/relax/utils_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/data/pipeline.py` & `alphapulldown-0.30.6/unifold/unifold/homo_search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,243 +1,313 @@
+# Copyright 2022 DP Technology
 # Copyright 2021 DeepMind Technologies Limited
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Functions for building the input features for the AlphaFold model."""
-
+"""Run CPU MSA & template searching to get pickled features."""
+import json
 import os
-from typing import Any, Mapping, MutableMapping, Optional, Sequence, Union
+import pickle
+from pathlib import Path
+import shutil
+import time
+import gzip
+
+from absl import app
+from absl import flags
 from absl import logging
-from alphafold.common import residue_constants
-from alphafold.data import msa_identifiers
-from alphafold.data import parsers
-from alphafold.data import templates
-from alphafold.data.tools import hhblits
-from alphafold.data.tools import hhsearch
-from alphafold.data.tools import hmmsearch
-from alphafold.data.tools import jackhmmer
-import numpy as np
-
-# Internal import (7716).
-
-FeatureDict = MutableMapping[str, np.ndarray]
-TemplateSearcher = Union[hhsearch.HHSearch, hmmsearch.Hmmsearch]
-
-
-def make_sequence_features(
-    sequence: str, description: str, num_res: int) -> FeatureDict:
-  """Constructs a feature dict of sequence features."""
-  features = {}
-  features['aatype'] = residue_constants.sequence_to_onehot(
-      sequence=sequence,
-      mapping=residue_constants.restype_order_with_x,
-      map_unknown_to_x=True)
-  features['between_segment_residues'] = np.zeros((num_res,), dtype=np.int32)
-  features['domain_name'] = np.array([description.encode('utf-8')],
-                                     dtype=np.object_)
-  features['residue_index'] = np.array(range(num_res), dtype=np.int32)
-  features['seq_length'] = np.array([num_res] * num_res, dtype=np.int32)
-  features['sequence'] = np.array([sequence.encode('utf-8')], dtype=np.object_)
-  return features
-
-
-def make_msa_features(msas: Sequence[parsers.Msa]) -> FeatureDict:
-  """Constructs a feature dict of MSA features."""
-  if not msas:
-    raise ValueError('At least one MSA must be provided.')
-
-  int_msa = []
-  deletion_matrix = []
-  species_ids = []
-  seen_sequences = set()
-  for msa_index, msa in enumerate(msas):
-    if not msa:
-      raise ValueError(f'MSA {msa_index} must contain at least one sequence.')
-    for sequence_index, sequence in enumerate(msa.sequences):
-      if sequence in seen_sequences:
-        continue
-      seen_sequences.add(sequence)
-      int_msa.append(
-          [residue_constants.HHBLITS_AA_TO_ID[res] for res in sequence])
-      deletion_matrix.append(msa.deletion_matrix[sequence_index])
-      identifiers = msa_identifiers.get_identifiers(
-          msa.descriptions[sequence_index])
-      species_ids.append(identifiers.species_id.encode('utf-8'))
-
-  num_res = len(msas[0].sequences[0])
-  num_alignments = len(int_msa)
-  features = {}
-  features['deletion_matrix_int'] = np.array(deletion_matrix, dtype=np.int32)
-  features['msa'] = np.array(int_msa, dtype=np.int32)
-  features['num_alignments'] = np.array(
-      [num_alignments] * num_res, dtype=np.int32)
-  features['msa_species_identifiers'] = np.array(species_ids, dtype=np.object_)
-  return features
-
-
-def run_msa_tool(msa_runner, input_fasta_path: str, msa_out_path: str,
-                 msa_format: str, use_precomputed_msas: bool,
-                 max_sto_sequences: Optional[int] = None
-                 ) -> Mapping[str, Any]:
-  """Runs an MSA tool, checking if output already exists first."""
-  if not use_precomputed_msas or not os.path.exists(msa_out_path):
-    if msa_format == 'sto' and max_sto_sequences is not None:
-      result = msa_runner.query(input_fasta_path, max_sto_sequences)[0]  # pytype: disable=wrong-arg-count
-    else:
-      result = msa_runner.query(input_fasta_path)[0]
-    with open(msa_out_path, 'w') as f:
-      f.write(result[msa_format])
-  else:
-    logging.warning('Reading MSA from file %s', msa_out_path)
-    if msa_format == 'sto' and max_sto_sequences is not None:
-      precomputed_msa = parsers.truncate_stockholm_msa(
-          msa_out_path, max_sto_sequences)
-      result = {'sto': precomputed_msa}
-    else:
-      with open(msa_out_path, 'r') as f:
-        result = {msa_format: f.read()}
-  return result
-
-
-class DataPipeline:
-  """Runs the alignment tools and assembles the input features."""
-
-  def __init__(self,
-               jackhmmer_binary_path: str,
-               hhblits_binary_path: str,
-               uniref90_database_path: str,
-               mgnify_database_path: str,
-               bfd_database_path: Optional[str],
-               uniref30_database_path: Optional[str],
-               small_bfd_database_path: Optional[str],
-               template_searcher: TemplateSearcher,
-               template_featurizer: templates.TemplateHitFeaturizer,
-               use_small_bfd: bool,
-               mgnify_max_hits: int = 501,
-               uniref_max_hits: int = 10000,
-               use_precomputed_msas: bool = False):
-    """Initializes the data pipeline."""
-    self._use_small_bfd = use_small_bfd
-    self.jackhmmer_uniref90_runner = jackhmmer.Jackhmmer(
-        binary_path=jackhmmer_binary_path,
-        database_path=uniref90_database_path)
-    if use_small_bfd:
-      self.jackhmmer_small_bfd_runner = jackhmmer.Jackhmmer(
-          binary_path=jackhmmer_binary_path,
-          database_path=small_bfd_database_path)
-    else:
-      self.hhblits_bfd_uniref_runner = hhblits.HHBlits(
-          binary_path=hhblits_binary_path,
-          databases=[bfd_database_path, uniref30_database_path])
-    self.jackhmmer_mgnify_runner = jackhmmer.Jackhmmer(
-        binary_path=jackhmmer_binary_path,
-        database_path=mgnify_database_path)
-    self.template_searcher = template_searcher
-    self.template_featurizer = template_featurizer
-    self.mgnify_max_hits = mgnify_max_hits
-    self.uniref_max_hits = uniref_max_hits
-    self.use_precomputed_msas = use_precomputed_msas
-
-  def process(self, input_fasta_path: str, msa_output_dir: str) -> FeatureDict:
-    """Runs alignment tools on the input sequence and creates features."""
-    with open(input_fasta_path) as f:
-      input_fasta_str = f.read()
-    input_seqs, input_descs = parsers.parse_fasta(input_fasta_str)
-    if len(input_seqs) != 1:
-      raise ValueError(
-          f'More than one input sequence found in {input_fasta_path}.')
-    input_sequence = input_seqs[0]
-    input_description = input_descs[0]
-    num_res = len(input_sequence)
-
-    uniref90_out_path = os.path.join(msa_output_dir, 'uniref90_hits.sto')
-    jackhmmer_uniref90_result = run_msa_tool(
-        msa_runner=self.jackhmmer_uniref90_runner,
-        input_fasta_path=input_fasta_path,
-        msa_out_path=uniref90_out_path,
-        msa_format='sto',
-        use_precomputed_msas=self.use_precomputed_msas,
-        max_sto_sequences=self.uniref_max_hits)
-    mgnify_out_path = os.path.join(msa_output_dir, 'mgnify_hits.sto')
-    jackhmmer_mgnify_result = run_msa_tool(
-        msa_runner=self.jackhmmer_mgnify_runner,
-        input_fasta_path=input_fasta_path,
-        msa_out_path=mgnify_out_path,
-        msa_format='sto',
-        use_precomputed_msas=self.use_precomputed_msas,
-        max_sto_sequences=self.mgnify_max_hits)
-
-    msa_for_templates = jackhmmer_uniref90_result['sto']
-    msa_for_templates = parsers.deduplicate_stockholm_msa(msa_for_templates)
-    msa_for_templates = parsers.remove_empty_columns_from_stockholm_msa(
-        msa_for_templates)
-
-    if self.template_searcher.input_format == 'sto':
-      pdb_templates_result = self.template_searcher.query(msa_for_templates)
-    elif self.template_searcher.input_format == 'a3m':
-      uniref90_msa_as_a3m = parsers.convert_stockholm_to_a3m(msa_for_templates)
-      pdb_templates_result = self.template_searcher.query(uniref90_msa_as_a3m)
-    else:
-      raise ValueError('Unrecognized template input format: '
-                       f'{self.template_searcher.input_format}')
 
-    pdb_hits_out_path = os.path.join(
-        msa_output_dir, f'pdb_hits.{self.template_searcher.output_format}')
-    with open(pdb_hits_out_path, 'w') as f:
-      f.write(pdb_templates_result)
-
-    uniref90_msa = parsers.parse_stockholm(jackhmmer_uniref90_result['sto'])
-    mgnify_msa = parsers.parse_stockholm(jackhmmer_mgnify_result['sto'])
-
-    pdb_template_hits = self.template_searcher.get_template_hits(
-        output_string=pdb_templates_result, input_sequence=input_sequence)
-
-    if self._use_small_bfd:
-      bfd_out_path = os.path.join(msa_output_dir, 'small_bfd_hits.sto')
-      jackhmmer_small_bfd_result = run_msa_tool(
-          msa_runner=self.jackhmmer_small_bfd_runner,
-          input_fasta_path=input_fasta_path,
-          msa_out_path=bfd_out_path,
-          msa_format='sto',
-          use_precomputed_msas=self.use_precomputed_msas)
-      bfd_msa = parsers.parse_stockholm(jackhmmer_small_bfd_result['sto'])
+from unifold.data.utils import compress_features
+from unifold.msa import parsers
+from unifold.msa import pipeline
+from unifold.msa import templates
+from unifold.msa.utils import divide_multi_chains
+from unifold.msa.tools import hmmsearch
+
+
+logging.set_verbosity(logging.INFO)
+
+flags.DEFINE_string(
+    "fasta_path",
+    None,
+    "Path to FASTA file, If a FASTA file contains multiple sequences, "
+    "then it will be divided into several single sequences. ",
+)
+
+flags.DEFINE_string(
+    "output_dir", None, "Path to a directory that will " "store the results."
+)
+flags.DEFINE_string(
+    "jackhmmer_binary_path",
+    shutil.which("jackhmmer"),
+    "Path to the JackHMMER executable.",
+)
+flags.DEFINE_string(
+    "hhblits_binary_path", shutil.which("hhblits"), "Path to the HHblits executable."
+)
+flags.DEFINE_string(
+    "hhsearch_binary_path", shutil.which("hhsearch"), "Path to the HHsearch executable."
+)
+flags.DEFINE_string(
+    "hmmsearch_binary_path",
+    shutil.which("hmmsearch"),
+    "Path to the hmmsearch executable.",
+)
+flags.DEFINE_string(
+    "hmmbuild_binary_path", shutil.which("hmmbuild"), "Path to the hmmbuild executable."
+)
+flags.DEFINE_string(
+    "kalign_binary_path", shutil.which("kalign"), "Path to the Kalign executable."
+)
+flags.DEFINE_string(
+    "uniref90_database_path",
+    None,
+    "Path to the Uniref90 database for use by JackHMMER.",
+)
+flags.DEFINE_string(
+    "mgnify_database_path", None, "Path to the MGnify database for use by JackHMMER."
+)
+flags.DEFINE_string(
+    "bfd_database_path", None, "Path to the BFD database for use by HHblits."
+)
+flags.DEFINE_string(
+    "small_bfd_database_path",
+    None,
+    'Path to the small version of BFD used with the "reduced_dbs" preset.',
+)
+flags.DEFINE_string(
+    "uniclust30_database_path",
+    None,
+    "Path to the Uniclust30 " "database for use by HHblits.",
+)
+flags.DEFINE_string(
+    "uniprot_database_path",
+    None,
+    "Path to the Uniprot database for use by JackHMMer.",
+)
+flags.DEFINE_string(
+    "pdb_seqres_database_path",
+    None,
+    "Path to the PDB seqres database for use by hmmsearch.",
+)
+flags.DEFINE_string(
+    "template_mmcif_dir",
+    None,
+    "Path to a directory with template mmCIF structures, each named " "<pdb_id>.cif",
+)
+flags.DEFINE_string(
+    "max_template_date",
+    None,
+    "Maximum template release date to consider. Important if folding "
+    "historical test sets.",
+)
+flags.DEFINE_string(
+    "obsolete_pdbs_path",
+    None,
+    "Path to file containing a mapping from obsolete PDB IDs to the PDB IDs "
+    "of their replacements.",
+)
+flags.DEFINE_enum(
+    "db_preset",
+    "full_dbs",
+    ["full_dbs", "reduced_dbs"],
+    "Choose preset MSA database configuration - smaller genetic database "
+    "config (reduced_dbs) or full genetic database config  (full_dbs)",
+)
+flags.DEFINE_boolean(
+    "use_precomputed_msas",
+    True,
+    "Whether to read MSAs that have been written to disk instead of running "
+    "the MSA tools. The MSA files are looked up in the output directory, "
+    "so it must stay the same between multiple runs that are to reuse the "
+    "MSAs. WARNING: This will not check if the sequence, database or "
+    "configuration have changed.",
+)
+flags.DEFINE_boolean("use_uniprot", True, "Whether to use UniProt MSAs.")
+
+FLAGS = flags.FLAGS
+
+MAX_TEMPLATE_HITS = 20
+
+
+def _check_flag(flag_name: str, other_flag_name: str, should_be_set: bool):
+    if should_be_set != bool(FLAGS[flag_name].value):
+        verb = "be" if should_be_set else "not be"
+        raise ValueError(
+            f"{flag_name} must {verb} set when running with "
+            f'"--{other_flag_name}={FLAGS[other_flag_name].value}".'
+        )
+
+
+def generate_pkl_features(
+    fasta_path: str,
+    fasta_name: str,
+    output_dir_base: str,
+    data_pipeline: pipeline.DataPipeline,
+    use_uniprot: bool,
+):
+    """
+    Predicts structure using AlphaFold for the given sequence.
+    """
+    logging.info(f"searching homogeneous Sequences & structures for {fasta_name}...")
+    timings = {}
+    output_dir = os.path.join(output_dir_base, fasta_name.split("_")[0])
+    if not os.path.exists(output_dir):
+        os.makedirs(output_dir)
+    chain_id = fasta_name.split("_")[1] if len(fasta_name.split("_")) > 1 else "A"
+    msa_output_dir = os.path.join(output_dir, chain_id)
+    if not os.path.exists(msa_output_dir):
+        os.makedirs(msa_output_dir)
+
+    # Get features.
+    features_output_path = os.path.join(
+        output_dir, "{}.feature.pkl.gz".format(chain_id)
+    )
+    if not os.path.exists(features_output_path):
+        t_0 = time.time()
+        feature_dict = data_pipeline.process(
+            input_fasta_path=fasta_path, msa_output_dir=msa_output_dir
+        )
+        timings["features"] = time.time() - t_0
+        feature_dict = compress_features(feature_dict)
+        pickle.dump(feature_dict, gzip.GzipFile(features_output_path, "wb"), protocol=4)
+
+    # Get uniprot
+    if use_uniprot:
+        uniprot_output_path = os.path.join(
+            output_dir, "{}.uniprot.pkl.gz".format(chain_id)
+        )
+        if not os.path.exists(uniprot_output_path):
+            t_0 = time.time()
+            all_seq_feature_dict = data_pipeline.process_uniprot(
+                input_fasta_path=fasta_path, msa_output_dir=msa_output_dir
+            )
+            timings["all_seq_features"] = time.time() - t_0
+            all_seq_feature_dict = compress_features(all_seq_feature_dict)
+            pickle.dump(
+                all_seq_feature_dict,
+                gzip.GzipFile(uniprot_output_path, "wb"),
+                protocol=4,
+            )
+
+    logging.info("Final timings for %s: %s", fasta_name, timings)
+
+    timings_output_path = os.path.join(output_dir, "{}.timings.json".format(chain_id))
+    with open(timings_output_path, "w") as f:
+        f.write(json.dumps(timings, indent=4))
+
+
+def main(argv):
+    if len(argv) > 1:
+        raise app.UsageError("Too many command-line arguments.")
+
+    for tool_name in (
+        "jackhmmer",
+        "hhblits",
+        "hhsearch",
+        "hmmsearch",
+        "hmmbuild",
+        "kalign",
+    ):
+        if not FLAGS[f"{tool_name}_binary_path"].value:
+            raise ValueError(
+                f'Could not find path to the "{tool_name}" binary. Make '
+                "sure it is installed on your system."
+            )
+
+    use_small_bfd = FLAGS.db_preset == "reduced_dbs"
+    _check_flag("small_bfd_database_path", "db_preset", should_be_set=use_small_bfd)
+    _check_flag("bfd_database_path", "db_preset", should_be_set=not use_small_bfd)
+    _check_flag(
+        "uniclust30_database_path", "db_preset", should_be_set=not use_small_bfd
+    )
+
+    template_searcher = hmmsearch.Hmmsearch(
+        binary_path=FLAGS.hmmsearch_binary_path,
+        hmmbuild_binary_path=FLAGS.hmmbuild_binary_path,
+        database_path=FLAGS.pdb_seqres_database_path,
+    )
+
+    template_featurizer = templates.HmmsearchHitFeaturizer(
+        mmcif_dir=FLAGS.template_mmcif_dir,
+        max_template_date=FLAGS.max_template_date,
+        max_hits=MAX_TEMPLATE_HITS,
+        kalign_binary_path=FLAGS.kalign_binary_path,
+        release_dates_path=None,
+        obsolete_pdbs_path=FLAGS.obsolete_pdbs_path,
+    )
+
+    data_pipeline = pipeline.DataPipeline(
+        jackhmmer_binary_path=FLAGS.jackhmmer_binary_path,
+        hhblits_binary_path=FLAGS.hhblits_binary_path,
+        uniref90_database_path=FLAGS.uniref90_database_path,
+        mgnify_database_path=FLAGS.mgnify_database_path,
+        bfd_database_path=FLAGS.bfd_database_path,
+        uniclust30_database_path=FLAGS.uniclust30_database_path,
+        small_bfd_database_path=FLAGS.small_bfd_database_path,
+        uniprot_database_path=FLAGS.uniprot_database_path,
+        template_searcher=template_searcher,
+        template_featurizer=template_featurizer,
+        use_small_bfd=use_small_bfd,
+        use_precomputed_msas=FLAGS.use_precomputed_msas,
+    )
+
+    fasta_path = FLAGS.fasta_path
+    fasta_name = Path(fasta_path).stem
+    input_fasta_str = open(fasta_path).read()
+    input_seqs, input_descs = parsers.parse_fasta(input_fasta_str)
+    if len(input_seqs) > 1:
+        temp_names, temp_paths = divide_multi_chains(
+            fasta_name, FLAGS.output_dir, input_seqs, input_descs
+        )
+        fasta_names = temp_names
+        fasta_paths = temp_paths
     else:
-      bfd_out_path = os.path.join(msa_output_dir, 'bfd_uniref_hits.a3m')
-      hhblits_bfd_uniref_result = run_msa_tool(
-          msa_runner=self.hhblits_bfd_uniref_runner,
-          input_fasta_path=input_fasta_path,
-          msa_out_path=bfd_out_path,
-          msa_format='a3m',
-          use_precomputed_msas=self.use_precomputed_msas)
-      bfd_msa = parsers.parse_a3m(hhblits_bfd_uniref_result['a3m'])
-
-    templates_result = self.template_featurizer.get_templates(
-        query_sequence=input_sequence,
-        hits=pdb_template_hits)
-
-    sequence_features = make_sequence_features(
-        sequence=input_sequence,
-        description=input_description,
-        num_res=num_res)
-
-    msa_features = make_msa_features((uniref90_msa, bfd_msa, mgnify_msa))
-
-    logging.info('Uniref90 MSA size: %d sequences.', len(uniref90_msa))
-    logging.info('BFD MSA size: %d sequences.', len(bfd_msa))
-    logging.info('MGnify MSA size: %d sequences.', len(mgnify_msa))
-    logging.info('Final (deduplicated) MSA size: %d sequences.',
-                 msa_features['num_alignments'][0])
-    logging.info('Total number of templates (NB: this can include bad '
-                 'templates and is later filtered to top 4): %d.',
-                 templates_result.features['template_domain_names'].shape[0])
+        output_dir = os.path.join(FLAGS.output_dir, fasta_name)
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir)
+        chain_order_path = os.path.join(output_dir, "chains.txt")
+        with open(chain_order_path, "w") as f:
+            f.write("A")
+        fasta_names = [fasta_name]
+        fasta_paths = [fasta_path]
+
+    # Check for duplicate FASTA file names.
+    if len(fasta_names) != len(set(fasta_names)):
+        raise ValueError("All FASTA paths must have a unique basename.")
+
+    # Predict structure for each of the sequences.
+    for i, fasta_path in enumerate(fasta_paths):
+        fasta_name = fasta_names[i]
+        generate_pkl_features(
+            fasta_path=fasta_path,
+            fasta_name=fasta_name,
+            output_dir_base=FLAGS.output_dir,
+            data_pipeline=data_pipeline,
+            use_uniprot=FLAGS.use_uniprot,
+        )
+
+
+if __name__ == "__main__":
+    flags.mark_flags_as_required(
+        [
+            "fasta_path",
+            "output_dir",
+            "uniref90_database_path",
+            "mgnify_database_path",
+            "template_mmcif_dir",
+            "max_template_date",
+            "obsolete_pdbs_path",
+        ]
+    )
 
-    return {**sequence_features, **msa_features, **templates_result.features}
+    app.run(main)
```

### Comparing `alphapulldown-0.30.5/alphafold/run_alphafold.py` & `alphapulldown-0.30.6/alphafold/run_alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/run_alphafold_test.py` & `alphapulldown-0.30.6/alphafold/run_alphafold_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphafold/setup.py` & `alphapulldown-0.30.6/alphafold/setup.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphapulldown/create_individual_features.py` & `alphapulldown-0.30.6/alphapulldown/create_individual_features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphapulldown/objects.py` & `alphapulldown-0.30.6/alphapulldown/objects.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphapulldown/plot_pae.py` & `alphapulldown-0.30.6/alphapulldown/plot_pae.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphapulldown/predict_structure.py` & `alphapulldown-0.30.6/alphapulldown/predict_structure.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphapulldown/prepare_seq_names.py` & `alphapulldown-0.30.6/alphapulldown/prepare_seq_names.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphapulldown/rename_colab_search_a3m.py` & `alphapulldown-0.30.6/alphapulldown/rename_colab_search_a3m.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphapulldown/run_multimer_jobs.py` & `alphapulldown-0.30.6/alphapulldown/run_multimer_jobs.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/alphapulldown/utils.py` & `alphapulldown-0.30.6/alphapulldown/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         model_params = data.get_model_haiku_params(
             model_name=model_name, data_dir=data_dir
         )
         model_runner = model.RunModel(model_config, model_params)
         for i in range(num_multimer_predictions_per_model):
             model_runners[f"{model_name}_pred_{i}"] = model_runner
     if random_seed is None:
-        random_seed = random.randrange(sys.maxsize // len(model_names))
+        random_seed = random.randrange(sys.maxsize // len(model_runners))
         logging.info("Using random seed %d for the data pipeline", random_seed)
     return model_runners, random_seed
 
 
 def save_meta_data(flag_dict, outfile):
     """A function to print out metadata"""
     with open(outfile, "w") as f:
```

### Comparing `alphapulldown-0.30.5/analysis_pipeline/af2_3dmol.py` & `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_3dmol.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/analysis_pipeline/calculate_mpdockq.py` & `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/calculate_mpdockq.py`

 * *Files 16% similar despite different names*

```diff
@@ -82,18 +82,20 @@
     for k,v in chain_lengths.items():
         curr_plddt = best_plddt[curr_len:curr_len+v]
         plddt_per_chain[k] = curr_plddt
         curr_len += v 
     return plddt_per_chain
 
 def score_complex(path_coords, path_CB_inds, path_plddt):
-    '''Score all interfaces in the current complex
     '''
-    metrics = {'Chain':[], 'n_ints':[], 'sum_av_IF_plDDT':[], 
-                'n_contacts':[], 'n_IF_residues':[]}
+    Score all interfaces in the current complex
+
+    Modified from the score_complex() function in MoLPC repo: 
+    https://gitlab.com/patrickbryant1/molpc/-/blob/main/src/complex_assembly/score_entire_complex.py#L106-154
+    '''
 
     chains = [*path_coords.keys()]
     chain_inds = np.arange(len(chains))
     complex_score = 0
     #Get interfaces per chain
     for i in chain_inds:
         chain_i = chains[i]
@@ -128,17 +130,41 @@
     """
     L = 0.827
     x_0 = 261.398
     k = 0.036
     b = 0.221
     return L/(1+math.exp(-1*k*(complex_score-x_0))) + b
 
-def calculate_pDockQ(complex_score):
-    """
-    A function that returns a complex's pDockQ score after 
-    calculating complex_score
-    """
-    L = 0.724
-    x_0 = 152.611
-    k = 0.052
-    b = 0.018
-    return L/(1+math.exp(-1*k*(complex_score-x_0))) + b
+
+def calc_pdockq(chain_coords, chain_plddt, t):
+    '''Calculate the pDockQ scores
+    pdockQ = L / (1 + np.exp(-k*(x-x0)))+b
+    L= 0.724 x0= 152.611 k= 0.052 and b= 0.018
+
+    Modified from the calc_pdockq() from FoldDock repo: 
+    https://gitlab.com/ElofssonLab/FoldDock/-/blob/main/src/pdockq.py#L62
+    '''
+
+    #Get coords and plddt per chain
+    ch1, ch2 = [*chain_coords.keys()]
+    coords1, coords2 = chain_coords[ch1], chain_coords[ch2]
+    plddt1, plddt2 = chain_plddt[ch1], chain_plddt[ch2]
+
+    #Calc 2-norm
+    mat = np.append(coords1, coords2,axis=0)
+    a_min_b = mat[:,np.newaxis,:] -mat[np.newaxis,:,:]
+    dists = np.sqrt(np.sum(a_min_b.T ** 2, axis=0)).T
+    l1 = len(coords1)
+    contact_dists = dists[:l1,l1:] #upper triangular --> first dim = chain 1
+    contacts = np.argwhere(contact_dists<=t)
+
+    if contacts.shape[0]<1:
+        pdockq=0
+    else:
+        #Get the average interface plDDT
+        avg_if_plddt = np.average(np.concatenate([plddt1[np.unique(contacts[:,0])], plddt2[np.unique(contacts[:,1])]]))
+        #Get the number of interface contacts
+        n_if_contacts = contacts.shape[0]
+        x = avg_if_plddt*np.log10(n_if_contacts)
+        pdockq = 0.724 / (1 + np.exp(-0.052*(x-152.611)))+0.018
+
+    return pdockq
```

### Comparing `alphapulldown-0.30.5/analysis_pipeline/create_notebook.py` & `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/create_notebook.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/analysis_pipeline/get_good_inter_pae.py` & `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/get_good_inter_pae.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,25 +34,28 @@
     """Returns mpDockQ if more than two chains otherwise return pDockQ"""
     pdb_path = os.path.join(work_dir,'ranked_0.pdb')
     pdb_chains, chain_coords, chain_CA_inds, chain_CB_inds = read_pdb(pdb_path)
     best_plddt = get_best_plddt(work_dir)
     plddt_per_chain = read_plddt(best_plddt,chain_CA_inds)
     complex_score,num_chains = score_complex(chain_coords,chain_CB_inds,plddt_per_chain)
     if complex_score is not None and num_chains>2:
-        mpDockq = calculate_mpDockQ(complex_score)
+        mpDockq_or_pdockq = calculate_mpDockQ(complex_score)
     elif complex_score is not None and num_chains==2:
-        mpDockq = calculate_pDockQ(complex_score)
+        mpDockq_or_pdockq = calc_pdockq(chain_coords,plddt_per_chain,t=8)
     else:
-        mpDockq = "None"
-    return mpDockq
+        mpDockq_or_pdockq = "None"
+    return mpDockq_or_pdockq
 
 def run_and_summarise_pi_score(workd_dir,jobs,surface_thres):
 
     """A function to calculate all predicted models' pi_scores and make a pandas df of the results"""
-    # os.makedirs(os.path.join(workd_dir,"pi_score_outputs"),exist_ok=True)
+    try:
+        os.remove(f"mkdir {workd_dir}/pi_score_outputs")
+    except:
+        pass
     subprocess.run(f"mkdir {workd_dir}/pi_score_outputs",shell=True,executable='/bin/bash')
     pi_score_outputs = os.path.join(workd_dir,"pi_score_outputs")
     for job in jobs:
         subdir = os.path.join(workd_dir,job)
         if not os.path.isfile(os.path.join(subdir,"ranked_0.pdb")):
             print(f"{job} failed. Cannot find ranked_0.pdb in {subdir}")
             sys.exit()
@@ -75,32 +78,37 @@
                 filtered_df[column] = ["None"]
             filtered_df['jobs'] = str(job)
             filtered_df['pi_score'] = "No interface detected"
         else:
             with open(os.path.join(subdir,pi_score_files[0]),'r') as f:
                 lines = [l for l in f.readlines() if "#" not in l]
                 if len(lines)>0:
-                    pi_score = float(lines[0].split(",")[-1])
+                    pi_score = pd.read_csv(os.path.join(subdir,pi_score_files[0]))
+                    pi_score['jobs']=str(job)
                 else:
-                    pi_score = 'SC:  mds: too many atoms'
+                    pi_score = pd.DataFrame.from_dict({"pi_score":['SC:  mds: too many atoms']})
                 f.close()
             filtered_df['jobs'] = str(job)
-            filtered_df['pi_score'] = pi_score
+            filtered_df=pd.merge(filtered_df,pi_score,on='jobs')
+            try:
+                filtered_df.drop(columns=["#PDB","pdb"," pvalue","chains","predicted_class"])
+            except:
+                pass
         
         output_df = pd.concat([output_df,filtered_df])
     return output_df
     
     
 
 def main(argv):
     jobs = os.listdir(FLAGS.output_dir)
     good_jobs = []
-    iptm_ptm = []
-    iptm = []
-    mpDockq_scores = []
+    iptm_ptm = list()
+    iptm = list()
+    mpDockq_scores = list()
     count = 0
     for job in jobs:
         logging.info(f"now processing {job}")
         if os.path.isfile(os.path.join(FLAGS.output_dir,job,'ranking_debug.json')):
             count=count +1
             result_subdir = os.path.join(FLAGS.output_dir,job)
             best_result_pkl = sorted([i for i in os.listdir(result_subdir) if "result_model_" in i])[0]
@@ -116,29 +124,26 @@
                 check = examine_inter_pae(pae_mtx,seqs,cutoff=FLAGS.cutoff)
                 mpDockq_score = obtain_mpdockq(os.path.join(FLAGS.output_dir,job))
                 if check:
                     good_jobs.append(str(job))
                     iptm_ptm.append(iptm_ptm_score)
                     iptm.append(iptm_score)
                     mpDockq_scores.append(mpDockq_score)
-
             logging.info(f"done for {job} {count} out of {len(jobs)} finished.")
+    other_measurements_df=pd.DataFrame.from_dict({
+        "jobs":good_jobs,
+        "iptm_ptm":iptm_ptm,
+        "iptm":iptm,
+        "mpDockQ/pDockQ":mpDockq_scores
+    })
     pi_score_df = run_and_summarise_pi_score(FLAGS.output_dir,good_jobs,FLAGS.surface_thres)
-    pi_score_df['iptm+ptm'] = iptm_ptm
-    pi_score_df['mpDockQ/pDockQ'] = mpDockq_scores
-    pi_score_df['iptm'] = iptm
+    pi_score_df=pd.merge(pi_score_df,other_measurements_df,on="jobs")
     columns = list(pi_score_df.columns.values)
     columns.pop(columns.index('jobs'))
     pi_score_df = pi_score_df[['jobs'] + columns]
     pi_score_df = pi_score_df.sort_values(by='iptm',ascending=False)
     
-    try:
-        pi_score_df = pi_score_df.drop(columns=['interface'])
-        pi_score_df = pi_score_df.drop(columns=[' pvalue'])
-        pi_score_df = pi_score_df.drop(columns=['pdb'])
-    except:
-        pass
     pi_score_df.to_csv(os.path.join(FLAGS.output_dir,"predictions_with_good_interpae.csv"),index=False)
     
 
 if __name__ =='__main__':
     app.run(main)
```

### Comparing `alphapulldown-0.30.5/analysis_pipeline/utils.py` & `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/alphafold/models.py` & `alphapulldown-0.30.6/colabfold/alphafold/models.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/alphafold/msa.py` & `alphapulldown-0.30.6/colabfold/alphafold/msa.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/batch.py` & `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/batch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/citations.py` & `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/citations.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/colabfold.py` & `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/colabfold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/colabfold_alphafold.py` & `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/colabfold_alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/download.py` & `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/download.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/mmseqs/merge_and_split_msas.py` & `alphapulldown-0.30.6/colabfold/mmseqs/merge_and_split_msas.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/mmseqs/search.py` & `alphapulldown-0.30.6/colabfold/mmseqs/search.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/mmseqs/split_msas.py` & `alphapulldown-0.30.6/colabfold/mmseqs/split_msas.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/pdb.py` & `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/pdb.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/plot.py` & `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/plot.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/colabfold/utils.py` & `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/stereo_chemical_props.txt` & `alphapulldown-0.30.6/stereo_chemical_props.txt`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/test/test_create_objects.py` & `alphapulldown-0.30.6/test/test_create_objects.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.5/test/test_predict_structure.py` & `alphapulldown-0.30.6/test/test_predict_structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,17 @@
     #Add setup that creates ampty output directory temprarily
     def setUp(self) -> None:
         #Call the setUp method of the parent class
         super().setUp()
 
         #Create a temporary directory for the output
         self.output_dir = tempfile.mkdtemp()
-        self.protein_lists = os.path.join(self.test_data_dir, "tiny_monomeric_features_homodimer.txt")
-        self.monomer_objects_dir = self.test_data_dir
+        self.example_data_dir = os.path.join(os.path.dirname(os.getcwd()),"example_data")
+        self.protein_lists = os.path.join(self.example_data_dir, "custom_mode.txt")
+        self.monomer_objects_dir = os.path.join(os.path.dirname(os.getcwd()),"example_data")
 
         #Get path of the alphapulldown module
         alphapulldown_path = alphapulldown.__path__[0]
         #join the path with the script name
         self.script_path = os.path.join(alphapulldown_path, "run_multimer_jobs.py")
         print(sys.executable)
         print(self.script_path)
@@ -95,19 +96,44 @@
         #Check if all files not empty
         for f in os.listdir(os.path.join(self.output_dir, dirname)):
             self.assertGreater(os.path.getsize(os.path.join(self.output_dir, dirname, f)), 0)
         #open the ranking_debug.json file and check if the number of models is 5
         with open(os.path.join(self.output_dir, dirname, "ranking_debug.json"), "r") as f:
             ranking_debug = json.load(f)
             self.assertEqual(len(ranking_debug["order"]), 5)
-            self.assertEqual(len(ranking_debug["iptm+ptm"]), 5)
-            #Check if order contains the correct models
-            self.assertSetEqual(set(ranking_debug["order"]), set(["model_1_multimer_v3_pred_0", "model_2_multimer_v3_pred_0", "model_3_multimer_v3_pred_0", "model_4_multimer_v3_pred_0", "model_5_multimer_v3_pred_0"]))
-            #Check if iptm+ptm contains the correct models
-            self.assertSetEqual(set(ranking_debug["iptm+ptm"].keys()), set(["model_1_multimer_v3_pred_0", "model_2_multimer_v3_pred_0", "model_3_multimer_v3_pred_0", "model_4_multimer_v3_pred_0", "model_5_multimer_v3_pred_0"]))
+            if "iptm+ptm" in ranking_debug:
+                expected_set = set(["model_1_multimer_v3_pred_0", "model_2_multimer_v3_pred_0", "model_3_multimer_v3_pred_0", "model_4_multimer_v3_pred_0", "model_5_multimer_v3_pred_0"])
+                self.assertEqual(len(ranking_debug["iptm+ptm"]), 5)
+                #Check if order contains the correct models
+                self.assertSetEqual(set(ranking_debug["order"]), expected_set)
+                #Check if iptm+ptm contains the correct models
+                self.assertSetEqual(set(ranking_debug["iptm+ptm"].keys()), expected_set)
+            elif "plddt" in ranking_debug:
+                expected_set = set(["model_1_pred_0", "model_2_pred_0", "model_3_pred_0", "model_4_pred_0", "model_5_pred_0"])
+                self.assertEqual(len(ranking_debug["plddt"]), 5)
+                self.assertSetEqual(set(ranking_debug["order"]), expected_set)
+                #Check if iptm+ptm contains the correct models
+                self.assertSetEqual(set(ranking_debug["plddt"].keys()), expected_set)
+
+    def testRunMonomer(self):
+        """test run monomer structure prediction"""
+        self.oligomer_state_file = os.path.join(os.path.dirname(os.getcwd()),"example_data/homooligomer_state.txt")
+        self.args = [
+            sys.executable,
+            self.script_path,
+            "--mode=homo-oligomer",
+            "--num_cycle=1",
+            "--num_predictions_per_model=1",
+            f"--output_path={self.output_dir}",
+            f"--data_dir={self.data_dir}",
+            f"--oligomer_state_file={self.oligomer_state_file}",
+            f"--monomer_objects_dir={self.monomer_objects_dir}"
+        ]
+        result = subprocess.run(self.args, capture_output=True, text=True)
+        self._runCommonTests(result)
 
     def _runAfterRelaxTests(self, result):
         dirname = os.listdir(self.output_dir)[0]
         #Check if the directory contains five files starting from relaxed and ending with .pdb
         self.assertEqual(len([f for f in os.listdir(os.path.join(self.output_dir, dirname)) if f.startswith("relaxed") and f.endswith(".pdb")]), 5)
 
     def testRunWithoutAmberRelax(self):
@@ -152,15 +178,15 @@
 
 
 #TODO: Add tests for other modeling examples subclassing the class above
 #TODO: Add tests that assess that the modeling results are as expected from native AlphaFold2
 #TODO: Add tests that assess that the ranking is correct
 #TODO: Add tests for features with and without templates
 #TODO: Add tests for the different modeling modes (pulldown, homo-oligomeric, all-against-all, custom)
-#TODO: Add tests for monomeric modeling
+#TODO: Add tests for monomeric modeling done
 
 class TestFunctions(_TestBase):
     def setUp(self):
         #Call the setUp method of the parent class
         super().setUp()
         
         from alphapulldown.utils import create_model_runners_and_random_seed
@@ -208,9 +234,22 @@
             results = json.load(f)
             #Get the expected score from the results
             expected_iptm_ptm = results["iptm+ptm"]
         self.assertDictEqual(ranking_confidences, expected_iptm_ptm)
 
     #TODO: Test monomeric runs (where score is pLDDT)
 
+class TestMonomerFunctions(_TestBase):
+    def setUp(self) -> None:
+        super().setUp()
+        from alphapulldown.utils import create_model_runners_and_random_seed
+        self.model_runners, random_seed = create_model_runners_and_random_seed(
+            "monomer",
+            3,
+            1,
+            self.data_dir,
+            1,
+        )
+
+
 if __name__ == '__main__':
     unittest.main()
```

