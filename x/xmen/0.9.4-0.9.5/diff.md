# Comparing `tmp/xmen-0.9.4.tar.gz` & `tmp/xmen-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmen-0.9.4.tar", max compression
+gzip compressed data, was "xmen-0.9.5.tar", max compression
```

## Comparing `xmen-0.9.4.tar` & `xmen-0.9.5.tar`

### file list

```diff
@@ -1,63 +1,62 @@
--rw-r--r--   0        0        0    11357 2023-05-15 13:45:24.103799 xmen-0.9.4/LICENSE
--rw-r--r--   0        0        0     9460 2023-05-16 18:34:48.659967 xmen-0.9.4/README.md
--rw-r--r--   0        0        0     1095 2023-05-16 20:24:10.337691 xmen-0.9.4/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-15 13:45:25.657861 xmen-0.9.4/xmen/__init__.py
--rw-r--r--   0        0        0     5068 2023-05-15 13:45:25.694863 xmen-0.9.4/xmen/analysis.py
--rw-r--r--   0        0        0        0 2023-05-15 13:45:25.753865 xmen-0.9.4/xmen/cli/__init__.py
--rw-r--r--   0        0        0     7675 2023-05-16 19:30:33.033752 xmen-0.9.4/xmen/cli/cli.py
--rw-r--r--   0        0        0     2730 2023-05-15 13:45:25.777866 xmen-0.9.4/xmen/cli/dict.py
--rw-r--r--   0        0        0     1880 2023-05-15 13:45:25.780866 xmen-0.9.4/xmen/cli/index.py
--rw-r--r--   0        0        0     6381 2023-05-15 13:45:25.804867 xmen-0.9.4/xmen/cli/utils.py
--rw-r--r--   0        0        0      933 2023-05-15 13:45:25.945873 xmen-0.9.4/xmen/confhelper.py
--rw-r--r--   0        0        0      139 2023-05-15 13:45:25.977874 xmen-0.9.4/xmen/data/__init__.py
--rw-r--r--   0        0        0     4237 2023-05-16 11:07:29.583327 xmen-0.9.4/xmen/data/dataloaders.py
--rw-r--r--   0        0        0     2612 2023-05-15 13:45:26.087879 xmen-0.9.4/xmen/data/indexed_dataset.py
--rw-r--r--   0        0        0     1826 2023-05-15 13:45:26.092879 xmen-0.9.4/xmen/data/integrations.py
--rw-r--r--   0        0        0     3228 2023-05-15 13:45:26.105879 xmen-0.9.4/xmen/data/util.py
--rw-r--r--   0        0        0    15482 2023-05-16 19:28:38.528152 xmen-0.9.4/xmen/evaluation.py
--rw-r--r--   0        0        0    18453 2023-05-16 10:44:55.440426 xmen-0.9.4/xmen/ext/neleval/annotation.py
--rw-r--r--   0        0        0    10874 2023-05-16 10:44:55.511428 xmen-0.9.4/xmen/ext/neleval/configs.py
--rw-r--r--   0        0        0     5429 2023-05-16 10:45:41.591263 xmen-0.9.4/xmen/ext/neleval/document.py
--rw-r--r--   0        0        0    10926 2023-05-16 10:44:55.603432 xmen-0.9.4/xmen/ext/neleval/evaluate.py
--rw-r--r--   0        0        0     5788 2023-05-16 10:44:55.635434 xmen-0.9.4/xmen/ext/neleval/prepare.py
--rw-r--r--   0        0        0     1086 2023-05-15 13:45:26.162881 xmen-0.9.4/xmen/ext/sapbert/LICENSE
--rw-r--r--   0        0        0     4663 2023-05-15 13:45:26.179882 xmen-0.9.4/xmen/ext/sapbert/README.md
--rw-r--r--   0        0        0      146 2023-05-15 13:45:26.202883 xmen-0.9.4/xmen/ext/sapbert/requirements.txt
--rwxr-xr-x   0        0        0      307 2023-05-15 13:45:26.250885 xmen-0.9.4/xmen/ext/sapbert/src/__init__.py
--rwxr-xr-x   0        0        0    11519 2023-05-16 19:26:23.559730 xmen-0.9.4/xmen/ext/sapbert/src/data_loader.py
--rwxr-xr-x   0        0        0     4898 2023-05-15 13:45:26.277886 xmen-0.9.4/xmen/ext/sapbert/src/metric_learning.py
--rwxr-xr-x   0        0        0     6626 2023-05-15 13:45:26.301887 xmen-0.9.4/xmen/ext/sapbert/src/model_wrapper.py
--rw-r--r--   0        0        0      533 2023-05-15 13:45:26.317888 xmen-0.9.4/xmen/ext/sapbert/train/.gitignore
--rwxr-xr-x   0        0        0      466 2023-05-15 13:45:26.320888 xmen-0.9.4/xmen/ext/sapbert/train/pretrain.sh
--rwxr-xr-x   0        0        0    10943 2023-05-15 13:45:26.338889 xmen-0.9.4/xmen/ext/sapbert/train/train.py
--rwxr-xr-x   0        0        0      522 2023-05-15 13:45:26.363890 xmen-0.9.4/xmen/ext/sapbert/train/xling_train.sh
--rw-r--r--   0        0        0     7632 2023-05-16 11:07:29.587327 xmen-0.9.4/xmen/ext/scispacy/umls_utils.py
--rw-r--r--   0        0        0     6328 2023-05-15 13:45:26.398891 xmen-0.9.4/xmen/knowledge_base.py
--rw-r--r--   0        0        0     1628 2023-05-15 13:45:26.428892 xmen-0.9.4/xmen/linkers/__init__.py
--rw-r--r--   0        0        0     6218 2023-05-15 13:45:26.447893 xmen-0.9.4/xmen/linkers/ensemble.py
--rw-r--r--   0        0        0     8770 2023-05-15 13:45:26.488895 xmen-0.9.4/xmen/linkers/faiss_indexer.py
--rw-r--r--   0        0        0    10317 2023-05-15 13:45:26.512895 xmen-0.9.4/xmen/linkers/sap_bert_linker.py
--rw-r--r--   0        0        0     9454 2023-05-15 13:45:26.518896 xmen-0.9.4/xmen/linkers/tf_idf_ngram_linker.py
--rw-r--r--   0        0        0      916 2023-05-15 13:45:26.567898 xmen-0.9.4/xmen/linkers/util.py
--rw-r--r--   0        0        0      510 2023-05-15 13:45:26.587899 xmen-0.9.4/xmen/log.py
--rw-r--r--   0        0        0      202 2023-05-15 13:45:26.653901 xmen-0.9.4/xmen/preprocessing/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-15 13:45:26.714904 xmen-0.9.4/xmen/preprocessing/abbrevations.py
--rw-r--r--   0        0        0      698 2023-05-15 13:45:26.718904 xmen-0.9.4/xmen/preprocessing/filter.py
--rw-r--r--   0        0        0     1308 2023-05-15 13:45:26.775906 xmen-0.9.4/xmen/preprocessing/merge_concepts.py
--rw-r--r--   0        0        0     2385 2023-05-16 19:24:43.663717 xmen-0.9.4/xmen/preprocessing/retired_cuis.py
--rw-r--r--   0        0        0     2497 2023-05-15 13:45:26.842909 xmen-0.9.4/xmen/preprocessing/sampling.py
--rw-r--r--   0        0        0     2093 2023-05-15 13:45:26.845909 xmen-0.9.4/xmen/preprocessing/semantic_groups.py
--rw-r--r--   0        0        0     2334 2023-05-15 13:45:26.862910 xmen-0.9.4/xmen/preprocessing/semantic_types.py
--rw-r--r--   0        0        0      452 2023-05-15 13:45:26.881910 xmen-0.9.4/xmen/reranking/__init__.py
--rw-r--r--   0        0        0    20467 2023-05-16 10:45:41.619264 xmen-0.9.4/xmen/reranking/cross_encoder.py
--rw-r--r--   0        0        0     9852 2023-05-15 13:45:26.951913 xmen-0.9.4/xmen/reranking/list_wise.py
--rw-r--r--   0        0        0     5179 2023-05-15 13:45:26.990915 xmen-0.9.4/xmen/reranking/multiple_choice_util.py
--rw-r--r--   0        0        0     4914 2023-05-15 13:45:27.008916 xmen-0.9.4/xmen/reranking/ranking_util.py
--rw-r--r--   0        0        0     1160 2023-05-15 13:45:27.045917 xmen-0.9.4/xmen/reranking/rule_based.py
--rw-r--r--   0        0        0    14602 2023-05-15 13:45:27.051917 xmen-0.9.4/xmen/reranking/scored_cross_encoder.py
--rw-r--r--   0        0        0        0 2023-05-15 13:45:27.128920 xmen-0.9.4/xmen/resources/.gitkeep
--rw-r--r--   0        0        0       70 2023-05-15 13:45:27.132920 xmen-0.9.4/xmen/resources/Readme.md
--rw-r--r--   0        0        0     5743 2023-05-15 13:45:27.176922 xmen-0.9.4/xmen/resources/SemGroups-v03.txt
--rw-r--r--   0        0        0     5468 2023-05-15 13:45:27.211923 xmen-0.9.4/xmen/resources/SemGroups.txt
--rw-r--r--   0        0        0    10177 2023-05-16 11:07:29.619328 xmen-0.9.4/xmen/umls.py
--rw-r--r--   0        0        0    10843 1970-01-01 00:00:00.000000 xmen-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 13:45:24.103799 xmen-0.9.5/LICENSE
+-rw-r--r--   0        0        0     9422 2023-05-24 13:46:51.648440 xmen-0.9.5/README.md
+-rw-r--r--   0        0        0     1061 2023-05-24 13:46:51.811443 xmen-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-15 13:45:25.657861 xmen-0.9.5/xmen/__init__.py
+-rw-r--r--   0        0        0     5068 2023-05-15 13:45:25.694863 xmen-0.9.5/xmen/analysis.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:45:25.753865 xmen-0.9.5/xmen/cli/__init__.py
+-rw-r--r--   0        0        0     7713 2023-05-16 20:37:32.742833 xmen-0.9.5/xmen/cli/cli.py
+-rw-r--r--   0        0        0     2730 2023-05-15 13:45:25.777866 xmen-0.9.5/xmen/cli/dict.py
+-rw-r--r--   0        0        0     1868 2023-05-24 13:46:51.862444 xmen-0.9.5/xmen/cli/index.py
+-rw-r--r--   0        0        0     6381 2023-05-15 13:45:25.804867 xmen-0.9.5/xmen/cli/utils.py
+-rw-r--r--   0        0        0      933 2023-05-15 13:45:25.945873 xmen-0.9.5/xmen/confhelper.py
+-rw-r--r--   0        0        0      438 2023-05-24 13:46:51.901445 xmen-0.9.5/xmen/data/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-24 13:46:51.921446 xmen-0.9.5/xmen/data/abbrevations.py
+-rw-r--r--   0        0        0     4208 2023-05-16 20:37:32.693831 xmen-0.9.5/xmen/data/dataloaders.py
+-rw-r--r--   0        0        0      698 2023-05-24 13:46:51.965447 xmen-0.9.5/xmen/data/filter.py
+-rw-r--r--   0        0        0     2612 2023-05-15 13:45:26.087879 xmen-0.9.5/xmen/data/indexed_dataset.py
+-rw-r--r--   0        0        0     1826 2023-05-15 13:45:26.092879 xmen-0.9.5/xmen/data/integrations.py
+-rw-r--r--   0        0        0     1308 2023-05-24 13:46:51.969447 xmen-0.9.5/xmen/data/merge_concepts.py
+-rw-r--r--   0        0        0     2386 2023-05-24 13:46:51.983447 xmen-0.9.5/xmen/data/retired_cuis.py
+-rw-r--r--   0        0        0     2497 2023-05-24 13:46:52.000447 xmen-0.9.5/xmen/data/sampling.py
+-rw-r--r--   0        0        0     2093 2023-05-24 13:46:52.039448 xmen-0.9.5/xmen/data/semantic_groups.py
+-rw-r--r--   0        0        0     2577 2023-05-24 13:46:52.043448 xmen-0.9.5/xmen/data/semantic_types.py
+-rw-r--r--   0        0        0     3228 2023-05-15 13:45:26.105879 xmen-0.9.5/xmen/data/util.py
+-rw-r--r--   0        0        0    15490 2023-05-16 20:37:32.795835 xmen-0.9.5/xmen/evaluation.py
+-rw-r--r--   0        0        0    18453 2023-05-16 10:44:55.440426 xmen-0.9.5/xmen/ext/neleval/annotation.py
+-rw-r--r--   0        0        0    10874 2023-05-16 10:44:55.511428 xmen-0.9.5/xmen/ext/neleval/configs.py
+-rw-r--r--   0        0        0     5429 2023-05-16 10:45:41.591263 xmen-0.9.5/xmen/ext/neleval/document.py
+-rw-r--r--   0        0        0    10926 2023-05-16 10:44:55.603432 xmen-0.9.5/xmen/ext/neleval/evaluate.py
+-rw-r--r--   0        0        0     5788 2023-05-16 10:44:55.635434 xmen-0.9.5/xmen/ext/neleval/prepare.py
+-rw-r--r--   0        0        0     1086 2023-05-15 13:45:26.162881 xmen-0.9.5/xmen/ext/sapbert/LICENSE
+-rw-r--r--   0        0        0     4663 2023-05-15 13:45:26.179882 xmen-0.9.5/xmen/ext/sapbert/README.md
+-rw-r--r--   0        0        0      146 2023-05-15 13:45:26.202883 xmen-0.9.5/xmen/ext/sapbert/requirements.txt
+-rwxr-xr-x   0        0        0      307 2023-05-15 13:45:26.250885 xmen-0.9.5/xmen/ext/sapbert/src/__init__.py
+-rwxr-xr-x   0        0        0    11519 2023-05-16 19:26:23.559730 xmen-0.9.5/xmen/ext/sapbert/src/data_loader.py
+-rwxr-xr-x   0        0        0     4898 2023-05-15 13:45:26.277886 xmen-0.9.5/xmen/ext/sapbert/src/metric_learning.py
+-rwxr-xr-x   0        0        0     6626 2023-05-15 13:45:26.301887 xmen-0.9.5/xmen/ext/sapbert/src/model_wrapper.py
+-rw-r--r--   0        0        0      533 2023-05-15 13:45:26.317888 xmen-0.9.5/xmen/ext/sapbert/train/.gitignore
+-rwxr-xr-x   0        0        0      466 2023-05-15 13:45:26.320888 xmen-0.9.5/xmen/ext/sapbert/train/pretrain.sh
+-rwxr-xr-x   0        0        0    10943 2023-05-15 13:45:26.338889 xmen-0.9.5/xmen/ext/sapbert/train/train.py
+-rwxr-xr-x   0        0        0      522 2023-05-15 13:45:26.363890 xmen-0.9.5/xmen/ext/sapbert/train/xling_train.sh
+-rw-r--r--   0        0        0     7632 2023-05-16 11:07:29.587327 xmen-0.9.5/xmen/ext/scispacy/umls_utils.py
+-rw-r--r--   0        0        0     6328 2023-05-24 13:46:52.063449 xmen-0.9.5/xmen/kb.py
+-rw-r--r--   0        0        0     1628 2023-05-15 13:45:26.428892 xmen-0.9.5/xmen/linkers/__init__.py
+-rw-r--r--   0        0        0     6218 2023-05-15 13:45:26.447893 xmen-0.9.5/xmen/linkers/ensemble.py
+-rw-r--r--   0        0        0     8770 2023-05-15 13:45:26.488895 xmen-0.9.5/xmen/linkers/faiss_indexer.py
+-rw-r--r--   0        0        0    10317 2023-05-15 13:45:26.512895 xmen-0.9.5/xmen/linkers/sap_bert_linker.py
+-rw-r--r--   0        0        0     9442 2023-05-24 13:46:52.069449 xmen-0.9.5/xmen/linkers/tf_idf_ngram_linker.py
+-rw-r--r--   0        0        0      916 2023-05-15 13:45:26.567898 xmen-0.9.5/xmen/linkers/util.py
+-rw-r--r--   0        0        0      510 2023-05-15 13:45:26.587899 xmen-0.9.5/xmen/log.py
+-rw-r--r--   0        0        0      452 2023-05-15 13:45:26.881910 xmen-0.9.5/xmen/reranking/__init__.py
+-rw-r--r--   0        0        0    20467 2023-05-16 10:45:41.619264 xmen-0.9.5/xmen/reranking/cross_encoder.py
+-rw-r--r--   0        0        0     9852 2023-05-15 13:45:26.951913 xmen-0.9.5/xmen/reranking/list_wise.py
+-rw-r--r--   0        0        0     5179 2023-05-15 13:45:26.990915 xmen-0.9.5/xmen/reranking/multiple_choice_util.py
+-rw-r--r--   0        0        0     4914 2023-05-15 13:45:27.008916 xmen-0.9.5/xmen/reranking/ranking_util.py
+-rw-r--r--   0        0        0     1160 2023-05-15 13:45:27.045917 xmen-0.9.5/xmen/reranking/rule_based.py
+-rw-r--r--   0        0        0    14602 2023-05-15 13:45:27.051917 xmen-0.9.5/xmen/reranking/scored_cross_encoder.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:45:27.128920 xmen-0.9.5/xmen/resources/.gitkeep
+-rw-r--r--   0        0        0       70 2023-05-15 13:45:27.132920 xmen-0.9.5/xmen/resources/Readme.md
+-rw-r--r--   0        0        0     5743 2023-05-15 13:45:27.176922 xmen-0.9.5/xmen/resources/SemGroups-v03.txt
+-rw-r--r--   0        0        0     5468 2023-05-15 13:45:27.211923 xmen-0.9.5/xmen/resources/SemGroups.txt
+-rw-r--r--   0        0        0    10168 2023-05-16 20:37:32.742833 xmen-0.9.5/xmen/umls.py
+-rw-r--r--   0        0        0    10805 1970-01-01 00:00:00.000000 xmen-0.9.5/PKG-INFO
```

### Comparing `xmen-0.9.4/LICENSE` & `xmen-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/README.md` & `xmen-0.9.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[![Build](https://github.com/hpi-dhc/xmen/actions/workflows/python-app.yml/badge.svg)](https://github.com/hpi-dhc/xmen/actions/workflows/python-app.yml)
 [![pypi Version](https://img.shields.io/pypi/v/xmen)](https://pypi.org/project/xmen/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 # ✖️MEN
 
 xMEN is an extensible toolkit for Cross-lingual (**x**) **M**edical **E**ntity **N**ormalization.
 Through its compatibility with the [BigBIO (BigScience Biomedical)](https://github.com/bigscience-workshop/biomedical) framework, it can be used out-of-the box to run experiments with many open biomedical datasets. It can also be easily integrated with existing Named Entity Recognition (NER) pipelines.
@@ -231,23 +232,22 @@
 
 When labelled training data is available, a trainable reranker can improve ranking of candidate lists a lot.
 
 To train a cross-encoder, first create a dataset of mention / candidate pairs:
 
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
-from xmen.knowledge_base import load_kb
+from xmen.kb import load_kb
 
 # Load a KB from a pre-computed dictionary (jsonl) to obtain synonyms for concept encoding
 kb = load_kb('path/to/my/dictionary.jsonl')
 
 candidates = linker.predict_batch(dataset) # obtain prediction from candidate generator (see above)
-context_length = 128 # set to adjust context length for mention encoding, more context causes larger memory footprint
 
-cross_enc_ds = CrossEncoderReranker.prepare_data(candidates, dataset, kb, context_length)
+cross_enc_ds = CrossEncoderReranker.prepare_data(candidates, dataset, kb)
 ```
 
 Then you can use this dataset to train a supervised reranking model:
 
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
 
@@ -269,19 +269,19 @@
 
 TODO
 
 ## 💡 Pre- and Post-Processing
 
 We support various optional components for transforming input data and result sets:
 
-- [Sampling](xmen/preprocessing/sampling.py)
-- [Abbrevation expansion](xmen/preprocessing/abbrevations.py)
-- [Filtering by UMLS semantic groups](xmen/preprocessing/semantic_groups.py)
-- [Filtering by UMLS semantic types](xmen/preprocessing/semantic_types.py)
-- [Replacement of retired CUIS](xmen/preprocessing/retired_cuis.py)
+- [Sampling](xmen/data/sampling.py)
+- [Abbrevation expansion](xmen/data/abbrevations.py)
+- [Filtering by UMLS semantic groups](xmen/data/semantic_groups.py)
+- [Filtering by UMLS semantic types](xmen/data/semantic_types.py)
+- [Replacement of retired CUIS](xmen/data/retired_cuis.py)
 
 ## 📊 Evaluation
 
 xMEN provides implementations of common entity linking metrics (e.g., a wrapper for [neleval](https://github.com/wikilinks/neleval))
 
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
```

### Comparing `xmen-0.9.4/pyproject.toml` & `xmen-0.9.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xmen"
-version = "0.9.4"
+version = "0.9.5"
 description = "An extensible toolkit for Cross-lingual (x) Medical Entity Normalization."
 license = "Apache-2.0"
 authors = ["Florian Borchert <florian.borchert@hpi.de>"]
 readme = "README.md"
 repository = "https://github.com/hpi-dhc/xmen"
 
 [tool.poetry.scripts]
@@ -27,15 +27,15 @@
 scispacy = "^0.5.2"
 sentence-transformers = "^2.2.2"
 faiss-gpu = {version = "^1.7.1", markers = 'sys_platform == "linux"'}
 faiss-cpu = {version = "^1.7.1", markers = 'sys_platform != "linux"'}
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.0"
-black = {extras = ["jupyter"], version = "^22.12.0"}
+black = "^22.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `xmen-0.9.4/xmen/analysis.py` & `xmen-0.9.5/xmen/analysis.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/cli/cli.py` & `xmen-0.9.5/xmen/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,17 @@
         write_path = output / "index" / "sapbert"
         if is_sapbert_selected and has_correct_keys(cfg, required_key) and can_write(write_path, overwrite):
             # check for GPUs
             if torch.cuda.is_available():
                 logger.info(f"CUDA is available. Running on GPU with ID {gpu_id}. To select another, use --gpu-id.")
             else:
                 gpu_id = -1
-                logger.warning("CUDA is not available on this system. Running on CPU. This can take considerably longer.")
+                logger.warning(
+                    "CUDA is not available on this system. Running on CPU. This can take considerably longer."
+                )
             logger.info("Building SapBERT indices.")
             build_sapbert(cfg, output, dict, gpu_id)
         else:
             logger.info("Skipping SapBERT indices.")
 
     else:
         logger.info(
```

### Comparing `xmen-0.9.4/xmen/cli/dict.py` & `xmen-0.9.5/xmen/cli/dict.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/cli/index.py` & `xmen-0.9.5/xmen/cli/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from omegaconf import DictConfig
 from ..log import logger
-from xmen.knowledge_base import create_flat_term_dict
+from xmen.kb import create_flat_term_dict
 from xmen.linkers import TFIDFNGramLinker, SapBERTLinker
 from pathlib import Path
 import torch
 
 
 def build_ngram(cfg: DictConfig, work_dir: Path, dict_dir: Path):
     """Build an N-Gram index for the given dictionary directory and store it in the working directory.
```

### Comparing `xmen-0.9.4/xmen/cli/utils.py` & `xmen-0.9.5/xmen/cli/utils.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/confhelper.py` & `xmen-0.9.5/xmen/confhelper.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/data/dataloaders.py` & `xmen-0.9.5/xmen/data/dataloaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,40 +108,35 @@
     return _load_bigbio_dataset(
         ["distemist_linking_bigbio_kb"],
         "distemist",
         lambda _: "es",
         splits=["train"],
     )
 
-def _load_bigbio_dataset(
-    config_names: List[str],
-    dataset_name: str,
-    lang_mapper,
-    splits
-):
+
+def _load_bigbio_dataset(config_names: List[str], dataset_name: str, lang_mapper, splits):
     """
     Loads a biomedical dataset and returns a concatenated dataset for the specified splits.
 
     Args:
     - config_names (List[str]): A list of configuration names to load the dataset for.
     - dataset_name (str): The name of the dataset to load.
     - lang_mapper (function): A function that maps configuration names to language codes.
     - splits (List[str]): A list of splits to concatenate the dataset for.
 
     Returns:
     - output (datasets.DatasetDict): A concatenated dataset for the specified splits.
     """
     # TODO: implement loading all available configs for a dataset
     assert config_names is not None, "Not implemented"
-        
-    
+
     ds_map = {c: datasets.load_dataset(f"bigscience-biomedical/{dataset_name}", c) for c in config_names}
     ds = []
     for conf, ds_dict in ds_map.items():
         for k in ds_dict.keys():
             ds_dict[k] = ds_dict[k].add_column("corpus_id", [conf] * len(ds_dict[k]))
             ds_dict[k] = ds_dict[k].add_column("lang", [lang_mapper(conf)] * len(ds_dict[k]))
         ds.append(ds_dict)
     output = datasets.dataset_dict.DatasetDict()
     for s in splits:
         output[s] = datasets.concatenate_datasets([d[s] for d in ds])
-    return output
+    return output
```

### Comparing `xmen-0.9.4/xmen/data/indexed_dataset.py` & `xmen-0.9.5/xmen/data/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/data/integrations.py` & `xmen-0.9.5/xmen/data/integrations.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/data/util.py` & `xmen-0.9.5/xmen/data/util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/evaluation.py` & `xmen-0.9.5/xmen/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,15 +397,16 @@
                     annotations.append(anno)
                 else:
                     for cand in candidates:
                         anno = Annotation(unit_id, start, end, [cand])
                         annotations.append(anno)
         yield Document(unit_id, annotations)
 
-def evaluate_at_k(ground_truth, pred, eval_k=[1,2,4,8,16,32,64], silent=False):
+
+def evaluate_at_k(ground_truth, pred, eval_k=[1, 2, 4, 8, 16, 32, 64], silent=False):
     """
     Runs evaluation for different values of k (number of candidates)
 
     Args:
     - ground_truth: ground truth annotations
     - pred: predicted candidates
     - eval_k: different values of k to evaluate
@@ -414,10 +415,10 @@
     Returns:
     - a dictionary of evaluation results for each k
     """
     res = {}
     for ki in eval_k:
         eval_res = evaluate(ground_truth, pred, top_k_predictions=ki)
         if not silent:
-            print(f'Perf@{ki}', eval_res["strict"]['recall'])
+            print(f"Perf@{ki}", eval_res["strict"]["recall"])
         res[ki] = eval_res
-    return res
+    return res
```

### Comparing `xmen-0.9.4/xmen/ext/neleval/annotation.py` & `xmen-0.9.5/xmen/ext/neleval/annotation.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/neleval/configs.py` & `xmen-0.9.5/xmen/ext/neleval/configs.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/neleval/document.py` & `xmen-0.9.5/xmen/ext/neleval/document.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/neleval/evaluate.py` & `xmen-0.9.5/xmen/ext/neleval/evaluate.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/neleval/prepare.py` & `xmen-0.9.5/xmen/ext/neleval/prepare.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/sapbert/LICENSE` & `xmen-0.9.5/xmen/ext/sapbert/LICENSE`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/sapbert/README.md` & `xmen-0.9.5/xmen/ext/sapbert/README.md`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/sapbert/src/data_loader.py` & `xmen-0.9.5/xmen/ext/sapbert/src/data_loader.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/sapbert/src/metric_learning.py` & `xmen-0.9.5/xmen/ext/sapbert/src/metric_learning.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/sapbert/src/model_wrapper.py` & `xmen-0.9.5/xmen/ext/sapbert/src/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/sapbert/train/.gitignore` & `xmen-0.9.5/xmen/ext/sapbert/train/.gitignore`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/sapbert/train/train.py` & `xmen-0.9.5/xmen/ext/sapbert/train/train.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/sapbert/train/xling_train.sh` & `xmen-0.9.5/xmen/ext/sapbert/train/xling_train.sh`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/ext/scispacy/umls_utils.py` & `xmen-0.9.5/xmen/ext/scispacy/umls_utils.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/knowledge_base.py` & `xmen-0.9.5/xmen/kb.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/linkers/__init__.py` & `xmen-0.9.5/xmen/linkers/__init__.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/linkers/ensemble.py` & `xmen-0.9.5/xmen/linkers/ensemble.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/linkers/faiss_indexer.py` & `xmen-0.9.5/xmen/linkers/faiss_indexer.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/linkers/sap_bert_linker.py` & `xmen-0.9.5/xmen/linkers/sap_bert_linker.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/linkers/tf_idf_ngram_linker.py` & `xmen-0.9.5/xmen/linkers/tf_idf_ngram_linker.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 
 import warnings
 
 from typing import Union, List
 
 from xmen.linkers import EntityLinker, logger
-from xmen.knowledge_base import CompositeKnowledgebase
+from xmen.kb import CompositeKnowledgebase
 
 from scispacy.candidate_generation import (
     CandidateGenerator,
     load_approximate_nearest_neighbours_index,
     LinkerPaths,
     create_tfidf_ann_index,
 )
```

### Comparing `xmen-0.9.4/xmen/linkers/util.py` & `xmen-0.9.5/xmen/linkers/util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/preprocessing/abbrevations.py` & `xmen-0.9.5/xmen/data/abbrevations.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/preprocessing/filter.py` & `xmen-0.9.5/xmen/data/filter.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/preprocessing/merge_concepts.py` & `xmen-0.9.5/xmen/data/merge_concepts.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/preprocessing/retired_cuis.py` & `xmen-0.9.5/xmen/data/retired_cuis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from xmen.ext.scispacy.umls_utils import read_umls_file_headers
 
+
 class CUIReplacer:
     """
     A class that replaces retired CUIs in normalized entities with their replacements.
 
     Args:
     - umls_meta_path (str): The path to the UMLS metadata directory
```

### Comparing `xmen-0.9.4/xmen/preprocessing/sampling.py` & `xmen-0.9.5/xmen/data/sampling.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/preprocessing/semantic_groups.py` & `xmen-0.9.5/xmen/data/semantic_groups.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/preprocessing/semantic_types.py` & `xmen-0.9.5/xmen/data/semantic_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 class SemanticTypeFilter:
     """
     A class to filter out examples based on semantic types.
 
     Args:
     - type_to_tui (Dict): A dictionary that maps a semantic type to a set of TUIs.
     - kb: A knowledge base object.
+    - expand_types: Whether to expand the given TUIs based on the semantic type tree
 
     Attributes:
     - type_to_tui (Dict): A dictionary that maps a semantic type to a set of TUIs.
     - kb: A knowledge base object.
     - tree: A semantic type tree object.
+    - expand_types: flag indicating whether to expand semantic types
     """
 
-    def __init__(self, type_to_tui: Dict, kb):
+    def __init__(self, type_to_tui: Dict, kb, expand_types=False):
         self.type_to_tui = type_to_tui
         self.kb = kb
         self.tree = get_sem_type_tree()
+        self.expand_types = expand_types
 
     def __getstate__(self):
         return {}
 
     def get_tuis(self, cui):
         """
         Returns the set of TUIs associated with a given CUI.
@@ -32,28 +35,29 @@
         - cui (str): A CUI string.
 
         Returns:
         - tuis (set): A set of TUIs associated with the given CUI.
         """
         return self.kb.cui_to_entity[cui].types
 
-    def filter_semantic_groups(self, example):
+    def filter_semantic_types(self, example):
         """
         Filters out normalized entities from the given example that are not associated with any of the valid TUIs.
 
         Args:
         - example (dict): A dictionary representing a single example, with keys "text" and "entities".
 
         Returns:
         - filtered_example (dict): A dictionary representing the filtered example, with key "entities".
         """
         entities = example["entities"]
         for e in entities:
             valid_tuis = self.type_to_tui[e["type"]]
-            valid_tuis = expand_tuis(valid_tuis, get_sem_type_tree)
+            if self.expand_types:
+                valid_tuis = expand_tuis(valid_tuis, self.tree)
             filtered = []
             for n in e["normalized"]:
                 concept_tuis = self.get_tuis(n["db_id"])
                 if any([t for t in concept_tuis if t in valid_tuis]):
                     filtered.append(n)
             e["normalized"] = filtered
         return {"entities": entities}
@@ -64,8 +68,8 @@
 
         Args:
         - ds (tf.data.Dataset): A dataset of examples.
 
         Returns:
         - transformed_ds (tf.data.Dataset): A transformed dataset of examples.
         """
-        return ds.map(lambda e: self.filter_semantic_groups(e), load_from_cache_file=False)
+        return ds.map(lambda e: self.filter_semantic_types(e), load_from_cache_file=False)
```

### Comparing `xmen-0.9.4/xmen/reranking/cross_encoder.py` & `xmen-0.9.5/xmen/reranking/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/reranking/list_wise.py` & `xmen-0.9.5/xmen/reranking/list_wise.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/reranking/multiple_choice_util.py` & `xmen-0.9.5/xmen/reranking/multiple_choice_util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/reranking/ranking_util.py` & `xmen-0.9.5/xmen/reranking/ranking_util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/reranking/rule_based.py` & `xmen-0.9.5/xmen/reranking/rule_based.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/reranking/scored_cross_encoder.py` & `xmen-0.9.5/xmen/reranking/scored_cross_encoder.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/resources/SemGroups-v03.txt` & `xmen-0.9.5/xmen/resources/SemGroups-v03.txt`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/resources/SemGroups.txt` & `xmen-0.9.5/xmen/resources/SemGroups.txt`

 * *Files identical despite different names*

### Comparing `xmen-0.9.4/xmen/umls.py` & `xmen-0.9.5/xmen/umls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from xmen.ext.scispacy.umls_utils import read_umls_file_headers, read_umls_concepts, read_umls_types, read_umls_definitions
+from xmen.ext.scispacy.umls_utils import (
+    read_umls_file_headers,
+    read_umls_concepts,
+    read_umls_types,
+    read_umls_definitions,
+)
 from scispacy import umls_semantic_type_tree
 from scispacy.linking_utils import DEFAULT_UMLS_TYPES_PATH
 from langcodes import Language
 import pandas as pd
 from pathlib import Path
 import os
 from .log import logger
@@ -214,17 +219,15 @@
     if not sabs:
         sabs = [None]
     for source in sabs:
         logger.info(
             f'>> Reading concepts from {"all sources" if not source else source} and {"all languages" if not langs else f"languages: {langs}"}'
         )
         for lang in langs if langs else [None]:
-            read_umls_concepts(
-                meta_path, concept_details, source=source, lang=lang, non_suppressed=non_suppressed_only
-            )
+            read_umls_concepts(meta_path, concept_details, source=source, lang=lang, non_suppressed=non_suppressed_only)
 
     logger.info(">> Reading types ... ")
     read_umls_types(meta_path, concept_details)
 
     if semantic_groups:
         logger.info(f"> Number of concepts before semantic group filtering: {len(concept_details)}")
         concept_details = filter_semantic_groups(semantic_groups, concept_details, semantic_group_file_version)
```

### Comparing `xmen-0.9.4/PKG-INFO` & `xmen-0.9.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmen
-Version: 0.9.4
+Version: 0.9.5
 Summary: An extensible toolkit for Cross-lingual (x) Medical Entity Normalization.
 Home-page: https://github.com/hpi-dhc/xmen
 License: Apache-2.0
 Author: Florian Borchert
 Author-email: florian.borchert@hpi.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,14 +27,15 @@
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: sentencepiece (>=0.1.96,<0.2.0)
 Requires-Dist: torch (>=1.13.0,<2.0.0)
 Requires-Dist: transformers (>=4.17.0,<5.0.0)
 Project-URL: Repository, https://github.com/hpi-dhc/xmen
 Description-Content-Type: text/markdown
 
+[![Build](https://github.com/hpi-dhc/xmen/actions/workflows/python-app.yml/badge.svg)](https://github.com/hpi-dhc/xmen/actions/workflows/python-app.yml)
 [![pypi Version](https://img.shields.io/pypi/v/xmen)](https://pypi.org/project/xmen/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 # ✖️MEN
 
 xMEN is an extensible toolkit for Cross-lingual (**x**) **M**edical **E**ntity **N**ormalization.
 Through its compatibility with the [BigBIO (BigScience Biomedical)](https://github.com/bigscience-workshop/biomedical) framework, it can be used out-of-the box to run experiments with many open biomedical datasets. It can also be easily integrated with existing Named Entity Recognition (NER) pipelines.
@@ -264,23 +265,22 @@
 
 When labelled training data is available, a trainable reranker can improve ranking of candidate lists a lot.
 
 To train a cross-encoder, first create a dataset of mention / candidate pairs:
 
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
-from xmen.knowledge_base import load_kb
+from xmen.kb import load_kb
 
 # Load a KB from a pre-computed dictionary (jsonl) to obtain synonyms for concept encoding
 kb = load_kb('path/to/my/dictionary.jsonl')
 
 candidates = linker.predict_batch(dataset) # obtain prediction from candidate generator (see above)
-context_length = 128 # set to adjust context length for mention encoding, more context causes larger memory footprint
 
-cross_enc_ds = CrossEncoderReranker.prepare_data(candidates, dataset, kb, context_length)
+cross_enc_ds = CrossEncoderReranker.prepare_data(candidates, dataset, kb)
 ```
 
 Then you can use this dataset to train a supervised reranking model:
 
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
 
@@ -302,19 +302,19 @@
 
 TODO
 
 ## 💡 Pre- and Post-Processing
 
 We support various optional components for transforming input data and result sets:
 
-- [Sampling](xmen/preprocessing/sampling.py)
-- [Abbrevation expansion](xmen/preprocessing/abbrevations.py)
-- [Filtering by UMLS semantic groups](xmen/preprocessing/semantic_groups.py)
-- [Filtering by UMLS semantic types](xmen/preprocessing/semantic_types.py)
-- [Replacement of retired CUIS](xmen/preprocessing/retired_cuis.py)
+- [Sampling](xmen/data/sampling.py)
+- [Abbrevation expansion](xmen/data/abbrevations.py)
+- [Filtering by UMLS semantic groups](xmen/data/semantic_groups.py)
+- [Filtering by UMLS semantic types](xmen/data/semantic_types.py)
+- [Replacement of retired CUIS](xmen/data/retired_cuis.py)
 
 ## 📊 Evaluation
 
 xMEN provides implementations of common entity linking metrics (e.g., a wrapper for [neleval](https://github.com/wikilinks/neleval))
 
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
```

