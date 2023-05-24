# Comparing `tmp/spacy-curated-transformers-0.1.0.tar.gz` & `tmp/spacy-curated-transformers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-curated-transformers-0.1.0.tar", last modified: Sun May  7 10:23:44 2023, max compression
+gzip compressed data, was "spacy-curated-transformers-0.1.1.tar", last modified: Wed May 24 06:33:00 2023, max compression
```

## Comparing `spacy-curated-transformers-0.1.0.tar` & `spacy-curated-transformers-0.1.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.585398 spacy-curated-transformers-0.1.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1285 2023-05-07 10:23:44.585398 spacy-curated-transformers-0.1.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      960 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     4230 2023-05-07 10:23:44.589398 spacy-curated-transformers-0.1.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      210 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.577397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      570 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4050 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/debug_pieces.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4697 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/quantize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3433 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      438 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24297 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/architectures.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1225 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19182 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/listeners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2704 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/output.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/pooling.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/remove_eos_bos.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4669 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7876 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10279 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17299 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/pipeline/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2222 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3177 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_hf_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2644 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_listeners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4556 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_pooling.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1425 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6181 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_transformer_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3194 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4325 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.585398 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17414 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/pipeline/test_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy
--rw-r--r--   0 vsts      (1001) docker     (122)      418 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/test_cli_app.py
--rw-r--r--   0 vsts      (1001) docker     (122)      794 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/test_torchscript_wrapper.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.585398 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3393 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4090 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1365 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2761 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7943 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4861 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)      138 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy-chars.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy.model
--rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.585398 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3612 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3713 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5394 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2500 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/sentencepiece_adapters.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3823 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5890 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2711 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1285 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3507 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     3466 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       91 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/zip-safe
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.625343 spacy-curated-transformers-0.1.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1285 2023-05-24 06:33:00.625343 spacy-curated-transformers-0.1.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      960 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     4241 2023-05-24 06:33:00.629343 spacy-curated-transformers-0.1.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      210 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.617343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      570 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4050 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/cli/debug_pieces.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4697 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/cli/quantize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3433 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      438 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24806 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1225 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19182 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2704 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/output.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/pooling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/remove_eos_bos.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4669 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7876 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10279 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17299 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/pipeline/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2340 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3393 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_hf_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2644 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4556 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_pooling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1425 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6191 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_transformer_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3194 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4325 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18102 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/test_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy
+-rw-r--r--   0 vsts      (1001) docker     (122)      418 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2513 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      794 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/test_torchscript_wrapper.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.625343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3393 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4090 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2716 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7943 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4907 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      138 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy-chars.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.625343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3623 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3713 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5394 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2500 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/sentencepiece_adapters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3834 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5901 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2711 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.617343 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1285 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3494 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     3466 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/zip-safe
```

### Comparing `spacy-curated-transformers-0.1.0/LICENSE` & `spacy-curated-transformers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/PKG-INFO` & `spacy-curated-transformers-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-curated-transformers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Curated transformer models
 Home-page: https://github.com/explosion/spacy-curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `spacy-curated-transformers-0.1.0/README.md` & `spacy-curated-transformers-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/setup.cfg` & `spacy-curated-transformers-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.1.0
+version = 0.1.1
 description = Curated transformer models
 url = https://github.com/explosion/spacy-curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
@@ -11,15 +11,15 @@
 
 [options]
 zip_safe = true
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
 	curated-transformers>=0.1.0,<0.2.0
-	cutlery>=0.0.3,<0.1.0
+	curated-tokenizers>=0.0.7,<0.1.0
 	spacy>=3.5.0,<4.0.0
 	torch>=1.12.0
 
 [options.entry_points]
 spacy_factories = 
 	curated_transformer = spacy_curated_transformers.pipeline.transformer:make_transformer
 spacy_architectures =
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/_compat.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/debug_pieces.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/cli/debug_pieces.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/quantize.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/cli/quantize.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/errors.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/errors.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/architectures.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/architectures.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,14 +137,15 @@
         transformer = _torchscript_encoder(
             model_max_length=model_max_length, padding_idx=padding_idx
         )
     else:
         encoder = AlbertEncoder(config)
         transformer = _pytorch_encoder(
             encoder,
+            hidden_width=hidden_width,
             mixed_precision=mixed_precision,
             grad_scaler_config=grad_scaler_config,
         )
 
     return build_transformer_model_v1(
         with_spans=with_spans,
         piece_encoder=piece_encoder,
@@ -237,14 +238,15 @@
         transformer = _torchscript_encoder(
             model_max_length=model_max_length, padding_idx=padding_idx
         )
     else:
         encoder = BertEncoder(config)
         transformer = _pytorch_encoder(
             encoder,
+            hidden_width=hidden_width,
             mixed_precision=mixed_precision,
             grad_scaler_config=grad_scaler_config,
         )
 
     return build_transformer_model_v1(
         with_spans=with_spans,
         piece_encoder=piece_encoder,
@@ -268,15 +270,17 @@
     layer_norm_eps: float = 1e-5,
     max_position_embeddings: int = 514,
     model_max_length: int = 512,
     num_attention_heads: int = 12,
     num_hidden_layers: int = 12,
     padding_idx: int = 1,
     type_vocab_size: int = 1,
+    mixed_precision: bool = False,
     torchscript=False,
+    grad_scaler_config: dict = SimpleFrozenDict(),
 ) -> TransformerModelT:
     """Construct a CamemBERT transformer model.
 
     vocab_size (int):
         Vocabulary size.
     with_spans (Callable):
         Callback that constructs a span generator model.
@@ -333,15 +337,20 @@
 
     if torchscript:
         transformer = _torchscript_encoder(
             model_max_length=model_max_length, padding_idx=padding_idx
         )
     else:
         encoder = RobertaEncoder(config)
-        transformer = _pytorch_encoder(encoder)
+        transformer = _pytorch_encoder(
+            encoder,
+            hidden_width=hidden_width,
+            mixed_precision=mixed_precision,
+            grad_scaler_config=grad_scaler_config,
+        )
 
     return build_transformer_model_v1(
         with_spans=with_spans,
         piece_encoder=piece_encoder,
         transformer=transformer,
     )
 
@@ -431,14 +440,15 @@
         transformer = _torchscript_encoder(
             model_max_length=model_max_length, padding_idx=padding_idx
         )
     else:
         encoder = RobertaEncoder(config)
         transformer = _pytorch_encoder(
             encoder,
+            hidden_width=hidden_width,
             mixed_precision=mixed_precision,
             grad_scaler_config=grad_scaler_config,
         )
 
     return build_transformer_model_v1(
         with_spans=with_spans,
         piece_encoder=piece_encoder,
@@ -531,14 +541,15 @@
         transformer = _torchscript_encoder(
             model_max_length=model_max_length, padding_idx=padding_idx
         )
     else:
         encoder = RobertaEncoder(config)
         transformer = _pytorch_encoder(
             encoder,
+            hidden_width=hidden_width,
             mixed_precision=mixed_precision,
             grad_scaler_config=grad_scaler_config,
         )
 
     return build_transformer_model_v1(
         with_spans=with_spans,
         piece_encoder=piece_encoder,
@@ -572,14 +583,15 @@
         init=transformer_model_init,
         layers=layers,
         refs=refs,  # type: ignore
         attrs={
             "replace_listener": _replace_listener,
             "replace_listener_cfg": _replace_listener_cfg,
         },
+        dims={"nO": transformer.get_dim("nO")},
     )
 
 
 def transformer_model_forward(
     model: TransformerModelT, docs: TransformerInT, is_train: bool
 ) -> Tuple[TransformerOutT, TransformerBackpropT]:
     Y, backprop_layer = model.layers[0](docs, is_train=is_train)
@@ -599,14 +611,15 @@
 ) -> Model:
     model.layers[0].initialize(X, Y)
     return model
 
 
 def _pytorch_encoder(
     encoder: CuratedEncoderT,
+    hidden_width: int,
     *,
     mixed_precision: bool = False,
     grad_scaler_config: dict = SimpleFrozenDict(),
 ) -> TorchTransformerModelT:
     if isinstance(grad_scaler_config, SimpleFrozenDict):
         # Create a new, mutable dict instance.
         grad_scaler_config = {}
@@ -621,14 +634,15 @@
             max_model_seq_len=encoder.max_seq_len,
             padding_idx=encoder.padding_idx,
         ),
         convert_outputs=_convert_outputs,
         mixed_precision=mixed_precision,
         grad_scaler=PyTorchGradScaler(**grad_scaler_config),
     )
+    model.set_dim("nO", hidden_width)
 
     # This attribute is set by the parent Pipe instance before each forward pass.
     model.attrs["_all_layer_outputs"] = True
 
     return model
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/hf_loader.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/hf_loader.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/listeners.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/listeners.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/output.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/output.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/pooling.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/pooling.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/remove_eos_bos.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/remove_eos_bos.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/scalar_weight.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/types.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/types.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/with_non_ws_tokens.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/with_strided_spans.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/pipeline/transformer.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/pipeline/transformer.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/conftest.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,14 +56,19 @@
     nlp = spacy.blank("en")
     doc1 = nlp.make_doc("I saw a girl with a telescope.")
     doc2 = nlp.make_doc("Today we will eat poké bowl.")
     return [doc1, doc2]
 
 
 @pytest.fixture
+def sentencepiece_toy_model_path():
+    return Path(__file__).parent / "tokenization" / "toy.model"
+
+
+@pytest.fixture
 def wordpiece_toy_model_path():
     return Path(__file__).parent / "tokenization" / "toy.wordpieces"
 
 
 @pytest.fixture
 def wordpiece_toy_encoder(wordpiece_toy_model_path):
     encoder = build_wordpiece_encoder_v1()
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_hf_model.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_hf_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,37 +8,52 @@
 from dataclasses import dataclass
 import pytest
 from thinc.api import get_torch_default_device
 from torch.nn import Module
 
 from spacy_curated_transformers._compat import has_hf_transformers, transformers
 from spacy_curated_transformers.models.architectures import _pytorch_encoder
-from spacy_curated_transformers.models.hf_loader import build_hf_transformer_encoder_loader_v1
+from spacy_curated_transformers.models.hf_loader import (
+    build_hf_transformer_encoder_loader_v1,
+)
 
 from ..util import torch_assertclose
 
 
 @dataclass
 class ModelConfig:
     config: BertConfig
     encoder: Callable[[BertConfig], Module]
     hf_model_name: str
+    hidden_width: int
 
 
 TEST_MODELS = [
-    ModelConfig(AlbertConfig(vocab_size=30000), AlbertEncoder, "albert-base-v2"),
-    ModelConfig(BertConfig(vocab_size=28996), BertEncoder, "bert-base-cased"),
-    ModelConfig(RobertaConfig(), RobertaEncoder, "roberta-base"),
-    ModelConfig(RobertaConfig(vocab_size=250002), RobertaEncoder, "xlm-roberta-base"),
+    ModelConfig(
+        AlbertConfig(vocab_size=30000),
+        AlbertEncoder,
+        "albert-base-v2",
+        hidden_width=768,
+    ),
+    ModelConfig(
+        BertConfig(vocab_size=28996), BertEncoder, "bert-base-cased", hidden_width=768
+    ),
+    ModelConfig(RobertaConfig(), RobertaEncoder, "roberta-base", hidden_width=768),
+    ModelConfig(
+        RobertaConfig(vocab_size=250002),
+        RobertaEncoder,
+        "xlm-roberta-base",
+        hidden_width=768,
+    ),
 ]
 
 
 def encoder_from_config(config: ModelConfig):
     encoder = config.encoder(config.config)
-    model = _pytorch_encoder(encoder)
+    model = _pytorch_encoder(encoder, config.hidden_width)
     model.init = build_hf_transformer_encoder_loader_v1(name=config.hf_model_name)
     return model
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("model_config", TEST_MODELS)
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_listeners.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_listeners.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_pooling.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_pooling.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_scalar_weight.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_scalar_weight.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_transformer_model.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_transformer_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import pytest
-from cutlery import SentencePieceProcessor
+from curated_tokenizers import SentencePieceProcessor
 from thinc.api import CupyOps, NumpyOps, Ragged, registry
 from thinc.compat import has_cupy
 
 from spacy_curated_transformers.models.architectures import (
     build_albert_transformer_model_v1,
     build_bert_transformer_model_v1,
     build_roberta_transformer_model_v1,
     build_xlmr_transformer_model_v1,
 )
-from spacy_curated_transformers.models.hf_loader import build_hf_transformer_encoder_loader_v1
+from spacy_curated_transformers.models.hf_loader import (
+    build_hf_transformer_encoder_loader_v1,
+)
 from spacy_curated_transformers.models.output import TransformerModelOutput
-from spacy_curated_transformers.models.with_strided_spans import build_with_strided_spans_v1
+from spacy_curated_transformers.models.with_strided_spans import (
+    build_with_strided_spans_v1,
+)
 from spacy_curated_transformers.tokenization import (
     build_bert_wordpiece_encoder_v1,
     build_byte_bpe_encoder_v1,
     build_hf_piece_encoder_loader_v1,
     build_sentencepiece_encoder_v1,
     build_xlmr_sentencepiece_encoder_v1,
 )
@@ -27,18 +31,16 @@
 
 OPS = [NumpyOps()]
 if has_cupy:
     OPS.append(CupyOps())
 
 
 @pytest.fixture
-def toy_model(test_dir):
-    return SentencePieceProcessor.from_file(
-        (str(test_dir / ".." / "tokenization" / "toy.model"))
-    )
+def toy_model(sentencepiece_toy_model_path):
+    return SentencePieceProcessor.from_file(sentencepiece_toy_model_path)
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("stride,window", [(2, 4), (96, 128)])
 @pytest.mark.parametrize("hf_model", [("xlm-roberta-base", 768, 250002)])
 def test_xlmr_model(sample_docs, stride, window, hf_model):
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_with_strided_spans.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/pipeline/test_transformer.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/test_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,31 @@
 
 from spacy_curated_transformers.models.architectures import (
     build_camembert_transformer_model_v1,
     build_xlmr_transformer_model_v1,
     build_bert_transformer_model_v1,
     build_roberta_transformer_model_v1,
 )
-from spacy_curated_transformers.models.hf_loader import build_hf_transformer_encoder_loader_v1
+from spacy_curated_transformers.models.hf_loader import (
+    build_hf_transformer_encoder_loader_v1,
+)
 from spacy_curated_transformers.models.with_strided_spans import (
     build_with_strided_spans_v1,
 )
 from spacy_curated_transformers.tokenization import (
     build_bert_wordpiece_encoder_v1,
     build_byte_bpe_encoder_v1,
     build_camembert_sentencepiece_encoder_v1,
     build_hf_piece_encoder_loader_v1,
     build_xlmr_sentencepiece_encoder_v1,
 )
 from spacy_curated_transformers.pipeline.transformer import make_transformer
+from spacy_curated_transformers.tokenization.sentencepiece_encoder import (
+    build_sentencepiece_encoder_loader_v1,
+)
 from spacy_curated_transformers.util import create_gradual_transformer_unfreezing
 from spacy_curated_transformers._compat import has_hf_transformers, transformers
 
 from ..util import torch_assertclose
 
 
 cfg_string_last_layer_listener = """
@@ -336,14 +341,32 @@
     ):
         torch_assertclose(
             hf_doc_encoding[:encoding_len][1:-1],
             torch.tensor(doc._.trf_data.last_hidden_layer_state.dataXd),
         )
 
 
+def test_empty_input(sentencepiece_toy_model_path):
+    nlp = spacy.blank("en")
+    model = build_xlmr_transformer_model_v1(
+        piece_encoder=build_xlmr_sentencepiece_encoder_v1(),
+        with_spans=build_with_strided_spans_v1(),
+        num_hidden_layers=2,
+        vocab_size=1000,
+        hidden_width=12,
+    )
+
+    model.get_ref("piece_encoder").init = build_sentencepiece_encoder_loader_v1(
+        path=sentencepiece_toy_model_path
+    )
+    model.initialize()
+    pipe = make_transformer(nlp, "transformer", model)
+    pipe(nlp.make_doc(""))
+
+
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 def test_xlmr_transformer_pipe_against_hf():
     nlp = spacy.blank("en")
     model = build_xlmr_transformer_model_v1(
         piece_encoder=build_xlmr_sentencepiece_encoder_v1(),
         with_spans=build_with_strided_spans_v1(),
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/test_torchscript_wrapper.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/test_torchscript_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_char_encoder.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_char_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import pytest
 from thinc.api import Ragged, registry, get_current_ops
 
 from spacy_curated_transformers.tokenization.sentencepiece_encoder import (
     build_sentencepiece_encoder_v1,
 )
-from spacy_curated_transformers.tokenization.hf_loader import build_hf_piece_encoder_loader_v1
+from spacy_curated_transformers.tokenization.hf_loader import (
+    build_hf_piece_encoder_loader_v1,
+)
 from spacy_curated_transformers._compat import has_hf_transformers
 
 
 @pytest.fixture
-def toy_model_path(test_dir):
-    return test_dir / "toy.model"
-
-
-@pytest.fixture
-def toy_encoder(toy_model_path):
+def toy_encoder(sentencepiece_toy_model_path):
     encoder = build_sentencepiece_encoder_v1()
     encoder.init = registry.model_loaders.get(
         "spacy-curated-transformers.SentencepieceLoader.v1"
-    )(path=toy_model_path)
+    )(path=sentencepiece_toy_model_path)
     encoder.initialize()
     return encoder
 
 
 def test_sentencepiece_encoder(toy_encoder, sample_docs):
     encoding = toy_encoder.predict(sample_docs)
     _check_toy_encoder(encoding)
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from cutlery import SentencePieceProcessor
+from curated_tokenizers import SentencePieceProcessor
 import pytest
 from thinc.api import Ragged, chain, Model, get_current_ops, NumpyOps
 from thinc.util import convert_recursive, is_cupy_array
 
 from spacy_curated_transformers._compat import has_hf_transformers, transformers
 from spacy_curated_transformers.tokenization.sentencepiece_encoder import (
     build_sentencepiece_encoder_v1,
@@ -11,22 +11,24 @@
 )
 from spacy_curated_transformers.tokenization.sentencepiece_adapters import (
     build_xlmr_adapter,
 )
 from spacy_curated_transformers.tokenization.wordpiece_encoder import (
     build_wordpiece_encoder_v1,
 )
-from spacy_curated_transformers.tokenization.hf_loader import build_hf_piece_encoder_loader_v1
+from spacy_curated_transformers.tokenization.hf_loader import (
+    build_hf_piece_encoder_loader_v1,
+)
 from spacy_curated_transformers.models.output import TransformerModelOutput
 from spacy_curated_transformers.models.remove_eos_bos import remove_bos_eos
 
 
 @pytest.fixture
-def toy_model(test_dir):
-    return SentencePieceProcessor.from_file(str(test_dir / "toy.model"))
+def toy_model(sentencepiece_toy_model_path):
+    return SentencePieceProcessor.from_file(str(sentencepiece_toy_model_path))
 
 
 @pytest.fixture
 def toy_encoder(toy_model):
     encoder = build_xlmr_sentencepiece_encoder_v1()
     encoder.get_ref("encoder").attrs["sentencepiece_processor"] = toy_model
     return encoder
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy-merges.txt` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy-merges.txt`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy-vocab.json` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy-vocab.json`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy.model` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy.model`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy.wordpieces` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy.wordpieces`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/__init__.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/bbpe_encoder.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/bbpe_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Callable, Optional, Tuple
 from pathlib import Path
 
-from cutlery import ByteBPEProcessor
+from curated_tokenizers import ByteBPEProcessor
 import srsly
 from thinc.api import Model, Ragged, deserialize_attr, serialize_attr
 
 from .types import (
     Tok2PiecesBackpropT,
     Tok2PiecesInT,
     Tok2PiecesModelT,
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/char_encoder.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/char_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/hf_loader.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/hf_loader.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/sentencepiece_adapters.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/sentencepiece_adapters.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/sentencepiece_encoder.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/sentencepiece_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable, Optional, Tuple
 from pathlib import Path
-from cutlery import SentencePieceProcessor
+from curated_tokenizers import SentencePieceProcessor
 from thinc.api import Model, Ragged, chain, deserialize_attr, serialize_attr
 
 from .sentencepiece_adapters import build_camembert_adapter, build_xlmr_adapter
 
 from .types import (
     Tok2PiecesBackpropT,
     Tok2PiecesInT,
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/types.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/types.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/wordpiece_encoder.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/wordpiece_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, List, Optional, Tuple
 from pathlib import Path
 import unicodedata
 
-from cutlery import WordPieceProcessor
+from curated_tokenizers import WordPieceProcessor
 from thinc.api import Model, Ragged, deserialize_attr, serialize_attr
 
 from .types import (
     Tok2PiecesBackpropT,
     Tok2PiecesInT,
     Tok2PiecesModelT,
     Tok2PiecesOutT,
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers/util.py` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers/util.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/PKG-INFO` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-curated-transformers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Curated transformer models
 Home-page: https://github.com/explosion/spacy-curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/SOURCES.txt` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 spacy_curated_transformers/models/with_strided_spans.py
 spacy_curated_transformers/pipeline/__init__.py
 spacy_curated_transformers/pipeline/transformer.py
 spacy_curated_transformers/tests/__init__.py
 spacy_curated_transformers/tests/conftest.py
 spacy_curated_transformers/tests/enable_gpu.py
 spacy_curated_transformers/tests/test_cli_app.py
+spacy_curated_transformers/tests/test_registry.py
 spacy_curated_transformers/tests/test_torchscript_wrapper.py
 spacy_curated_transformers/tests/util.py
 spacy_curated_transformers/tests/models/__init__.py
 spacy_curated_transformers/tests/models/test_hf_model.py
 spacy_curated_transformers/tests/models/test_listeners.py
 spacy_curated_transformers/tests/models/test_pooling.py
 spacy_curated_transformers/tests/models/test_scalar_weight.py
@@ -47,15 +48,14 @@
 spacy_curated_transformers/tests/models/test_with_strided_spans.py
 spacy_curated_transformers/tests/pipeline/__init__.py
 spacy_curated_transformers/tests/pipeline/test_transformer.py
 spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy
 spacy_curated_transformers/tests/tokenization/__init__.py
 spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
 spacy_curated_transformers/tests/tokenization/test_char_encoder.py
-spacy_curated_transformers/tests/tokenization/test_registry.py
 spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
 spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
 spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
 spacy_curated_transformers/tests/tokenization/toy-chars.txt
 spacy_curated_transformers/tests/tokenization/toy-merges.txt
 spacy_curated_transformers/tests/tokenization/toy-vocab.json
 spacy_curated_transformers/tests/tokenization/toy.model
```

### Comparing `spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/entry_points.txt` & `spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

