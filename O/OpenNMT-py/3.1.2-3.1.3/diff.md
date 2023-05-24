# Comparing `tmp/OpenNMT-py-3.1.2.tar.gz` & `tmp/OpenNMT-py-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenNMT-py-3.1.2.tar", last modified: Wed May 10 17:39:07 2023, max compression
+gzip compressed data, was "OpenNMT-py-3.1.3.tar", last modified: Wed May 24 10:41:35 2023, max compression
```

## Comparing `OpenNMT-py-3.1.2.tar` & `OpenNMT-py-3.1.3.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.110291 OpenNMT-py-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.098291 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-10 17:39:07.110291 OpenNMT-py-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.098291 OpenNMT-py-3.1.2/onmt/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.098291 OpenNMT-py-3.1.2/onmt/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/average_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/build_vocab.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/release_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5186 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.098291 OpenNMT-py-3.1.2/onmt/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/decoders/cnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/decoders/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/decoders/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    26303 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/decoders/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.098291 OpenNMT-py-3.1.2/onmt/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/cnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/ggnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/mean_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/rnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.102291 OpenNMT-py-3.1.2/onmt/inputters/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/inputters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/inputters/dynamic_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/inputters/inputter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/inputters/text_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/inputters/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.102291 OpenNMT-py-3.1.2/onmt/models/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/models/model_saver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.102291 OpenNMT-py-3.1.2/onmt/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/average_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/conv_multi_step_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/copy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/global_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/multi_headed_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/position_ffn.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/rmsnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/sparse_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/sparse_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    24384 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/stacked_rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/structured_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/util_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/weight_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/opts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.102291 OpenNMT-py-3.1.2/onmt/scorers/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/scorers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/scorers/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/scorers/scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/scorers/ter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.106291 OpenNMT-py-3.1.2/onmt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    28824 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_copy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    18449 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_greedy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_structured_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_subword_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_text_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_translation_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/utils_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/train_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    23568 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.106291 OpenNMT-py-3.1.2/onmt/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/bart.py
--rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/docify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/fuzzymatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/inlinetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/uppercase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.106291 OpenNMT-py-3.1.2/onmt/translate/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19338 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/decode_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/greedy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/penalties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/process_zh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    37183 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/translation_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    42702 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.110291 OpenNMT-py-3.1.2/onmt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/cnn_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/earlystopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    28164 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/report_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/rnn_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/scoring_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 17:39:07.110291 OpenNMT-py-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.644069 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.644069 OpenNMT-py-3.1.3/onmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.644069 OpenNMT-py-3.1.3/onmt/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1651 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/average_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/build_vocab.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/release_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5237 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.648069 OpenNMT-py-3.1.3/onmt/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/decoders/cnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/decoders/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/decoders/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26060 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/decoders/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.648069 OpenNMT-py-3.1.3/onmt/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/cnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/ggnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/mean_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/rnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.648069 OpenNMT-py-3.1.3/onmt/inputters/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/inputters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/inputters/dynamic_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/inputters/inputter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/inputters/text_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/inputters/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.648069 OpenNMT-py-3.1.3/onmt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/models/model_saver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.652069 OpenNMT-py-3.1.3/onmt/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/alibi_position_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/average_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/conv_multi_step_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/copy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/global_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/multi_headed_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/position_ffn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/rmsnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/sparse_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/sparse_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/stacked_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/structured_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/util_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/weight_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52017 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/opts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.652069 OpenNMT-py-3.1.3/onmt/scorers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/scorers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/scorers/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/scorers/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/scorers/ter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.652069 OpenNMT-py-3.1.3/onmt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30982 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_copy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_greedy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_structured_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_subword_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10008 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_translation_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/utils_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/train_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23544 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/onmt/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/bart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/docify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/fuzzymatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/inlinetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24101 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/uppercase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/onmt/translate/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/decode_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/greedy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/penalties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/process_zh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36570 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/translation_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41387 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/onmt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/cnn_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/earlystopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28025 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/report_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/rnn_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/scoring_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/setup.py
```

### Comparing `OpenNMT-py-3.1.2/LICENSE.md` & `OpenNMT-py-3.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.2/OpenNMT_py.egg-info/PKG-INFO` & `OpenNMT-py-3.1.3/OpenNMT_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenNMT-py
-Version: 3.1.2
+Version: 3.1.3
 Summary: A python implementation of OpenNMT
 Project-URL: Documentation, http://opennmt.net/OpenNMT-py/
 Project-URL: Forum, http://forum.opennmt.net/
 Project-URL: Gitter, https://gitter.im/OpenNMT/OpenNMT-py
 Project-URL: Source, https://github.com/OpenNMT/OpenNMT-py/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `OpenNMT-py-3.1.2/OpenNMT_py.egg-info/SOURCES.txt` & `OpenNMT-py-3.1.3/OpenNMT_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE.md
 README.md
+setup.cfg
 setup.py
 OpenNMT_py.egg-info/PKG-INFO
 OpenNMT_py.egg-info/SOURCES.txt
 OpenNMT_py.egg-info/dependency_links.txt
 OpenNMT_py.egg-info/entry_points.txt
 OpenNMT_py.egg-info/requires.txt
 OpenNMT_py.egg-info/top_level.txt
@@ -37,14 +38,15 @@
 onmt/inputters/inputter.py
 onmt/inputters/text_corpus.py
 onmt/inputters/text_utils.py
 onmt/models/__init__.py
 onmt/models/model.py
 onmt/models/model_saver.py
 onmt/modules/__init__.py
+onmt/modules/alibi_position_bias.py
 onmt/modules/average_attn.py
 onmt/modules/conv_multi_step_attention.py
 onmt/modules/copy_generator.py
 onmt/modules/embeddings.py
 onmt/modules/gate.py
 onmt/modules/global_attention.py
 onmt/modules/lora.py
```

### Comparing `OpenNMT-py-3.1.2/PKG-INFO` & `OpenNMT-py-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenNMT-py
-Version: 3.1.2
+Version: 3.1.3
 Summary: A python implementation of OpenNMT
 Project-URL: Documentation, http://opennmt.net/OpenNMT-py/
 Project-URL: Forum, http://forum.opennmt.net/
 Project-URL: Gitter, https://gitter.im/OpenNMT/OpenNMT-py
 Project-URL: Source, https://github.com/OpenNMT/OpenNMT-py/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `OpenNMT-py-3.1.2/README.md` & `OpenNMT-py-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.2/onmt/bin/average_models.py` & `OpenNMT-py-3.1.3/onmt/bin/average_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,48 +6,54 @@
 def average_models(model_files, fp32=False):
     vocab = None
     opt = None
     avg_model = None
     avg_generator = None
 
     for i, model_file in enumerate(model_files):
-        m = torch.load(model_file, map_location='cpu')
-        model_weights = m['model']
-        generator_weights = m['generator']
+        m = torch.load(model_file, map_location="cpu")
+        model_weights = m["model"]
+        generator_weights = m["generator"]
 
         if fp32:
             for k, v in model_weights.items():
                 model_weights[k] = v.float()
             for k, v in generator_weights.items():
                 generator_weights[k] = v.float()
 
         if i == 0:
-            vocab, opt = m['vocab'], m['opt']
+            vocab, opt = m["vocab"], m["opt"]
             avg_model = model_weights
             avg_generator = generator_weights
         else:
-            for (k, v) in avg_model.items():
+            for k, v in avg_model.items():
                 avg_model[k].mul_(i).add_(model_weights[k]).div_(i + 1)
 
-            for (k, v) in avg_generator.items():
+            for k, v in avg_generator.items():
                 avg_generator[k].mul_(i).add_(generator_weights[k]).div_(i + 1)
 
-    final = {"vocab": vocab, "opt": opt, "optim": None,
-             "generator": avg_generator, "model": avg_model}
+    final = {
+        "vocab": vocab,
+        "opt": opt,
+        "optim": None,
+        "generator": avg_generator,
+        "model": avg_model,
+    }
     return final
 
 
 def main():
     parser = argparse.ArgumentParser(description="")
-    parser.add_argument("-models", "-m", nargs="+", required=True,
-                        help="List of models")
-    parser.add_argument("-output", "-o", required=True,
-                        help="Output file")
-    parser.add_argument("-fp32", "-f", action="store_true",
-                        help="Cast params to float32")
+    parser.add_argument(
+        "-models", "-m", nargs="+", required=True, help="List of models"
+    )
+    parser.add_argument("-output", "-o", required=True, help="Output file")
+    parser.add_argument(
+        "-fp32", "-f", action="store_true", help="Cast params to float32"
+    )
     opt = parser.parse_args()
 
     final = average_models(opt.models, opt.fp32)
     torch.save(final, opt.output)
 
 
 if __name__ == "__main__":
```

### Comparing `OpenNMT-py-3.1.2/onmt/bin/build_vocab.py` & `OpenNMT-py-3.1.3/onmt/bin/build_vocab.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,71 +22,76 @@
 def write_files_from_queues(sample_path, queues):
     """
     Standalone process that reads data from
     queues in order and write to sample files.
     """
     os.makedirs(sample_path, exist_ok=True)
     for c_name in queues.keys():
-        dest_base = os.path.join(
-            sample_path, "{}.{}".format(c_name, CorpusName.SAMPLE))
-        with open(dest_base + ".src", 'w', encoding="utf-8") as f_src,\
-                open(dest_base + ".tgt", 'w', encoding="utf-8") as f_tgt:
+        dest_base = os.path.join(sample_path, "{}.{}".format(c_name, CorpusName.SAMPLE))
+        with open(dest_base + ".src", "w", encoding="utf-8") as f_src, open(
+            dest_base + ".tgt", "w", encoding="utf-8"
+        ) as f_tgt:
             while True:
                 _next = False
                 for q in queues[c_name]:
                     item = q.get()
                     if item == "blank":
                         continue
                     if item == "break":
                         _next = True
                         break
                     _, src_line, tgt_line = item
-                    f_src.write(src_line + '\n')
-                    f_tgt.write(tgt_line + '\n')
+                    f_src.write(src_line + "\n")
+                    f_tgt.write(tgt_line + "\n")
                 if _next:
                     break
 
 
 def build_sub_vocab(corpora, transforms, opts, n_sample, stride, offset):
     """Build vocab on (strided) subpart of the data."""
     sub_counter_src = Counter()
     sub_counter_tgt = Counter()
     sub_counter_src_feats = [Counter() for _ in range(opts.n_src_feats)]
     datasets_iterables = build_corpora_iters(
-        corpora, transforms, opts.data,
+        corpora,
+        transforms,
+        opts.data,
         skip_empty_level=opts.skip_empty_level,
-        stride=stride, offset=offset)
+        stride=stride,
+        offset=offset,
+    )
     for c_name, c_iter in datasets_iterables.items():
         for i, item in enumerate(c_iter):
             maybe_example = process(CorpusTask.TRAIN, [item])
             if maybe_example is not None:
                 maybe_example = maybe_example[0]
             else:
                 if opts.dump_samples:
                     build_sub_vocab.queues[c_name][offset].put("blank")
                 continue
-            src_line, tgt_line = (maybe_example['src']['src'],
-                                  maybe_example['tgt']['tgt'])
-            sub_counter_src.update(src_line.split(' '))
-            sub_counter_tgt.update(tgt_line.split(' '))
+            src_line, tgt_line = (
+                maybe_example["src"]["src"],
+                maybe_example["tgt"]["tgt"],
+            )
+            sub_counter_src.update(src_line.split(" "))
+            sub_counter_tgt.update(tgt_line.split(" "))
 
-            if 'feats' in maybe_example['src']:
-                src_feats_lines = maybe_example['src']['feats']
+            if "feats" in maybe_example["src"]:
+                src_feats_lines = maybe_example["src"]["feats"]
                 for k in range(opts.n_src_feats):
-                    sub_counter_src_feats[k].update(
-                        src_feats_lines[k].split(' '))
+                    sub_counter_src_feats[k].update(src_feats_lines[k].split(" "))
             else:
                 src_feats_lines = []
 
             if opts.dump_samples:
-                src_pretty_line = append_features_to_text(
-                    src_line, src_feats_lines)
+                src_pretty_line = append_features_to_text(src_line, src_feats_lines)
                 build_sub_vocab.queues[c_name][offset].put(
-                    (i, src_pretty_line, tgt_line))
-            if n_sample > 0 and ((i+1) * stride + offset) >= n_sample:
+                    (i, src_pretty_line, tgt_line)
+                )
+            if n_sample > 0 and ((i + 1) * stride + offset) >= n_sample:
                 if opts.dump_samples:
                     build_sub_vocab.queues[c_name][offset].put("break")
                 break
         if opts.dump_samples:
             build_sub_vocab.queues[c_name][offset].put("break")
     return sub_counter_src, sub_counter_tgt, sub_counter_src_feats
 
@@ -103,67 +108,76 @@
         logger.info(f"n_sample={n_sample}: Build vocab on full datasets.")
     elif n_sample > 0:
         logger.info(f"Build vocab on {n_sample} transformed examples/corpus.")
     else:
         raise ValueError(f"n_sample should > 0 or == -1, get {n_sample}.")
 
     if opts.dump_samples:
-        logger.info("The samples on which the vocab is built will be "
-                    "dumped to disk. It may slow down the process.")
+        logger.info(
+            "The samples on which the vocab is built will be "
+            "dumped to disk. It may slow down the process."
+        )
     corpora = get_corpora(opts, task=CorpusTask.TRAIN)
     counter_src = Counter()
     counter_tgt = Counter()
     counter_src_feats = [Counter() for _ in range(opts.n_src_feats)]
 
-    queues = {c_name: [mp.Queue(opts.vocab_sample_queue_size)
-                       for i in range(opts.num_threads)]
-              for c_name in corpora.keys()}
-    sample_path = os.path.join(
-        os.path.dirname(opts.save_data), CorpusName.SAMPLE)
+    queues = {
+        c_name: [
+            mp.Queue(opts.vocab_sample_queue_size) for i in range(opts.num_threads)
+        ]
+        for c_name in corpora.keys()
+    }
+    sample_path = os.path.join(os.path.dirname(opts.save_data), CorpusName.SAMPLE)
     if opts.dump_samples:
         write_process = mp.Process(
-            target=write_files_from_queues,
-            args=(sample_path, queues),
-            daemon=True)
+            target=write_files_from_queues, args=(sample_path, queues), daemon=True
+        )
         write_process.start()
     with mp.Pool(opts.num_threads, init_pool, [queues]) as p:
         func = partial(
-            build_sub_vocab, corpora, transforms,
-            opts, n_sample, opts.num_threads)
+            build_sub_vocab, corpora, transforms, opts, n_sample, opts.num_threads
+        )
         for sub_counter_src, sub_counter_tgt, sub_counter_src_feats in p.imap(
-                func, range(0, opts.num_threads)):
+            func, range(0, opts.num_threads)
+        ):
             counter_src.update(sub_counter_src)
             counter_tgt.update(sub_counter_tgt)
             for i in range(opts.n_src_feats):
                 counter_src_feats[i].update(sub_counter_src_feats[i])
     if opts.dump_samples:
         write_process.join()
     return counter_src, counter_tgt, counter_src_feats
 
 
 def ingest_tokens(opts, transforms, n_sample, learner, stride, offset):
     def _mp_ingest(data):
         func = partial(process, CorpusName.TRAIN)
         chunk = len(data) // opts.num_threads
         with mp.Pool(opts.num_threads) as pool:
-            buckets = pool.map(func, [data[i * chunk: (i + 1) * chunk]
-                                      for i in range(0, opts.num_threads)])
+            buckets = pool.map(
+                func,
+                [data[i * chunk : (i + 1) * chunk] for i in range(0, opts.num_threads)],
+            )
         for bucket in buckets:
             for ex in bucket:
                 if ex is not None:
-                    src_line, tgt_line = (ex['src']['src'],
-                                          ex['tgt']['tgt'])
+                    src_line, tgt_line = (ex["src"]["src"], ex["tgt"]["tgt"])
                     learner.ingest(src_line)
                     learner.ingest(tgt_line)
 
     corpora = get_corpora(opts, task=CorpusTask.TRAIN)
     datasets_iterables = build_corpora_iters(
-        corpora, transforms, opts.data,
+        corpora,
+        transforms,
+        opts.data,
         skip_empty_level=opts.skip_empty_level,
-        stride=stride, offset=offset)
+        stride=stride,
+        offset=offset,
+    )
     to_ingest = []
     for c_name, c_iter in datasets_iterables.items():
         for i, item in enumerate(c_iter):
             if n_sample >= 0 and i >= n_sample:
                 break
             if len(to_ingest) >= MAXBUCKETSIZE:
                 _mp_ingest(to_ingest)
@@ -171,20 +185,20 @@
             to_ingest.append(item)
         _mp_ingest(to_ingest)
 
 
 def make_learner(tokenization_type, symbols):
     if tokenization_type == "bpe":
         # BPE training
-        learner = pyonmttok.BPELearner(tokenizer=None,
-                                       symbols=symbols)
+        learner = pyonmttok.BPELearner(tokenizer=None, symbols=symbols)
     elif tokenization_type == "sentencepiece":
         # SentencePiece training
-        learner = pyonmttok.SentencePieceLearner(vocab_size=symbols,
-                                                 character_coverage=0.98)
+        learner = pyonmttok.SentencePieceLearner(
+            vocab_size=symbols, character_coverage=0.98
+        )
     return learner
 
 
 def build_vocab_main(opts):
     """Apply transforms to samples of specified data and build vocab from it.
 
     Transforms that need vocab will be disabled in this.
@@ -193,49 +207,49 @@
     ```
     <tok_0>\t<count_0>
     <tok_1>\t<count_1>
     ```
     """
 
     ArgumentParser.validate_prepare_opts(opts, build_vocab_only=True)
-    assert opts.n_sample == -1 or opts.n_sample > 1, \
-        f"Illegal argument n_sample={opts.n_sample}."
+    assert (
+        opts.n_sample == -1 or opts.n_sample > 1
+    ), f"Illegal argument n_sample={opts.n_sample}."
 
     logger = init_logger()
     set_random_seed(opts.seed, False)
     transforms_cls = get_transforms_cls(opts._all_transform)
 
     if opts.learn_subwords:
         logger.info(f"Ingesting {opts.src_subword_type} model from corpus")
-        learner = make_learner(opts.src_subword_type,
-                               opts.learn_subwords_size)
+        learner = make_learner(opts.src_subword_type, opts.learn_subwords_size)
         if opts.src_subword_model is not None:
             tok_path = opts.src_subword_model
         else:
             data_dir = os.path.split(opts.save_data)[0]
             if not os.path.exists(data_dir):
                 os.makedirs(data_dir)
-            tok_path = os.path.join(
-                data_dir, f"{opts.src_subword_type}.model")
+            tok_path = os.path.join(data_dir, f"{opts.src_subword_type}.model")
         save_opts = copy.deepcopy(opts)
-        opts.src_subword_type = 'none'
-        opts.tgt_subword_type = 'none'
+        opts.src_subword_type = "none"
+        opts.tgt_subword_type = "none"
         opts.src_onmttok_kwargs["joiner_annotate"] = False
         opts.tgt_onmttok_kwargs["joiner_annotate"] = False
         transforms = make_transforms(opts, transforms_cls, None)
         ingest_tokens(opts, transforms, opts.n_sample, learner, 1, 0)
         logger.info(f"Learning {tok_path} model, patience")
         learner.learn(tok_path)
         opts = save_opts
 
     transforms = make_transforms(opts, transforms_cls, None)
 
     logger.info(f"Counter vocab from {opts.n_sample} samples.")
     src_counter, tgt_counter, src_feats_counter = build_vocab(
-        opts, transforms, n_sample=opts.n_sample)
+        opts, transforms, n_sample=opts.n_sample
+    )
 
     logger.info(f"Counters src: {len(src_counter)}")
     logger.info(f"Counters tgt: {len(tgt_counter)}")
     for i, feat_counter in enumerate(src_feats_counter):
         logger.info(f"Counters src feat_{i}: {len(feat_counter)}")
 
     def save_counter(counter, save_path):
@@ -254,20 +268,20 @@
         save_counter(tgt_counter, opts.tgt_vocab)
 
     for i, c in enumerate(src_feats_counter):
         save_counter(c, f"{opts.src_vocab}_feat{i}")
 
 
 def _get_parser():
-    parser = ArgumentParser(description='build_vocab.py')
+    parser = ArgumentParser(description="build_vocab.py")
     dynamic_prepare_opts(parser, build_vocab_only=True)
     return parser
 
 
 def main():
     parser = _get_parser()
     opts, unknown = parser.parse_known_args()
     build_vocab_main(opts)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `OpenNMT-py-3.1.2/onmt/bin/release_model.py` & `OpenNMT-py-3.1.3/onmt/bin/release_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 #!/usr/bin/env python
 import argparse
 import torch
 
 
 def main():
     parser = argparse.ArgumentParser(
-        description="Release an OpenNMT-py model for inference")
-    parser.add_argument("--model", "-m",
-                        help="The model path", required=True)
-    parser.add_argument("--output", "-o",
-                        help="The output path", required=True)
-    parser.add_argument("--format",
-                        choices=["pytorch", "ctranslate2"],
-                        default="pytorch",
-                        help="The format of the released model")
-    parser.add_argument("--quantization", "-q",
-                        choices=["int8", "int16", "float16", "int8_float16"],
-                        default=None,
-                        help="Quantization type for CT2 model.")
+        description="Release an OpenNMT-py model for inference"
+    )
+    parser.add_argument("--model", "-m", help="The model path", required=True)
+    parser.add_argument("--output", "-o", help="The output path", required=True)
+    parser.add_argument(
+        "--format",
+        choices=["pytorch", "ctranslate2"],
+        default="pytorch",
+        help="The format of the released model",
+    )
+    parser.add_argument(
+        "--quantization",
+        "-q",
+        choices=["int8", "int16", "float16", "int8_float16"],
+        default=None,
+        help="Quantization type for CT2 model.",
+    )
     opt = parser.parse_args()
 
     model = torch.load(opt.model, map_location=torch.device("cpu"))
     if opt.format == "pytorch":
         model["optim"] = None
         torch.save(model, opt.output)
     elif opt.format == "ctranslate2":
         import ctranslate2
+
         converter = ctranslate2.converters.OpenNMTPyConverter(opt.model)
-        converter.convert(opt.output, force=True,
-                          quantization=opt.quantization)
+        converter.convert(opt.output, force=True, quantization=opt.quantization)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `OpenNMT-py-3.1.2/onmt/bin/server.py` & `OpenNMT-py-3.1.3/onmt/bin/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,153 +7,161 @@
 import logging
 from logging.handlers import RotatingFileHandler
 
 STATUS_OK = "ok"
 STATUS_ERROR = "error"
 
 
-def start(config_file,
-          url_root="./translator",
-          host="0.0.0.0",
-          port=5000,
-          debug=False):
-    def prefix_route(route_function, prefix='', mask='{0}{1}'):
+def start(config_file, url_root="./translator", host="0.0.0.0", port=5000, debug=False):
+    def prefix_route(route_function, prefix="", mask="{0}{1}"):
         def newroute(route, *args, **kwargs):
             return route_function(mask.format(prefix, route), *args, **kwargs)
+
         return newroute
 
     if debug:
         logger = logging.getLogger("main")
-        log_format = logging.Formatter(
-            "[%(asctime)s %(levelname)s] %(message)s")
+        log_format = logging.Formatter("[%(asctime)s %(levelname)s] %(message)s")
         file_handler = RotatingFileHandler(
-            "debug_requests.log",
-            maxBytes=1000000, backupCount=10)
+            "debug_requests.log", maxBytes=1000000, backupCount=10
+        )
         file_handler.setFormatter(log_format)
         logger.addHandler(file_handler)
 
     app = Flask(__name__)
     app.route = prefix_route(app.route, url_root)
     translation_server = TranslationServer()
     translation_server.start(config_file)
 
-    @app.route('/models', methods=['GET'])
+    @app.route("/models", methods=["GET"])
     def get_models():
         out = translation_server.list_models()
         return jsonify(out)
 
-    @app.route('/health', methods=['GET'])
+    @app.route("/health", methods=["GET"])
     def health():
         out = {}
-        out['status'] = STATUS_OK
+        out["status"] = STATUS_OK
         return jsonify(out)
 
-    @app.route('/clone_model/<int:model_id>', methods=['POST'])
+    @app.route("/clone_model/<int:model_id>", methods=["POST"])
     def clone_model(model_id):
         out = {}
         data = request.get_json(force=True)
         timeout = -1
-        if 'timeout' in data:
-            timeout = data['timeout']
-            del data['timeout']
+        if "timeout" in data:
+            timeout = data["timeout"]
+            del data["timeout"]
 
-        opt = data.get('opt', None)
+        opt = data.get("opt", None)
         try:
-            model_id, load_time = translation_server.clone_model(
-                model_id, opt, timeout)
+            model_id, load_time = translation_server.clone_model(model_id, opt, timeout)
         except ServerModelError as e:
-            out['status'] = STATUS_ERROR
-            out['error'] = str(e)
+            out["status"] = STATUS_ERROR
+            out["error"] = str(e)
         else:
-            out['status'] = STATUS_OK
-            out['model_id'] = model_id
-            out['load_time'] = load_time
+            out["status"] = STATUS_OK
+            out["model_id"] = model_id
+            out["load_time"] = load_time
 
         return jsonify(out)
 
-    @app.route('/unload_model/<int:model_id>', methods=['GET'])
+    @app.route("/unload_model/<int:model_id>", methods=["GET"])
     def unload_model(model_id):
         out = {"model_id": model_id}
 
         try:
             translation_server.unload_model(model_id)
-            out['status'] = STATUS_OK
+            out["status"] = STATUS_OK
         except Exception as e:
-            out['status'] = STATUS_ERROR
-            out['error'] = str(e)
+            out["status"] = STATUS_ERROR
+            out["error"] = str(e)
 
         return jsonify(out)
 
-    @app.route('/translate', methods=['POST'])
+    @app.route("/translate", methods=["POST"])
     def translate():
         inputs = request.get_json(force=True)
         if debug:
             logger.info(inputs)
         out = {}
         try:
-            trans, scores, n_best, _, aligns, align_scores = \
-                translation_server.run(inputs)
+            trans, scores, n_best, _, aligns, align_scores = translation_server.run(
+                inputs
+            )
             assert len(trans) == len(inputs) * n_best
             assert len(scores) == len(inputs) * n_best
             assert len(aligns) == len(inputs) * n_best
 
             out = [[] for _ in range(n_best)]
             for i in range(len(trans)):
-                response = {"src": inputs[i // n_best]['src'], "tgt": trans[i],
-                            "n_best": n_best, "pred_score": scores[i]}
+                response = {
+                    "src": inputs[i // n_best]["src"],
+                    "tgt": trans[i],
+                    "n_best": n_best,
+                    "pred_score": scores[i],
+                }
                 if len(aligns[i]) > 0 and aligns[i][0] is not None:
                     response["align"] = aligns[i]
                     response["align_score"] = align_scores[i]
                 out[i % n_best].append(response)
         except ServerModelError as e:
             model_id = inputs[0].get("id")
             if debug:
-                logger.warning("Unload model #{} "
-                               "because of an error".format(model_id))
+                logger.warning(
+                    "Unload model #{} " "because of an error".format(model_id)
+                )
             translation_server.models[model_id].unload()
-            out['error'] = str(e)
-            out['status'] = STATUS_ERROR
+            out["error"] = str(e)
+            out["status"] = STATUS_ERROR
         if debug:
             logger.info(out)
         return jsonify(out)
 
-    @app.route('/to_cpu/<int:model_id>', methods=['GET'])
+    @app.route("/to_cpu/<int:model_id>", methods=["GET"])
     def to_cpu(model_id):
-        out = {'model_id': model_id}
+        out = {"model_id": model_id}
         translation_server.models[model_id].to_cpu()
 
-        out['status'] = STATUS_OK
+        out["status"] = STATUS_OK
         return jsonify(out)
 
-    @app.route('/to_gpu/<int:model_id>', methods=['GET'])
+    @app.route("/to_gpu/<int:model_id>", methods=["GET"])
     def to_gpu(model_id):
-        out = {'model_id': model_id}
+        out = {"model_id": model_id}
         translation_server.models[model_id].to_gpu()
 
-        out['status'] = STATUS_OK
+        out["status"] = STATUS_OK
         return jsonify(out)
 
     serve(app, host=host, port=port)
 
 
 def _get_parser():
     parser = configargparse.ArgumentParser(
         config_file_parser_class=configargparse.YAMLConfigFileParser,
-        description="OpenNMT-py REST Server")
+        description="OpenNMT-py REST Server",
+    )
     parser.add_argument("--ip", type=str, default="0.0.0.0")
     parser.add_argument("--port", type=int, default="5000")
     parser.add_argument("--url_root", type=str, default="/translator")
     parser.add_argument("--debug", "-d", action="store_true")
-    parser.add_argument("--config", "-c", type=str,
-                        default="./available_models/conf.json")
+    parser.add_argument(
+        "--config", "-c", type=str, default="./available_models/conf.json"
+    )
     return parser
 
 
 def main():
     parser = _get_parser()
     args = parser.parse_args()
-    start(args.config, url_root=args.url_root, host=args.ip, port=args.port,
-          debug=args.debug)
+    start(
+        args.config,
+        url_root=args.url_root,
+        host=args.ip,
+        port=args.port,
+        debug=args.debug,
+    )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `OpenNMT-py-3.1.2/onmt/bin/train.py` & `OpenNMT-py-3.1.3/onmt/bin/train.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,53 +11,55 @@
 
 
 # Set sharing strategy manually instead of default based on the OS.
 # torch.multiprocessing.set_sharing_strategy('file_system')
 
 
 def train(opt):
-
     init_logger(opt.log_file)
 
     ArgumentParser.validate_train_opts(opt)
     ArgumentParser.update_model_opts(opt)
     ArgumentParser.validate_model_opts(opt)
 
     set_random_seed(opt.seed, False)
 
-    train_process = partial(
-        single_main)
+    train_process = partial(single_main)
 
     nb_gpu = len(opt.gpu_ranks)
 
     if opt.world_size > 1:
-        mp = torch.multiprocessing.get_context('spawn')
+        mp = torch.multiprocessing.get_context("spawn")
         # Create a thread to listen for errors in the child processes.
         error_queue = mp.SimpleQueue()
         error_handler = ErrorHandler(error_queue)
         # Train with multiprocessing.
         procs = []
         for device_id in range(nb_gpu):
-            procs.append(mp.Process(target=consumer, args=(
-                train_process, opt, device_id, error_queue),
-                daemon=False))
+            procs.append(
+                mp.Process(
+                    target=consumer,
+                    args=(train_process, opt, device_id, error_queue),
+                    daemon=False,
+                )
+            )
             procs[device_id].start()
             logger.info(" Starting process pid: %d  " % procs[device_id].pid)
             error_handler.add_child(procs[device_id].pid)
         for p in procs:
             p.join()
 
     elif nb_gpu == 1:  # case 1 GPU only
         train_process(opt, device_id=0)
-    else:   # case only CPU
+    else:  # case only CPU
         train_process(opt, device_id=-1)
 
 
 def _get_parser():
-    parser = ArgumentParser(description='train.py')
+    parser = ArgumentParser(description="train.py")
     train_opts(parser)
     return parser
 
 
 def main():
     parser = _get_parser()
```

### Comparing `OpenNMT-py-3.1.2/onmt/bin/translate.py` & `OpenNMT-py-3.1.3/onmt/bin/translate.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,42 +16,46 @@
     ArgumentParser._get_all_transform_translate(opt)
     ArgumentParser._validate_transforms_opts(opt)
     ArgumentParser.validate_translate_opts_dynamic(opt)
     logger = init_logger(opt.log_file)
 
     set_random_seed(opt.seed, use_gpu(opt))
 
-    translator = build_translator(opt, logger=logger,
-                                  report_score=True)
+    translator = build_translator(opt, logger=logger, report_score=True)
 
     transforms_cls = get_transforms_cls(opt._all_transform)
 
     infer_iter = build_dynamic_dataset_iter(
-        opt, transforms_cls, translator.vocabs, task=CorpusTask.INFER,
-        copy=translator.copy_attn)
+        opt,
+        transforms_cls,
+        translator.vocabs,
+        task=CorpusTask.INFER,
+        copy=translator.copy_attn,
+    )
 
     data_transform = [
-        infer_iter.transforms[name] for name in
-        opt.transforms if name in infer_iter.transforms
+        infer_iter.transforms[name]
+        for name in opt.transforms
+        if name in infer_iter.transforms
     ]
     transform = TransformPipe.build_from(data_transform)
 
     if infer_iter is not None:
         infer_iter = IterOnDevice(infer_iter, opt.gpu)
 
     _, _ = translator._translate(
         infer_iter,
         transform=transform,
         attn_debug=opt.attn_debug,
-        align_debug=opt.align_debug
-        )
+        align_debug=opt.align_debug,
+    )
 
 
 def _get_parser():
-    parser = ArgumentParser(description='translate.py')
+    parser = ArgumentParser(description="translate.py")
 
     opts.config_opts(parser)
     opts.translate_opts(parser, dynamic=True)
     return parser
 
 
 def main():
```

### Comparing `OpenNMT-py-3.1.2/onmt/constants.py` & `OpenNMT-py-3.1.3/onmt/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """Define constant values used across the project."""
 
 
 class DefaultTokens(object):
-    PAD = '<blank>'
-    BOS = '<s>'
-    EOS = '</s>'
-    UNK = '<unk>'
-    MASK = '<mask>'
-    VOCAB_PAD = 'averyunlikelytoken'
+    PAD = "<blank>"
+    BOS = "<s>"
+    EOS = "</s>"
+    UNK = "<unk>"
+    MASK = "<mask>"
+    VOCAB_PAD = "averyunlikelytoken"
     SENT_FULL_STOPS = [".", "?", "!"]
-    PHRASE_TABLE_SEPARATOR = '|||'
-    ALIGNMENT_SEPARATOR = ' ||| '
-    SEP = '｟newline｠'
+    PHRASE_TABLE_SEPARATOR = "|||"
+    ALIGNMENT_SEPARATOR = " ||| "
+    SEP = "｟newline｠"
 
 
 class CorpusName(object):
-    VALID = 'valid'
-    TRAIN = 'train'
-    SAMPLE = 'sample'
-    INFER = 'infer'
+    VALID = "valid"
+    TRAIN = "train"
+    SAMPLE = "sample"
+    INFER = "infer"
 
 
 class CorpusTask(object):
-    TRAIN = 'train'
-    VALID = 'valid'
-    INFER = 'infer'
+    TRAIN = "train"
+    VALID = "valid"
+    INFER = "infer"
 
 
 class SubwordMarker(object):
-    SPACER = '▁'
-    JOINER = '￭'
+    SPACER = "▁"
+    JOINER = "￭"
     BEGIN_UPPERCASE = "｟mrk_begin_case_region_U｠"
     END_UPPERCASE = "｟mrk_end_case_region_U｠"
     BEGIN_CASED = "｟mrk_case_modifier_C｠"
 
 
 class ModelTask(object):
-    LANGUAGE_MODEL = 'lm'
-    SEQ2SEQ = 'seq2seq'
+    LANGUAGE_MODEL = "lm"
+    SEQ2SEQ = "seq2seq"
```

### Comparing `OpenNMT-py-3.1.2/onmt/decoders/__init__.py` & `OpenNMT-py-3.1.3/onmt/decoders/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 """Module defining decoders."""
-from onmt.decoders.decoder import DecoderBase, InputFeedRNNDecoder, \
-    StdRNNDecoder
+from onmt.decoders.decoder import DecoderBase, InputFeedRNNDecoder, StdRNNDecoder
 from onmt.decoders.transformer import TransformerDecoder, TransformerLMDecoder
 from onmt.decoders.cnn_decoder import CNNDecoder
 
 
-str2dec = {"rnn": StdRNNDecoder, "ifrnn": InputFeedRNNDecoder,
-           "cnn": CNNDecoder, "transformer": TransformerDecoder,
-           "transformer_lm": TransformerLMDecoder}
+str2dec = {
+    "rnn": StdRNNDecoder,
+    "ifrnn": InputFeedRNNDecoder,
+    "cnn": CNNDecoder,
+    "transformer": TransformerDecoder,
+    "transformer_lm": TransformerLMDecoder,
+}
 
-__all__ = ["DecoderBase", "TransformerDecoder", "StdRNNDecoder", "CNNDecoder",
-           "InputFeedRNNDecoder", "str2dec", "TransformerLMDecoder"]
+__all__ = [
+    "DecoderBase",
+    "TransformerDecoder",
+    "StdRNNDecoder",
+    "CNNDecoder",
+    "InputFeedRNNDecoder",
+    "str2dec",
+    "TransformerLMDecoder",
+]
```

### Comparing `OpenNMT-py-3.1.2/onmt/decoders/cnn_decoder.py` & `OpenNMT-py-3.1.3/onmt/decoders/cnn_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,66 +4,76 @@
 import torch
 import torch.nn as nn
 
 from onmt.modules import ConvMultiStepAttention, GlobalAttention
 from onmt.utils.cnn_factory import shape_transform, GatedConv
 from onmt.decoders.decoder import DecoderBase
 
-SCALE_WEIGHT = 0.5 ** 0.5
+SCALE_WEIGHT = 0.5**0.5
 
 
 class CNNDecoder(DecoderBase):
     """Decoder based on "Convolutional Sequence to Sequence Learning"
     :cite:`DBLP:journals/corr/GehringAGYD17`.
 
     Consists of residual convolutional layers, with ConvMultiStepAttention.
     """
 
-    def __init__(self, num_layers, hidden_size, attn_type,
-                 copy_attn, cnn_kernel_width, dropout, embeddings,
-                 copy_attn_type):
+    def __init__(
+        self,
+        num_layers,
+        hidden_size,
+        attn_type,
+        copy_attn,
+        cnn_kernel_width,
+        dropout,
+        embeddings,
+        copy_attn_type,
+    ):
         super(CNNDecoder, self).__init__()
 
         self.cnn_kernel_width = cnn_kernel_width
         self.embeddings = embeddings
 
         # Decoder State
         self.state = {}
 
         input_size = self.embeddings.embedding_size
         self.linear = nn.Linear(input_size, hidden_size)
         self.conv_layers = nn.ModuleList(
-            [GatedConv(hidden_size, cnn_kernel_width, dropout, True)
-             for i in range(num_layers)]
+            [
+                GatedConv(hidden_size, cnn_kernel_width, dropout, True)
+                for i in range(num_layers)
+            ]
         )
         self.attn_layers = nn.ModuleList(
             [ConvMultiStepAttention(hidden_size) for i in range(num_layers)]
         )
 
         # CNNDecoder has its own attention mechanism.
         # Set up a separate copy attention layer if needed.
         assert not copy_attn, "Copy mechanism not yet tested in conv2conv"
         if copy_attn:
-            self.copy_attn = GlobalAttention(
-                hidden_size, attn_type=copy_attn_type)
+            self.copy_attn = GlobalAttention(hidden_size, attn_type=copy_attn_type)
         else:
             self.copy_attn = None
 
     @classmethod
     def from_opt(cls, opt, embeddings):
         """Alternate constructor."""
         return cls(
             opt.dec_layers,
             opt.dec_hid_size,
             opt.global_attention,
             opt.copy_attn,
             opt.cnn_kernel_width,
             opt.dropout[0] if type(opt.dropout) is list else opt.dropout,
             embeddings,
-            opt.copy_attn_type)
+            opt.copy_attn_type,
+        )
 
     def init_state(self, _, enc_out, enc_hidden):
         """Init decoder state."""
         self.state["src"] = (enc_out + enc_hidden) * SCALE_WEIGHT
         self.state["previous_input"] = None
 
     def map_state(self, fn):
@@ -71,15 +81,15 @@
         if self.state["previous_input"] is not None:
             self.state["previous_input"] = fn(self.state["previous_input"], 0)
 
     def detach_state(self):
         self.state["previous_input"] = self.state["previous_input"].detach()
 
     def forward(self, tgt, enc_out, step=None, **kwargs):
-        """ See :obj:`onmt.modules.RNNDecoderBase.forward()`"""
+        """See :obj:`onmt.modules.RNNDecoderBase.forward()`"""
 
         if self.state["previous_input"] is not None:
             tgt = torch.cat([self.state["previous_input"], tgt], 1)
 
         dec_outs = []
         attns = {"std": []}
         if self.copy_attn is not None:
@@ -90,38 +100,36 @@
 
         tgt_emb = emb
         # The output of CNNEncoder.
         enc_out_t = enc_out
         # The combination of output of CNNEncoder and source embeddings.
         enc_out_c = self.state["src"]
 
-        emb_reshape = tgt_emb.view(
-            tgt_emb.size(0) * tgt_emb.size(1), -1)
+        emb_reshape = tgt_emb.view(tgt_emb.size(0) * tgt_emb.size(1), -1)
         linear_out = self.linear(emb_reshape)
         x = linear_out.view(tgt_emb.size(0), tgt_emb.size(1), -1)
         x = shape_transform(x)
 
         pad = torch.zeros(x.size(0), x.size(1), self.cnn_kernel_width - 1, 1)
 
         pad = pad.type_as(x)
         base_target_emb = x
 
         for conv, attention in zip(self.conv_layers, self.attn_layers):
             new_target_input = torch.cat([pad, x], 2)
             out = conv(new_target_input)
-            c, attn = attention(base_target_emb, out,
-                                enc_out_t, enc_out_c)
+            c, attn = attention(base_target_emb, out, enc_out_t, enc_out_c)
             x = (x + (c + out) * SCALE_WEIGHT) * SCALE_WEIGHT
 
         dec_outs = x.squeeze(3).transpose(1, 2)
 
         # Process the result and update the attentions.
         if self.state["previous_input"] is not None:
-            dec_outs = dec_outs[:, self.state["previous_input"].size(1):, :]
-            attn = attn[:, self.state["previous_input"].size(1):].squeeze()
+            dec_outs = dec_outs[:, self.state["previous_input"].size(1) :, :]
+            attn = attn[:, self.state["previous_input"].size(1) :].squeeze()
             attn = torch.stack([attn])
         attns["std"] = attn
         if self.copy_attn is not None:
             attns["copy"] = attn
 
         # Update the state.
         self.state["previous_input"] = tgt
```

### Comparing `OpenNMT-py-3.1.2/onmt/decoders/decoder.py` & `OpenNMT-py-3.1.3/onmt/decoders/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,62 +47,76 @@
        dropout (float) : dropout value for :class:`torch.nn.Dropout`
        embeddings (onmt.modules.Embeddings): embedding module to use
        reuse_copy_attn (bool): reuse the attention for copying
        copy_attn_type (str): The copy attention style. See
         :class:`~onmt.modules.GlobalAttention`.
     """
 
-    def __init__(self, rnn_type, bidirectional_encoder, num_layers,
-                 hidden_size, attn_type="general", attn_func="softmax",
-                 coverage_attn=False, context_gate=None,
-                 copy_attn=False, dropout=0.0, embeddings=None,
-                 reuse_copy_attn=False, copy_attn_type="general"):
+    def __init__(
+        self,
+        rnn_type,
+        bidirectional_encoder,
+        num_layers,
+        hidden_size,
+        attn_type="general",
+        attn_func="softmax",
+        coverage_attn=False,
+        context_gate=None,
+        copy_attn=False,
+        dropout=0.0,
+        embeddings=None,
+        reuse_copy_attn=False,
+        copy_attn_type="general",
+    ):
         super(RNNDecoderBase, self).__init__(
-            attentional=attn_type != "none" and attn_type is not None)
+            attentional=attn_type != "none" and attn_type is not None
+        )
 
         self.bidirectional_encoder = bidirectional_encoder
         self.num_layers = num_layers
         self.hidden_size = hidden_size
         self.embeddings = embeddings
         self.dropout = nn.Dropout(dropout)
 
         # Decoder state
         self.state = {}
 
         # Build the RNN.
-        self.rnn = self._build_rnn(rnn_type,
-                                   input_size=self._input_size,
-                                   hidden_size=hidden_size,
-                                   num_layers=num_layers,
-                                   dropout=dropout)
+        self.rnn = self._build_rnn(
+            rnn_type,
+            input_size=self._input_size,
+            hidden_size=hidden_size,
+            num_layers=num_layers,
+            dropout=dropout,
+        )
 
         # Set up the context gate.
         self.context_gate = None
         if context_gate is not None:
             self.context_gate = context_gate_factory(
-                context_gate, self._input_size,
-                hidden_size, hidden_size, hidden_size
+                context_gate, self._input_size, hidden_size, hidden_size, hidden_size
             )
 
         # Set up the standard attention.
         self._coverage = coverage_attn
         if not self.attentional:
             if self._coverage:
                 raise ValueError("Cannot use coverage term with no attention.")
             self.attn = None
         else:
             self.attn = GlobalAttention(
-                hidden_size, coverage=coverage_attn,
-                attn_type=attn_type, attn_func=attn_func
+                hidden_size,
+                coverage=coverage_attn,
+                attn_type=attn_type,
+                attn_func=attn_func,
             )
 
         if copy_attn and not reuse_copy_attn:
             if copy_attn_type == "none" or copy_attn_type is None:
-                raise ValueError(
-                    "Cannot use copy_attn with copy_attn_type none")
+                raise ValueError("Cannot use copy_attn with copy_attn_type none")
             self.copy_attn = GlobalAttention(
                 hidden_size, attn_type=copy_attn_type, attn_func=attn_func
             )
         else:
             self.copy_attn = None
 
         self._reuse_copy_attn = reuse_copy_attn and copy_attn
@@ -118,42 +132,46 @@
             opt.dec_layers,
             opt.dec_hid_size,
             opt.global_attention,
             opt.global_attention_function,
             opt.coverage_attn,
             opt.context_gate,
             opt.copy_attn,
-            opt.dropout[0] if type(opt.dropout) is list
-            else opt.dropout,
+            opt.dropout[0] if type(opt.dropout) is list else opt.dropout,
             embeddings,
             opt.reuse_copy_attn,
-            opt.copy_attn_type)
+            opt.copy_attn_type,
+        )
 
     def init_state(self, src, _, enc_final_hs):
         """Initialize decoder state with last state of the encoder."""
+
         def _fix_enc_hidden(hidden):
             # The encoder hidden is  (layers*directions) x batch x dim.
             # We need to convert it to layers x batch x (directions*dim).
             if self.bidirectional_encoder:
-                hidden = torch.cat([hidden[0:hidden.size(0):2],
-                                    hidden[1:hidden.size(0):2]], 2)
+                hidden = torch.cat(
+                    [hidden[0 : hidden.size(0) : 2], hidden[1 : hidden.size(0) : 2]], 2
+                )
             return hidden
 
         if isinstance(enc_final_hs, tuple):  # LSTM
-            self.state["hidden"] = tuple(_fix_enc_hidden(enc_hid)
-                                         for enc_hid in enc_final_hs)
+            self.state["hidden"] = tuple(
+                _fix_enc_hidden(enc_hid) for enc_hid in enc_final_hs
+            )
         else:  # GRU
-            self.state["hidden"] = (_fix_enc_hidden(enc_final_hs), )
+            self.state["hidden"] = (_fix_enc_hidden(enc_final_hs),)
 
         # Init the input feed.
         batch_size = self.state["hidden"][0].size(1)
 
         h_size = (batch_size, self.hidden_size)
-        self.state["input_feed"] = \
+        self.state["input_feed"] = (
             self.state["hidden"][0].data.new(*h_size).zero_().unsqueeze(0)
+        )
 
         self.state["coverage"] = None
 
     def map_state(self, fn):
         self.state["hidden"] = tuple(fn(h, 1) for h in self.state["hidden"])
         self.state["input_feed"] = fn(self.state["input_feed"], 1)
         if self._coverage and self.state["coverage"] is not None:
@@ -161,16 +179,15 @@
 
     def detach_state(self):
         self.state["hidden"] = tuple(h.detach() for h in self.state["hidden"])
         self.state["input_feed"] = self.state["input_feed"].detach()
         if self._coverage and self.state["coverage"] is not None:
             self.state["coverage"] = self.state["coverage"].detach()
 
-    def forward(self, tgt, enc_out, src_len=None, step=None,
-                **kwargs):
+    def forward(self, tgt, enc_out, src_len=None, step=None, **kwargs):
         """
         Args:
             tgt (LongTensor): sequences of padded tokens
                  ``(batch, tgt_len, nfeats)``.
             enc_out (FloatTensor): vectors from the encoder
                  ``(batch, src_len, hidden)``.
             src_len (LongTensor): the padded source lengths
@@ -181,15 +198,16 @@
 
             * dec_outs: output from the decoder (after attn)
               ``(batch, tgt_len, hidden)``.
             * attns: distribution over src at each tgt
               ``(batch, tgt_len, src_len)``.
         """
         dec_state, dec_outs, attns = self._run_forward_pass(
-            tgt, enc_out, src_len=src_len)
+            tgt, enc_out, src_len=src_len
+        )
 
         # Update the state with the result.
         if not isinstance(dec_state, tuple):
             dec_state = (dec_state,)
         self.state["hidden"] = dec_state
 
         # Concatenates sequence of tensors along a new dimension.
@@ -267,27 +285,23 @@
 
         tgt_batch, tgt_len, _ = tgt.size()
 
         # Calculate the attention.
         if not self.attentional:
             dec_outs = rnn_out
         else:
-            dec_outs, p_attn = self.attn(
-                rnn_out,
-                enc_out,
-                src_len=src_len
-            )
+            dec_outs, p_attn = self.attn(rnn_out, enc_out, src_len=src_len)
             attns["std"] = p_attn
 
         # Calculate the context gate.
         if self.context_gate is not None:
             dec_outs = self.context_gate(
                 emb.view(-1, emb.size(2)),
                 rnn_out.view(-1, rnn_out.size(2)),
-                dec_outs.view(-1, dec_outs.size(2))
+                dec_outs.view(-1, dec_outs.size(2)),
             )
             dec_outs = dec_outs.view(tgt_batch, tgt_len, self.hidden_size)
 
         dec_outs = self.dropout(dec_outs)
 
         return dec_state, dec_outs, attns
 
@@ -329,64 +343,60 @@
             attns["coverage"] = []
 
         emb = self.embeddings(tgt)
         assert emb.dim() == 3  # batch x len x embedding_dim
 
         dec_state = self.state["hidden"]
 
-        coverage = self.state["coverage"].squeeze(0) \
-            if self.state["coverage"] is not None else None
+        coverage = (
+            self.state["coverage"].squeeze(0)
+            if self.state["coverage"] is not None
+            else None
+        )
 
         # Input feed concatenates hidden state with
         # input at every time step.
         for emb_t in emb.split(1, dim=1):
             dec_in = torch.cat([emb_t.squeeze(1), input_feed], 1)
             rnn_out, dec_state = self.rnn(dec_in, dec_state)
             if self.attentional:
-                dec_out, p_attn = self.attn(
-                    rnn_out,
-                    enc_out,
-                    src_len=src_len)
+                dec_out, p_attn = self.attn(rnn_out, enc_out, src_len=src_len)
                 attns["std"].append(p_attn)
             else:
                 dec_out = rnn_out
             if self.context_gate is not None:
                 # TODO: context gate should be employed
                 # instead of second RNN transform.
-                dec_out = self.context_gate(
-                    dec_in, rnn_out, dec_out
-                )
+                dec_out = self.context_gate(dec_in, rnn_out, dec_out)
             dec_out = self.dropout(dec_out)
             input_feed = dec_out
 
             dec_outs += [dec_out]
 
             # Update the coverage attention.
             # attns["coverage"] is actually c^(t+1) of See et al(2017)
             # 1-index shifted
             if self._coverage:
                 coverage = p_attn if coverage is None else p_attn + coverage
                 attns["coverage"] += [coverage]
 
             if self.copy_attn is not None:
-                _, copy_attn = self.copy_attn(
-                    dec_out, enc_out)
+                _, copy_attn = self.copy_attn(dec_out, enc_out)
                 attns["copy"] += [copy_attn]
             elif self._reuse_copy_attn:
                 attns["copy"] = attns["std"]
 
         return dec_state, dec_outs, attns
 
-    def _build_rnn(self, rnn_type, input_size,
-                   hidden_size, num_layers, dropout):
-        assert rnn_type != "SRU", "SRU doesn't support input feed! " \
-            "Please set -input_feed 0!"
+    def _build_rnn(self, rnn_type, input_size, hidden_size, num_layers, dropout):
+        assert rnn_type != "SRU", (
+            "SRU doesn't support input feed! " "Please set -input_feed 0!"
+        )
         stacked_cell = StackedLSTM if rnn_type == "LSTM" else StackedGRU
-        return stacked_cell(num_layers, input_size,
-                            hidden_size, dropout)
+        return stacked_cell(num_layers, input_size, hidden_size, dropout)
 
     @property
     def _input_size(self):
         """Using input feed by concatenating input with attention vectors."""
         return self.embeddings.embedding_size + self.hidden_size
 
     def update_dropout(self, dropout, attention_dropout=None):
```

### Comparing `OpenNMT-py-3.1.2/onmt/decoders/ensemble.py` & `OpenNMT-py-3.1.3/onmt/decoders/ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,130 +12,139 @@
 from onmt.decoders.decoder import DecoderBase
 from onmt.models import NMTModel
 import onmt.model_builder
 
 
 class EnsembleDecoderOutput(object):
     """Wrapper around multiple decoder final hidden states."""
+
     def __init__(self, model_dec_outs):
         self.model_dec_outs = tuple(model_dec_outs)
 
     def squeeze(self, dim=None):
         """Delegate squeeze to avoid modifying
         :func:`onmt.translate.translator.Translator.translate_batch()`
         """
-        return EnsembleDecoderOutput([
-            x.squeeze(dim) for x in self.model_dec_outs])
+        return EnsembleDecoderOutput([x.squeeze(dim) for x in self.model_dec_outs])
 
     def __getitem__(self, index):
         return self.model_dec_outs[index]
 
 
 class EnsembleEncoder(EncoderBase):
     """Dummy Encoder that delegates to individual real Encoders."""
+
     def __init__(self, model_encoders):
         super(EnsembleEncoder, self).__init__()
         self.model_encoders = nn.ModuleList(model_encoders)
 
     def forward(self, src, src_len=None):
-        enc_out, enc_final_hs, _ = zip(*[
-            model_encoder(src, src_len)
-            for model_encoder in self.model_encoders])
+        enc_out, enc_final_hs, _ = zip(
+            *[model_encoder(src, src_len) for model_encoder in self.model_encoders]
+        )
         return enc_out, enc_final_hs, src_len
 
 
 class EnsembleDecoder(DecoderBase):
     """Dummy Decoder that delegates to individual real Decoders."""
+
     def __init__(self, model_decoders):
         model_decoders = nn.ModuleList(model_decoders)
         attentional = any([dec.attentional for dec in model_decoders])
         super(EnsembleDecoder, self).__init__(attentional)
         self.model_decoders = model_decoders
 
-    def forward(self, tgt, enc_out, src_len=None, step=None,
-                **kwargs):
+    def forward(self, tgt, enc_out, src_len=None, step=None, **kwargs):
         """See :func:`onmt.decoders.decoder.DecoderBase.forward()`."""
         # src_len is a single tensor shared between all models.
         # This assumption will not hold if Translator is modified
         # to calculate src_len as something other than the length
         # of the input.
-        dec_outs, attns = zip(*[
-            model_decoder(
-                tgt, enc_out[i],
-                src_len=src_len, step=step, **kwargs)
-            for i, model_decoder in enumerate(self.model_decoders)])
+        dec_outs, attns = zip(
+            *[
+                model_decoder(tgt, enc_out[i], src_len=src_len, step=step, **kwargs)
+                for i, model_decoder in enumerate(self.model_decoders)
+            ]
+        )
         mean_attns = self.combine_attns(attns)
         return EnsembleDecoderOutput(dec_outs), mean_attns
 
     def combine_attns(self, attns):
         result = {}
         for key in attns[0].keys():
             result[key] = torch.stack(
-                [attn[key] for attn in attns if attn[key] is not None]).mean(0)
+                [attn[key] for attn in attns if attn[key] is not None]
+            ).mean(0)
         return result
 
     def init_state(self, src, enc_out, enc_hidden):
-        """ See :obj:`RNNDecoderBase.init_state()` """
+        """See :obj:`RNNDecoderBase.init_state()`"""
         for i, model_decoder in enumerate(self.model_decoders):
             model_decoder.init_state(src, enc_out[i], enc_hidden[i])
 
     def map_state(self, fn):
         for model_decoder in self.model_decoders:
             model_decoder.map_state(fn)
 
 
 class EnsembleGenerator(nn.Module):
     """
     Dummy Generator that delegates to individual real Generators,
     and then averages the resulting target distributions.
     """
+
     def __init__(self, model_generators, raw_probs=False):
         super(EnsembleGenerator, self).__init__()
         self.model_generators = nn.ModuleList(model_generators)
         self._raw_probs = raw_probs
 
     def forward(self, hidden, attn=None, src_map=None):
         """
         Compute a distribution over the target dictionary
         by averaging distributions from models in the ensemble.
         All models in the ensemble must share a target vocabulary.
         """
         distributions = torch.stack(
-                [mg(h) if attn is None else mg(h, attn, src_map)
-                 for h, mg in zip(hidden, self.model_generators)]
-            )
+            [
+                mg(h) if attn is None else mg(h, attn, src_map)
+                for h, mg in zip(hidden, self.model_generators)
+            ]
+        )
         if self._raw_probs:
             return torch.log(torch.exp(distributions).mean(0))
         else:
             return distributions.mean(0)
 
 
 class EnsembleModel(NMTModel):
     """Dummy NMTModel wrapping individual real NMTModels."""
+
     def __init__(self, models, raw_probs=False):
         encoder = EnsembleEncoder(model.encoder for model in models)
         decoder = EnsembleDecoder(model.decoder for model in models)
         super(EnsembleModel, self).__init__(encoder, decoder)
         self.generator = EnsembleGenerator(
-            [model.generator for model in models], raw_probs)
+            [model.generator for model in models], raw_probs
+        )
         self.models = nn.ModuleList(models)
 
 
 def load_test_model(opt):
     """Read in multiple models for ensemble."""
     shared_vocabs = None
     shared_model_opt = None
     models = []
     for model_path in opt.models:
-        vocabs, model, model_opt = \
-            onmt.model_builder.load_test_model(opt, model_path=model_path)
+        vocabs, model, model_opt = onmt.model_builder.load_test_model(
+            opt, model_path=model_path
+        )
         if shared_vocabs is None:
             shared_vocabs = vocabs
         else:
-            assert shared_vocabs['src'].tokens_to_ids == \
-                vocabs['src'].tokens_to_ids, \
-                "Ensemble models must use the same vocabs "
+            assert (
+                shared_vocabs["src"].tokens_to_ids == vocabs["src"].tokens_to_ids
+            ), "Ensemble models must use the same vocabs "
         models.append(model)
         if shared_model_opt is None:
             shared_model_opt = model_opt
     ensemble_model = EnsembleModel(models, opt.avg_raw_probs)
     return shared_vocabs, ensemble_model, shared_model_opt
```

### Comparing `OpenNMT-py-3.1.2/onmt/decoders/transformer.py` & `OpenNMT-py-3.1.3/onmt/decoders/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self_attn_type="scaled-dot",
         max_relative_positions=0,
         aan_useffn=False,
         full_context_alignment=False,
         alignment_heads=0,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
-        layer_norm='standard'
+        layer_norm="standard",
     ):
         """
         Args:
             d_model (int): the dimension of keys/values/queries in
                 :class:`MultiHeadedAttention`, also the input size of
                 the first-layer of the :class:`PositionwiseFeedForward`.
             heads (int): the number of heads for MultiHeadedAttention.
@@ -66,30 +66,30 @@
         if self_attn_type == "scaled-dot":
             self.self_attn = MultiHeadedAttention(
                 heads,
                 d_model,
                 dropout=attention_dropout,
                 max_relative_positions=max_relative_positions,
                 attn_type="self",
-                add_qkvbias=add_qkvbias
+                add_qkvbias=add_qkvbias,
             )
         elif self_attn_type == "average":
             self.self_attn = AverageAttention(
                 d_model, dropout=attention_dropout, aan_useffn=aan_useffn
             )
 
-        self.feed_forward = PositionwiseFeedForward(d_model, d_ff, dropout,
-                                                    pos_ffn_activation_fn,
-                                                    layer_norm)
-        if layer_norm == 'standard':
+        self.feed_forward = PositionwiseFeedForward(
+            d_model, d_ff, dropout, pos_ffn_activation_fn, layer_norm
+        )
+        if layer_norm == "standard":
             self.layer_norm_1 = nn.LayerNorm(d_model, eps=1e-6)
-        elif layer_norm == 'rms':
+        elif layer_norm == "rms":
             self.layer_norm_1 = RMSNorm(d_model, eps=1e-6)
         else:
-            raise ValueError(f'{layer_norm} layer norm type is not supported')
+            raise ValueError(f"{layer_norm} layer norm type is not supported")
         self.drop = nn.Dropout(dropout)
         self.full_context_alignment = full_context_alignment
         self.alignment_heads = alignment_heads
 
     def forward(self, *args, **kwargs):
         """Extend `_forward` for (possibly) multiple decoder pass:
         Always a default (future masked) decoder forward pass,
@@ -151,28 +151,20 @@
         else:  # only mask padding, result mask in (B, 1, T)
             dec_mask = tgt_pad_mask
         return dec_mask
 
     def _forward_self_attn(self, layer_in_norm, dec_mask, step):
         if self.self_attn_type == "scaled-dot":
             return self.self_attn(
-                layer_in_norm,
-                layer_in_norm,
-                layer_in_norm,
-                mask=dec_mask,
-                step=step
+                layer_in_norm, layer_in_norm, layer_in_norm, mask=dec_mask, step=step
             )
         elif self.self_attn_type == "average":
-            return self.self_attn(
-                layer_in_norm, mask=dec_mask, step=step
-            )
+            return self.self_attn(layer_in_norm, mask=dec_mask, step=step)
         else:
-            raise ValueError(
-                f"self attention {type(self.self_attn)} not supported"
-            )
+            raise ValueError(f"self attention {type(self.self_attn)} not supported")
 
 
 class TransformerDecoderLayer(TransformerDecoderLayerBase):
     """Transformer Decoder layer block in Pre-Norm style.
     Pre-Norm style is an improvement w.r.t. Original paper's Post-Norm style,
     providing better converge speed and performance. This is also the actual
     implementation in tensor2tensor and also avalable in fairseq.
@@ -190,15 +182,15 @@
         self_attn_type="scaled-dot",
         max_relative_positions=0,
         aan_useffn=False,
         full_context_alignment=False,
         alignment_heads=0,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
-        layer_norm='standard'
+        layer_norm="standard",
     ):
         """
         Args:
             See TransformerDecoderLayerBase
         """
         super(TransformerDecoderLayer, self).__init__(
             d_model,
@@ -209,32 +201,32 @@
             self_attn_type,
             max_relative_positions,
             aan_useffn,
             full_context_alignment,
             alignment_heads,
             pos_ffn_activation_fn=pos_ffn_activation_fn,
             add_qkvbias=add_qkvbias,
-            layer_norm=layer_norm
+            layer_norm=layer_norm,
         )
         self.context_attn = MultiHeadedAttention(
-            heads, d_model, dropout=attention_dropout,
+            heads,
+            d_model,
+            dropout=attention_dropout,
             attn_type="context",
-            add_qkvbias=add_qkvbias
+            add_qkvbias=add_qkvbias,
         )
-        if layer_norm == 'standard':
+        if layer_norm == "standard":
             self.layer_norm_2 = nn.LayerNorm(d_model, eps=1e-6)
-        elif layer_norm == 'rms':
+        elif layer_norm == "rms":
             self.layer_norm_2 = RMSNorm(d_model, eps=1e-6)
         else:
-            raise ValueError(f'{layer_norm} layer norm type is not supported')
+            raise ValueError(f"{layer_norm} layer norm type is not supported")
 
     def update_dropout(self, dropout, attention_dropout):
-        super(TransformerDecoderLayer, self).update_dropout(
-            dropout, attention_dropout
-        )
+        super(TransformerDecoderLayer, self).update_dropout(dropout, attention_dropout)
         self.context_attn.update_dropout(attention_dropout)
 
     def _forward(
         self,
         layer_in,
         enc_out,
         src_pad_mask,
@@ -271,53 +263,45 @@
             dec_mask = dec_mask.expand(-1, -1, dec_mask.size(3), -1)
             src_pad_mask = src_pad_mask.expand(-1, -1, dec_mask.size(3), -1)
             # mask now are (batch x 1 x tlen x s or t len)
             # 1 = heads to be expanded in MHA
 
         layer_in_norm = self.layer_norm_1(layer_in)
 
-        query, _ = self._forward_self_attn(
-            layer_in_norm, dec_mask, step
-        )
+        query, _ = self._forward_self_attn(layer_in_norm, dec_mask, step)
 
         query = self.drop(query) + layer_in
 
         query_norm = self.layer_norm_2(query)
 
-        mid, attns = self.context_attn(
-            enc_out,
-            enc_out,
-            query_norm,
-            mask=src_pad_mask
-        )
+        mid, attns = self.context_attn(enc_out, enc_out, query_norm, mask=src_pad_mask)
         layer_out = self.feed_forward(self.drop(mid) + query)
 
         return layer_out, attns
 
 
 class TransformerDecoderBase(DecoderBase):
-    def __init__(self, d_model, copy_attn, embeddings, alignment_layer,
-                 layer_norm):
+    def __init__(self, d_model, copy_attn, embeddings, alignment_layer, layer_norm):
         super(TransformerDecoderBase, self).__init__()
 
         self.embeddings = embeddings
 
         # Decoder State
         self.state = {}
 
         # previously, there was a GlobalAttention module here for copy
         # attention. But it was never actually used -- the "copy" attention
         # just reuses the context attention.
         self._copy = copy_attn
-        if layer_norm == 'standard':
+        if layer_norm == "standard":
             self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
-        elif layer_norm == 'rms':
+        elif layer_norm == "rms":
             self.layer_norm = RMSNorm(d_model, eps=1e-6)
         else:
-            raise ValueError(f'{layer_norm} layer norm type is not supported')
+            raise ValueError(f"{layer_norm} layer norm type is not supported")
 
         self.alignment_layer = alignment_layer
 
     @classmethod
     def from_opt(cls, opt, embeddings):
         """Alternate constructor."""
         return cls(
@@ -335,42 +319,39 @@
             opt.max_relative_positions,
             opt.aan_useffn,
             opt.full_context_alignment,
             opt.alignment_layer,
             alignment_heads=opt.alignment_heads,
             pos_ffn_activation_fn=opt.pos_ffn_activation_fn,
             add_qkvbias=opt.add_qkvbias,
-            layer_norm=opt.layer_norm
+            layer_norm=opt.layer_norm,
         )
 
     def init_state(self, src, enc_out, enc_final_hs):
         """Initialize decoder state."""
         self.state["src"] = src
 
     def map_state(self, fn):
-
         if self.state["src"] is not None:
             self.state["src"] = fn(self.state["src"], 0)
         for layer in self.transformer_layers:
-            if hasattr(layer, 'context_attn'):
-                if layer.context_attn.layer_cache[1]['keys'].numel() != 0:
-                    x = fn(layer.context_attn.layer_cache[1]['keys'], 0)
-                    y = fn(layer.context_attn.layer_cache[1]['values'], 0)
-                    layer.context_attn.layer_cache = True, {'keys': x,
-                                                            'values': y}
+            if hasattr(layer, "context_attn"):
+                if layer.context_attn.layer_cache[1]["keys"].numel() != 0:
+                    x = fn(layer.context_attn.layer_cache[1]["keys"], 0)
+                    y = fn(layer.context_attn.layer_cache[1]["values"], 0)
+                    layer.context_attn.layer_cache = True, {"keys": x, "values": y}
             if isinstance(layer.self_attn, AverageAttention):
-                if layer.self_attn.layer_cache[1]['prev_g'].numel() != 0:
-                    x = fn(layer.self_attn.layer_cache[1]['prev_g'], 0)
-                    layer.self_attn.layer_cache = True, {'prev_g': x}
+                if layer.self_attn.layer_cache[1]["prev_g"].numel() != 0:
+                    x = fn(layer.self_attn.layer_cache[1]["prev_g"], 0)
+                    layer.self_attn.layer_cache = True, {"prev_g": x}
             else:
-                if layer.self_attn.layer_cache[1]['keys'].numel() != 0:
-                    x = fn(layer.self_attn.layer_cache[1]['keys'], 0)
-                    y = fn(layer.self_attn.layer_cache[1]['values'], 0)
-                    layer.self_attn.layer_cache = True, {'keys': x,
-                                                         'values': y}
+                if layer.self_attn.layer_cache[1]["keys"].numel() != 0:
+                    x = fn(layer.self_attn.layer_cache[1]["keys"], 0)
+                    y = fn(layer.self_attn.layer_cache[1]["values"], 0)
+                    layer.self_attn.layer_cache = True, {"keys": x, "values": y}
 
     def detach_state(self):
         raise NotImplementedError
 
     def forward(self, *args, **kwargs):
         raise NotImplementedError
 
@@ -421,15 +402,15 @@
         max_relative_positions,
         aan_useffn,
         full_context_alignment,
         alignment_layer,
         alignment_heads,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
-        layer_norm='standard'
+        layer_norm="standard",
     ):
         super(TransformerDecoder, self).__init__(
             d_model, copy_attn, embeddings, alignment_layer, layer_norm
         )
 
         self.transformer_layers = nn.ModuleList(
             [
@@ -442,15 +423,15 @@
                     self_attn_type=self_attn_type,
                     max_relative_positions=max_relative_positions,
                     aan_useffn=aan_useffn,
                     full_context_alignment=full_context_alignment,
                     alignment_heads=alignment_heads,
                     pos_ffn_activation_fn=pos_ffn_activation_fn,
                     add_qkvbias=add_qkvbias,
-                    layer_norm=layer_norm
+                    layer_norm=layer_norm,
                 )
                 for i in range(num_layers)
             ]
         )
 
     def detach_state(self):
         self.state["src"] = self.state["src"].detach()
@@ -465,23 +446,24 @@
         if enc_out is None:
             enc_out = self.embeddings(tgt)
         if step == 0:
             self._init_cache(enc_out)
         elif step is None:
             for layer in self.transformer_layers:
                 if isinstance(layer.self_attn, AverageAttention):
-                    layer.self_attn.layer_cache =\
-                        False, {'prev_g': torch.tensor([])}
+                    layer.self_attn.layer_cache = False, {"prev_g": torch.tensor([])}
                 else:
                     layer.self_attn.layer_cache = (
-                        False, {'keys': torch.tensor([]),
-                                'values': torch.tensor([])})
+                        False,
+                        {"keys": torch.tensor([]), "values": torch.tensor([])},
+                    )
                 layer.context_attn.layer_cache = (
-                    False, {'keys': torch.tensor([]),
-                            'values': torch.tensor([])})
+                    False,
+                    {"keys": torch.tensor([]), "values": torch.tensor([])},
+                )
 
         tgt_words = tgt[:, :, 0]
 
         emb = self.embeddings(tgt, step=step)
         dec_out = emb
         assert emb.dim() == 3  # len x batch x embedding_dim
 
@@ -516,47 +498,50 @@
             attns["align"] = attn_aligns[self.alignment_layer]  # `(B, Q, K)`
             # attns["align"] = torch.stack(attn_aligns, 0).mean(0)  # All avg
 
         # TODO change the way attns is returned dict => list or tuple (onnx)
         return dec_out, attns
 
     def _init_cache(self, enc_out):
-
         batch_size = enc_out.size(0)
         depth = enc_out.size(-1)
 
         for layer in self.transformer_layers:
             # first value set to True triggered by the beginning of decoding
             # layer_cache becomes active in the MultiHeadedAttention fwd
             layer.context_attn.layer_cache = (
                 True,
-                {'keys': torch.tensor([], device=enc_out.device),
-                 'values': torch.tensor([], device=enc_out.device)}
-                )
+                {
+                    "keys": torch.tensor([], device=enc_out.device),
+                    "values": torch.tensor([], device=enc_out.device),
+                },
+            )
             if isinstance(layer.self_attn, AverageAttention):
-                layer.self_attn.layer_cache = True, {'prev_g': torch.zeros(
-                     (batch_size, 1, depth), device=enc_out.device
-                ).to(enc_out.dtype)}
+                layer.self_attn.layer_cache = True, {
+                    "prev_g": torch.zeros(
+                        (batch_size, 1, depth), device=enc_out.device
+                    ).to(enc_out.dtype)
+                }
             else:
                 layer.self_attn.layer_cache = (
                     True,
-                    {'keys': torch.tensor([], device=enc_out.device),
-                     'values': torch.tensor([], device=enc_out.device)}
-                    )
+                    {
+                        "keys": torch.tensor([], device=enc_out.device),
+                        "values": torch.tensor([], device=enc_out.device),
+                    },
+                )
 
 
 class TransformerLMDecoderLayer(TransformerDecoderLayerBase):
     """Transformer Decoder only layer block in GPT style.
-   Args:
-        See TransformerDecoderLayerBase
+    Args:
+         See TransformerDecoderLayerBase
     """
 
-    def _forward(
-        self, layer_in, tgt_pad_mask, step=None, future=False
-    ):
+    def _forward(self, layer_in, tgt_pad_mask, step=None, future=False):
         """A naive forward pass for transformer decoder.
 
         # T: could be 1 in the case of stepwise decoding or tgt_len
 
         Args:
             layer_in (FloatTensor): ``(batch_size, T, model_dim)``
             tgt_pad_mask (bool): ``(batch_size, 1, T)``
@@ -579,42 +564,40 @@
             dec_mask = dec_mask.unsqueeze(1)
             dec_mask = dec_mask.expand(-1, -1, dec_mask.size(3), -1)
             # mask now are (batch x 1 x tlen x tlen)
             # 1 = heads to be expanded in MHA
 
         layer_in_norm = self.layer_norm_1(layer_in)
 
-        query, attns = self._forward_self_attn(
-            layer_in_norm, dec_mask, step
-        )
+        query, attns = self._forward_self_attn(layer_in_norm, dec_mask, step)
 
         layer_out = self.drop(query) + layer_in
 
         layer_out = self.feed_forward(layer_out)
 
         return layer_out, attns
 
 
 class TransformerLMDecoder(TransformerDecoderBase):
     """The Transformer decoder from GPT-2
-   Args:
-        num_layers (int): number of decoder layers.
-        d_model (int): size of the model
-        heads (int): number of heads
-        d_ff (int): size of the inner FF layer
-        copy_attn (bool): if using a separate copy attention
-        self_attn_type (str): type of self-attention scaled-dot, average
-        dropout (float): dropout in residual, self-attn(dot) and feed-forward
-        attention_dropout (float): dropout in context_attn (and self-attn(avg))
-        embeddings (onmt.modules.Embeddings):
-            embeddings to use, should have positional encodings
-        max_relative_positions (int):
-            Max distance between inputs in relative positions representations
-        aan_useffn (bool): Turn on the FFN layer in the AAN decoder
-        add_qkvbias (bool): whether to add bias to the Key/Value nn.Linear
+    Args:
+         num_layers (int): number of decoder layers.
+         d_model (int): size of the model
+         heads (int): number of heads
+         d_ff (int): size of the inner FF layer
+         copy_attn (bool): if using a separate copy attention
+         self_attn_type (str): type of self-attention scaled-dot, average
+         dropout (float): dropout in residual, self-attn(dot) and feed-forward
+         attention_dropout (float): dropout in context_attn (and self-attn(avg))
+         embeddings (onmt.modules.Embeddings):
+             embeddings to use, should have positional encodings
+         max_relative_positions (int):
+             Max distance between inputs in relative positions representations
+         aan_useffn (bool): Turn on the FFN layer in the AAN decoder
+         add_qkvbias (bool): whether to add bias to the Key/Value nn.Linear
     """
 
     def __init__(
         self,
         num_layers,
         d_model,
         heads,
@@ -627,15 +610,15 @@
         max_relative_positions,
         aan_useffn,
         full_context_alignment=None,
         alignment_layer=None,
         alignment_heads=None,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
-        layer_norm='standard'
+        layer_norm="standard",
     ):
         super(TransformerLMDecoder, self).__init__(
             d_model, copy_attn, embeddings, alignment_layer, layer_norm
         )
         self.transformer_layers = nn.ModuleList(
             [
                 TransformerLMDecoderLayer(
@@ -647,15 +630,15 @@
                     self_attn_type=self_attn_type,
                     max_relative_positions=max_relative_positions,
                     aan_useffn=aan_useffn,
                     full_context_alignment=None,
                     alignment_heads=None,
                     pos_ffn_activation_fn=pos_ffn_activation_fn,
                     add_qkvbias=add_qkvbias,
-                    layer_norm=layer_norm
+                    layer_norm=layer_norm,
                 )
                 for i in range(num_layers)
             ]
         )
 
     def init_state(self, src=None, enc_out=None, enc_final_hs=None):
         super(TransformerLMDecoder, self).init_state(None, None, None)
@@ -666,16 +649,17 @@
     def forward(self, tgt, enc_out=None, step=None, **kwargs):
         """Decode, possibly stepwise."""
         if step == 0:
             self._init_cache(tgt)
         elif step is None:
             for layer in self.transformer_layers:
                 layer.self_attn.layer_cache = (
-                    False, {'keys': torch.tensor([]),
-                            'values': torch.tensor([])})
+                    False,
+                    {"keys": torch.tensor([]), "values": torch.tensor([])},
+                )
 
         tgt_words = tgt[:, :, 0]
 
         dec_out = self.embeddings(tgt, step=step)
 
         assert dec_out.dim() == 3  # batch x len x embedding_dim
 
@@ -699,17 +683,18 @@
         if self._copy:
             attns["copy"] = attn
 
         # TODO change the way attns is returned dict => list or tuple (onnx)
         return dec_out, attns
 
     def _init_cache(self, tgt=None):
-
         for layer in self.transformer_layers:
             if isinstance(layer.self_attn, AverageAttention):
                 raise NotImplementedError
             else:
                 layer.self_attn.layer_cache = (
                     True,
-                    {'keys': torch.tensor([], device=tgt.device),
-                     'values': torch.tensor([], device=tgt.device)}
-                    )
+                    {
+                        "keys": torch.tensor([], device=tgt.device),
+                        "values": torch.tensor([], device=tgt.device),
+                    },
+                )
```

### Comparing `OpenNMT-py-3.1.2/onmt/encoders/__init__.py` & `OpenNMT-py-3.1.3/onmt/encoders/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,13 +3,24 @@
 from onmt.encoders.transformer import TransformerEncoder
 from onmt.encoders.ggnn_encoder import GGNNEncoder
 from onmt.encoders.rnn_encoder import RNNEncoder
 from onmt.encoders.cnn_encoder import CNNEncoder
 from onmt.encoders.mean_encoder import MeanEncoder
 
 
-str2enc = {"ggnn": GGNNEncoder, "rnn": RNNEncoder, "brnn": RNNEncoder,
-           "cnn": CNNEncoder, "transformer": TransformerEncoder,
-           "mean": MeanEncoder}
+str2enc = {
+    "ggnn": GGNNEncoder,
+    "rnn": RNNEncoder,
+    "brnn": RNNEncoder,
+    "cnn": CNNEncoder,
+    "transformer": TransformerEncoder,
+    "mean": MeanEncoder,
+}
 
-__all__ = ["EncoderBase", "TransformerEncoder", "RNNEncoder", "CNNEncoder",
-           "MeanEncoder", "str2enc"]
+__all__ = [
+    "EncoderBase",
+    "TransformerEncoder",
+    "RNNEncoder",
+    "CNNEncoder",
+    "MeanEncoder",
+    "str2enc",
+]
```

### Comparing `OpenNMT-py-3.1.2/onmt/encoders/cnn_encoder.py` & `OpenNMT-py-3.1.3/onmt/encoders/cnn_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,41 +2,40 @@
 Implementation of "Convolutional Sequence to Sequence Learning"
 """
 import torch.nn as nn
 
 from onmt.encoders.encoder import EncoderBase
 from onmt.utils.cnn_factory import shape_transform, StackedCNN
 
-SCALE_WEIGHT = 0.5 ** 0.5
+SCALE_WEIGHT = 0.5**0.5
 
 
 class CNNEncoder(EncoderBase):
     """Encoder based on "Convolutional Sequence to Sequence Learning"
     :cite:`DBLP:journals/corr/GehringAGYD17`.
     """
 
-    def __init__(self, num_layers, hidden_size,
-                 cnn_kernel_width, dropout, embeddings):
+    def __init__(self, num_layers, hidden_size, cnn_kernel_width, dropout, embeddings):
         super(CNNEncoder, self).__init__()
 
         self.embeddings = embeddings
         input_size = embeddings.embedding_size
         self.linear = nn.Linear(input_size, hidden_size)
-        self.cnn = StackedCNN(num_layers, hidden_size,
-                              cnn_kernel_width, dropout)
+        self.cnn = StackedCNN(num_layers, hidden_size, cnn_kernel_width, dropout)
 
     @classmethod
     def from_opt(cls, opt, embeddings):
         """Alternate constructor."""
         return cls(
             opt.enc_layers,
             opt.enc_hid_size,
             opt.cnn_kernel_width,
             opt.dropout[0] if type(opt.dropout) is list else opt.dropout,
-            embeddings)
+            embeddings,
+        )
 
     def forward(self, input, src_len=None, hidden=None):
         """See :func:`EncoderBase.forward()`"""
         # batch x len x dim
         emb = self.embeddings(input)
 
         emb_reshape = emb.view(emb.size(0) * emb.size(1), -1)
```

### Comparing `OpenNMT-py-3.1.2/onmt/encoders/encoder.py` & `OpenNMT-py-3.1.3/onmt/encoders/encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.2/onmt/encoders/ggnn_encoder.py` & `OpenNMT-py-3.1.3/onmt/encoders/ggnn_encoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,49 +9,48 @@
 
 class GGNNAttrProxy(object):
     """
     Translates index lookups into attribute lookups.
     To implement some trick which able to use list of nn.Module in a nn.Module
     see https://discuss.pytorch.org/t/list-of-nn-module-in-a-nn-module/219/2
     """
+
     def __init__(self, module, prefix):
         self.module = module
         self.prefix = prefix
 
     def __getitem__(self, i):
         return getattr(self.module, self.prefix + str(i))
 
 
 class GGNNPropogator(nn.Module):
     """
     Gated Propogator for GGNN
     Using LSTM gating mechanism
     """
+
     def __init__(self, state_dim, n_node, n_edge_types):
         super(GGNNPropogator, self).__init__()
 
         self.n_node = n_node
         self.n_edge_types = n_edge_types
 
         self.reset_gate = nn.Sequential(
-            nn.Linear(state_dim*3, state_dim),
-            nn.Sigmoid()
+            nn.Linear(state_dim * 3, state_dim), nn.Sigmoid()
         )
         self.update_gate = nn.Sequential(
-            nn.Linear(state_dim*3, state_dim),
-            nn.Sigmoid()
+            nn.Linear(state_dim * 3, state_dim), nn.Sigmoid()
         )
         self.tansform = nn.Sequential(
-            nn.Linear(state_dim*3, state_dim),
-            nn.LeakyReLU()
+            nn.Linear(state_dim * 3, state_dim), nn.LeakyReLU()
         )
 
     def forward(self, state_in, state_out, state_cur, edges, nodes):
-        edges_in = edges[:, :, :nodes*self.n_edge_types]
-        edges_out = edges[:, :, nodes*self.n_edge_types:]
+        edges_in = edges[:, :, : nodes * self.n_edge_types]
+        edges_out = edges[:, :, nodes * self.n_edge_types :]
 
         a_in = torch.bmm(edges_in, state_in)
         a_out = torch.bmm(edges_out, state_out)
         a = torch.cat((a_in, a_out, state_cur), 2)
 
         r = self.reset_gate(a)
         z = self.update_gate(a)
@@ -60,15 +59,15 @@
 
         prop_out = (1 - z) * state_cur + z * h_hat
 
         return prop_out
 
 
 class GGNNEncoder(EncoderBase):
-    """ A gated graph neural network configured as an encoder.
+    """A gated graph neural network configured as an encoder.
        Based on github.com/JamesChuanggg/ggnn.pytorch.git,
        which is based on the paper "Gated Graph Sequence Neural Networks"
        by Y. Li, D. Tarlow, M. Brockschmidt, and R. Zemel.
 
     Args:
        rnn_type (str):
           style of recurrent unit to use, one of [LSTM]
@@ -82,17 +81,27 @@
           (after token listing) should be used for decoder init.
        n_steps (int): Steps to advance graph encoder for stabilization
        src_vocab (int): Path to source vocabulary.(The ggnn uses src_vocab
             during training because the graph is built using edge information
             which requires parsing the input sequence.)
     """
 
-    def __init__(self, rnn_type, src_word_vec_size, src_ggnn_size,
-                 state_dim, bidir_edges, n_edge_types, n_node,
-                 bridge_extra_node, n_steps, src_vocab):
+    def __init__(
+        self,
+        rnn_type,
+        src_word_vec_size,
+        src_ggnn_size,
+        state_dim,
+        bidir_edges,
+        n_edge_types,
+        n_node,
+        bridge_extra_node,
+        n_steps,
+        src_vocab,
+    ):
         super(GGNNEncoder, self).__init__()
 
         self.src_word_vec_size = src_word_vec_size
         self.src_ggnn_size = src_ggnn_size
         self.state_dim = state_dim
         self.n_edge_types = n_edge_types
         self.n_node = n_node
@@ -114,97 +123,103 @@
         f = open(src_vocab, "r")
         idx = 0
         self.COMMA = -1
         self.DELIMITER = -1
         self.idx2num = []
         found_n_minus_one = False
         for ln in f:
-            ln = ln.strip('\n')
-            ln = ln.split('\t')[0]
+            ln = ln.strip("\n")
+            ln = ln.split("\t")[0]
             if idx == 0 and ln != "<unk>":
                 idx += 1
                 self.idx2num.append(-1)
             if idx == 1 and ln != "<blank>":
                 idx += 1
                 self.idx2num.append(-1)
             if ln == ",":
                 self.COMMA = idx
             if ln == "<EOT>":
                 self.DELIMITER = idx
             if ln.isdigit():
                 self.idx2num.append(int(ln))
-                if int(ln) == n_node-1:
+                if int(ln) == n_node - 1:
                     found_n_minus_one = True
             else:
                 self.idx2num.append(-1)
             idx += 1
 
-        assert self.COMMA >= 0, \
-            "GGNN src_vocab must include ',' character"
-        assert self.DELIMITER >= 0, \
-            "GGNN src_vocab must include <EOT> token"
-        assert found_n_minus_one, \
-            "GGNN src_vocab must include node numbers for edge connections"
+        assert self.COMMA >= 0, "GGNN src_vocab must include ',' character"
+        assert self.DELIMITER >= 0, "GGNN src_vocab must include <EOT> token"
+        assert (
+            found_n_minus_one
+        ), "GGNN src_vocab must include node numbers for edge connections"
 
         # Propogation Model
-        self.propogator = GGNNPropogator(self.state_dim, self.n_node,
-                                         self.n_edge_types)
+        self.propogator = GGNNPropogator(self.state_dim, self.n_node, self.n_edge_types)
 
         self._initialization()
 
         # Initialize the bridge layer
         self._initialize_bridge(rnn_type, self.state_dim, 1)
 
         # Token embedding
         if src_ggnn_size > 0:
             self.embed = nn.Sequential(
-                nn.Linear(src_ggnn_size, src_word_vec_size),
-                nn.LeakyReLU()
+                nn.Linear(src_ggnn_size, src_word_vec_size), nn.LeakyReLU()
             )
-            assert self.src_ggnn_size >= self.DELIMITER, \
-                "Embedding input must be larger than vocabulary"
-            assert self.src_word_vec_size < self.state_dim, \
-                "Embedding size must be smaller than state_dim"
+            assert (
+                self.src_ggnn_size >= self.DELIMITER
+            ), "Embedding input must be larger than vocabulary"
+            assert (
+                self.src_word_vec_size < self.state_dim
+            ), "Embedding size must be smaller than state_dim"
         else:
-            assert self.DELIMITER < self.state_dim, \
-                "Vocabulary too large, consider -src_ggnn_size"
+            assert (
+                self.DELIMITER < self.state_dim
+            ), "Vocabulary too large, consider -src_ggnn_size"
 
     @classmethod
     def from_opt(cls, opt, embeddings):
         """Alternate constructor."""
         return cls(
             opt.rnn_type,
             opt.src_word_vec_size,
             opt.src_ggnn_size,
             opt.state_dim,
             opt.bidir_edges,
             opt.n_edge_types,
             opt.n_node,
             opt.bridge_extra_node,
             opt.n_steps,
-            opt.src_vocab)
+            opt.src_vocab,
+        )
 
     def _initialization(self):
         for m in self.modules():
             if isinstance(m, nn.Linear):
                 m.weight.data.normal_(0.0, 0.02)
                 m.bias.data.fill_(0)
 
     def forward(self, src, src_len=None):
         """See :func:`EncoderBase.forward()`"""
 
         nodes = self.n_node
         batch_size = src.size()[0]
         first_extra = np.zeros(batch_size, dtype=np.int32)
-        token_onehot = np.zeros((batch_size, nodes,
-                                 self.src_ggnn_size if self.src_ggnn_size > 0
-                                 else self.state_dim),
-                                dtype=np.int32)
-        edges = np.zeros((batch_size, nodes, nodes*self.n_edge_types*2),
-                         dtype=np.int32)
+        token_onehot = np.zeros(
+            (
+                batch_size,
+                nodes,
+                self.src_ggnn_size if self.src_ggnn_size > 0 else self.state_dim,
+            ),
+            dtype=np.int32,
+        )
+        edges = np.zeros(
+            (batch_size, nodes, nodes * self.n_edge_types * 2), dtype=np.int32
+        )
         npsrc = src[:, :, 0].cpu().data.numpy().astype(np.int32)
 
         # Initialize graph using formatted input sequence
         for i in range(batch_size):
             tokens_done = False
             # Number of flagged nodes defines node count for this sample
             # (Nodes can have no flags on them, but must be in 'flags' list).
@@ -228,97 +243,108 @@
                     # The total number of integers in the vocab should allow
                     # for all features and edges to be defined.
                     if token == self.COMMA:
                         flag_node = 0
                     else:
                         num = self.idx2num[token]
                         if num >= 0:
-                            token_onehot[i][flag_node][num+self.DELIMITER] = 1
+                            token_onehot[i][flag_node][num + self.DELIMITER] = 1
                         flag_node += 1
                 elif token == self.COMMA:
                     edge += 1
-                    assert source_node == -1, \
-                        f'Error in graph edge input: {source_node} unpaired'
-                    assert edge < self.n_edge_types, \
-                        "Too many edge types in input"
+                    assert (
+                        source_node == -1
+                    ), f"Error in graph edge input: {source_node} unpaired"
+                    assert edge < self.n_edge_types, "Too many edge types in input"
                 else:
                     num = self.idx2num[token]
                     if source_node < 0:
                         source_node = num
                     else:
-                        edges[i][source_node][num+nodes*edge] = 1
+                        edges[i][source_node][num + nodes * edge] = 1
                         if self.bidir_edges:
-                            edges[i][num][nodes*(edge+self.n_edge_types)
-                                          + source_node] = 1
+                            edges[i][num][
+                                nodes * (edge + self.n_edge_types) + source_node
+                            ] = 1
                         source_node = -1
 
         token_onehot = torch.from_numpy(token_onehot).float().to(src.device)
         if self.src_ggnn_size > 0:
             token_embed = self.embed(token_onehot)
-            prop_state = torch.cat((token_embed, torch.zeros(
-                (batch_size, nodes, self.state_dim - self.src_word_vec_size)
-                 ).float().to(src.device)), 2)
+            prop_state = torch.cat(
+                (
+                    token_embed,
+                    torch.zeros(
+                        (batch_size, nodes, self.state_dim - self.src_word_vec_size)
+                    )
+                    .float()
+                    .to(src.device),
+                ),
+                2,
+            )
         else:
             prop_state = token_onehot
         edges = torch.from_numpy(edges).float().to(src.device)
 
         for i_step in range(self.n_steps):
             in_states = []
             out_states = []
             for i in range(self.n_edge_types):
                 in_states.append(self.in_fcs[i](prop_state))
                 out_states.append(self.out_fcs[i](prop_state))
             in_states = torch.stack(in_states).transpose(0, 1).contiguous()
-            in_states = in_states.view(-1, nodes*self.n_edge_types,
-                                       self.state_dim)
+            in_states = in_states.view(-1, nodes * self.n_edge_types, self.state_dim)
             out_states = torch.stack(out_states).transpose(0, 1).contiguous()
-            out_states = out_states.view(-1, nodes*self.n_edge_types,
-                                         self.state_dim)
+            out_states = out_states.view(-1, nodes * self.n_edge_types, self.state_dim)
 
-            prop_state = self.propogator(in_states, out_states, prop_state,
-                                         edges, nodes)
+            prop_state = self.propogator(
+                in_states, out_states, prop_state, edges, nodes
+            )
 
         if self.bridge_extra_node:
             # Use first extra node as only source for decoder init
             join_state = prop_state[first_extra, torch.arange(batch_size)]
         else:
             # Average all nodes to get bridge input
             join_state = prop_state.mean(0)
-        join_state = torch.stack((join_state, join_state,
-                                  join_state, join_state))
+        join_state = torch.stack((join_state, join_state, join_state, join_state))
         join_state = (join_state, join_state)
 
         enc_final_hs = self._bridge(join_state)
 
         return prop_state, enc_final_hs, src_len
 
-    def _initialize_bridge(self, rnn_type,
-                           hidden_size,
-                           num_layers):
-
+    def _initialize_bridge(self, rnn_type, hidden_size, num_layers):
         # LSTM has hidden and cell state, other only one
         number_of_states = 2 if rnn_type == "LSTM" else 1
         # Total number of states
         self.total_hidden_dim = hidden_size * num_layers
 
         # Build a linear layer for each
-        self.bridge = nn.ModuleList([nn.Linear(self.total_hidden_dim,
-                                               self.total_hidden_dim,
-                                               bias=True)
-                                     for _ in range(number_of_states)])
+        self.bridge = nn.ModuleList(
+            [
+                nn.Linear(self.total_hidden_dim, self.total_hidden_dim, bias=True)
+                for _ in range(number_of_states)
+            ]
+        )
 
     def _bridge(self, hidden):
         """Forward hidden state through bridge."""
+
         def bottle_hidden(linear, states):
             """
             Transform from 3D to 2D, apply linear and return initial size
             """
             size = states.size()
             result = linear(states.view(-1, self.total_hidden_dim))
             return F.leaky_relu(result).view(size)
 
         if isinstance(hidden, tuple):  # LSTM
-            outs = tuple([bottle_hidden(layer, hidden[ix])
-                          for ix, layer in enumerate(self.bridge)])
+            outs = tuple(
+                [
+                    bottle_hidden(layer, hidden[ix])
+                    for ix, layer in enumerate(self.bridge)
+                ]
+            )
         else:
             outs = bottle_hidden(self.bridge[0], hidden)
         return outs
```

### Comparing `OpenNMT-py-3.1.2/onmt/encoders/mean_encoder.py` & `OpenNMT-py-3.1.3/onmt/encoders/mean_encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,17 +16,15 @@
         super(MeanEncoder, self).__init__()
         self.num_layers = num_layers
         self.embeddings = embeddings
 
     @classmethod
     def from_opt(cls, opt, embeddings):
         """Alternate constructor."""
-        return cls(
-            opt.enc_layers,
-            embeddings)
+        return cls(opt.enc_layers, embeddings)
 
     def forward(self, src, src_len=None):
         """See :func:`EncoderBase.forward()`"""
 
         emb = self.embeddings(src)
         batch, _, emb_dim = emb.size()
```

### Comparing `OpenNMT-py-3.1.2/onmt/encoders/rnn_encoder.py` & `OpenNMT-py-3.1.3/onmt/encoders/rnn_encoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,117 +6,127 @@
 from torch.nn.utils.rnn import pad_packed_sequence as unpack
 
 from onmt.encoders.encoder import EncoderBase
 from onmt.utils.rnn_factory import rnn_factory
 
 
 class RNNEncoder(EncoderBase):
-    """ A generic recurrent neural network encoder.
+    """A generic recurrent neural network encoder.
 
     Args:
        rnn_type (str):
           style of recurrent unit to use, one of [RNN, LSTM, GRU, SRU]
        bidirectional (bool) : use a bidirectional RNN
        num_layers (int) : number of stacked layers
        hidden_size (int) : hidden size of each layer
        dropout (float) : dropout value for :class:`torch.nn.Dropout`
        embeddings (onmt.modules.Embeddings): embedding module to use
     """
 
-    def __init__(self, rnn_type, bidirectional, num_layers,
-                 hidden_size, dropout=0.0, embeddings=None,
-                 use_bridge=False):
+    def __init__(
+        self,
+        rnn_type,
+        bidirectional,
+        num_layers,
+        hidden_size,
+        dropout=0.0,
+        embeddings=None,
+        use_bridge=False,
+    ):
         super(RNNEncoder, self).__init__()
         assert embeddings is not None
 
         num_directions = 2 if bidirectional else 1
         assert hidden_size % num_directions == 0
         hidden_size = hidden_size // num_directions
         self.embeddings = embeddings
 
-        self.rnn, self.no_pack_padded_seq = \
-            rnn_factory(rnn_type,
-                        input_size=embeddings.embedding_size,
-                        hidden_size=hidden_size,
-                        num_layers=num_layers,
-                        dropout=dropout,
-                        bidirectional=bidirectional)
+        self.rnn, self.no_pack_padded_seq = rnn_factory(
+            rnn_type,
+            input_size=embeddings.embedding_size,
+            hidden_size=hidden_size,
+            num_layers=num_layers,
+            dropout=dropout,
+            bidirectional=bidirectional,
+        )
 
         # Initialize the bridge layer
         self.use_bridge = use_bridge
         if self.use_bridge:
-            self._initialize_bridge(rnn_type,
-                                    hidden_size,
-                                    num_layers)
+            self._initialize_bridge(rnn_type, hidden_size, num_layers)
 
     @classmethod
     def from_opt(cls, opt, embeddings):
         """Alternate constructor."""
         return cls(
             opt.rnn_type,
             opt.brnn,
             opt.enc_layers,
             opt.enc_hid_size,
             opt.dropout[0] if type(opt.dropout) is list else opt.dropout,
             embeddings,
-            opt.bridge)
+            opt.bridge,
+        )
 
     def forward(self, src, src_len=None):
         """See :func:`EncoderBase.forward()`"""
 
         emb = self.embeddings(src)
 
         packed_emb = emb
         if src_len is not None and not self.no_pack_padded_seq:
             # src lengths data is wrapped inside a Tensor.
             src_len_list = src_len.view(-1).tolist()
-            packed_emb = pack(emb, src_len_list, batch_first=True,
-                              enforce_sorted=False)
+            packed_emb = pack(emb, src_len_list, batch_first=True, enforce_sorted=False)
 
         enc_out, enc_final_hs = self.rnn(packed_emb)
 
         if src_len is not None and not self.no_pack_padded_seq:
             enc_out = unpack(enc_out, batch_first=True)[0]
 
         if self.use_bridge:
             enc_final_hs = self._bridge(enc_final_hs)
 
         return enc_out, enc_final_hs, src_len
 
-    def _initialize_bridge(self, rnn_type,
-                           hidden_size,
-                           num_layers):
-
+    def _initialize_bridge(self, rnn_type, hidden_size, num_layers):
         # LSTM has hidden and cell state, other only one
         number_of_states = 2 if rnn_type == "LSTM" else 1
         # Total number of states
         self.total_hidden_dim = hidden_size * num_layers
 
         # Build a linear layer for each
-        self.bridge = nn.ModuleList([nn.Linear(self.total_hidden_dim,
-                                               self.total_hidden_dim,
-                                               bias=True)
-                                     for _ in range(number_of_states)])
+        self.bridge = nn.ModuleList(
+            [
+                nn.Linear(self.total_hidden_dim, self.total_hidden_dim, bias=True)
+                for _ in range(number_of_states)
+            ]
+        )
 
     def _bridge(self, hidden):
         """Forward hidden state through bridge.
-           final hidden state ``(num_layers x dir, batch, hidden_size)``
+        final hidden state ``(num_layers x dir, batch, hidden_size)``
         """
+
         def bottle_hidden(linear, states):
             """
             Transform from 3D to 2D, apply linear and return initial size
             """
             states = states.permute(1, 0, 2).contiguous()
             size = states.size()
             result = linear(states.view(-1, self.total_hidden_dim))
             result = F.relu(result).view(size)
             return result.permute(1, 0, 2).contiguous()
 
         if isinstance(hidden, tuple):  # LSTM
-            outs = tuple([bottle_hidden(layer, hidden[ix])
-                          for ix, layer in enumerate(self.bridge)])
+            outs = tuple(
+                [
+                    bottle_hidden(layer, hidden[ix])
+                    for ix, layer in enumerate(self.bridge)
+                ]
+            )
         else:
             outs = bottle_hidden(self.bridge[0], hidden)
         return outs
 
     def update_dropout(self, dropout, attention_dropout=None):
         self.rnn.dropout = dropout
```

### Comparing `OpenNMT-py-3.1.2/onmt/encoders/transformer.py` & `OpenNMT-py-3.1.3/onmt/encoders/transformer.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,42 +22,53 @@
         heads (int): the number of head for MultiHeadedAttention.
         d_ff (int): the second-layer of the PositionwiseFeedForward.
         dropout (float): dropout probability(0-1.0).
         pos_ffn_activation_fn (ActivationFunction):
             activation function choice for PositionwiseFeedForward layer
     """
 
-    def __init__(self, d_model, heads, d_ff, dropout, attention_dropout,
-                 max_relative_positions=0,
-                 pos_ffn_activation_fn=ActivationFunction.relu,
-                 add_qkvbias=False):
+    def __init__(
+        self,
+        d_model,
+        heads,
+        d_ff,
+        dropout,
+        attention_dropout,
+        max_relative_positions=0,
+        pos_ffn_activation_fn=ActivationFunction.relu,
+        add_qkvbias=False,
+    ):
         super(TransformerEncoderLayer, self).__init__()
 
         self.self_attn = MultiHeadedAttention(
-            heads, d_model, dropout=attention_dropout,
+            heads,
+            d_model,
+            dropout=attention_dropout,
             max_relative_positions=max_relative_positions,
-            attn_type="self", add_qkvbias=add_qkvbias)
-        self.feed_forward = PositionwiseFeedForward(d_model, d_ff, dropout,
-                                                    pos_ffn_activation_fn)
+            attn_type="self",
+            add_qkvbias=add_qkvbias,
+        )
+        self.feed_forward = PositionwiseFeedForward(
+            d_model, d_ff, dropout, pos_ffn_activation_fn
+        )
         self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
         self.dropout = nn.Dropout(dropout)
 
     def forward(self, layer_in, mask):
         """
         Args:
             layer_in (FloatTensor): ``(batch_size, src_len, model_dim)``
             mask (LongTensor): ``(batch_size, 1, src_len)``
 
         Returns:
             (FloatTensor):
             * layer_out ``(batch_size, src_len, model_dim)``
         """
         input_norm = self.layer_norm(layer_in)
-        context, _ = self.self_attn(input_norm, input_norm, input_norm,
-                                    mask=mask)
+        context, _ = self.self_attn(input_norm, input_norm, input_norm, mask=mask)
         layer_out = self.dropout(context) + layer_in
         layer_out = self.feed_forward(layer_out)
         return layer_out
 
     def update_dropout(self, dropout, attention_dropout):
         self.self_attn.update_dropout(attention_dropout)
         self.feed_forward.update_dropout(dropout)
@@ -83,45 +94,63 @@
         (torch.FloatTensor, torch.FloatTensor):
 
         * enc_out ``(batch_size, src_len, model_dim)``
         * encoder final state: None in the case of Transformer
         * src_len ``(batch_size)``
     """
 
-    def __init__(self, num_layers, d_model, heads, d_ff, dropout,
-                 attention_dropout, embeddings, max_relative_positions,
-                 pos_ffn_activation_fn=ActivationFunction.relu,
-                 add_qkvbias=False):
+    def __init__(
+        self,
+        num_layers,
+        d_model,
+        heads,
+        d_ff,
+        dropout,
+        attention_dropout,
+        embeddings,
+        max_relative_positions,
+        pos_ffn_activation_fn=ActivationFunction.relu,
+        add_qkvbias=False,
+    ):
         super(TransformerEncoder, self).__init__()
 
         self.embeddings = embeddings
         self.transformer = nn.ModuleList(
-            [TransformerEncoderLayer(
-                d_model, heads, d_ff, dropout, attention_dropout,
-                max_relative_positions=max_relative_positions,
-                pos_ffn_activation_fn=pos_ffn_activation_fn,
-                add_qkvbias=add_qkvbias)
-             for i in range(num_layers)])
+            [
+                TransformerEncoderLayer(
+                    d_model,
+                    heads,
+                    d_ff,
+                    dropout,
+                    attention_dropout,
+                    max_relative_positions=max_relative_positions,
+                    pos_ffn_activation_fn=pos_ffn_activation_fn,
+                    add_qkvbias=add_qkvbias,
+                )
+                for i in range(num_layers)
+            ]
+        )
         self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
 
     @classmethod
     def from_opt(cls, opt, embeddings):
         """Alternate constructor."""
         return cls(
             opt.enc_layers,
             opt.enc_hid_size,
             opt.heads,
             opt.transformer_ff,
             opt.dropout[0] if type(opt.dropout) is list else opt.dropout,
-            opt.attention_dropout[0] if type(opt.attention_dropout)
-            is list else opt.attention_dropout,
+            opt.attention_dropout[0]
+            if type(opt.attention_dropout) is list
+            else opt.attention_dropout,
             embeddings,
             opt.max_relative_positions,
             pos_ffn_activation_fn=opt.pos_ffn_activation_fn,
-            add_qkvbias=opt.add_qkvbias
+            add_qkvbias=opt.add_qkvbias,
         )
 
     def forward(self, src, src_len=None):
         """See :func:`EncoderBase.forward()`"""
         enc_out = self.embeddings(src)
         mask = ~sequence_mask(src_len).unsqueeze(1)
         mask = mask.unsqueeze(1)
```

### Comparing `OpenNMT-py-3.1.2/onmt/inputters/__init__.py` & `OpenNMT-py-3.1.3/onmt/inputters/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 """Module defining inputters.
 
 Inputters implement the logic of transforming raw data to vectorized inputs,
 e.g., from a line of text to a sequence of vectors.
 """
 from onmt.inputters.inputter import build_vocab, IterOnDevice
-from onmt.inputters.text_utils import text_sort_key, process,\
-    numericalize, tensorify
+from onmt.inputters.text_utils import text_sort_key, process, numericalize, tensorify
 from onmt.inputters.text_corpus import ParallelCorpus, ParallelCorpusIterator
-from onmt.inputters.dynamic_iterator import MixingStrategy, SequentialMixer,\
-    WeightedMixer, DynamicDatasetIter
+from onmt.inputters.dynamic_iterator import (
+    MixingStrategy,
+    SequentialMixer,
+    WeightedMixer,
+    DynamicDatasetIter,
+)
 
 
-__all__ = ['IterOnDevice', 'build_vocab', 'text_sort_key',
-           'process', 'numericalize', 'tensorify',
-           'ParallelCorpus', 'ParallelCorpusIterator',
-           'MixingStrategy', 'SequentialMixer', 'WeightedMixer',
-           'DynamicDatasetIter']
+__all__ = [
+    "IterOnDevice",
+    "build_vocab",
+    "text_sort_key",
+    "process",
+    "numericalize",
+    "tensorify",
+    "ParallelCorpus",
+    "ParallelCorpusIterator",
+    "MixingStrategy",
+    "SequentialMixer",
+    "WeightedMixer",
+    "DynamicDatasetIter",
+]
```

### Comparing `OpenNMT-py-3.1.2/onmt/inputters/dynamic_iterator.py` & `OpenNMT-py-3.1.3/onmt/inputters/dynamic_iterator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Module that contain iterator used for dynamic data."""
 import torch
 from itertools import cycle
 from onmt.constants import CorpusTask
 from onmt.inputters.text_corpus import get_corpora, build_corpora_iters
-from onmt.inputters.text_utils import text_sort_key, process,\
-    numericalize, tensorify, _addcopykeys
+from onmt.inputters.text_utils import (
+    text_sort_key,
+    process,
+    numericalize,
+    tensorify,
+    _addcopykeys,
+)
 from onmt.transforms import make_transforms
 from onmt.utils.logging import init_logger, logger
 from onmt.utils.misc import RandomShuffler
 from torch.utils.data import DataLoader
 
 
 class MixingStrategy(object):
@@ -20,16 +25,15 @@
         self.iterables = iterables
         self.weights = weights
 
     def _valid_iterable(self, iterables, weights):
         iter_keys = iterables.keys()
         weight_keys = weights.keys()
         if iter_keys != weight_keys:
-            raise ValueError(
-                f"keys in {iterables} & {iterables} should be equal.")
+            raise ValueError(f"keys in {iterables} & {iterables} should be equal.")
 
     def __iter__(self):
         raise NotImplementedError
 
 
 class SequentialMixer(MixingStrategy):
     """Generate data sequentially from `iterables` which is exhaustible."""
@@ -58,15 +62,15 @@
     def _logging(self):
         """Report corpora loading statistics."""
         msgs = []
         # patch to log stdout spawned processes of dataloader
         logger = init_logger()
         for ds_name, ds_count in self._counts.items():
             msgs.append(f"\t\t\t* {ds_name}: {ds_count}")
-        logger.info("Weighted corpora loaded so far:\n"+"\n".join(msgs))
+        logger.info("Weighted corpora loaded so far:\n" + "\n".join(msgs))
 
     def _reset_iter(self, ds_name):
         self._iterators[ds_name] = iter(self.iterables[ds_name])
         self._counts[ds_name] = self._counts.get(ds_name, 0) + 1
         self._logging()
 
     def _iter_datasets(self):
@@ -111,94 +115,120 @@
         offset (int): iterate data files with this offset.
 
     Attributes:
         sort_key (function): functions define how to sort examples;
         mixer (MixingStrategy): the strategy to iterate corpora.
     """
 
-    def __init__(self, corpora, corpora_info, transforms, vocabs, task,
-                 batch_type, batch_size, batch_size_multiple, data_type="text",
-                 bucket_size=2048, bucket_size_init=-1,
-                 bucket_size_increment=0, copy=False,
-                 skip_empty_level='warning', stride=1, offset=0):
+    def __init__(
+        self,
+        corpora,
+        corpora_info,
+        transforms,
+        vocabs,
+        task,
+        batch_type,
+        batch_size,
+        batch_size_multiple,
+        data_type="text",
+        bucket_size=2048,
+        bucket_size_init=-1,
+        bucket_size_increment=0,
+        copy=False,
+        skip_empty_level="warning",
+        stride=1,
+        offset=0,
+    ):
         super(DynamicDatasetIter).__init__()
         self.corpora = corpora
         self.transforms = transforms
         self.vocabs = vocabs
         self.corpora_info = corpora_info
         self.task = task
         self.init_iterators = False
         self.batch_size = batch_size
         self.batch_type = batch_type
         self.batch_size_multiple = batch_size_multiple
-        self.device = 'cpu'
+        self.device = "cpu"
         self.sort_key = text_sort_key
         self.bucket_size = bucket_size
         self.bucket_size_init = bucket_size_init
         self.bucket_size_increment = bucket_size_increment
         self.copy = copy
         if stride <= 0:
             raise ValueError(f"Invalid argument for stride={stride}.")
         self.stride = stride
         self.offset = offset
-        if skip_empty_level not in ['silent', 'warning', 'error']:
-            raise ValueError(
-                f"Invalid argument skip_empty_level={skip_empty_level}")
+        if skip_empty_level not in ["silent", "warning", "error"]:
+            raise ValueError(f"Invalid argument skip_empty_level={skip_empty_level}")
         self.skip_empty_level = skip_empty_level
         self.random_shuffler = RandomShuffler()
 
     @classmethod
-    def from_opt(cls, corpora, transforms, vocabs, opt, task, copy,
-                 stride=1, offset=0):
+    def from_opt(cls, corpora, transforms, vocabs, opt, task, copy, stride=1, offset=0):
         """Initilize `DynamicDatasetIter` with options parsed from `opt`."""
         corpora_info = {}
-        batch_size = opt.valid_batch_size if (task == CorpusTask.VALID) \
-            else opt.batch_size
+        batch_size = (
+            opt.valid_batch_size if (task == CorpusTask.VALID) else opt.batch_size
+        )
         if task != CorpusTask.INFER:
             if opt.batch_size_multiple is not None:
                 batch_size_multiple = opt.batch_size_multiple
             else:
                 batch_size_multiple = 8 if opt.model_dtype == "fp16" else 1
             corpora_info = opt.data
             bucket_size = opt.bucket_size
             bucket_size_init = opt.bucket_size_init
             bucket_size_increment = opt.bucket_size_increment
             skip_empty_level = opt.skip_empty_level
         else:
             batch_size_multiple = 1
-            corpora_info[CorpusTask.INFER] = {'transforms': opt.transforms}
-            corpora_info[CorpusTask.INFER]['weight'] = 1
+            corpora_info[CorpusTask.INFER] = {"transforms": opt.transforms}
+            corpora_info[CorpusTask.INFER]["weight"] = 1
             # bucket_size = batch_size
             bucket_size = 16384
             bucket_size_init = -1
             bucket_size_increment = 0
-            skip_empty_level = 'warning'
+            skip_empty_level = "warning"
         return cls(
-            corpora, corpora_info, transforms, vocabs, task, opt.batch_type,
-            batch_size, batch_size_multiple, data_type=opt.data_type,
-            bucket_size=bucket_size, bucket_size_init=bucket_size_init,
+            corpora,
+            corpora_info,
+            transforms,
+            vocabs,
+            task,
+            opt.batch_type,
+            batch_size,
+            batch_size_multiple,
+            data_type=opt.data_type,
+            bucket_size=bucket_size,
+            bucket_size_init=bucket_size_init,
             bucket_size_increment=bucket_size_increment,
             copy=copy,
             skip_empty_level=skip_empty_level,
-            stride=stride, offset=offset
+            stride=stride,
+            offset=offset,
         )
 
     def _init_datasets(self, worker_id):
         if self.num_workers > 0:
             stride = self.stride * self.num_workers
             offset = self.offset * self.num_workers + worker_id
         else:
             stride = self.stride
             offset = self.offset
         datasets_iterables = build_corpora_iters(
-            self.corpora, self.transforms, self.corpora_info,
+            self.corpora,
+            self.transforms,
+            self.corpora_info,
             skip_empty_level=self.skip_empty_level,
-            stride=stride, offset=offset)
+            stride=stride,
+            offset=offset,
+        )
         datasets_weights = {
-            ds_name: int(self.corpora_info[ds_name]['weight'])
+            ds_name: int(self.corpora_info[ds_name]["weight"])
             for ds_name in datasets_iterables.keys()
         }
         if self.task == CorpusTask.TRAIN:
             self.mixer = WeightedMixer(datasets_iterables, datasets_weights)
         else:
             self.mixer = SequentialMixer(datasets_iterables, datasets_weights)
         self.init_iterators = True
@@ -232,57 +262,53 @@
                 if _bucket_size < self.bucket_size:
                     _bucket_size += self.bucket_size_increment
                 else:
                     _bucket_size = self.bucket_size
         if bucket:
             yield self._tuple_to_json_with_tokIDs(bucket)
 
-    def batch_iter(self, data, batch_size, batch_type="sents",
-                   batch_size_multiple=1):
+    def batch_iter(self, data, batch_size, batch_type="sents", batch_size_multiple=1):
         """Yield elements from data in chunks of batch_size,
         where each chunk size is a multiple of batch_size_multiple.
         """
+
         def batch_size_fn(nbsents, maxlen):
-            if batch_type == 'sents':
+            if batch_type == "sents":
                 return nbsents
-            elif batch_type == 'tokens':
+            elif batch_type == "tokens":
                 return nbsents * maxlen
             else:
-                raise ValueError(
-                    f"Invalid argument batch_type={batch_type}")
+                raise ValueError(f"Invalid argument batch_type={batch_type}")
 
         minibatch, maxlen, size_so_far, seen = [], 0, 0, []
         for ex in data:
-            if (
-                   (ex['src']['src'] not in seen) or
-                   (self.task != CorpusTask.TRAIN)
-            ):
-                seen.append(ex['src']['src'])
+            if (ex["src"]["src"] not in seen) or (self.task != CorpusTask.TRAIN):
+                seen.append(ex["src"]["src"])
                 minibatch.append(ex)
                 nbsents = len(minibatch)
                 maxlen = max(text_sort_key(ex), maxlen)
                 size_so_far = batch_size_fn(nbsents, maxlen)
                 if size_so_far >= batch_size:
                     overflowed = 0
                     if size_so_far > batch_size:
                         overflowed += 1
                     if batch_size_multiple > 1:
                         overflowed += (
-                            (len(minibatch) - overflowed)
-                            % batch_size_multiple)
+                            len(minibatch) - overflowed
+                        ) % batch_size_multiple
                     if overflowed == 0:
                         yield minibatch
                         minibatch, maxlen, size_so_far, seen = [], 0, 0, []
                     else:
                         if overflowed == len(minibatch):
                             logger.warning(
-                                 "The batch will be filled until we reach"
-                                 " %d, its size may exceed %d tokens"
-                                 % (batch_size_multiple, batch_size)
-                                 )
+                                "The batch will be filled until we reach"
+                                " %d, its size may exceed %d tokens"
+                                % (batch_size_multiple, batch_size)
+                            )
                         else:
                             yield minibatch[:-overflowed]
                             minibatch = minibatch[-overflowed:]
                             maxlen, size_so_far, seen = 0, 0, []
                             for i, ex in enumerate(minibatch):
                                 maxlen = max(text_sort_key(ex), maxlen)
                                 size_so_far = batch_size_fn(i + 1, maxlen)
@@ -292,33 +318,37 @@
 
     def __iter__(self):
         for bucket in self._bucketing():
             # For TRAIN we need to group examples by length
             # for faster performance, but otherwise, sequential.
             if self.task == CorpusTask.TRAIN:
                 bucket = sorted(bucket, key=self.sort_key)
-            p_batch = list(self.batch_iter(
-                bucket,
-                self.batch_size,
-                batch_type=self.batch_type,
-                batch_size_multiple=self.batch_size_multiple))
+            p_batch = list(
+                self.batch_iter(
+                    bucket,
+                    self.batch_size,
+                    batch_type=self.batch_type,
+                    batch_size_multiple=self.batch_size_multiple,
+                )
+            )
             # For TRAIN we shuffle batches within the bucket
             # otherwise sequential
             if self.task == CorpusTask.TRAIN:
                 p_batch = self.random_shuffler(p_batch)
             for minibatch in p_batch:
                 # for specific case of rnn_packed need to be sorted
                 # within the batch
                 minibatch.sort(key=self.sort_key, reverse=True)
                 tensor_batch = tensorify(self.vocabs, minibatch)
                 yield tensor_batch
 
 
-def build_dynamic_dataset_iter(opt, transforms_cls, vocabs, copy=False,
-                               task=CorpusTask.TRAIN, stride=1, offset=0):
+def build_dynamic_dataset_iter(
+    opt, transforms_cls, vocabs, copy=False, task=CorpusTask.TRAIN, stride=1, offset=0
+):
     """
     Build `DynamicDatasetIter` from opt.
     Typically this function is called for CorpusTask.[TRAIN,VALID,INFER]
     from the main tain / translate scripts
     We disable automatic batching in the DataLoader.
     The custom optimized batching is performed by the
     custom class DynamicDatasetIter inherited from IterableDataset
@@ -331,22 +361,24 @@
     """
     transforms = make_transforms(opt, transforms_cls, vocabs)
     corpora = get_corpora(opt, task)
     if corpora is None:
         assert task != CorpusTask.TRAIN, "only valid corpus is ignorable."
         return None
     data_iter = DynamicDatasetIter.from_opt(
-        corpora, transforms, vocabs, opt, task, copy=copy,
-        stride=stride, offset=offset)
-    data_iter.num_workers = opt.num_workers if \
-        hasattr(opt, 'num_workers') else 0
+        corpora, transforms, vocabs, opt, task, copy=copy, stride=stride, offset=offset
+    )
+    data_iter.num_workers = opt.num_workers if hasattr(opt, "num_workers") else 0
     if data_iter.num_workers == 0 or task == CorpusTask.INFER:
         data_iter._init_datasets(0)  # when workers=0 init_fn not called
         data_loader = data_iter
     else:
-        data_loader = DataLoader(data_iter, batch_size=None,
-                                 pin_memory=True,
-                                 multiprocessing_context="spawn",
-                                 num_workers=data_iter.num_workers,
-                                 worker_init_fn=data_iter._init_datasets,
-                                 prefetch_factor=opt.prefetch_factor)
+        data_loader = DataLoader(
+            data_iter,
+            batch_size=None,
+            pin_memory=True,
+            multiprocessing_context="spawn",
+            num_workers=data_iter.num_workers,
+            worker_init_fn=data_iter._init_datasets,
+            prefetch_factor=opt.prefetch_factor,
+        )
     return data_loader
```

### Comparing `OpenNMT-py-3.1.2/onmt/inputters/inputter.py` & `OpenNMT-py-3.1.3/onmt/inputters/inputter.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,100 +14,105 @@
         super(IterOnDevice).__init__()
         self.iterable = iterable
         self.device_id = device_id
 
     @staticmethod
     def batch_to_device(tensor_batch, device_id):
         """Move `batch` to `device_id`, cpu if `device_id` < 0."""
-        device = torch.device(device_id) if device_id >= 0 \
-            else torch.device('cpu')
+        device = torch.device(device_id) if device_id >= 0 else torch.device("cpu")
         for key in tensor_batch.keys():
-            if key != 'src_ex_vocab':
+            if key != "src_ex_vocab":
                 tensor_batch[key] = tensor_batch[key].to(device)
 
     def __iter__(self):
         for tensor_batch in self.iterable:
             self.batch_to_device(tensor_batch, self.device_id)
             yield tensor_batch
 
 
 def build_vocab(opt, specials):
-    """ Build vocabs dict to be stored in the checkpoint
+    """Build vocabs dict to be stored in the checkpoint
         based on vocab files having each line [token, count]
     Args:
         opt: src_vocab, tgt_vocab, n_src_feats
     Return:
         vocabs: {'src': pyonmttok.Vocab, 'tgt': pyonmttok.Vocab,
                  'src_feats' : [pyonmttok.Vocab, ...]},
                  'data_task': seq2seq or lm
                  'decoder_start_token': DefaultTokens.BOS
                 }
     """
+
     def _pad_vocab_to_multiple(vocab, multiple):
         vocab_size = len(vocab)
         if vocab_size % multiple == 0:
             return vocab
         target_size = int(math.ceil(vocab_size / multiple)) * multiple
         for i in range(target_size - vocab_size):
             vocab.add_token(DefaultTokens.VOCAB_PAD + str(i))
         return vocab
 
-    default_specials = [DefaultTokens.UNK,
-                        DefaultTokens.PAD,
-                        DefaultTokens.BOS,
-                        DefaultTokens.EOS]
+    default_specials = opt.default_specials
     vocabs = {}
     src_vocab = _read_vocab_file(opt.src_vocab, opt.src_words_min_frequency)
 
-    src_specials = [item for item in (default_specials + specials['src'])
-                    if item not in src_vocab]
+    src_specials = [
+        item for item in (default_specials + specials["src"]) if item not in src_vocab
+    ]
+
+    if DefaultTokens.SEP in src_specials and "<0x0A>" in src_vocab:
+        src_specials.remove(DefaultTokens.SEP)
+
     src_vocab = pyonmttok.build_vocab_from_tokens(
-        src_vocab,
-        maximum_size=opt.src_vocab_size,
-        special_tokens=src_specials)
+        src_vocab, maximum_size=opt.src_vocab_size, special_tokens=src_specials
+    )
     src_vocab.default_id = src_vocab[DefaultTokens.UNK]
 
     if opt.vocab_size_multiple > 1:
         src_vocab = _pad_vocab_to_multiple(src_vocab, opt.vocab_size_multiple)
-    vocabs['src'] = src_vocab
+    vocabs["src"] = src_vocab
     if opt.share_vocab:
-        vocabs['tgt'] = src_vocab
+        vocabs["tgt"] = src_vocab
     else:
-        tgt_vocab = _read_vocab_file(opt.tgt_vocab,
-                                     opt.tgt_words_min_frequency)
-        tgt_specials = [item for item in (default_specials + specials['tgt'])
-                        if item not in tgt_vocab]
+        tgt_vocab = _read_vocab_file(opt.tgt_vocab, opt.tgt_words_min_frequency)
+        tgt_specials = [
+            item
+            for item in (default_specials + specials["tgt"])
+            if item not in tgt_vocab
+        ]
+        if DefaultTokens.SEP in tgt_specials and "<0x0A>" in tgt_vocab:
+            tgt_specials.remove(DefaultTokens.SEP)
         tgt_vocab = pyonmttok.build_vocab_from_tokens(
-            tgt_vocab,
-            maximum_size=opt.tgt_vocab_size,
-            special_tokens=tgt_specials)
+            tgt_vocab, maximum_size=opt.tgt_vocab_size, special_tokens=tgt_specials
+        )
         tgt_vocab.default_id = tgt_vocab[DefaultTokens.UNK]
         if opt.vocab_size_multiple > 1:
-            tgt_vocab = _pad_vocab_to_multiple(tgt_vocab,
-                                               opt.vocab_size_multiple)
-        vocabs['tgt'] = tgt_vocab
+            tgt_vocab = _pad_vocab_to_multiple(tgt_vocab, opt.vocab_size_multiple)
+        vocabs["tgt"] = tgt_vocab
 
     if opt.n_src_feats > 0:
         src_feats_vocabs = []
         for i in range(opt.n_src_feats):
             src_f_vocab = _read_vocab_file(f"{opt.src_vocab}_feat{i}", 1)
             src_f_vocab = pyonmttok.build_vocab_from_tokens(
                 src_f_vocab,
                 maximum_size=0,
                 minimum_frequency=1,
-                special_tokens=default_specials)
+                special_tokens=default_specials,
+            )
             src_f_vocab.default_id = src_f_vocab[DefaultTokens.UNK]
             if opt.vocab_size_multiple > 1:
-                src_f_vocab = _pad_vocab_to_multiple(src_f_vocab,
-                                                     opt.vocab_size_multiple)
+                src_f_vocab = _pad_vocab_to_multiple(
+                    src_f_vocab, opt.vocab_size_multiple
+                )
             src_feats_vocabs.append(src_f_vocab)
         vocabs["src_feats"] = src_feats_vocabs
 
-    vocabs['data_task'] = opt.data_task
-    vocabs['decoder_start_token'] = opt.decoder_start_token
+    vocabs["data_task"] = opt.data_task
+    vocabs["decoder_start_token"] = opt.decoder_start_token
 
     return vocabs
 
 
 def _read_vocab_file(vocab_path, min_count):
     """Loads a vocabulary from the given path.
 
@@ -115,21 +120,20 @@
         vocab_path (str): Path to utf-8 text file containing vocabulary.
             Each token should be on a line, may followed with a count number
             seperate by space if `with_count`. No extra whitespace is allowed.
         min_count (int): retains only tokens with min_count frequency.
     """
 
     if not os.path.exists(vocab_path):
-        raise RuntimeError(
-            "Vocabulary not found at {}".format(vocab_path))
+        raise RuntimeError("Vocabulary not found at {}".format(vocab_path))
     else:
-        with codecs.open(vocab_path, 'rb', 'utf-8') as f:
-            lines = [line.strip('\n') for line in f if line.strip('\n')]
+        with codecs.open(vocab_path, "rb", "utf-8") as f:
+            lines = [line.strip("\n") for line in f if line.strip("\n")]
             first_line = lines[0].split(None, 1)
-            has_count = (len(first_line) == 2 and first_line[-1].isdigit())
+            has_count = len(first_line) == 2 and first_line[-1].isdigit()
             if has_count:
                 vocab = []
                 for line in lines:
                     if int(line.split(None, 1)[1]) >= min_count:
                         vocab.append(line.split(None, 1)[0])
             else:
                 vocab = lines
@@ -138,42 +142,42 @@
 
 def vocabs_to_dict(vocabs):
     """
     Convert a dict of pyonmttok vocabs
     into a plain text dict to be saved in the checkpoint
     """
     vocabs_dict = {}
-    vocabs_dict['src'] = vocabs['src'].ids_to_tokens
-    vocabs_dict['tgt'] = vocabs['tgt'].ids_to_tokens
-    if 'src_feats' in vocabs.keys():
-        vocabs_dict['src_feats'] = [feat_vocab.ids_to_tokens
-                                    for feat_vocab in vocabs['src_feats']]
-    vocabs_dict['data_task'] = vocabs['data_task']
-    if 'decoder_start_token' in vocabs.keys():
-        vocabs_dict['decoder_start_token'] = vocabs['decoder_start_token']
+    vocabs_dict["src"] = vocabs["src"].ids_to_tokens
+    vocabs_dict["tgt"] = vocabs["tgt"].ids_to_tokens
+    if "src_feats" in vocabs.keys():
+        vocabs_dict["src_feats"] = [
+            feat_vocab.ids_to_tokens for feat_vocab in vocabs["src_feats"]
+        ]
+    vocabs_dict["data_task"] = vocabs["data_task"]
+    if "decoder_start_token" in vocabs.keys():
+        vocabs_dict["decoder_start_token"] = vocabs["decoder_start_token"]
     else:
-        vocabs_dict['decoder_start_token'] = DefaultTokens.BOS
+        vocabs_dict["decoder_start_token"] = DefaultTokens.BOS
     return vocabs_dict
 
 
 def dict_to_vocabs(vocabs_dict):
     """
     Convert a dict formatted vocabs (as stored in a checkpoint)
     into a dict of pyonmttok vocabs objects.
     """
     vocabs = {}
-    vocabs['data_task'] = vocabs_dict['data_task']
-    if 'decoder_start_token' in vocabs_dict.keys():
-        vocabs['decoder_start_token'] = vocabs_dict['decoder_start_token']
+    vocabs["data_task"] = vocabs_dict["data_task"]
+    if "decoder_start_token" in vocabs_dict.keys():
+        vocabs["decoder_start_token"] = vocabs_dict["decoder_start_token"]
     else:
-        vocabs['decoder_start_token'] = DefaultTokens.BOS
-    vocabs['src'] = pyonmttok.build_vocab_from_tokens(vocabs_dict['src'])
-    if vocabs_dict['src'] == vocabs_dict['tgt']:
-        vocabs['tgt'] = vocabs['src']
+        vocabs["decoder_start_token"] = DefaultTokens.BOS
+    vocabs["src"] = pyonmttok.build_vocab_from_tokens(vocabs_dict["src"])
+    if vocabs_dict["src"] == vocabs_dict["tgt"]:
+        vocabs["tgt"] = vocabs["src"]
     else:
-        vocabs['tgt'] = pyonmttok.build_vocab_from_tokens(vocabs_dict['tgt'])
-    if 'src_feats' in vocabs_dict.keys():
-        vocabs['src_feats'] = []
-        for feat_vocab in vocabs_dict['src_feats']:
-            vocabs['src_feats'].append(
-                pyonmttok.build_vocab_from_tokens(feat_vocab))
+        vocabs["tgt"] = pyonmttok.build_vocab_from_tokens(vocabs_dict["tgt"])
+    if "src_feats" in vocabs_dict.keys():
+        vocabs["src_feats"] = []
+        for feat_vocab in vocabs_dict["src_feats"]:
+            vocabs["src_feats"].append(pyonmttok.build_vocab_from_tokens(feat_vocab))
     return vocabs
```

### Comparing `OpenNMT-py-3.1.2/onmt/inputters/text_corpus.py` & `OpenNMT-py-3.1.3/onmt/inputters/text_corpus.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Module that contain shard utils for dynamic data."""
 import os
 from onmt.utils.logging import logger
 from onmt.constants import CorpusName, CorpusTask
 from onmt.transforms import TransformPipe
-from onmt.inputters.text_utils import (
-    process, parse_features, append_features_to_text)
+from onmt.inputters.text_utils import process, parse_features, append_features_to_text
 from contextlib import contextmanager
 
 
 @contextmanager
 def exfile_open(filename, *args, **kwargs):
     """Extended file opener enables open(filename=None).
 
@@ -23,210 +22,223 @@
 
     Yields:
         `None` repeatly if filename==None,
         else yield from file specified in `filename`.
     """
     if filename is None:
         from itertools import repeat
+
         _file = repeat(None)
     else:
         import codecs
+
         _file = codecs.open(filename, *args, **kwargs)
     yield _file
     if filename is not None and _file:
         _file.close()
 
 
 class ParallelCorpus(object):
     """A parallel corpus file pair that can be loaded to iterate."""
 
-    def __init__(self, name, src, tgt, align=None,
-                 n_src_feats=0, src_feats_defaults=None):
+    def __init__(
+        self, name, src, tgt, align=None, n_src_feats=0, src_feats_defaults=None
+    ):
         """Initialize src & tgt side file path."""
         self.id = name
         self.src = src
         self.tgt = tgt
         self.align = align
         self.n_src_feats = n_src_feats
         self.src_feats_defaults = src_feats_defaults
 
     def load(self, offset=0, stride=1):
         """
         Load file and iterate by lines.
         `offset` and `stride` allow to iterate only on every
         `stride` example, starting from `offset`.
         """
-        with exfile_open(self.src, mode='rb') as fs,\
-                exfile_open(self.tgt, mode='rb') as ft,\
-                exfile_open(self.align, mode='rb') as fa:
-            for i, (sline, tline, align) in \
-                    enumerate(zip(fs, ft, fa)):
+        with exfile_open(self.src, mode="rb") as fs, exfile_open(
+            self.tgt, mode="rb"
+        ) as ft, exfile_open(self.align, mode="rb") as fa:
+            for i, (sline, tline, align) in enumerate(zip(fs, ft, fa)):
                 if (i // stride) % stride == offset:
-                    sline = sline.decode('utf-8')
+                    sline = sline.decode("utf-8")
                     sline, sfeats = parse_features(
                         sline,
                         n_feats=self.n_src_feats,
-                        defaults=self.src_feats_defaults)
+                        defaults=self.src_feats_defaults,
+                    )
                     if tline is not None:
-                        tline = tline.decode('utf-8')
+                        tline = tline.decode("utf-8")
                     # 'src_original' and 'tgt_original' store the
                     # original line before tokenization. These
                     # fields are used later on in the feature
                     # transforms.
                     example = {
-                        'src': sline,
-                        'tgt': tline,
-                        'src_original': sline,
-                        'tgt_original': tline
+                        "src": sline,
+                        "tgt": tline,
+                        "src_original": sline,
+                        "tgt_original": tline,
                     }
                     if align is not None:
-                        example['align'] = align.decode('utf-8')
+                        example["align"] = align.decode("utf-8")
 
                     if sfeats is not None:
-                        example['src_feats'] = [f for f in sfeats]
+                        example["src_feats"] = [f for f in sfeats]
                     yield example
 
     def __str__(self):
         cls_name = type(self).__name__
-        return f'{cls_name}({self.id}, {self.src}, {self.tgt}, ' \
-               f'align={self.align}, ' \
-               f'n_src_feats={self.n_src_feats}, ' \
-               f'src_feats_defaults="{self.src_feats_defaults}")'
+        return (
+            f"{cls_name}({self.id}, {self.src}, {self.tgt}, "
+            f"align={self.align}, "
+            f"n_src_feats={self.n_src_feats}, "
+            f'src_feats_defaults="{self.src_feats_defaults}")'
+        )
 
 
 def get_corpora(opts, task=CorpusTask.TRAIN):
     corpora_dict = {}
     if task == CorpusTask.TRAIN:
         for corpus_id, corpus_dict in opts.data.items():
             if corpus_id != CorpusName.VALID:
                 corpora_dict[corpus_id] = ParallelCorpus(
                     corpus_id,
                     corpus_dict["path_src"],
                     corpus_dict["path_tgt"],
                     corpus_dict["path_align"],
                     n_src_feats=opts.n_src_feats,
-                    src_feats_defaults=opts.src_feats_defaults)
+                    src_feats_defaults=opts.src_feats_defaults,
+                )
     elif task == CorpusTask.VALID:
         if CorpusName.VALID in opts.data.keys():
             corpora_dict[CorpusName.VALID] = ParallelCorpus(
                 CorpusName.VALID,
                 opts.data[CorpusName.VALID]["path_src"],
                 opts.data[CorpusName.VALID]["path_tgt"],
                 opts.data[CorpusName.VALID]["path_align"],
                 n_src_feats=opts.n_src_feats,
-                src_feats_defaults=opts.src_feats_defaults)
+                src_feats_defaults=opts.src_feats_defaults,
+            )
         else:
             return None
     else:
         corpora_dict[CorpusName.INFER] = ParallelCorpus(
-                CorpusName.INFER,
-                opts.src,
-                opts.tgt,
-                n_src_feats=opts.n_src_feats,
-                src_feats_defaults=opts.src_feats_defaults)
+            CorpusName.INFER,
+            opts.src,
+            opts.tgt,
+            n_src_feats=opts.n_src_feats,
+            src_feats_defaults=opts.src_feats_defaults,
+        )
     return corpora_dict
 
 
 class ParallelCorpusIterator(object):
     """An iterator dedicated to ParallelCorpus.
 
     Args:
         corpus (ParallelCorpus): corpus to iterate;
         transform (TransformPipe): transforms to be applied to corpus;
         skip_empty_level (str): security level when encouter empty line;
         stride (int): iterate corpus with this line stride;
         offset (int): iterate corpus with this line offset.
     """
 
-    def __init__(self, corpus, transform,
-                 skip_empty_level='warning', stride=1, offset=0):
+    def __init__(
+        self, corpus, transform, skip_empty_level="warning", stride=1, offset=0
+    ):
         self.cid = corpus.id
         self.corpus = corpus
         self.transform = transform
-        if skip_empty_level not in ['silent', 'warning', 'error']:
-            raise ValueError(
-                f"Invalid argument skip_empty_level={skip_empty_level}")
+        if skip_empty_level not in ["silent", "warning", "error"]:
+            raise ValueError(f"Invalid argument skip_empty_level={skip_empty_level}")
         self.skip_empty_level = skip_empty_level
         self.stride = stride
         self.offset = offset
 
     def _tokenize(self, stream):
         for example in stream:
-            example['src'] = example['src'].strip('\n').split()
-            example['src_original'] = \
-                example['src_original'].strip("\n").split()
+            example["src"] = example["src"].strip("\n").split()
+            example["src_original"] = example["src_original"].strip("\n").split()
             if "src_feats" in example:
-                example["src_feats"] = [feat.strip('\n').split()
-                                        for feat in example["src_feats"]]
-            if example['tgt'] is not None:
-                example['tgt'] = example['tgt'].strip('\n').split()
-                example['tgt_original'] = \
-                    example['tgt_original'].strip("\n").split()
-            if 'align' in example:
-                example['align'] = example['align'].strip('\n').split()
+                example["src_feats"] = [
+                    feat.strip("\n").split() for feat in example["src_feats"]
+                ]
+            if example["tgt"] is not None:
+                example["tgt"] = example["tgt"].strip("\n").split()
+                example["tgt_original"] = example["tgt_original"].strip("\n").split()
+            if "align" in example:
+                example["align"] = example["align"].strip("\n").split()
             yield example
 
     def _transform(self, stream):
         for example in stream:
             # NOTE: moved to dynamic_iterator.py cf process()
             # item = self.transform.apply(
             # example, is_train=self.infinitely, corpus_name=self.cid)
             item = (example, self.transform, self.cid)
             if item is not None:
                 yield item
         report_msg = self.transform.stats()
-        if report_msg != '':
+        if report_msg != "":
             logger.info(
                 "* Transform statistics for {}({:.2f}%):\n{}\n".format(
-                    self.cid, 100/self.stride, report_msg
+                    self.cid, 100 / self.stride, report_msg
                 )
             )
 
     def _add_index(self, stream):
         for i, item in enumerate(stream):
             example = item[0]
             line_number = i * self.stride + self.offset
-            example['indices'] = line_number
-            if example['tgt'] is not None:
-                if (len(example['src']) == 0 or len(example['tgt']) == 0 or
-                        ('align' in example and example['align'] == 0)):
+            example["indices"] = line_number
+            if example["tgt"] is not None:
+                if (
+                    len(example["src"]) == 0
+                    or len(example["tgt"]) == 0
+                    or ("align" in example and example["align"] == 0)
+                ):
                     # empty example: skip
                     empty_msg = f"Empty line  in {self.cid}#{line_number}."
-                    if self.skip_empty_level == 'error':
+                    if self.skip_empty_level == "error":
                         raise IOError(empty_msg)
-                    elif self.skip_empty_level == 'warning':
+                    elif self.skip_empty_level == "warning":
                         logger.warning(empty_msg)
-                    if len(example['src']) == 0 and len(example['tgt']) == 0:
+                    if len(example["src"]) == 0 and len(example["tgt"]) == 0:
                         yield item
                     continue
             yield item
 
     def __iter__(self):
-        corpus_stream = self.corpus.load(
-            stride=self.stride, offset=self.offset
-        )
+        corpus_stream = self.corpus.load(stride=self.stride, offset=self.offset)
         tokenized_corpus = self._tokenize(corpus_stream)
         transformed_corpus = self._transform(tokenized_corpus)
         indexed_corpus = self._add_index(transformed_corpus)
         yield from indexed_corpus
 
 
-def build_corpora_iters(corpora, transforms, corpora_info,
-                        skip_empty_level='warning', stride=1, offset=0):
+def build_corpora_iters(
+    corpora, transforms, corpora_info, skip_empty_level="warning", stride=1, offset=0
+):
     """Return `ParallelCorpusIterator` for all corpora defined in opts."""
     corpora_iters = dict()
     for c_id, corpus in corpora.items():
-        transform_names = corpora_info[c_id].get('transforms', [])
+        transform_names = corpora_info[c_id].get("transforms", [])
         corpus_transform = [
             transforms[name] for name in transform_names if name in transforms
         ]
         transform_pipe = TransformPipe.build_from(corpus_transform)
         corpus_iter = ParallelCorpusIterator(
-            corpus, transform_pipe,
-            skip_empty_level=skip_empty_level, stride=stride, offset=offset)
+            corpus,
+            transform_pipe,
+            skip_empty_level=skip_empty_level,
+            stride=stride,
+            offset=offset,
+        )
         corpora_iters[c_id] = corpus_iter
     return corpora_iters
 
 
 def save_transformed_sample(opts, transforms, n_sample=3):
     """Save transformed data sample as specified in opts."""
 
@@ -238,40 +250,42 @@
     elif n_sample > 0:
         logger.info(f"Save {n_sample} transformed example/corpus.")
     else:
         raise ValueError(f"n_sample should >= -1, get {n_sample}.")
 
     corpora = get_corpora(opts, CorpusTask.TRAIN)
     datasets_iterables = build_corpora_iters(
-        corpora, transforms, opts.data,
-        skip_empty_level=opts.skip_empty_level)
-    sample_path = os.path.join(
-        os.path.dirname(opts.save_data), CorpusName.SAMPLE)
+        corpora, transforms, opts.data, skip_empty_level=opts.skip_empty_level
+    )
+    sample_path = os.path.join(os.path.dirname(opts.save_data), CorpusName.SAMPLE)
     os.makedirs(sample_path, exist_ok=True)
     for c_name, c_iter in datasets_iterables.items():
-        dest_base = os.path.join(
-            sample_path, "{}.{}".format(c_name, CorpusName.SAMPLE))
-        with open(dest_base + ".src", 'w', encoding="utf-8") as f_src,\
-                open(dest_base + ".tgt", 'w', encoding="utf-8") as f_tgt:
+        dest_base = os.path.join(sample_path, "{}.{}".format(c_name, CorpusName.SAMPLE))
+        with open(dest_base + ".src", "w", encoding="utf-8") as f_src, open(
+            dest_base + ".tgt", "w", encoding="utf-8"
+        ) as f_tgt:
             bucket = []
             for i, ex in enumerate(c_iter):
                 if i > n_sample:
                     break
                 else:
                     bucket.append(ex)
             pro_bucket = process(CorpusTask.TRAIN, bucket)
             if pro_bucket is not None:
                 for maybe_example in pro_bucket:
                     if maybe_example is not None:
-                        src_line, tgt_line = (maybe_example['src']['src'],
-                                              maybe_example['tgt']['tgt'])
+                        src_line, tgt_line = (
+                            maybe_example["src"]["src"],
+                            maybe_example["tgt"]["tgt"],
+                        )
 
-                        if 'feats' in maybe_example['src']:
-                            src_feats_lines = maybe_example['src']['feats']
+                        if "feats" in maybe_example["src"]:
+                            src_feats_lines = maybe_example["src"]["feats"]
                         else:
                             src_feats_lines = []
 
                         src_pretty_line = append_features_to_text(
-                            src_line, src_feats_lines)
+                            src_line, src_feats_lines
+                        )
 
-                        f_src.write(src_pretty_line + '\n')
-                        f_tgt.write(tgt_line + '\n')
+                        f_src.write(src_pretty_line + "\n")
+                        f_tgt.write(tgt_line + "\n")
```

### Comparing `OpenNMT-py-3.1.2/onmt/inputters/text_utils.py` & `OpenNMT-py-3.1.3/onmt/inputters/text_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,74 +9,77 @@
 def parse_features(line, n_feats=0, defaults=None):
     """
     Parses text lines with features appended to each token.
     Ex.: This￨A￨B is￨A￨A a￨C￨A test￨A￨B
     """
     text, feats = [], [[] for _ in range(n_feats)]
     check, count = 0, 0
-    for token in line.split(' '):
+    for token in line.split(" "):
         tok, *fts = token.strip().split("￨")
         check += len(fts)
         count += 1
         if not fts and defaults is not None:
             if isinstance(defaults, str):
                 defaults = defaults.split("￨")
             if n_feats > 0:
                 assert len(defaults) == n_feats  # Security check
                 fts = defaults
-        assert len(fts) == n_feats, \
-            f"The number of fetures does not match the " \
-            f"expected number of features. Found {len(fts)} " \
+        assert len(fts) == n_feats, (
+            f"The number of fetures does not match the "
+            f"expected number of features. Found {len(fts)} "
             f"features in the data but {n_feats} were expected."
+        )
         text.append(tok)
         for i in range(n_feats):
             feats[i].append(fts[i])
     # Check if all tokens have features or none at all
-    assert check == 0 or check == count*n_feats, \
-        "Some tokens are missing features. Please check your data."
+    assert (
+        check == 0 or check == count * n_feats
+    ), "Some tokens are missing features. Please check your data."
     feats = [" ".join(x) for x in feats] if n_feats > 0 else None
     return " ".join(text), feats
 
 
 def append_features_to_text(text, features):
     """
     It appends features to subwords when dumping to file
     """
-    text_tok = text.split(' ')
-    feats_tok = [x.split(' ') for x in features]
+    text_tok = text.split(" ")
+    feats_tok = [x.split(" ") for x in features]
 
     pretty_toks = []
     for tok, *feats in zip(text_tok, *feats_tok):
-        feats = '￨'.join(feats)
+        feats = "￨".join(feats)
         if feats:
             pretty_toks.append(f"{tok}￨{feats}")
         else:
             pretty_toks.append(tok)
     return " ".join(pretty_toks)
 
 
 def text_sort_key(ex):
     """Sort using the number of tokens in the sequence."""
-    if ex['tgt']:
-        return max(len(ex['src']['src_ids']), len(ex['tgt']['tgt_ids']))
-    return len(ex['src']['src_ids'])
+    if ex["tgt"]:
+        return max(len(ex["src"]["src_ids"]), len(ex["tgt"]["tgt_ids"]))
+    return len(ex["src"]["src_ids"])
 
 
 def clean_example(maybe_example):
-    maybe_example['src'] = {"src": ' '.join(maybe_example['src'])}
+    maybe_example["src"] = {"src": " ".join(maybe_example["src"])}
     # Make features part of src like
     # {'src': {'src': ..., 'feats': [...., ....]}}
-    if 'src_feats' in maybe_example:
-        maybe_example['src']['feats'] = \
-            [' '.join(x) for x in maybe_example["src_feats"]]
-        del maybe_example['src_feats']
-    if maybe_example['tgt'] is not None:
-        maybe_example['tgt'] = {'tgt': ' '.join(maybe_example['tgt'])}
-    if 'align' in maybe_example:
-        maybe_example['align'] = ' '.join(maybe_example['align'])
+    if "src_feats" in maybe_example:
+        maybe_example["src"]["feats"] = [
+            " ".join(x) for x in maybe_example["src_feats"]
+        ]
+        del maybe_example["src_feats"]
+    if maybe_example["tgt"] is not None:
+        maybe_example["tgt"] = {"tgt": " ".join(maybe_example["tgt"])}
+    if "align" in maybe_example:
+        maybe_example["align"] = " ".join(maybe_example["align"])
     return maybe_example
 
 
 def process(task, bucket, **kwargs):
     """Returns valid transformed bucket from bucket."""
     transform_cid_to_examples = {}
     for example in bucket:
@@ -84,19 +87,19 @@
         if transform_cid not in transform_cid_to_examples:
             transform_cid_to_examples[transform_cid] = []
         transform_cid_to_examples[transform_cid].append(example)
 
     processed_bucket = []
     for (transform, cid), sub_bucket in transform_cid_to_examples.items():
         transf_bucket = transform.batch_apply(
-            sub_bucket, is_train=(task == CorpusTask.TRAIN),
-            corpus_name=cid)
+            sub_bucket, is_train=(task == CorpusTask.TRAIN), corpus_name=cid
+        )
         for example, transform, cid in transf_bucket:
             example = clean_example(example)
-            if len(example['src']['src']) > 0:
+            if len(example["src"]["src"]) > 0:
                 processed_bucket.append(example)
 
         # at this point an example looks like:
         # {'src': {'src': ..., 'feats': [....]},
         #  'tgt': {'tgt': ...},
         #  'src_original': ['tok1', ...'tokn'],
         #  'tgt_original': ['tok1', ...'tokm'],
@@ -106,62 +109,58 @@
     if len(processed_bucket) > 0:
         return processed_bucket
     else:
         return None
 
 
 def numericalize(vocabs, example):
-    """
-    """
-    decoder_start_token = vocabs['decoder_start_token']
+    """ """
+    decoder_start_token = vocabs["decoder_start_token"]
     numeric = example
-    numeric['src']['src_ids'] = []
-    if vocabs['data_task'] == ModelTask.SEQ2SEQ:
-        src_text = example['src']['src'].split()
-        numeric['src']['src_ids'] = vocabs['src'](src_text)
-        if example['tgt'] is not None:
-            numeric['tgt']['tgt_ids'] = []
-            tgt_text = example['tgt']['tgt'].split()
-            numeric['tgt']['tgt_ids'] = \
-                vocabs['tgt']([decoder_start_token] + tgt_text
-                              + [DefaultTokens.EOS])
-
-    elif vocabs['data_task'] == ModelTask.LANGUAGE_MODEL:
-        src_text = example['src']['src'].split()
-        numeric['src']['src_ids'] = \
-            vocabs['src']([decoder_start_token] + src_text)
-        if example['tgt'] is not None:
-            numeric['tgt']['tgt_ids'] = []
-            tgt_text = example['tgt']['tgt'].split()
-            numeric['tgt']['tgt_ids'] = \
-                vocabs['tgt'](tgt_text + [DefaultTokens.EOS])
+    numeric["src"]["src_ids"] = []
+    if vocabs["data_task"] == ModelTask.SEQ2SEQ:
+        src_text = example["src"]["src"].split()
+        numeric["src"]["src_ids"] = vocabs["src"](src_text)
+        if example["tgt"] is not None:
+            numeric["tgt"]["tgt_ids"] = []
+            tgt_text = example["tgt"]["tgt"].split()
+            numeric["tgt"]["tgt_ids"] = vocabs["tgt"](
+                [decoder_start_token] + tgt_text + [DefaultTokens.EOS]
+            )
+
+    elif vocabs["data_task"] == ModelTask.LANGUAGE_MODEL:
+        src_text = example["src"]["src"].split()
+        if decoder_start_token != "":
+            src_text = [decoder_start_token] + src_text
+        numeric["src"]["src_ids"] = vocabs["src"](src_text)
+        if example["tgt"] is not None:
+            numeric["tgt"]["tgt_ids"] = []
+            tgt_text = example["tgt"]["tgt"].split()
+            numeric["tgt"]["tgt_ids"] = vocabs["tgt"](tgt_text + [DefaultTokens.EOS])
     else:
-        raise ValueError(
-                f"Something went wrong with task {vocabs['data_task']}"
-        )
+        raise ValueError(f"Something went wrong with task {vocabs['data_task']}")
 
     if "feats" in example["src"]:
         numeric_feats = []
-        for fv, feat in zip(vocabs["src_feats"],
-                            example["src"]["feats"]):
+        for fv, feat in zip(vocabs["src_feats"], example["src"]["feats"]):
             numeric_feats.append(fv(feat.split()))
-        numeric['src']['feats'] = numeric_feats
+        numeric["src"]["feats"] = numeric_feats
 
     return numeric
 
 
 def parse_align_idx(align_pharaoh):
     """
     Parse Pharaoh alignment into [[<src>, <tgt>], ...]
     """
-    align_list = align_pharaoh.strip().split(' ')
+    align_list = align_pharaoh.strip().split(" ")
     flatten_align_idx = []
     for align in align_list:
         try:
-            src_idx, tgt_idx = align.split('-')
+            src_idx, tgt_idx = align.split("-")
         except ValueError:
             logger.warning("{} in `{}`".format(align, align_pharaoh))
             logger.warning("Bad alignement line exists. Please check file!")
             raise
         flatten_align_idx.append([int(src_idx), int(tgt_idx)])
     return flatten_align_idx
 
@@ -183,79 +182,74 @@
          'indices' : [batchsize],
          'srclen': [batchsize],
          'tgtlen': [batchsize],
          'align': alignment sparse tensor
         }
     """
     tensor_batch = {}
-    tbatchsrc = [torch.LongTensor(ex['src']['src_ids']) for ex in minibatch]
-    padidx = vocabs['src'][DefaultTokens.PAD]
-    tbatchsrc = pad_sequence(tbatchsrc, batch_first=True,
-                             padding_value=padidx)
-    if "feats" in minibatch[0]['src']:
+    tbatchsrc = [torch.LongTensor(ex["src"]["src_ids"]) for ex in minibatch]
+    padidx = vocabs["src"][DefaultTokens.PAD]
+    tbatchsrc = pad_sequence(tbatchsrc, batch_first=True, padding_value=padidx)
+    if "feats" in minibatch[0]["src"]:
         tbatchfs = [tbatchsrc]
-        for feat_id in range(len(minibatch[0]['src']["feats"])):
-            tbatchfeat = [torch.LongTensor(ex['src']['feats'][feat_id])
-                          for ex in minibatch]
-            padidx = vocabs['src_feats'][feat_id][DefaultTokens.PAD]
-            tbatchfeat = pad_sequence(tbatchfeat, batch_first=True,
-                                      padding_value=padidx)
+        for feat_id in range(len(minibatch[0]["src"]["feats"])):
+            tbatchfeat = [
+                torch.LongTensor(ex["src"]["feats"][feat_id]) for ex in minibatch
+            ]
+            padidx = vocabs["src_feats"][feat_id][DefaultTokens.PAD]
+            tbatchfeat = pad_sequence(
+                tbatchfeat, batch_first=True, padding_value=padidx
+            )
             tbatchfs.append(tbatchfeat)
         tbatchsrc = torch.stack(tbatchfs, dim=2)
     else:
         # Need to add features in last dimensions
         tbatchsrc = tbatchsrc[:, :, None]
 
-    tensor_batch['src'] = tbatchsrc
-    tensor_batch['indices'] = torch.LongTensor([ex['indices']
-                                                for ex in minibatch])
-    tensor_batch['srclen'] = torch.LongTensor([len(ex['src']['src_ids'])
-                                               for ex in minibatch])
-
-    if minibatch[0]['tgt'] is not None:
-        tbatchtgt = [torch.LongTensor(ex['tgt']['tgt_ids'])
-                     for ex in minibatch]
-        padidx = vocabs['tgt'][DefaultTokens.PAD]
-        tbatchtgt = pad_sequence(tbatchtgt, batch_first=True,
-                                 padding_value=padidx)
+    tensor_batch["src"] = tbatchsrc
+    tensor_batch["indices"] = torch.LongTensor([ex["indices"] for ex in minibatch])
+    tensor_batch["srclen"] = torch.LongTensor(
+        [len(ex["src"]["src_ids"]) for ex in minibatch]
+    )
+
+    if minibatch[0]["tgt"] is not None:
+        tbatchtgt = [torch.LongTensor(ex["tgt"]["tgt_ids"]) for ex in minibatch]
+        padidx = vocabs["tgt"][DefaultTokens.PAD]
+        tbatchtgt = pad_sequence(tbatchtgt, batch_first=True, padding_value=padidx)
         tbatchtgt = tbatchtgt[:, :, None]
-        tbatchtgtlen = torch.LongTensor([len(ex['tgt']['tgt_ids'])
-                                         for ex in minibatch])
-        tensor_batch['tgt'] = tbatchtgt
-        tensor_batch['tgtlen'] = tbatchtgtlen
+        tbatchtgtlen = torch.LongTensor([len(ex["tgt"]["tgt_ids"]) for ex in minibatch])
+        tensor_batch["tgt"] = tbatchtgt
+        tensor_batch["tgtlen"] = tbatchtgtlen
 
-    if 'align' in minibatch[0].keys() and minibatch[0]['align'] is not None:
+    if "align" in minibatch[0].keys() and minibatch[0]["align"] is not None:
         sparse_idx = []
         for i, ex in enumerate(minibatch):
-            for src, tgt in parse_align_idx(ex['align']):
+            for src, tgt in parse_align_idx(ex["align"]):
                 sparse_idx.append([i, tgt + 1, src])
         tbatchalign = torch.LongTensor(sparse_idx)
-        tensor_batch['align'] = tbatchalign
+        tensor_batch["align"] = tbatchalign
 
-    if 'src_map' in minibatch[0].keys():
-        src_vocab_size = max([max(ex['src_map']) for ex in minibatch]) + 1
-        src_map = torch.zeros(len(tensor_batch['srclen']),
-                              tbatchsrc.size(1),
-                              src_vocab_size)
+    if "src_map" in minibatch[0].keys():
+        src_vocab_size = max([max(ex["src_map"]) for ex in minibatch]) + 1
+        src_map = torch.zeros(
+            len(tensor_batch["srclen"]), tbatchsrc.size(1), src_vocab_size
+        )
         for i, ex in enumerate(minibatch):
-            for j, t in enumerate(ex['src_map']):
+            for j, t in enumerate(ex["src_map"]):
                 src_map[i, j, t] = 1
-        tensor_batch['src_map'] = src_map
+        tensor_batch["src_map"] = src_map
 
-    if 'alignment' in minibatch[0].keys():
-        alignment = torch.zeros(len(tensor_batch['srclen']),
-                                tbatchtgt.size(1)).long()
+    if "alignment" in minibatch[0].keys():
+        alignment = torch.zeros(len(tensor_batch["srclen"]), tbatchtgt.size(1)).long()
         for i, ex in enumerate(minibatch):
-            alignment[i, :len(ex['alignment'])] = \
-                torch.LongTensor(ex['alignment'])
-        tensor_batch['alignment'] = alignment
-
-    if 'src_ex_vocab' in minibatch[0].keys():
-        tensor_batch['src_ex_vocab'] = [ex['src_ex_vocab']
-                                        for ex in minibatch]
+            alignment[i, : len(ex["alignment"])] = torch.LongTensor(ex["alignment"])
+        tensor_batch["alignment"] = alignment
+
+    if "src_ex_vocab" in minibatch[0].keys():
+        tensor_batch["src_ex_vocab"] = [ex["src_ex_vocab"] for ex in minibatch]
 
     return tensor_batch
 
 
 def textbatch_to_tensor(vocabs, batch, is_train=False):
     """
     This is a hack to transform a simple batch of texts
@@ -285,32 +279,37 @@
     Args:
         vocabs
         example (dict): An example dictionary with a ``"src"`` key and
             maybe a ``"tgt"`` key. (This argument changes in place!)
     Returns:
         ``example``, changed as described.
     """
-    src = example['src']['src'].split()
+    src = example["src"]["src"].split()
     src_ex_vocab = pyonmttok.build_vocab_from_tokens(
         Counter(src),
         maximum_size=0,
         minimum_frequency=1,
-        special_tokens=[DefaultTokens.UNK,
-                        DefaultTokens.PAD,
-                        DefaultTokens.BOS,
-                        DefaultTokens.EOS])
+        special_tokens=[
+            DefaultTokens.UNK,
+            DefaultTokens.PAD,
+            DefaultTokens.BOS,
+            DefaultTokens.EOS,
+        ],
+    )
     src_ex_vocab.default_id = src_ex_vocab[DefaultTokens.UNK]
     # make a small vocab containing just the tokens in the source sequence
 
     # Map source tokens to indices in the dynamic dict.
-    example['src_map'] = src_ex_vocab(src)
-    example['src_ex_vocab'] = src_ex_vocab
+    example["src_map"] = src_ex_vocab(src)
+    example["src_ex_vocab"] = src_ex_vocab
 
-    if example['tgt'] is not None:
-        if vocabs['data_task'] == ModelTask.SEQ2SEQ:
-            tgt = [DefaultTokens.UNK] + example['tgt']['tgt'].split() \
-                  + [DefaultTokens.UNK]
-        elif vocabs['data_task'] == ModelTask.LANGUAGE_MODEL:
-            tgt = example['tgt']['tgt'].split() \
-                  + [DefaultTokens.UNK]
-        example['alignment'] = src_ex_vocab(tgt)
+    if example["tgt"] is not None:
+        if vocabs["data_task"] == ModelTask.SEQ2SEQ:
+            tgt = (
+                [DefaultTokens.UNK]
+                + example["tgt"]["tgt"].split()
+                + [DefaultTokens.UNK]
+            )
+        elif vocabs["data_task"] == ModelTask.LANGUAGE_MODEL:
+            tgt = example["tgt"]["tgt"].split() + [DefaultTokens.UNK]
+        example["alignment"] = src_ex_vocab(tgt)
     return example
```

### Comparing `OpenNMT-py-3.1.2/onmt/model_builder.py` & `OpenNMT-py-3.1.3/onmt/model_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,38 +34,37 @@
                 module.bias is not None,
                 has_fp16_weights=False,
                 threshold=threshold,
             )
     return model
 
 
-def replace_lora_linear(model, r=2, lora_alpha=1,
-                        lora_dropout=0, layer=""):
+def replace_lora_linear(model, r=2, lora_alpha=1, lora_dropout=0, layer=""):
     """
     Function replacing layers with LoRa layers recursively.
     Args:
         model:
         r: rank of matrix of the Low Rank layer
         lora_alpha: cf paper
         lora_dropout: cf paper
         layer: layer name of the model to be replaced
     """
     for name, module in model.named_children():
         if len(list(module.children())) > 0:
-            replace_lora_linear(module, r, lora_alpha,
-                                lora_dropout, layer)
+            replace_lora_linear(module, r, lora_alpha, lora_dropout, layer)
 
         if isinstance(module, nn.Linear) and name == layer:
             model._modules[name] = Linear(
                 module.in_features,
                 module.out_features,
                 r=r,
                 lora_alpha=lora_alpha,
                 lora_dropout=lora_dropout,
-                bias=module.bias is not None)
+                bias=module.bias is not None,
+            )
     return model
 
 
 def replace_lora_embedding(model, r=2, lora_alpha=1):
     """
     Function replacing Embeddings with LoRa ones recursively.
     Args:
@@ -79,41 +78,40 @@
         if isinstance(module, nn.Embedding):
             model._modules[name] = Embedding(
                 module.num_embeddings,
                 module.embedding_dim,
                 r=r,
                 lora_alpha=lora_alpha,
                 padding_idx=module.padding_idx,
-                sparse=module.sparse)
+                sparse=module.sparse,
+            )
     return model
 
 
 def build_embeddings(opt, vocabs, for_encoder=True):
     """
     Args:
         opt: the option in current environment.
         vocab.
         for_encoder(bool): build Embeddings for encoder or decoder?
     """
     feat_pad_indices = []
     num_feat_embeddings = []
     if for_encoder:
         emb_dim = opt.src_word_vec_size
-        word_padding_idx = vocabs['src'][DefaultTokens.PAD]
-        num_word_embeddings = len(vocabs['src'])
-        if 'src_feats' in vocabs:
-            feat_pad_indices = \
-                [fv[DefaultTokens.PAD] for fv in vocabs['src_feats']]
-            num_feat_embeddings = \
-                [len(fv) for fv in vocabs['src_feats']]
+        word_padding_idx = vocabs["src"][DefaultTokens.PAD]
+        num_word_embeddings = len(vocabs["src"])
+        if "src_feats" in vocabs:
+            feat_pad_indices = [fv[DefaultTokens.PAD] for fv in vocabs["src_feats"]]
+            num_feat_embeddings = [len(fv) for fv in vocabs["src_feats"]]
         freeze_word_vecs = opt.freeze_word_vecs_enc
     else:
         emb_dim = opt.tgt_word_vec_size
-        word_padding_idx = vocabs['tgt'][DefaultTokens.PAD]
-        num_word_embeddings = len(vocabs['tgt'])
+        word_padding_idx = vocabs["tgt"][DefaultTokens.PAD]
+        num_word_embeddings = len(vocabs["tgt"])
         freeze_word_vecs = opt.freeze_word_vecs_dec
 
     emb = Embeddings(
         word_vec_size=emb_dim,
         position_encoding=opt.position_encoding,
         position_encoding_type=opt.position_encoding_type,
         feat_merge=opt.feat_merge,
@@ -121,15 +119,15 @@
         feat_vec_size=opt.feat_vec_size,
         dropout=opt.dropout[0] if type(opt.dropout) is list else opt.dropout,
         word_padding_idx=word_padding_idx,
         feat_padding_idx=feat_pad_indices,
         word_vocab_size=num_word_embeddings,
         feat_vocab_sizes=num_feat_embeddings,
         sparse=opt.optim == "sparseadam",
-        freeze_word_vecs=freeze_word_vecs
+        freeze_word_vecs=freeze_word_vecs,
     )
     return emb
 
 
 def build_encoder(opt, embeddings):
     """
     Various encoder dispatcher function.
@@ -144,44 +142,43 @@
 def build_decoder(opt, embeddings):
     """
     Various decoder dispatcher function.
     Args:
         opt: the option in current environment.
         embeddings (Embeddings): vocab embeddings for this decoder.
     """
-    dec_type = "ifrnn" if opt.decoder_type == "rnn" and opt.input_feed \
-               else opt.decoder_type
+    dec_type = (
+        "ifrnn" if opt.decoder_type == "rnn" and opt.input_feed else opt.decoder_type
+    )
     return str2dec[dec_type].from_opt(opt, embeddings)
 
 
 def load_test_model(opt, model_path=None):
     if model_path is None:
         model_path = opt.models[0]
-    checkpoint = torch.load(model_path,
-                            map_location=lambda storage, loc: storage)
+    checkpoint = torch.load(model_path, map_location=lambda storage, loc: storage)
 
-    model_opt = ArgumentParser.ckpt_model_opts(checkpoint['opt'])
+    model_opt = ArgumentParser.ckpt_model_opts(checkpoint["opt"])
 
     ArgumentParser.update_model_opts(model_opt)
     ArgumentParser.validate_model_opts(model_opt)
-    vocabs = dict_to_vocabs(checkpoint['vocab'])
+    vocabs = dict_to_vocabs(checkpoint["vocab"])
 
     # Avoid functionality on inference
     model_opt.update_vocab = False
 
     model = build_base_model(model_opt, vocabs, checkpoint)
 
-    if opt.precision == 'fp32':
+    if opt.precision == "fp32":
         model.float()
-    elif opt.precision == 'fp16':
+    elif opt.precision == "fp16":
         model.half()
-    elif opt.precision == 'int8':
+    elif opt.precision == "int8":
         if opt.gpu >= 0:
-            raise ValueError(
-                "Dynamic 8-bit quantization is not supported on GPU")
+            raise ValueError("Dynamic 8-bit quantization is not supported on GPU")
         torch.quantization.quantize_dynamic(model, inplace=True)
 
     if use_gpu(opt) and opt.gpu >= 0:
         model.to(torch.device("cuda", opt.gpu))
 
     model.eval()
     model.generator.eval()
@@ -219,15 +216,15 @@
 
 
 def build_task_specific_model(model_opt, vocabs):
     # Share the embedding matrix - preprocess with share_vocab required.
     if model_opt.share_embeddings:
         # src/tgt vocab should be the same if `-share_vocab` is specified.
         assert (
-            vocabs['src'] == vocabs['tgt']
+            vocabs["src"] == vocabs["tgt"]
         ), "preprocess with -share_vocab if you use share_embeddings"
 
     if model_opt.model_task == ModelTask.SEQ2SEQ:
         encoder, src_emb = build_encoder_with_embeddings(model_opt, vocabs)
         decoder, _ = build_decoder_with_embeddings(
             model_opt,
             vocabs,
@@ -245,44 +242,40 @@
         raise ValueError(f"No model defined for {model_opt.model_task} task")
 
 
 def use_embeddings_from_checkpoint(vocabs, model, generator, checkpoint):
     # Update vocabulary embeddings with checkpoint embeddings
     logger.info("Updating vocabulary embeddings with checkpoint embeddings")
     # Embedding layers
-    enc_emb_name = 'encoder.embeddings.make_embedding.emb_luts.0.weight'
-    dec_emb_name = 'decoder.embeddings.make_embedding.emb_luts.0.weight'
+    enc_emb_name = "encoder.embeddings.make_embedding.emb_luts.0.weight"
+    dec_emb_name = "decoder.embeddings.make_embedding.emb_luts.0.weight"
     model_dict = model.state_dict()
     generator_dict = generator.state_dict()
-    for side, emb_name in [('src', enc_emb_name), ('tgt', dec_emb_name)]:
-        if emb_name not in checkpoint['model']:
+    for side, emb_name in [("src", enc_emb_name), ("tgt", dec_emb_name)]:
+        if emb_name not in checkpoint["model"]:
             continue
         new_tokens = []
-        ckp_vocabs = dict_to_vocabs(checkpoint['vocab'])
+        ckp_vocabs = dict_to_vocabs(checkpoint["vocab"])
         for i, tok in enumerate(vocabs[side].ids_to_tokens):
             if tok in ckp_vocabs[side]:
                 old_i = ckp_vocabs[side].lookup_token(tok)
-                model_dict[emb_name][i] = checkpoint['model'][
-                    emb_name
-                ][old_i]
-                if side == 'tgt':
-                    generator_dict['weight'][i] = checkpoint[
-                        'generator'
-                    ]['weight'][old_i]
-                    generator_dict['bias'][i] = checkpoint[
-                        'generator'
-                    ]['bias'][old_i]
+                model_dict[emb_name][i] = checkpoint["model"][emb_name][old_i]
+                if side == "tgt":
+                    generator_dict["weight"][i] = checkpoint["generator"]["weight"][
+                        old_i
+                    ]
+                    generator_dict["bias"][i] = checkpoint["generator"]["bias"][old_i]
             else:
                 # Just for debugging purposes
                 new_tokens.append(tok)
         logger.info("%s: %d new tokens" % (side, len(new_tokens)))
 
         # Remove old vocabulary associated embeddings
-        del checkpoint['model'][emb_name]
-    del checkpoint['generator']['weight'], checkpoint['generator']['bias']
+        del checkpoint["model"][emb_name]
+    del checkpoint["generator"]["weight"], checkpoint["generator"]["bias"]
     model.load_state_dict(model_dict)
     generator.load_state_dict(generator_dict)
 
 
 def build_base_model(model_opt, vocabs, checkpoint=None):
     """Build a model from opts.
 
@@ -304,50 +297,53 @@
         model_opt.attention_dropout
     except AttributeError:
         model_opt.attention_dropout = model_opt.dropout
 
     # Build Model
     model = build_task_specific_model(model_opt, vocabs)
 
-    if hasattr(model_opt, 'quant_layers') and len(model_opt.quant_layers) > 0:
+    if hasattr(model_opt, "quant_layers") and len(model_opt.quant_layers) > 0:
         for layer in model_opt.quant_layers:
             logger.info("8bit compression of layer %s" % layer)
             model = replace_8bit_linear(model, module_to_convert=layer)
 
     mark_lora = False
-    if hasattr(model_opt, 'lora_layers') and len(model_opt.lora_layers) > 0:
+    if hasattr(model_opt, "lora_layers") and len(model_opt.lora_layers) > 0:
         if model_opt.freeze_encoder or model_opt.freeze_decoder:
             raise ValueError("Cannot use LoRa with Enc/Dec-oder freezing")
         for layer in model_opt.lora_layers:
             logger.info("Adding LoRa layers for %s" % layer)
-            model = replace_lora_linear(model, r=model_opt.lora_rank,
-                                        lora_alpha=model_opt.lora_alpha,
-                                        lora_dropout=model_opt.lora_dropout,
-                                        layer=layer)
+            model = replace_lora_linear(
+                model,
+                r=model_opt.lora_rank,
+                lora_alpha=model_opt.lora_alpha,
+                lora_dropout=model_opt.lora_dropout,
+                layer=layer,
+            )
         mark_lora = True
-    if hasattr(model_opt, 'lora_embedding') and model_opt.lora_embedding:
+    if hasattr(model_opt, "lora_embedding") and model_opt.lora_embedding:
         if model_opt.freeze_encoder or model_opt.freeze_decoder:
             raise ValueError("Cannot use LoRa with Enc/Dec-oder freezing")
         logger.info("Adding LoRa Embeddings")
-        model = replace_lora_embedding(model, r=model_opt.lora_rank,
-                                       lora_alpha=model_opt.lora_alpha)
+        model = replace_lora_embedding(
+            model, r=model_opt.lora_rank, lora_alpha=model_opt.lora_alpha
+        )
         mark_lora = True
 
     if mark_lora:
-        mark_only_lora_as_trainable(model, bias='lora_only')
+        mark_only_lora_as_trainable(model, bias="lora_only")
 
     # Build Generator.
     if not model_opt.copy_attn:
-        generator = nn.Linear(model_opt.dec_hid_size,
-                              len(vocabs['tgt']))
+        generator = nn.Linear(model_opt.dec_hid_size, len(vocabs["tgt"]))
         if model_opt.share_decoder_embeddings:
             generator.weight = model.decoder.embeddings.word_lut.weight
     else:
-        vocab_size = len(vocabs['tgt'])
-        pad_idx = vocabs['tgt'][DefaultTokens.PAD]
+        vocab_size = len(vocabs["tgt"])
+        pad_idx = vocabs["tgt"][DefaultTokens.PAD]
         generator = CopyGenerator(model_opt.dec_hid_size, vocab_size, pad_idx)
         if model_opt.share_decoder_embeddings:
             generator.linear.weight = model.decoder.embeddings.word_lut.weight
 
     # Load the model states from checkpoint or initialize them.
     if checkpoint is None or model_opt.update_vocab:
         if model_opt.param_init != 0.0:
@@ -361,72 +357,68 @@
                     xavier_uniform_(p)
             for p in generator.parameters():
                 if p.dim() > 1:
                     xavier_uniform_(p)
 
         if hasattr(model, "encoder") and hasattr(model.encoder, "embeddings"):
             model.encoder.embeddings.load_pretrained_vectors(
-                model_opt.pre_word_vecs_enc)
-        if hasattr(model.decoder, 'embeddings'):
+                model_opt.pre_word_vecs_enc
+            )
+        if hasattr(model.decoder, "embeddings"):
             model.decoder.embeddings.load_pretrained_vectors(
-                model_opt.pre_word_vecs_dec)
+                model_opt.pre_word_vecs_dec
+            )
 
     if checkpoint is not None:
         # This preserves backward-compat for models using customed layernorm
         def fix_key(s):
-            s = re.sub(r'(.*)\.layer_norm((_\d+)?)\.b_2',
-                       r'\1.layer_norm\2.bias', s)
-            s = re.sub(r'(.*)\.layer_norm((_\d+)?)\.a_2',
-                       r'\1.layer_norm\2.weight', s)
+            s = re.sub(r"(.*)\.layer_norm((_\d+)?)\.b_2", r"\1.layer_norm\2.bias", s)
+            s = re.sub(r"(.*)\.layer_norm((_\d+)?)\.a_2", r"\1.layer_norm\2.weight", s)
             return s
 
-        checkpoint['model'] = {fix_key(k): v
-                               for k, v in checkpoint['model'].items()}
+        checkpoint["model"] = {fix_key(k): v for k, v in checkpoint["model"].items()}
 
-        if '0.weight' in checkpoint['generator']:
-            checkpoint['generator']['weight'] =\
-                checkpoint['generator'].pop('0.weight')
-        if '0.bias' in checkpoint['generator']:
-            checkpoint['generator']['bias'] =\
-                checkpoint['generator'].pop('0.bias')
+        if "0.weight" in checkpoint["generator"]:
+            checkpoint["generator"]["weight"] = checkpoint["generator"].pop("0.weight")
+        if "0.bias" in checkpoint["generator"]:
+            checkpoint["generator"]["bias"] = checkpoint["generator"].pop("0.bias")
         # end of patch for backward compatibility
 
         if model_opt.update_vocab:
             # Update model embeddings with those from the checkpoint
             # after initialization
-            use_embeddings_from_checkpoint(vocabs, model, generator,
-                                           checkpoint)
+            use_embeddings_from_checkpoint(vocabs, model, generator, checkpoint)
 
         # when using LoRa or updating the vocab (no more embeddings in ckpt)
         # => strict=False when loading state_dict
         strict = (not model_opt.update_vocab) and (not mark_lora)
-        model.load_state_dict(checkpoint['model'],
-                              strict=strict)
-        generator.load_state_dict(checkpoint['generator'],
-                                  strict=strict)
+        model.load_state_dict(checkpoint["model"], strict=strict)
+        generator.load_state_dict(checkpoint["generator"], strict=strict)
 
     model.generator = generator
 
     return model
 
 
 def build_model(model_opt, opt, vocabs, checkpoint):
-    logger.info('Building model...')
+    logger.info("Building model...")
     model = build_base_model(model_opt, vocabs, checkpoint)
 
     if model_opt.freeze_encoder:
         model.encoder.requires_grad_(False)
         model.encoder.embeddings.requires_grad_()
 
     if model_opt.freeze_decoder:
         model.decoder.requires_grad_(False)
         model.decoder.embeddings.requires_grad_()
 
-    if model_opt.model_dtype == 'fp16' and \
-            model_opt.apex_opt_level not in ['O0', 'O1', 'O2', 'O3'] and \
-            model_opt.optim == 'fusedadam':
-        model.half()   # with amp pytorch requires NOT to half the model
+    if (
+        model_opt.model_dtype == "fp16"
+        and model_opt.apex_opt_level not in ["O0", "O1", "O2", "O3"]
+        and model_opt.optim == "fusedadam"
+    ):
+        model.half()  # with amp pytorch requires NOT to half the model
 
     if use_gpu(opt):
         model.to(torch.device("cuda"))
     logger.info(model)
     return model
```

### Comparing `OpenNMT-py-3.1.2/onmt/models/model.py` & `OpenNMT-py-3.1.3/onmt/models/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def count_parameters(self, log=print):
         raise NotImplementedError
 
 
 class NMTModel(BaseModel):
     """NMTModel Class
-        See :class:`~onmt.models.BaseModel` for options."""
+    See :class:`~onmt.models.BaseModel` for options."""
 
     def __init__(self, encoder, decoder):
         super(NMTModel, self).__init__(encoder, decoder)
         self.encoder = encoder
         self.decoder = decoder
 
     def forward(self, src, tgt, src_len, bptt=False, with_align=False):
@@ -62,17 +62,17 @@
         * enc_out + enc_final_hs in the case of CNNs
         * src in the case of Transformer"""
 
         dec_in = tgt[:, :-1, :]
         enc_out, enc_final_hs, src_len = self.encoder(src, src_len)
         if not bptt:
             self.decoder.init_state(src, enc_out, enc_final_hs)
-        dec_out, attns = self.decoder(dec_in, enc_out,
-                                      src_len=src_len,
-                                      with_align=with_align)
+        dec_out, attns = self.decoder(
+            dec_in, enc_out, src_len=src_len, with_align=with_align
+        )
         return dec_out, attns
 
     def update_dropout(self, dropout, attention_dropout):
         self.encoder.update_dropout(dropout, attention_dropout)
         self.decoder.update_dropout(dropout, attention_dropout)
 
     def count_parameters(self, log=print):
@@ -81,48 +81,46 @@
         Returns:
             (int, int):
             * encoder side parameter count
             * decoder side parameter count"""
 
         enc, dec = 0, 0
         for name, param in self.named_parameters():
-            if 'encoder' in name:
+            if "encoder" in name:
                 enc += param.nelement()
             else:
                 dec += param.nelement()
         if callable(log):
-            log('encoder: {}'.format(enc))
-            log('decoder: {}'.format(dec))
-            log('* number of parameters: {}'.format(enc + dec))
+            log("encoder: {}".format(enc))
+            log("decoder: {}".format(dec))
+            log("* number of parameters: {}".format(enc + dec))
         return enc, dec
 
 
 class LanguageModel(BaseModel):
     """NMTModel Class
     Currently TransformerLMDecoder is the only LM decoder implemented
 
     Args:
         decoder (onmt.decoders.TransformerLMDecoder): a transformer decoder"""
 
     def __init__(self, encoder=None, decoder=None):
         super(LanguageModel, self).__init__(encoder, decoder)
         if encoder is not None:
-            raise ValueError("LanguageModel should not be used"
-                             "with an encoder")
+            raise ValueError("LanguageModel should not be used" "with an encoder")
         self.decoder = decoder
 
     def forward(self, src, tgt, src_len, bptt=False, with_align=False):
         """A LanguageModel forward the src side to the decoder along
         with the source lengths vector. It is a decoder only LM (cf GPT-2)"""
 
         if not bptt:
             self.decoder.init_state()
         dec_out, attns = self.decoder(
-            src, enc_out=None, src_len=src_len,
-            with_align=with_align
+            src, enc_out=None, src_len=src_len, with_align=with_align
         )
         return dec_out, attns
 
     def update_dropout(self, dropout, attention_dropout):
         self.decoder.update_dropout(dropout, attention_dropout)
 
     def count_parameters(self, log=print):
```

### Comparing `OpenNMT-py-3.1.2/onmt/models/model_saver.py` & `OpenNMT-py-3.1.3/onmt/models/model_saver.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,43 +7,38 @@
 
 
 def build_model_saver(model_opt, opt, model, vocabs, optim):
     # _check_save_model_path
     save_model_path = os.path.abspath(opt.save_model)
     os.makedirs(os.path.dirname(save_model_path), exist_ok=True)
 
-    model_saver = ModelSaver(opt.save_model,
-                             model,
-                             model_opt,
-                             vocabs,
-                             optim,
-                             opt.keep_checkpoint)
+    model_saver = ModelSaver(
+        opt.save_model, model, model_opt, vocabs, optim, opt.keep_checkpoint
+    )
     return model_saver
 
 
 def load_checkpoint(ckpt_path):
     """Load checkpoint from `ckpt_path` if any else return `None`."""
     checkpoint = None
     if ckpt_path:
-        logger.info('Loading checkpoint from %s' % ckpt_path)
-        checkpoint = torch.load(ckpt_path,
-                                map_location=lambda storage, loc: storage)
+        logger.info("Loading checkpoint from %s" % ckpt_path)
+        checkpoint = torch.load(ckpt_path, map_location=lambda storage, loc: storage)
     return checkpoint
 
 
 class ModelSaverBase(object):
     """Base class for model saving operations
 
     Inherited classes must implement private methods:
     * `_save`
     * `_rm_checkpoint
     """
 
-    def __init__(self, base_path, model, model_opt, vocabs, optim,
-                 keep_checkpoint=-1):
+    def __init__(self, base_path, model, model_opt, vocabs, optim, keep_checkpoint=-1):
         self.base_path = base_path
         self.model = model
         self.model_opt = model_opt
         self.vocabs = vocabs
         self.optim = optim
         self.last_saved_step = None
         self.keep_checkpoint = keep_checkpoint
@@ -67,16 +62,15 @@
                 model_params_data.append(param.data)
                 param.data = avg.data
 
         chkpt, chkpt_name = self._save(step, save_model)
         self.last_saved_step = step
 
         if moving_average:
-            for param_data, param in zip(model_params_data,
-                                         save_model.parameters()):
+            for param_data, param in zip(model_params_data, save_model.parameters()):
                 param.data = param_data
 
         if self.keep_checkpoint > 0:
             if len(self.checkpoint_queue) == self.checkpoint_queue.maxlen:
                 todel = self.checkpoint_queue.popleft()
                 self._rm_checkpoint(todel)
             self.checkpoint_queue.append(chkpt_name)
@@ -108,35 +102,38 @@
         raise NotImplementedError()
 
 
 class ModelSaver(ModelSaverBase):
     """Simple model saver to filesystem"""
 
     def _save(self, step, model):
-        if (hasattr(self.model_opt, 'lora_layers') and
-                len(self.model_opt.lora_layers) > 0) or \
-                (hasattr(self.model_opt, 'lora_embedding') and
-                 self.model_opt.lora_embedding):
-            model_state_dict = lora_state_dict(model, bias='lora_only')
+        if (
+            hasattr(self.model_opt, "lora_layers")
+            and len(self.model_opt.lora_layers) > 0
+        ) or (
+            hasattr(self.model_opt, "lora_embedding") and self.model_opt.lora_embedding
+        ):
+            model_state_dict = lora_state_dict(model, bias="lora_only")
             generator_state_dict = None
         else:
             model_state_dict = model.state_dict()
-            model_state_dict = {k: v for k, v in model_state_dict.items()
-                                if 'generator' not in k}
+            model_state_dict = {
+                k: v for k, v in model_state_dict.items() if "generator" not in k
+            }
             generator_state_dict = model.generator.state_dict()
 
         checkpoint = {
-            'model': model_state_dict,
-            'generator': generator_state_dict,
-            'vocab': vocabs_to_dict(self.vocabs),
-            'opt': self.model_opt,
-            'optim': self.optim.state_dict(),
+            "model": model_state_dict,
+            "generator": generator_state_dict,
+            "vocab": vocabs_to_dict(self.vocabs),
+            "opt": self.model_opt,
+            "optim": self.optim.state_dict(),
         }
 
         logger.info("Saving checkpoint %s_step_%d.pt" % (self.base_path, step))
-        checkpoint_path = '%s_step_%d.pt' % (self.base_path, step)
+        checkpoint_path = "%s_step_%d.pt" % (self.base_path, step)
         torch.save(checkpoint, checkpoint_path)
         return checkpoint, checkpoint_path
 
     def _rm_checkpoint(self, name):
         if os.path.exists(name):
             os.remove(name)
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/__init__.py` & `OpenNMT-py-3.1.3/onmt/modules/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,35 @@
 from onmt.modules.global_attention import GlobalAttention
 from onmt.modules.conv_multi_step_attention import ConvMultiStepAttention
 from onmt.modules.copy_generator import CopyGenerator, CopyGeneratorLoss
 from onmt.modules.multi_headed_attn import MultiHeadedAttention
 from onmt.modules.embeddings import Embeddings, PositionalEncoding
 from onmt.modules.weight_norm import WeightNormConv2d
 from onmt.modules.average_attn import AverageAttention
+from onmt.modules.alibi_position_bias import AlibiPositionalBias
 from onmt.modules.lora import LoRALayer, Embedding, Linear, MergedLinear
 from onmt.modules.lora import mark_only_lora_as_trainable, lora_state_dict
 from onmt.modules.rmsnorm import RMSNorm
 
-__all__ = ["Elementwise", "context_gate_factory", "ContextGate",
-           "GlobalAttention", "ConvMultiStepAttention", "CopyGenerator",
-           "CopyGeneratorLoss", "CopyGeneratorLMLossCompute",
-           "MultiHeadedAttention", "Embeddings", "PositionalEncoding",
-           "WeightNormConv2d", "AverageAttention", "RMSNorm",
-           "LoRALayer", "Embedding", "Linear", "MergedLinear",
-           "mark_only_lora_as_trainable", "lora_state_dict"]
+__all__ = [
+    "Elementwise",
+    "context_gate_factory",
+    "ContextGate",
+    "GlobalAttention",
+    "ConvMultiStepAttention",
+    "CopyGenerator",
+    "CopyGeneratorLoss",
+    "CopyGeneratorLMLossCompute",
+    "MultiHeadedAttention",
+    "Embeddings",
+    "PositionalEncoding",
+    "AlibiPositionalBias",
+    "WeightNormConv2d",
+    "AverageAttention",
+    "RMSNorm",
+    "LoRALayer",
+    "Embedding",
+    "Linear",
+    "MergedLinear",
+    "mark_only_lora_as_trainable",
+    "lora_state_dict",
+]
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/average_attn.py` & `OpenNMT-py-3.1.3/onmt/modules/average_attn.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,39 +5,41 @@
 import torch.nn as nn
 from torch import Tensor
 from typing import Optional
 from onmt.modules.position_ffn import PositionwiseFeedForward
 from onmt.modules.position_ffn import ActivationFunction
 
 
-def cumulative_average_mask(batch_size: int, t_len: int,
-                            device: Optional[torch.device] = None) -> Tensor:
+def cumulative_average_mask(
+    batch_size: int, t_len: int, device: Optional[torch.device] = None
+) -> Tensor:
     """
     Builds the mask to compute the cumulative average as described in
     :cite:`DBLP:journals/corr/abs-1805-00631` -- Figure 3
     Args:
         batch_size (int): batch size
         t_len (int): length of the layer_in
 
     Returns:
         (Tensor):
         * A Tensor of shape ``(batch_size, t_len, t_len)``
     """
 
-    triangle = torch.tril(torch.ones(t_len, t_len,
-                          dtype=torch.float, device=device))
-    weights = torch.ones(1, t_len, dtype=torch.float, device=device) \
-        / torch.arange(1, t_len + 1, dtype=torch.float, device=device)
+    triangle = torch.tril(torch.ones(t_len, t_len, dtype=torch.float, device=device))
+    weights = torch.ones(1, t_len, dtype=torch.float, device=device) / torch.arange(
+        1, t_len + 1, dtype=torch.float, device=device
+    )
     mask = triangle * weights.transpose(0, 1)
 
     return mask.unsqueeze(0).expand(batch_size, t_len, t_len)
 
 
-def cumulative_average(layer_in: Tensor, layer_cache: tuple,
-                       mask=None, step=None) -> Tensor:
+def cumulative_average(
+    layer_in: Tensor, layer_cache: tuple, mask=None, step=None
+) -> Tensor:
     """
     Computes the cumulative average as described in
     :cite:`DBLP:journals/corr/abs-1805-00631` -- Equations (1) (5) (6)
 
     Args:
         layer_in (FloatTensor): sequence to average
             ``(batch_size, input_len, dimension)``
@@ -47,17 +49,16 @@
         step: current step of the dynamic decoding
 
     Returns:
         a tensor of the same shape and type as ``layer_in``.
     """
 
     if layer_cache[0]:
-        average_attention = (layer_in + step *
-                             layer_cache[1]['prev_g']) / (step + 1)
-        layer_cache[1]['prev_g'] = average_attention
+        average_attention = (layer_in + step * layer_cache[1]["prev_g"]) / (step + 1)
+        layer_cache[1]["prev_g"] = average_attention
         return average_attention
     else:
         return torch.matmul(mask.to(layer_in.dtype), layer_in)
 
 
 class AverageAttention(nn.Module):
     # class AverageAttention(torch.jit.ScriptModule):
@@ -70,26 +71,30 @@
        model_dim (int): the dimension of keys/values/queries,
            must be divisible by head_count
        dropout (float): dropout parameter
        pos_ffn_activation_fn (ActivationFunction):
            activation function choice for PositionwiseFeedForward layer
     """
 
-    def __init__(self, model_dim, dropout=0.1, aan_useffn=False,
-                 pos_ffn_activation_fn=ActivationFunction.relu):
+    def __init__(
+        self,
+        model_dim,
+        dropout=0.1,
+        aan_useffn=False,
+        pos_ffn_activation_fn=ActivationFunction.relu,
+    ):
         self.model_dim = model_dim
         self.aan_useffn = aan_useffn
         super(AverageAttention, self).__init__()
         if aan_useffn:
-            self.average_layer = PositionwiseFeedForward(model_dim, model_dim,
-                                                         dropout,
-                                                         pos_ffn_activation_fn
-                                                         )
+            self.average_layer = PositionwiseFeedForward(
+                model_dim, model_dim, dropout, pos_ffn_activation_fn
+            )
         self.gating_layer = nn.Linear(model_dim * 2, model_dim * 2)
-        self.layer_cache = False, {'prev_g': torch.tensor([])}
+        self.layer_cache = False, {"prev_g": torch.tensor([])}
 
     # @torch.jit.script
     def forward(self, layer_in, mask=None, step=None):
         """
         Args:
             layer_in (FloatTensor): ``(batch, t_len, dim)``
 
@@ -99,20 +104,23 @@
             * gating_out ``(batch, tlen, dim)``
             * average_out average attention
                 ``(batch, input_len, dim)``
         """
 
         batch_size = layer_in.size(0)
         t_len = layer_in.size(1)
-        mask = cumulative_average_mask(batch_size, t_len, layer_in.device)\
-            if not self.layer_cache[0] else None
-        average_out = cumulative_average(
-          layer_in, self.layer_cache, mask, step)
+        mask = (
+            cumulative_average_mask(batch_size, t_len, layer_in.device)
+            if not self.layer_cache[0]
+            else None
+        )
+        average_out = cumulative_average(layer_in, self.layer_cache, mask, step)
         if self.aan_useffn:
             average_out = self.average_layer(average_out)
-        gating_out = self.gating_layer(torch.cat((layer_in,
-                                                  average_out), -1))
+        gating_out = self.gating_layer(torch.cat((layer_in, average_out), -1))
         input_gate, forget_gate = torch.chunk(gating_out, 2, dim=2)
-        gating_out = torch.sigmoid(input_gate) * layer_in + \
-            torch.sigmoid(forget_gate) * average_out
+        gating_out = (
+            torch.sigmoid(input_gate) * layer_in
+            + torch.sigmoid(forget_gate) * average_out
+        )
 
         return gating_out, average_out
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/conv_multi_step_attention.py` & `OpenNMT-py-3.1.3/onmt/modules/conv_multi_step_attention.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """ Multi Step Attention for CNN """
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 
-SCALE_WEIGHT = 0.5 ** 0.5
+SCALE_WEIGHT = 0.5**0.5
 
 
 def seq_linear(linear, x):
-    """ linear transform for 3-d tensor """
+    """linear transform for 3-d tensor"""
     batch, hidden_size, length, _ = x.size()
-    h = linear(torch.transpose(x, 1, 2).contiguous().view(
-        batch * length, hidden_size))
+    h = linear(torch.transpose(x, 1, 2).contiguous().view(batch * length, hidden_size))
     return torch.transpose(h.view(batch, length, hidden_size, 1), 1, 2)
 
 
 class ConvMultiStepAttention(nn.Module):
     """
     Conv attention takes a key matrix, a value matrix and a query vector.
     Attention weight is calculated by key matrix with the query vector
@@ -25,19 +24,20 @@
 
     def __init__(self, input_size):
         super(ConvMultiStepAttention, self).__init__()
         self.linear_in = nn.Linear(input_size, input_size)
         self.mask = None
 
     def apply_mask(self, mask):
-        """ Apply mask """
+        """Apply mask"""
         self.mask = mask
 
-    def forward(self, base_target_emb, input_from_dec, encoder_out_top,
-                encoder_out_combine):
+    def forward(
+        self, base_target_emb, input_from_dec, encoder_out_top, encoder_out_combine
+    ):
         """
         Args:
             base_target_emb: target emb tensor
                 ``(batch, channel, height, width)``
             input_from_dec: output of dec conv
                 ``(batch, channel, height, width)``
             encoder_out_top: the key matrix for calc of attention weight,
@@ -51,16 +51,14 @@
         target = (base_target_emb + preatt) * SCALE_WEIGHT
         target = torch.squeeze(target, 3)
         target = torch.transpose(target, 1, 2)
 
         pre_attn = torch.bmm(target, encoder_out_top)
 
         if self.mask is not None:
-            pre_attn.data.masked_fill_(self.mask, -float('inf'))
+            pre_attn.data.masked_fill_(self.mask, -float("inf"))
 
         attn = F.softmax(pre_attn, dim=2)
 
-        context_output = torch.bmm(
-            attn, torch.transpose(encoder_out_combine, 1, 2))
-        context_output = torch.transpose(
-            torch.unsqueeze(context_output, 3), 1, 2)
+        context_output = torch.bmm(attn, torch.transpose(encoder_out_combine, 1, 2))
+        context_output = torch.transpose(torch.unsqueeze(context_output, 3), 1, 2)
         return context_output, attn
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/copy_generator.py` & `OpenNMT-py-3.1.3/onmt/modules/copy_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import torch
 import torch.nn as nn
 
 
-def collapse_copy_scores(scores, batch, tgt_vocab, src_vocabs=None,
-                         batch_dim=1, batch_offset=None):
+def collapse_copy_scores(
+    scores, batch, tgt_vocab, src_vocabs=None, batch_dim=1, batch_offset=None
+):
     """
     Given scores from an expanded dictionary
     corresponeding to a batch, sums together copies,
     with a dictionary word when it is ambiguous.
     """
     offset = len(tgt_vocab)
     for b in range(scores.size(batch_dim)):
         blank = []
         fill = []
 
         if src_vocabs is None:
-            src_vocab = batch['src_ex_vocab'][b]
+            src_vocab = batch["src_ex_vocab"][b]
         else:
             batch_id = batch_offset[b] if batch_offset is not None else b
-            index = batch['indices'].data[batch_id]
+            index = batch["indices"].data[batch_id]
             src_vocab = src_vocabs[index]
 
         for i in range(1, len(src_vocab)):
             sw = src_vocab.ids_to_tokens[i]
             ti = tgt_vocab[sw]
             if ti != 0:
                 blank.append(offset + i)
                 fill.append(ti)
         if blank:
-            blank = torch.Tensor(blank).type_as(batch['indices'].data)
-            fill = torch.Tensor(fill).type_as(batch['indices'].data)
+            blank = torch.Tensor(blank).type_as(batch["indices"].data)
+            fill = torch.Tensor(fill).type_as(batch["indices"].data)
             score = scores[:, b] if batch_dim == 1 else scores[b]
             score.index_add_(1, fill, score.index_select(1, blank))
             score.index_fill_(1, blank, 1e-10)
     return scores
 
 
 class CopyGenerator(nn.Module):
@@ -84,34 +85,33 @@
                ``(batch, src_len, extra_words)``
         """
         _, slen = attn.size()
         batch, _, cvocab = src_map.size()
 
         # Original probabilities.
         logits = self.linear(hidden)
-        logits[:, self.pad_idx] = -float('inf')
+        logits[:, self.pad_idx] = -float("inf")
         prob = torch.softmax(logits, 1)
 
         # Probability of copying p(z=1) batch.
         p_copy = torch.sigmoid(self.linear_copy(hidden))
         # Probability of not copying: p_{word}(w) * (1 - p(z))
         out_prob = torch.mul(prob, 1 - p_copy)
         mul_attn = torch.mul(attn, p_copy)
-        copy_prob = torch.bmm(
-            mul_attn.view(-1, batch, slen).transpose(0, 1),
-            src_map
-        )
+        copy_prob = torch.bmm(mul_attn.view(-1, batch, slen).transpose(0, 1), src_map)
         copy_prob = copy_prob.contiguous().view(-1, cvocab)
         return torch.cat([out_prob, copy_prob], 1)
 
 
 class CopyGeneratorLoss(nn.Module):
     """Copy generator criterion."""
-    def __init__(self, vocab_size, force_copy, unk_index=0,
-                 ignore_index=-100, eps=1e-20):
+
+    def __init__(
+        self, vocab_size, force_copy, unk_index=0, ignore_index=-100, eps=1e-20
+    ):
         super(CopyGeneratorLoss, self).__init__()
         self.force_copy = force_copy
         self.eps = eps
         self.vocab_size = vocab_size
         self.ignore_index = ignore_index
         self.unk_index = unk_index
 
@@ -135,15 +135,13 @@
         copy_tok_probs += self.eps  # to avoid -inf logs
 
         # find the indices in which you do not use the copy mechanism
         non_copy = align == self.unk_index
         if not self.force_copy:
             non_copy = non_copy | (target != self.unk_index)
 
-        probs = torch.where(
-            non_copy, copy_tok_probs + vocab_probs, copy_tok_probs
-        )
+        probs = torch.where(non_copy, copy_tok_probs + vocab_probs, copy_tok_probs)
 
         loss = -probs.log()  # just NLLLoss; can the module be incorporated?
         # Drop padding.
         loss[target == self.ignore_index] = 0
         return loss
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/embeddings.py` & `OpenNMT-py-3.1.3/onmt/modules/embeddings.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,38 +21,43 @@
 
     Args:
        dim (int): embedding size
     """
 
     def __init__(self, dim, enc_type, max_len=5000):
         if dim % 2 != 0:
-            raise ValueError("Cannot use sin/cos positional encoding with "
-                             "odd dim (got dim={:d})".format(dim))
-        if enc_type == 'SinusoidalInterleaved':
+            raise ValueError(
+                "Cannot use sin/cos positional encoding with "
+                "odd dim (got dim={:d})".format(dim)
+            )
+        if enc_type == "SinusoidalInterleaved":
             pe = torch.zeros(max_len, dim)
             position = torch.arange(0, max_len).unsqueeze(1)
-            div_term = torch.exp((torch.arange(0, dim, 2, dtype=torch.float) *
-                                 -(math.log(10000.0) / dim)))
+            div_term = torch.exp(
+                (
+                    torch.arange(0, dim, 2, dtype=torch.float)
+                    * -(math.log(10000.0) / dim)
+                )
+            )
             pe[:, 0::2] = torch.sin(position.float() * div_term)
             pe[:, 1::2] = torch.cos(position.float() * div_term)
-        elif enc_type == 'SinusoidalConcat':
+        elif enc_type == "SinusoidalConcat":
             half_dim = dim // 2
             pe = math.log(10000) / (half_dim - 1)
             pe = torch.exp(torch.arange(half_dim, dtype=torch.float) * -pe)
-            pe = torch.arange(max_len,
-                              dtype=torch.float).unsqueeze(1) * pe.unsqueeze(0)
-            pe = torch.cat([torch.sin(pe),
-                            torch.cos(pe)], dim=1).view(max_len, -1)
+            pe = torch.arange(max_len, dtype=torch.float).unsqueeze(1) * pe.unsqueeze(0)
+            pe = torch.cat([torch.sin(pe), torch.cos(pe)], dim=1).view(max_len, -1)
         else:
             raise ValueError(
                 "Choice of Position encoding is SinusoidalInterleaved or"
-                " SinusoidalConcat.")
+                " SinusoidalConcat."
+            )
         pe = pe.unsqueeze(1)  # we keep pe (len x batch x dim) for back comp
         super(PositionalEncoding, self).__init__()
-        self.register_buffer('pe', pe)
+        self.register_buffer("pe", pe)
         self.dim = dim
 
     def forward(self, emb, step=None):
         """Embed inputs.
 
         Args:
             emb (FloatTensor): Sequence of word vectors
@@ -64,15 +69,15 @@
         emb = emb * math.sqrt(self.dim)
         step = step or 0
         if pe.size(1) < step + emb.size(1):
             raise SequenceTooLongError(
                 f"Sequence is {emb.size(1) + step} but PositionalEncoding is"
                 f" limited to {self.pe.size(1)}. See max_len argument."
             )
-        emb = emb + pe[:, step:emb.size(1)+step, :]
+        emb = emb + pe[:, step : emb.size(1) + step, :]
 
         return emb
 
 
 class Embeddings(nn.Module):
     """Words embeddings for encoder/decoder.
 
@@ -111,119 +116,141 @@
         feat_vocab_sizes (List[int], optional): list of size of dictionary
             of embeddings for each feature.
         dropout (float): dropout probability.
         sparse (bool): sparse embbedings default False
         freeze_word_vecs (bool): freeze weights of word vectors.
     """
 
-    def __init__(self, word_vec_size,
-                 word_vocab_size,
-                 word_padding_idx,
-                 position_encoding=False,
-                 position_encoding_type='SinusoidalInterleaved',
-                 feat_merge="concat",
-                 feat_vec_exponent=0.7,
-                 feat_vec_size=-1,
-                 feat_padding_idx=[],
-                 feat_vocab_sizes=[],
-                 dropout=0,
-                 sparse=False,
-                 freeze_word_vecs=False):
-        self._validate_args(feat_merge, feat_vocab_sizes, feat_vec_exponent,
-                            feat_vec_size, feat_padding_idx)
+    def __init__(
+        self,
+        word_vec_size,
+        word_vocab_size,
+        word_padding_idx,
+        position_encoding=False,
+        position_encoding_type="SinusoidalInterleaved",
+        feat_merge="concat",
+        feat_vec_exponent=0.7,
+        feat_vec_size=-1,
+        feat_padding_idx=[],
+        feat_vocab_sizes=[],
+        dropout=0,
+        sparse=False,
+        freeze_word_vecs=False,
+    ):
+        self._validate_args(
+            feat_merge,
+            feat_vocab_sizes,
+            feat_vec_exponent,
+            feat_vec_size,
+            feat_padding_idx,
+        )
 
         if feat_padding_idx is None:
             feat_padding_idx = []
         self.word_padding_idx = word_padding_idx
 
         self.word_vec_size = word_vec_size
 
         # Dimensions and padding for constructing the word embedding matrix
         vocab_sizes = [word_vocab_size]
         emb_dims = [word_vec_size]
         pad_indices = [word_padding_idx]
 
         # Dimensions and padding for feature embedding matrices
         # (these have no effect if feat_vocab_sizes is empty)
-        if feat_merge == 'sum':
+        if feat_merge == "sum":
             feat_dims = [word_vec_size] * len(feat_vocab_sizes)
         elif feat_vec_size > 0:
             feat_dims = [feat_vec_size] * len(feat_vocab_sizes)
         else:
-            feat_dims = [int(vocab ** feat_vec_exponent)
-                         for vocab in feat_vocab_sizes]
+            feat_dims = [int(vocab**feat_vec_exponent) for vocab in feat_vocab_sizes]
         vocab_sizes.extend(feat_vocab_sizes)
         emb_dims.extend(feat_dims)
         pad_indices.extend(feat_padding_idx)
 
         # The embedding matrix look-up tables. The first look-up table
         # is for words. Subsequent ones are for features, if any exist.
         emb_params = zip(vocab_sizes, emb_dims, pad_indices)
-        embeddings = [nn.Embedding(vocab, dim, padding_idx=pad, sparse=sparse)
-                      for vocab, dim, pad in emb_params]
+        embeddings = [
+            nn.Embedding(vocab, dim, padding_idx=pad, sparse=sparse)
+            for vocab, dim, pad in emb_params
+        ]
         emb_luts = Elementwise(feat_merge, embeddings)
 
         # The final output size of word + feature vectors. This can vary
         # from the word vector size if and only if features are defined.
         # This is the attribute you should access if you need to know
         # how big your embeddings are going to be.
-        self.embedding_size = (sum(emb_dims) if feat_merge == 'concat'
-                               else word_vec_size)
+        self.embedding_size = sum(emb_dims) if feat_merge == "concat" else word_vec_size
 
         # The sequence of operations that converts the input sequence
         # into a sequence of embeddings. At minimum this consists of
         # looking up the embeddings for each word and feature in the
         # input. Model parameters may require the sequence to contain
         # additional operations as well.
         super(Embeddings, self).__init__()
         self.make_embedding = nn.Sequential()
-        self.make_embedding.add_module('emb_luts', emb_luts)
+        self.make_embedding.add_module("emb_luts", emb_luts)
 
-        if feat_merge == 'mlp' and len(feat_vocab_sizes) > 0:
+        if feat_merge == "mlp" and len(feat_vocab_sizes) > 0:
             in_dim = sum(emb_dims)
             mlp = nn.Sequential(nn.Linear(in_dim, word_vec_size), nn.ReLU())
-            self.make_embedding.add_module('mlp', mlp)
+            self.make_embedding.add_module("mlp", mlp)
 
         self.position_encoding = position_encoding
         self.dropout = nn.Dropout(p=dropout)
 
         if self.position_encoding:
-            pe = PositionalEncoding(self.embedding_size,
-                                    position_encoding_type)
-            self.make_embedding.add_module('pe', pe)
+            pe = PositionalEncoding(self.embedding_size, position_encoding_type)
+            self.make_embedding.add_module("pe", pe)
 
         if freeze_word_vecs:
             self.word_lut.weight.requires_grad = False
 
-    def _validate_args(self, feat_merge, feat_vocab_sizes, feat_vec_exponent,
-                       feat_vec_size, feat_padding_idx):
+    def _validate_args(
+        self,
+        feat_merge,
+        feat_vocab_sizes,
+        feat_vec_exponent,
+        feat_vec_size,
+        feat_padding_idx,
+    ):
         if feat_merge == "sum":
             # features must use word_vec_size
             if feat_vec_exponent != 0.7:
-                warnings.warn("Merging with sum, but got non-default "
-                              "feat_vec_exponent. It will be unused.")
+                warnings.warn(
+                    "Merging with sum, but got non-default "
+                    "feat_vec_exponent. It will be unused."
+                )
             if feat_vec_size != -1:
-                warnings.warn("Merging with sum, but got non-default "
-                              "feat_vec_size. It will be unused.")
+                warnings.warn(
+                    "Merging with sum, but got non-default "
+                    "feat_vec_size. It will be unused."
+                )
         elif feat_vec_size > 0:
             # features will use feat_vec_size
             if feat_vec_exponent != -1:
-                warnings.warn("Not merging with sum and positive "
-                              "feat_vec_size, but got non-default "
-                              "feat_vec_exponent. It will be unused.")
+                warnings.warn(
+                    "Not merging with sum and positive "
+                    "feat_vec_size, but got non-default "
+                    "feat_vec_exponent. It will be unused."
+                )
         else:
             if feat_vec_exponent <= 0:
-                raise ValueError("Using feat_vec_exponent to determine "
-                                 "feature vec size, but got feat_vec_exponent "
-                                 "less than or equal to 0.")
+                raise ValueError(
+                    "Using feat_vec_exponent to determine "
+                    "feature vec size, but got feat_vec_exponent "
+                    "less than or equal to 0."
+                )
         n_feats = len(feat_vocab_sizes)
         if n_feats != len(feat_padding_idx):
-            raise ValueError("Got unequal number of feat_vocab_sizes and "
-                             "feat_padding_idx ({:d} != {:d})".format(
-                                n_feats, len(feat_padding_idx)))
+            raise ValueError(
+                "Got unequal number of feat_vocab_sizes and "
+                "feat_padding_idx ({:d} != {:d})".format(n_feats, len(feat_padding_idx))
+            )
 
     @property
     def word_lut(self):
         """Word look-up table."""
         return self.make_embedding[0][0]
 
     @property
@@ -240,16 +267,15 @@
 
         if emb_file:
             pretrained = torch.load(emb_file)
             pretrained_vec_size = pretrained.size(1)
             if self.word_vec_size > pretrained_vec_size:
                 self.word_lut.weight.data[:, :pretrained_vec_size] = pretrained
             elif self.word_vec_size < pretrained_vec_size:
-                self.word_lut.weight.data \
-                    .copy_(pretrained[:, :self.word_vec_size])
+                self.word_lut.weight.data.copy_(pretrained[:, : self.word_vec_size])
             else:
                 self.word_lut.weight.data.copy_(pretrained)
 
     def forward(self, source, step=None):
         """Computes the embeddings for words and features.
 
         Args:
@@ -272,127 +298,125 @@
 
     def update_dropout(self, dropout):
         self.dropout.p = dropout
 
 
 # Some utilitary functions for pretrained embeddings
 
+
 def read_embeddings(path, skip_lines=0, filter_set=None):
     """
     Read an embeddings file in the glove format.
     """
     embs = dict()
     total_vectors_in_file = 0
-    with open(path, 'rb') as f:
+    with open(path, "rb") as f:
         for i, line in enumerate(f):
             if i < skip_lines:
                 continue
             if not line:
                 break
             if len(line) == 0:
                 # is this reachable?
                 continue
 
-            l_split = line.decode('utf8').strip().split(' ')
+            l_split = line.decode("utf8").strip().split(" ")
             if len(l_split) == 2:
                 continue
             total_vectors_in_file += 1
             if filter_set is not None and l_split[0] not in filter_set:
                 continue
             embs[l_split[0]] = [float(em) for em in l_split[1:]]
     return embs, total_vectors_in_file
 
 
 def calc_vocab_load_stats(vocab, loaded_embed_dict):
-    matching_count = len(
-        set(vocab.ids_to_tokens) & set(loaded_embed_dict.keys()))
+    matching_count = len(set(vocab.ids_to_tokens) & set(loaded_embed_dict.keys()))
     missing_count = len(vocab) - matching_count
     percent_matching = matching_count / len(vocab) * 100
     return matching_count, missing_count, percent_matching
 
 
 def convert_to_torch_tensor(word_to_float_list_dict, vocab):
     dim = len(next(iter(word_to_float_list_dict.values())))
     tensor = torch.zeros((len(vocab), dim))
     for word, values in word_to_float_list_dict.items():
         tensor[vocab.tokens_to_ids[word]] = torch.Tensor(values)
     return tensor
 
 
 def prepare_pretrained_embeddings(opt, vocabs):
-    if all([opt.both_embeddings is None,
+    if all(
+        [
+            opt.both_embeddings is None,
             opt.src_embeddings is None,
-            opt.tgt_embeddings is None]):
+            opt.tgt_embeddings is None,
+        ]
+    ):
         return
 
-    assert opt.save_data, "-save_data is required when using \
+    assert (
+        opt.save_data
+    ), "-save_data is required when using \
         pretrained embeddings."
 
     vocs = []
-    for side in ['src', 'tgt']:
+    for side in ["src", "tgt"]:
         vocab = vocabs[side]
         vocs.append(vocab)
     enc_vocab, dec_vocab = vocs
 
     skip_lines = 1 if opt.embeddings_type == "word2vec" else 0
     if opt.both_embeddings is not None:
-        set_of_src_and_tgt_vocab = \
-            set(enc_vocab.ids_to_tokens) | set(dec_vocab.ids_to_tokens)
-        logger.info("Reading encoder and decoder embeddings from {}".format(
-            opt.both_embeddings))
-        src_vectors, total_vec_count = \
-            read_embeddings(opt.both_embeddings, skip_lines,
-                            set_of_src_and_tgt_vocab)
+        set_of_src_and_tgt_vocab = set(enc_vocab.ids_to_tokens) | set(
+            dec_vocab.ids_to_tokens
+        )
+        logger.info(
+            "Reading encoder and decoder embeddings from {}".format(opt.both_embeddings)
+        )
+        src_vectors, total_vec_count = read_embeddings(
+            opt.both_embeddings, skip_lines, set_of_src_and_tgt_vocab
+        )
         tgt_vectors = src_vectors
         logger.info("\tFound {} total vectors in file".format(total_vec_count))
     else:
         if opt.src_embeddings is not None:
-            logger.info("Reading encoder embeddings from {}".format(
-                opt.src_embeddings))
+            logger.info("Reading encoder embeddings from {}".format(opt.src_embeddings))
             src_vectors, total_vec_count = read_embeddings(
-                opt.src_embeddings, skip_lines,
-                filter_set=set(enc_vocab.ids_to_tokens)
+                opt.src_embeddings, skip_lines, filter_set=set(enc_vocab.ids_to_tokens)
             )
-            logger.info("\tFound {} total vectors in file.".format(
-                total_vec_count))
+            logger.info("\tFound {} total vectors in file.".format(total_vec_count))
         else:
             src_vectors = None
         if opt.tgt_embeddings is not None:
-            logger.info("Reading decoder embeddings from {}".format(
-                opt.tgt_embeddings))
+            logger.info("Reading decoder embeddings from {}".format(opt.tgt_embeddings))
             tgt_vectors, total_vec_count = read_embeddings(
-                opt.tgt_embeddings, skip_lines,
-                filter_set=set(dec_vocab.ids_to_tokens)
+                opt.tgt_embeddings, skip_lines, filter_set=set(dec_vocab.ids_to_tokens)
             )
-            logger.info(
-                "\tFound {} total vectors in file".format(total_vec_count))
+            logger.info("\tFound {} total vectors in file".format(total_vec_count))
         else:
             tgt_vectors = None
     logger.info("After filtering to vectors in vocab:")
     if opt.src_embeddings is not None or opt.both_embeddings is not None:
-        logger.info("\t* enc: %d match, %d missing, (%.2f%%)"
-                    % calc_vocab_load_stats(enc_vocab, src_vectors))
+        logger.info(
+            "\t* enc: %d match, %d missing, (%.2f%%)"
+            % calc_vocab_load_stats(enc_vocab, src_vectors)
+        )
     if opt.tgt_embeddings is not None or opt.both_embeddings is not None:
-        logger.info("\t* dec: %d match, %d missing, (%.2f%%)"
-                    % calc_vocab_load_stats(dec_vocab, tgt_vectors))
+        logger.info(
+            "\t* dec: %d match, %d missing, (%.2f%%)"
+            % calc_vocab_load_stats(dec_vocab, tgt_vectors)
+        )
 
     # Write to file
     enc_output_file = opt.save_data + ".enc_embeddings.pt"
     dec_output_file = opt.save_data + ".dec_embeddings.pt"
     if opt.src_embeddings is not None or opt.both_embeddings is not None:
-        logger.info("\nSaving encoder embeddings as:\n\t* enc: %s"
-                    % enc_output_file)
-        torch.save(
-            convert_to_torch_tensor(src_vectors, enc_vocab),
-            enc_output_file
-        )
+        logger.info("\nSaving encoder embeddings as:\n\t* enc: %s" % enc_output_file)
+        torch.save(convert_to_torch_tensor(src_vectors, enc_vocab), enc_output_file)
         # set the opt in place
         opt.pre_word_vecs_enc = enc_output_file
     if opt.tgt_embeddings is not None or opt.both_embeddings is not None:
-        logger.info("\nSaving decoder embeddings as:\n\t* dec: %s"
-                    % dec_output_file)
-        torch.save(
-            convert_to_torch_tensor(tgt_vectors, dec_vocab),
-            dec_output_file
-        )
+        logger.info("\nSaving decoder embeddings as:\n\t* dec: %s" % dec_output_file)
+        torch.save(convert_to_torch_tensor(tgt_vectors, dec_vocab), dec_output_file)
         # set the opt in place
         opt.pre_word_vecs_dec = dec_output_file
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/gate.py` & `OpenNMT-py-3.1.3/onmt/modules/gate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,90 @@
 """ ContextGate module """
 import torch
 import torch.nn as nn
 
 
-def context_gate_factory(gate_type, embeddings_size, decoder_size,
-                         attention_size, output_size):
+def context_gate_factory(
+    gate_type, embeddings_size, decoder_size, attention_size, output_size
+):
     """Returns the correct ContextGate class"""
 
-    gate_types = {'source': SourceContextGate,
-                  'target': TargetContextGate,
-                  'both': BothContextGate}
-
-    assert gate_type in gate_types, "Not valid ContextGate type: {0}".format(
-        gate_type)
-    return gate_types[gate_type](embeddings_size, decoder_size, attention_size,
-                                 output_size)
+    gate_types = {
+        "source": SourceContextGate,
+        "target": TargetContextGate,
+        "both": BothContextGate,
+    }
+
+    assert gate_type in gate_types, "Not valid ContextGate type: {0}".format(gate_type)
+    return gate_types[gate_type](
+        embeddings_size, decoder_size, attention_size, output_size
+    )
 
 
 class ContextGate(nn.Module):
     """
     Context gate is a decoder module that takes as input the previous word
     embedding, the current decoder state and the attention state, and
     produces a gate.
     The gate can be used to select the input from the target side context
     (decoder state), from the source context (attention state) or both.
     """
 
-    def __init__(self, embeddings_size, decoder_size,
-                 attention_size, output_size):
+    def __init__(self, embeddings_size, decoder_size, attention_size, output_size):
         super(ContextGate, self).__init__()
         input_size = embeddings_size + decoder_size + attention_size
         self.gate = nn.Linear(input_size, output_size, bias=True)
         self.sig = nn.Sigmoid()
         self.source_proj = nn.Linear(attention_size, output_size)
-        self.target_proj = nn.Linear(embeddings_size + decoder_size,
-                                     output_size)
+        self.target_proj = nn.Linear(embeddings_size + decoder_size, output_size)
 
     def forward(self, prev_emb, dec_state, attn_state):
         input_tensor = torch.cat((prev_emb, dec_state, attn_state), dim=1)
         z = self.sig(self.gate(input_tensor))
         proj_source = self.source_proj(attn_state)
-        proj_target = self.target_proj(
-            torch.cat((prev_emb, dec_state), dim=1))
+        proj_target = self.target_proj(torch.cat((prev_emb, dec_state), dim=1))
         return z, proj_source, proj_target
 
 
 class SourceContextGate(nn.Module):
     """Apply the context gate only to the source context"""
 
-    def __init__(self, embeddings_size, decoder_size,
-                 attention_size, output_size):
+    def __init__(self, embeddings_size, decoder_size, attention_size, output_size):
         super(SourceContextGate, self).__init__()
-        self.context_gate = ContextGate(embeddings_size, decoder_size,
-                                        attention_size, output_size)
+        self.context_gate = ContextGate(
+            embeddings_size, decoder_size, attention_size, output_size
+        )
         self.tanh = nn.Tanh()
 
     def forward(self, prev_emb, dec_state, attn_state):
-        z, source, target = self.context_gate(
-            prev_emb, dec_state, attn_state)
+        z, source, target = self.context_gate(prev_emb, dec_state, attn_state)
         return self.tanh(target + z * source)
 
 
 class TargetContextGate(nn.Module):
     """Apply the context gate only to the target context"""
 
-    def __init__(self, embeddings_size, decoder_size,
-                 attention_size, output_size):
+    def __init__(self, embeddings_size, decoder_size, attention_size, output_size):
         super(TargetContextGate, self).__init__()
-        self.context_gate = ContextGate(embeddings_size, decoder_size,
-                                        attention_size, output_size)
+        self.context_gate = ContextGate(
+            embeddings_size, decoder_size, attention_size, output_size
+        )
         self.tanh = nn.Tanh()
 
     def forward(self, prev_emb, dec_state, attn_state):
         z, source, target = self.context_gate(prev_emb, dec_state, attn_state)
         return self.tanh(z * target + source)
 
 
 class BothContextGate(nn.Module):
     """Apply the context gate to both contexts"""
 
-    def __init__(self, embeddings_size, decoder_size,
-                 attention_size, output_size):
+    def __init__(self, embeddings_size, decoder_size, attention_size, output_size):
         super(BothContextGate, self).__init__()
-        self.context_gate = ContextGate(embeddings_size, decoder_size,
-                                        attention_size, output_size)
+        self.context_gate = ContextGate(
+            embeddings_size, decoder_size, attention_size, output_size
+        )
         self.tanh = nn.Tanh()
 
     def forward(self, prev_emb, dec_state, attn_state):
         z, source, target = self.context_gate(prev_emb, dec_state, attn_state)
-        return self.tanh((1. - z) * target + z * source)
+        return self.tanh((1.0 - z) * target + z * source)
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/global_attention.py` & `OpenNMT-py-3.1.3/onmt/modules/global_attention.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,25 +64,28 @@
        dim (int): dimensionality of query and key
        coverage (bool): use coverage term
        attn_type (str): type of attention to use, options [dot,general,mlp]
        attn_func (str): attention function to use, options [softmax,sparsemax]
 
     """
 
-    def __init__(self, dim, coverage=False, attn_type="dot",
-                 attn_func="softmax"):
+    def __init__(self, dim, coverage=False, attn_type="dot", attn_func="softmax"):
         super(GlobalAttention, self).__init__()
 
         self.dim = dim
-        assert attn_type in ["dot", "general", "mlp"], (
-            "Please select a valid attention type (got {:s}).".format(
-                attn_type))
+        assert attn_type in [
+            "dot",
+            "general",
+            "mlp",
+        ], "Please select a valid attention type (got {:s}).".format(attn_type)
         self.attn_type = attn_type
-        assert attn_func in ["softmax", "sparsemax"], (
-            "Please select a valid attention function.")
+        assert attn_func in [
+            "softmax",
+            "sparsemax",
+        ], "Please select a valid attention function."
         self.attn_func = attn_func
 
         if self.attn_type == "general":
             self.linear_in = nn.Linear(dim, dim, bias=False)
         elif self.attn_type == "mlp":
             self.linear_context = nn.Linear(dim, dim, bias=False)
             self.linear_query = nn.Linear(dim, dim, bias=True)
@@ -164,29 +167,29 @@
 
         # compute attention scores, as in Luong et al.
         align = self.score(src, enc_out)
 
         if src_len is not None:
             mask = sequence_mask(src_len, max_len=align.size(-1))
             mask = mask.unsqueeze(1)  # Make it broadcastable.
-            align.masked_fill_(~mask, -float('inf'))
+            align.masked_fill_(~mask, -float("inf"))
 
         # Softmax or sparsemax to normalize attention weights
         if self.attn_func == "softmax":
-            align_vectors = F.softmax(align.view(batch*target_l, src_l), -1)
+            align_vectors = F.softmax(align.view(batch * target_l, src_l), -1)
         else:
-            align_vectors = sparsemax(align.view(batch*target_l, src_l), -1)
+            align_vectors = sparsemax(align.view(batch * target_l, src_l), -1)
         align_vectors = align_vectors.view(batch, target_l, src_l)
 
         # each context vector c_t is the weighted average
         # over all the source hidden states
         c = torch.bmm(align_vectors, enc_out)
 
         # concatenate
-        concat_c = torch.cat([c, src], 2).view(batch*target_l, dim*2)
+        concat_c = torch.cat([c, src], 2).view(batch * target_l, dim * 2)
         attn_h = self.linear_out(concat_c).view(batch, target_l, dim)
         if self.attn_type in ["general", "dot"]:
             attn_h = torch.tanh(attn_h)
 
         if one_step:
             attn_h = attn_h.squeeze(1)
             align_vectors = align_vectors.squeeze(1)
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/lora.py` & `OpenNMT-py-3.1.3/onmt/modules/lora.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 import torch.nn as nn
 import torch.nn.functional as F
 
 import math
 from typing import List, Dict
 
 
-class LoRALayer():
+class LoRALayer:
     def __init__(
         self,
         r: int,
         lora_alpha: int,
         lora_dropout: float,
         merge_weights: bool,
     ):
         self.r = r
         self.lora_alpha = lora_alpha
         # Optional dropout
-        if lora_dropout > 0.:
+        if lora_dropout > 0.0:
             self.lora_dropout = nn.Dropout(p=lora_dropout)
         else:
             self.lora_dropout = lambda x: x
         # Mark the weight as unmerged
         self.merged = False
         self.merge_weights = merge_weights
 
@@ -40,283 +40,298 @@
         embedding_dim: int,
         r: int = 0,
         lora_alpha: int = 1,
         merge_weights: bool = True,
         **kwargs
     ):
         nn.Embedding.__init__(self, num_embeddings, embedding_dim, **kwargs)
-        LoRALayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=0,
-                           merge_weights=merge_weights)
+        LoRALayer.__init__(
+            self,
+            r=r,
+            lora_alpha=lora_alpha,
+            lora_dropout=0,
+            merge_weights=merge_weights,
+        )
         # Actual trainable parameters
         if r > 0:
-            self.lora_A = \
-                nn.Parameter(self.weight.new_zeros((r, num_embeddings)))
-            self.lora_B = \
-                nn.Parameter(self.weight.new_zeros((embedding_dim, r)))
+            self.lora_A = nn.Parameter(self.weight.new_zeros((r, num_embeddings)))
+            self.lora_B = nn.Parameter(self.weight.new_zeros((embedding_dim, r)))
             self.scaling = self.lora_alpha / self.r
             # Freezing the pre-trained weight matrix
             self.weight.requires_grad = False
         self.reset_parameters()
 
     def reset_parameters(self):
         nn.Embedding.reset_parameters(self)
-        if hasattr(self, 'lora_A'):
+        if hasattr(self, "lora_A"):
             # initialize A the same way as the default
             # for nn.Linear and B to zero
             nn.init.zeros_(self.lora_A)
             nn.init.normal_(self.lora_B)
 
     def train(self, mode: bool = True):
         nn.Embedding.train(self, mode)
         if mode:
             if self.merge_weights and self.merged:
                 # Make sure that the weights are not merged
                 if self.r > 0:
-                    self.weight.data -= \
-                        (self.lora_B @
-                         self.lora_A).transpose(0, 1) * self.scaling
+                    self.weight.data -= (self.lora_B @ self.lora_A).transpose(
+                        0, 1
+                    ) * self.scaling
                 self.merged = False
         else:
             if self.merge_weights and not self.merged:
                 # Merge the weights and mark it
                 if self.r > 0:
-                    self.weight.data += \
-                        (self.lora_B @
-                         self.lora_A).transpose(0, 1) * self.scaling
+                    self.weight.data += (self.lora_B @ self.lora_A).transpose(
+                        0, 1
+                    ) * self.scaling
                 self.merged = True
 
     def forward(self, x: torch.Tensor):
         if self.r > 0 and not self.merged:
             result = nn.Embedding.forward(self, x)
             if self.r > 0:
                 after_A = F.embedding(
-                    x, self.lora_A.transpose(0, 1),
-                    self.padding_idx, self.max_norm,
-                    self.norm_type, self.scale_grad_by_freq, self.sparse
+                    x,
+                    self.lora_A.transpose(0, 1),
+                    self.padding_idx,
+                    self.max_norm,
+                    self.norm_type,
+                    self.scale_grad_by_freq,
+                    self.sparse,
                 )
-                result += (after_A @
-                           self.lora_B.transpose(0, 1)) * self.scaling
+                result += (after_A @ self.lora_B.transpose(0, 1)) * self.scaling
             return result
         else:
             return nn.Embedding.forward(self, x)
 
 
 class Linear(nn.Linear, LoRALayer):
     # LoRA implemented in a dense layer
     def __init__(
         self,
         in_features: int,
         out_features: int,
         r: int = 0,
         lora_alpha: int = 1,
-        lora_dropout: float = 0.,
+        lora_dropout: float = 0.0,
         fan_in_fan_out: bool = False,
         # Set this to True if the layer to replace stores
         # weight like (fan_in, fan_out)
         merge_weights: bool = True,
         **kwargs
     ):
         nn.Linear.__init__(self, in_features, out_features, **kwargs)
-        LoRALayer.__init__(self, r=r, lora_alpha=lora_alpha,
-                           lora_dropout=lora_dropout,
-                           merge_weights=merge_weights)
+        LoRALayer.__init__(
+            self,
+            r=r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            merge_weights=merge_weights,
+        )
 
         self.fan_in_fan_out = fan_in_fan_out
         # Actual trainable parameters
         if r > 0:
-            self.lora_A = \
-                nn.Parameter(self.weight.new_zeros((r, in_features)))
-            self.lora_B = \
-                nn.Parameter(self.weight.new_zeros((out_features, r)))
+            self.lora_A = nn.Parameter(self.weight.new_zeros((r, in_features)))
+            self.lora_B = nn.Parameter(self.weight.new_zeros((out_features, r)))
             self.scaling = self.lora_alpha / self.r
             # Freezing the pre-trained weight matrix
             self.weight.requires_grad = False
         self.reset_parameters()
         if fan_in_fan_out:
             self.weight.data = self.weight.data.transpose(0, 1)
 
     def reset_parameters(self):
         nn.Linear.reset_parameters(self)
-        if hasattr(self, 'lora_A'):
+        if hasattr(self, "lora_A"):
             # initialize A the same way as the default
             # for nn.Linear and B to zero
             nn.init.kaiming_uniform_(self.lora_A, a=math.sqrt(5))
             nn.init.zeros_(self.lora_B)
 
     def train(self, mode: bool = True):
         def T(w):
             return w.transpose(0, 1) if self.fan_in_fan_out else w
+
         nn.Linear.train(self, mode)
         if mode:
             if self.merge_weights and self.merged:
                 # Make sure that the weights are not merged
                 if self.r > 0:
-                    self.weight.data -= \
-                        T(self.lora_B @ self.lora_A) * self.scaling
+                    self.weight.data -= T(self.lora_B @ self.lora_A) * self.scaling
                 self.merged = False
         else:
             if self.merge_weights and not self.merged:
                 # Merge the weights and mark it
                 if self.r > 0:
-                    self.weight.data += \
-                        T(self.lora_B @ self.lora_A) * self.scaling
+                    self.weight.data += T(self.lora_B @ self.lora_A) * self.scaling
                 self.merged = True
 
     def forward(self, x: torch.Tensor):
         def T(w):
             return w.transpose(0, 1) if self.fan_in_fan_out else w
+
         if self.r > 0 and not self.merged:
             result = F.linear(x, T(self.weight), bias=self.bias)
             if self.r > 0:
-                result += \
-                    (self.lora_dropout(x) @ self.lora_A.transpose(0, 1)
-                     @ self.lora_B.transpose(0, 1)) * self.scaling
+                result += (
+                    self.lora_dropout(x)
+                    @ self.lora_A.transpose(0, 1)
+                    @ self.lora_B.transpose(0, 1)
+                ) * self.scaling
             return result
         else:
             return F.linear(x, T(self.weight), bias=self.bias)
 
 
 class MergedLinear(nn.Linear, LoRALayer):
     # LoRA implemented in a dense layer
     def __init__(
         self,
         in_features: int,
         out_features: int,
         r: int = 0,
         lora_alpha: int = 1,
-        lora_dropout: float = 0.,
+        lora_dropout: float = 0.0,
         enable_lora: List[bool] = [False],
         fan_in_fan_out: bool = False,
         merge_weights: bool = True,
         **kwargs
     ):
         nn.Linear.__init__(self, in_features, out_features, **kwargs)
-        LoRALayer.__init__(self, r=r, lora_alpha=lora_alpha,
-                           lora_dropout=lora_dropout,
-                           merge_weights=merge_weights)
-        assert out_features % len(enable_lora) == 0, \
-            'The length of enable_lora must divide out_features'
+        LoRALayer.__init__(
+            self,
+            r=r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            merge_weights=merge_weights,
+        )
+        assert (
+            out_features % len(enable_lora) == 0
+        ), "The length of enable_lora must divide out_features"
         self.enable_lora = enable_lora
         self.fan_in_fan_out = fan_in_fan_out
         # Actual trainable parameters
         if r > 0 and any(enable_lora):
             self.lora_A = nn.Parameter(
-                self.weight.new_zeros((r * sum(enable_lora), in_features)))
+                self.weight.new_zeros((r * sum(enable_lora), in_features))
+            )
             self.lora_B = nn.Parameter(
-                self.weight.new_zeros((out_features // len(enable_lora)
-                                      * sum(enable_lora), r))
+                self.weight.new_zeros(
+                    (out_features // len(enable_lora) * sum(enable_lora), r)
+                )
             )  # weights for Conv1D with groups=sum(enable_lora)
             self.scaling = self.lora_alpha / self.r
             # Freezing the pre-trained weight matrix
             self.weight.requires_grad = False
             # Compute the indices
             self.lora_ind = self.weight.new_zeros(
-                (out_features, ), dtype=torch.bool
+                (out_features,), dtype=torch.bool
             ).view(len(enable_lora), -1)
             self.lora_ind[enable_lora, :] = True
             self.lora_ind = self.lora_ind.view(-1)
         self.reset_parameters()
         if fan_in_fan_out:
             self.weight.data = self.weight.data.transpose(0, 1)
 
     def reset_parameters(self):
         nn.Linear.reset_parameters(self)
-        if hasattr(self, 'lora_A'):
+        if hasattr(self, "lora_A"):
             # initialize A the same way as the default
             # for nn.Linear and B to zero
             nn.init.kaiming_uniform_(self.lora_A, a=math.sqrt(5))
             nn.init.zeros_(self.lora_B)
 
     def zero_pad(self, x):
         result = x.new_zeros((*x.shape[:-1], self.out_features))
         result = result.view(-1, self.out_features)
         result[:, self.lora_ind] = x.reshape(
-            -1, self.out_features
-            // len(self.enable_lora) * sum(self.enable_lora)
+            -1, self.out_features // len(self.enable_lora) * sum(self.enable_lora)
         )
         return result.view((*x.shape[:-1], self.out_features))
 
     def train(self, mode: bool = True):
         def T(w):
             return w.transpose(0, 1) if self.fan_in_fan_out else w
+
         nn.Linear.train(self, mode)
         if mode:
             if self.merge_weights and self.merged:
                 # Make sure that the weights are not merged
                 if self.r > 0 and any(self.enable_lora):
                     delta_w = F.conv1d(
                         self.lora_A.data.unsqueeze(0),
                         self.lora_B.data.unsqueeze(-1),
-                        groups=sum(self.enable_lora)
+                        groups=sum(self.enable_lora),
                     ).squeeze(0)
-                    self.weight.data -= self.zero_pad(T(delta_w *
-                                                        self.scaling))
+                    self.weight.data -= self.zero_pad(T(delta_w * self.scaling))
                 self.merged = False
         else:
             if self.merge_weights and not self.merged:
                 # Merge the weights and mark it
                 if self.r > 0 and any(self.enable_lora):
                     delta_w = F.conv1d(
                         self.lora_A.data.unsqueeze(0),
                         self.lora_B.data.unsqueeze(-1),
-                        groups=sum(self.enable_lora)
+                        groups=sum(self.enable_lora),
                     ).squeeze(0)
-                    self.weight.data += self.zero_pad(T(delta_w *
-                                                        self.scaling))
+                    self.weight.data += self.zero_pad(T(delta_w * self.scaling))
                 self.merged = True
 
     def forward(self, x: torch.Tensor):
         def T(w):
             return w.transpose(0, 1) if self.fan_in_fan_out else w
+
         if self.merged:
             return F.linear(x, T(self.weight), bias=self.bias)
         else:
             result = F.linear(x, T(self.weight), bias=self.bias)
             if self.r > 0:
                 after_A = F.linear(self.lora_dropout(x), self.lora_A)
                 after_B = F.conv1d(
                     after_A.transpose(-2, -1),
                     self.lora_B.unsqueeze(-1),
-                    groups=sum(self.enable_lora)
+                    groups=sum(self.enable_lora),
                 ).transpose(-2, -1)
                 result += self.zero_pad(after_B) * self.scaling
             return result
 
 
-def mark_only_lora_as_trainable(model: nn.Module, bias: str = 'none') -> None:
+def mark_only_lora_as_trainable(model: nn.Module, bias: str = "none") -> None:
     for n, p in model.named_parameters():
-        if 'lora_' not in n:
+        if "lora_" not in n:
             p.requires_grad = False
-    if bias == 'none':
+    if bias == "none":
         return
-    elif bias == 'all':
+    elif bias == "all":
         for n, p in model.named_parameters():
-            if 'bias' in n:
+            if "bias" in n:
                 p.requires_grad = True
-    elif bias == 'lora_only':
+    elif bias == "lora_only":
         for m in model.modules():
-            if (isinstance(m, LoRALayer) and hasattr(m, 'bias') and
-                    m.bias is not None):
+            if isinstance(m, LoRALayer) and hasattr(m, "bias") and m.bias is not None:
                 m.bias.requires_grad = True
     else:
         raise NotImplementedError
 
 
-def lora_state_dict(model: nn.Module,
-                    bias: str = 'none') -> Dict[str, torch.Tensor]:
+def lora_state_dict(model: nn.Module, bias: str = "none") -> Dict[str, torch.Tensor]:
     my_state_dict = model.state_dict()
-    if bias == 'none':
-        return {k: my_state_dict[k] for k in my_state_dict if 'lora_' in k}
-    elif bias == 'all':
-        return {k: my_state_dict[k] for k in
-                my_state_dict if 'lora_' in k or 'bias' in k}
-    elif bias == 'lora_only':
+    if bias == "none":
+        return {k: my_state_dict[k] for k in my_state_dict if "lora_" in k}
+    elif bias == "all":
+        return {
+            k: my_state_dict[k] for k in my_state_dict if "lora_" in k or "bias" in k
+        }
+    elif bias == "lora_only":
         to_return = {}
         for k in my_state_dict:
-            if 'lora_' in k:
+            if "lora_" in k:
                 to_return[k] = my_state_dict[k]
-                bias_name = k.split('lora_')[0]+'bias'
+                bias_name = k.split("lora_")[0] + "bias"
                 if bias_name in my_state_dict:
                     to_return[bias_name] = my_state_dict[bias_name]
         return to_return
     else:
         raise NotImplementedError
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/multi_headed_attn.py` & `OpenNMT-py-3.1.3/onmt/modules/multi_headed_attn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """ Multi-Head Attention module """
 import math
 import torch
 from torch import Tensor
 from typing import Optional, Tuple
 import torch.nn as nn
+from .alibi_position_bias import AlibiPositionalBias
 
 
 # Help functions for Rotary Embeddings
 # https://arxiv.org/pdf/2104.09864.pdf
 # too convoluted to make maxseqlen a parameter.
 # we suppose src_seq_len at training and max_length at inference
 # are both < 2048 tokens.
 
+
 def rotaryembeddings(dim: int, maxseqlen=4096, base=10000):
     inv_freq = 1.0 / (base ** (torch.arange(0, dim, 2).float() / dim))
     tmax = torch.arange(maxseqlen, device=inv_freq.device)
     rope = torch.outer(tmax, inv_freq).float()
     # rope is now matrix [maxseqlen, dim/2]
     rope = torch.polar(torch.ones_like(rope), rope)
     return rope
@@ -31,16 +33,16 @@
     key_out = torch.view_as_real(key_ * rope).flatten(3)
     return query_out.type_as(query), key_out.type_as(key)
 
 
 # Help functions for max_relative positions
 # https://arxiv.org/abs/1803.02155
 
-def relative_matmul(x: Tensor, z: Tensor,
-                    transpose: bool) -> Tensor:
+
+def relative_matmul(x: Tensor, z: Tensor, transpose: bool) -> Tensor:
     """
     Helper function for relative positions attention.
     https://arxiv.org/pdf/1803.02155.pdf
     x shape [batch_size x heads x q_len x k_len]
     """
     batch_size = x.size(0)
     heads = x.size(1)
@@ -51,56 +53,55 @@
         z = z.transpose(1, 2)
     x_tz_matmul = torch.matmul(x_t_r, z)
     x_tz_matmul_r = x_tz_matmul.view(length, batch_size, heads, -1)
     x_tz_matmul_r_t = x_tz_matmul_r.permute(1, 2, 0, 3)
     return x_tz_matmul_r_t
 
 
-def gen_relative_positions(length: int,
-                           max_relative_positions: int,
-                           cache: bool = False,
-                           device: Optional[torch.device] = None
-                           ) -> Tensor:
+def gen_relative_positions(
+    length: int,
+    max_relative_positions: int,
+    cache: bool = False,
+    device: Optional[torch.device] = None,
+) -> Tensor:
     """Generate the clipped relative positions matrix
-       for a given length and maximum relative positions"""
+    for a given length and maximum relative positions"""
     if cache:
-        distance_mat = torch.arange(-length+1, 1, 1,
-                                    device=device).unsqueeze(0)
+        distance_mat = torch.arange(-length + 1, 1, 1, device=device).unsqueeze(0)
     else:
         range_vec = torch.arange(length, device=device)
         range_mat = range_vec.unsqueeze(-1).expand(-1, length).transpose(0, 1)
         distance_mat = range_mat - range_mat.transpose(0, 1)
-    distance_mat_clipped = torch.clamp(distance_mat,
-                                       min=-max_relative_positions,
-                                       max=max_relative_positions)
+    distance_mat_clipped = torch.clamp(
+        distance_mat, min=-max_relative_positions, max=max_relative_positions
+    )
     # Shift values to be >= 0
     final_mat = distance_mat_clipped + max_relative_positions
     return final_mat
 
 
 # Help functions to split model dim per head
 
+
 def shape(x: Tensor, dim_per_head: int) -> Tensor:
     """
     Projection.
     [batchsize x length x modeldim]
     -> [batchsize x heads x length x dimperhead]
     """
-    return x.view(x.size(0), x.size(1), -1, dim_per_head) \
-        .transpose(1, 2)
+    return x.view(x.size(0), x.size(1), -1, dim_per_head).transpose(1, 2)
 
 
 def unshape(x: Tensor) -> Tensor:
     """
     Compute context.
     [batchsize x heads x length x dimperhead]
     -> [batchsize x length x modeldim]
     """
-    return x.transpose(1, 2).contiguous() \
-        .view(x.size(0), -1, x.size(1) * x.size(3))
+    return x.transpose(1, 2).contiguous().view(x.size(0), -1, x.size(1) * x.size(3))
 
 
 class MultiHeadedAttention(nn.Module):
     # class MultiHeadedAttention(torch.jit.ScriptModule):
     """Multi-Head Attention module from "Attention is All You Need"
     :cite:`DBLP:journals/corr/VaswaniSPUJGKP17`.
 
@@ -138,57 +139,72 @@
        model_dim (int): the dimension of keys/values/queries,
            must be divisible by head_count
        dropout (float): dropout parameter
        max_relative_positions (int): max relative positions
        attn_type: "self" or "context"
     """
 
-    def __init__(self, head_count: int, model_dim: int, dropout: float = 0.1,
-                 max_relative_positions: int = 0,
-                 attn_type: str = None, add_qkvbias=False) -> None:
-
+    def __init__(
+        self,
+        head_count: int,
+        model_dim: int,
+        dropout: float = 0.1,
+        max_relative_positions: int = 0,
+        attn_type: str = None,
+        add_qkvbias=False,
+    ) -> None:
         assert model_dim % head_count == 0
         self.dim_per_head = model_dim // head_count
         super(MultiHeadedAttention, self).__init__()
         self.head_count = head_count
 
         self.linear_keys = nn.Linear(model_dim, model_dim, bias=add_qkvbias)
         self.linear_values = nn.Linear(model_dim, model_dim, bias=add_qkvbias)
         self.linear_query = nn.Linear(model_dim, model_dim, bias=add_qkvbias)
         self.softmax = nn.Softmax(dim=-1)
         self.dropout = nn.Dropout(dropout)
         self.final_linear = nn.Linear(model_dim, model_dim, bias=add_qkvbias)
 
         self.max_relative_positions = max_relative_positions
         self.attn_type = attn_type
-        self.layer_cache = (False, {'keys': torch.tensor([]),
-                                    'values': torch.tensor([])})
+        self.layer_cache = (
+            False,
+            {"keys": torch.tensor([]), "values": torch.tensor([])},
+        )
         if max_relative_positions > 0:
             # https://arxiv.org/pdf/1803.02155.pdf
             # in the paper they suggest either two embeds
             # relative_key / relative_value or only
             # relative_key. We implemented the same embed
             # for both.
             vocab_size = max_relative_positions * 2 + 1
             self.relative_positions_embeddings = nn.Embedding(
-                vocab_size, self.dim_per_head)
+                vocab_size, self.dim_per_head
+            )
         else:
             self.relative_positions_embeddings = None
 
             if max_relative_positions == -1:  # rotary embeddings
                 self.rope = rotaryembeddings(self.dim_per_head)
 
+            if max_relative_positions == -2:  # alibi positional bias
+                self.alibi = AlibiPositionalBias(head_count)
+
     def update_dropout(self, dropout: float) -> None:
         self.dropout.p = dropout
 
     # @torch.jit.script_method
-    def forward(self, key: Tensor, value: Tensor,
-                query: Tensor, mask: Optional[Tensor] = None,
-                step: Optional[int] = 0
-                ) -> Tuple[Tensor, Tensor]:
+    def forward(
+        self,
+        key: Tensor,
+        value: Tensor,
+        query: Tensor,
+        mask: Optional[Tensor] = None,
+        step: Optional[int] = 0,
+    ) -> Tuple[Tensor, Tensor]:
         """
         Compute the context vector and the attention vectors.
 
         Args:
            key (Tensor): set of `key_len`
                key vectors ``(batch, key_len, dim)``
            value (Tensor): set of `key_len`
@@ -204,98 +220,94 @@
            * output context vectors ``(batch, query_len, dim)``
            * Attention vector in heads ``(batch, head, query_len, key_len)``.
         """
         # 1) Project key, value, and query.
         # as a reminder at training layer_cache[0] remains False
         if self.layer_cache[0]:
             if self.attn_type == "self":
-                query, key, value = self.linear_query(query),\
-                                    self.linear_keys(query),\
-                                    self.linear_values(query)
+                query, key, value = (
+                    self.linear_query(query),
+                    self.linear_keys(query),
+                    self.linear_values(query),
+                )
                 query = shape(query, self.dim_per_head)
                 key = shape(key, self.dim_per_head)
                 value = shape(value, self.dim_per_head)
 
                 if self.max_relative_positions == -1:  # Rotary Embeddings
                     start_pos = step
                     seqlen = query.size(2)
-                    rope = self.rope[start_pos:
-                                     start_pos +
-                                     seqlen].to(query.device)
+                    rope = self.rope[start_pos : start_pos + seqlen].to(query.device)
 
                     query = query.transpose(1, 2)
                     key = key.transpose(1, 2)
-                    query, key = apply_rotary_emb(query,
-                                                  key,
-                                                  rope=rope)
+                    query, key = apply_rotary_emb(query, key, rope=rope)
                     query = query.transpose(1, 2)
                     key = key.transpose(1, 2)
 
-                if self.layer_cache[1]['keys'].numel() != 0:
-                    key = torch.cat(
-                        (self.layer_cache[1]['keys'], key),
-                        dim=2)
-
-                if self.layer_cache[1]['values'].numel() != 0:
-                    value = torch.cat(
-                        (self.layer_cache[1]['values'], value),
-                        dim=2)
-                self.layer_cache[1]['keys'] = key
-                self.layer_cache[1]['values'] = value
+                if self.layer_cache[1]["keys"].numel() != 0:
+                    key = torch.cat((self.layer_cache[1]["keys"], key), dim=2)
+
+                if self.layer_cache[1]["values"].numel() != 0:
+                    value = torch.cat((self.layer_cache[1]["values"], value), dim=2)
+                self.layer_cache[1]["keys"] = key
+                self.layer_cache[1]["values"] = value
             elif self.attn_type == "context":
                 query = self.linear_query(query)
                 query = shape(query, self.dim_per_head)
-                if self.layer_cache[1]['keys'].numel() == 0:
-                    key, value = self.linear_keys(key),\
-                                 self.linear_values(value)
+                if self.layer_cache[1]["keys"].numel() == 0:
+                    key, value = self.linear_keys(key), self.linear_values(value)
                     key = shape(key, self.dim_per_head)
                     value = shape(value, self.dim_per_head)
                 else:
-                    key, value = self.layer_cache[1]['keys'],\
-                               self.layer_cache[1]['values']
-                self.layer_cache[1]['keys'] = key
-                self.layer_cache[1]['values'] = value
+                    key, value = (
+                        self.layer_cache[1]["keys"],
+                        self.layer_cache[1]["values"],
+                    )
+                self.layer_cache[1]["keys"] = key
+                self.layer_cache[1]["values"] = value
         else:
             key = self.linear_keys(key)
             value = self.linear_values(value)
             query = self.linear_query(query)
             key = shape(key, self.dim_per_head)
             value = shape(value, self.dim_per_head)
             query = shape(query, self.dim_per_head)
 
             if self.max_relative_positions == -1:  # Rotary Embeddings
                 start_pos = 0
                 seqlen = query.size(2)
-                rope = self.rope[start_pos:
-                                 start_pos +
-                                 seqlen].to(query.device)
+                rope = self.rope[start_pos : start_pos + seqlen].to(query.device)
 
                 query = query.transpose(1, 2)
                 key = key.transpose(1, 2)
-                query, key = apply_rotary_emb(query,
-                                              key,
-                                              rope=rope)
+                query, key = apply_rotary_emb(query, key, rope=rope)
                 query = query.transpose(1, 2)
                 key = key.transpose(1, 2)
         # 2) Calculate and scale scores.
         query = query / math.sqrt(self.dim_per_head)
         # batch x num_heads x query_len x key_len
         query_key = torch.matmul(query, key.transpose(2, 3))
 
         if self.relative_positions_embeddings is not None:
             key_len = key.size(2)
             # 1 or key_len x key_len
             relative_positions_matrix = gen_relative_positions(
-                key_len, self.max_relative_positions,
+                key_len,
+                self.max_relative_positions,
                 cache=self.layer_cache[0],
-                device=key.device)
+                device=key.device,
+            )
             #  1 or key_len x key_len x dim_per_head
             relations_keys = self.relative_positions_embeddings(
-                relative_positions_matrix)
+                relative_positions_matrix
+            )
             scores = query_key + relative_matmul(query, relations_keys, True)
+        elif self.max_relative_positions == -2:
+            scores = self.alibi(query_key)
         else:
             scores = query_key
 
         scores = scores.float()
 
         if mask is not None:
             # not 100% necessary but expand to nb of heads
@@ -308,17 +320,16 @@
         drop_attn = self.dropout(attn)
 
         context_original = torch.matmul(drop_attn, value)
 
         if self.relative_positions_embeddings is not None:
             # We use the same embeddings for key and value
             relations_values = relations_keys
-            context = unshape(context_original
-                              + relative_matmul(drop_attn,
-                                                relations_values,
-                                                False))
+            context = unshape(
+                context_original + relative_matmul(drop_attn, relations_values, False)
+            )
         else:
             context = unshape(context_original)
 
         output = self.final_linear(context)
 
         return output, attn
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/position_ffn.py` & `OpenNMT-py-3.1.3/onmt/modules/position_ffn.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,60 +17,65 @@
     ActivationFunction.relu: F.relu,
     ActivationFunction.gelu: F.gelu,
     ActivationFunction.silu: F.silu,
 }
 
 
 class PositionwiseFeedForward(nn.Module):
-    """ A two-layer Feed-Forward-Network with residual layer norm.
+    """A two-layer Feed-Forward-Network with residual layer norm.
 
     Args:
         d_model (int): the size of input for the first-layer of the FFN.
         d_ff (int): the hidden layer size of the second-layer
             of the FNN.
         dropout (float): dropout probability in :math:`[0, 1)`.
         activation_fn (ActivationFunction): activation function used.
         layer_norm (string): 'standard' or 'rms'
     """
 
-    def __init__(self, d_model, d_ff, dropout=0.1,
-                 activation_fn=ActivationFunction.relu,
-                 layer_norm='standard'):
+    def __init__(
+        self,
+        d_model,
+        d_ff,
+        dropout=0.1,
+        activation_fn=ActivationFunction.relu,
+        layer_norm="standard",
+    ):
         super(PositionwiseFeedForward, self).__init__()
         self.w_1 = nn.Linear(d_model, d_ff)
         self.w_2 = nn.Linear(d_ff, d_model)
-        if layer_norm == 'standard':
+        if layer_norm == "standard":
             self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
-        elif layer_norm == 'rms':
+        elif layer_norm == "rms":
             self.layer_norm = RMSNorm(d_model, eps=1e-6)
         else:
-            raise ValueError(f'{layer_norm} layer norm type is not supported')
+            raise ValueError(f"{layer_norm} layer norm type is not supported")
         self.dropout_1 = nn.Dropout(dropout)
         self.activation = ACTIVATION_FUNCTIONS[activation_fn]
         self.dropout_2 = nn.Dropout(dropout)
-        if activation_fn == 'silu':
+        if activation_fn == "silu":
             self.w_3 = nn.Linear(d_model, d_ff)
         else:
             self.w_3 = None
 
     def forward(self, x):
         """Layer definition.
 
         Args:
             x: ``(batch_size, input_len, model_dim)``
 
         Returns:
             (FloatTensor): Output ``(batch_size, input_len, model_dim)``.
         """
         if self.w_3 is None:
-            inter = self.dropout_1(self.activation(
-                self.w_1(self.layer_norm(x))))
+            inter = self.dropout_1(self.activation(self.w_1(self.layer_norm(x))))
         else:
             inter = self.dropout_1(
                 self.activation(self.w_1(self.layer_norm(x)))
-                * self.w_3(self.layer_norm(x)))
+                * self.w_3(self.layer_norm(x))
+            )
         output = self.dropout_2(self.w_2(inter))
         return output + x
 
     def update_dropout(self, dropout):
         self.dropout_1.p = dropout
         self.dropout_2.p = dropout
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/rmsnorm.py` & `OpenNMT-py-3.1.3/onmt/modules/rmsnorm.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 
 class RMSNorm(torch.nn.Module):
     """RMSNorm: https://arxiv.org/abs/1910.07467
     Args:
         hidden_size (int): layer hidden_sizeension.
     """
+
     def __init__(self, hidden_size: int, eps: float = 1e-6):
         super().__init__()
         self.eps = eps
         self.weight = nn.Parameter(torch.ones(hidden_size))
 
     def forward(self, hidden_states):
-        variance = hidden_states.to(torch.float32).pow(2).mean(-1,
-                                                               keepdim=True)
+        variance = hidden_states.to(torch.float32).pow(2).mean(-1, keepdim=True)
         hidden_states = hidden_states * torch.rsqrt(variance + self.eps)
         hidden_states = hidden_states.to(self.weight.dtype)
         return hidden_states * self.weight
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/sparse_activations.py` & `OpenNMT-py-3.1.3/onmt/modules/sparse_activations.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     support_size = support.sum(dim=dim).unsqueeze(dim)
     tau = input_cumsum.gather(dim, support_size - 1)
     tau /= support_size.to(input.dtype)
     return tau, support_size
 
 
 class SparsemaxFunction(Function):
-
     @staticmethod
     @custom_fwd
     def forward(ctx, input, dim=0):
         """sparsemax: normalizing sparse transform (a la softmax)
 
         Parameters:
             input (Tensor): any shape
@@ -77,24 +76,22 @@
         return grad_input, None
 
 
 sparsemax = SparsemaxFunction.apply
 
 
 class Sparsemax(nn.Module):
-
     def __init__(self, dim=0):
         self.dim = dim
         super(Sparsemax, self).__init__()
 
     def forward(self, input):
         return sparsemax(input, self.dim)
 
 
 class LogSparsemax(nn.Module):
-
     def __init__(self, dim=0):
         self.dim = dim
         super(LogSparsemax, self).__init__()
 
     def forward(self, input):
         return torch.log(sparsemax(input, self.dim))
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/sparse_losses.py` & `OpenNMT-py-3.1.3/onmt/modules/sparse_losses.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 import torch.nn as nn
 from torch.autograd import Function
 from torch.cuda.amp import custom_fwd, custom_bwd
 from onmt.modules.sparse_activations import _threshold_and_support
 
 
 class SparsemaxLossFunction(Function):
-
     @staticmethod
     @custom_fwd
     def forward(ctx, input, target):
         """
         input (FloatTensor): ``(n, num_classes)``.
         target (LongTensor): ``(n,)``, the indices of the target classes
         """
         input_batch, classes = input.size()
 
         z_k = input.gather(1, target.unsqueeze(1)).squeeze()
         tau_z, support_size = _threshold_and_support(input, dim=1)
         support = input > tau_z
         x = torch.where(
-            support, input**2 - tau_z**2,
-            torch.tensor(0.0, device=input.device)
+            support, input**2 - tau_z**2, torch.tensor(0.0, device=input.device)
         ).sum(dim=1)
         ctx.save_for_backward(input, target, tau_z)
         # clamping necessary because of numerical errors: loss should be lower
         # bounded by zero, but negative values near zero are possible without
         # the clamp
         return torch.clamp(x / 2 - z_k + 0.5, min=0.0)
 
@@ -49,28 +47,27 @@
     a sparse output layer, it is not possible to use negative log likelihood
     because the loss is infinite in the case the target is assigned zero
     probability. Inputs to SparsemaxLoss are arbitrary dense real-valued
     vectors (like in nn.CrossEntropyLoss), not probability vectors (like in
     nn.NLLLoss).
     """
 
-    def __init__(self, weight=None, ignore_index=-100,
-                 reduction='elementwise_mean'):
-        assert reduction in ['elementwise_mean', 'sum', 'none']
+    def __init__(self, weight=None, ignore_index=-100, reduction="elementwise_mean"):
+        assert reduction in ["elementwise_mean", "sum", "none"]
         self.reduction = reduction
         self.weight = weight
         self.ignore_index = ignore_index
         super(SparsemaxLoss, self).__init__()
 
     def forward(self, input, target):
         loss = sparsemax_loss(input, target)
         if self.ignore_index >= 0:
             ignored_positions = target == self.ignore_index
             size = float((target.size(0) - ignored_positions.sum()).item())
             loss.masked_fill_(ignored_positions, 0.0)
         else:
             size = float(target.size(0))
-        if self.reduction == 'sum':
+        if self.reduction == "sum":
             loss = loss.sum()
-        elif self.reduction == 'elementwise_mean':
+        elif self.reduction == "elementwise_mean":
             loss = loss.sum() / size
         return loss
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/sru.py` & `OpenNMT-py-3.1.3/onmt/modules/sru.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # For command-line option parsing
 class CheckSRU(configargparse.Action):
     def __init__(self, option_strings, dest, **kwargs):
         super(CheckSRU, self).__init__(option_strings, dest, **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
-        if values == 'SRU':
+        if values == "SRU":
             check_sru_requirement(abort=True)
         # Check pass, set the args.
         setattr(namespace, self.dest, values)
 
 
 # This SRU version implements its own cuda-level optimization,
 # so it requires that:
@@ -34,42 +34,43 @@
     """
     Return True if check pass; if check fails and abort is True,
     raise an Exception, othereise return False.
     """
 
     # Check 1.
     try:
-        if platform.system() == 'Windows':
-            subprocess.check_output('pip freeze | findstr cupy', shell=True)
-            subprocess.check_output('pip freeze | findstr pynvrtc',
-                                    shell=True)
+        if platform.system() == "Windows":
+            subprocess.check_output("pip freeze | findstr cupy", shell=True)
+            subprocess.check_output("pip freeze | findstr pynvrtc", shell=True)
         else:  # Unix-like systems
-            subprocess.check_output('pip freeze | grep -w cupy', shell=True)
-            subprocess.check_output('pip freeze | grep -w pynvrtc',
-                                    shell=True)
+            subprocess.check_output("pip freeze | grep -w cupy", shell=True)
+            subprocess.check_output("pip freeze | grep -w pynvrtc", shell=True)
     except subprocess.CalledProcessError:
         if not abort:
             return False
-        raise AssertionError("Using SRU requires 'cupy' and 'pynvrtc' "
-                             "python packages installed.")
+        raise AssertionError(
+            "Using SRU requires 'cupy' and 'pynvrtc' " "python packages installed."
+        )
 
     # Check 2.
     if torch.cuda.is_available() is False:
         if not abort:
             return False
         raise AssertionError("Using SRU requires pytorch built with cuda.")
 
     # Check 3.
     pattern = re.compile(".*cuda/lib.*")
-    ld_path = os.getenv('LD_LIBRARY_PATH', "")
+    ld_path = os.getenv("LD_LIBRARY_PATH", "")
     if re.match(pattern, ld_path) is None:
         if not abort:
             return False
-        raise AssertionError("Using SRU requires setting cuda lib path, e.g. "
-                             "export LD_LIBRARY_PATH=/usr/local/cuda/lib64.")
+        raise AssertionError(
+            "Using SRU requires setting cuda lib path, e.g. "
+            "export LD_LIBRARY_PATH=/usr/local/cuda/lib64."
+        )
 
     return True
 
 
 SRU_CODE = """
 extern "C" {
     __forceinline__ __device__ float sigmoidf(float x)
@@ -358,31 +359,29 @@
         from cupy.cuda import function
         from pynvrtc.compiler import Program
 
         # This sets up device to use.
         device = torch.device("cuda")
         tmp_ = torch.rand(1, 1).to(device)
 
-        sru_prog = Program(SRU_CODE.encode('utf-8'),
-                           'sru_prog.cu'.encode('utf-8'))
+        sru_prog = Program(SRU_CODE.encode("utf-8"), "sru_prog.cu".encode("utf-8"))
         sru_ptx = sru_prog.compile()
         sru_mod = function.Module()
         sru_mod.load(bytes(sru_ptx.encode()))
 
-        SRU_FWD_FUNC = sru_mod.get_function('sru_fwd')
-        SRU_BWD_FUNC = sru_mod.get_function('sru_bwd')
-        SRU_BiFWD_FUNC = sru_mod.get_function('sru_bi_fwd')
-        SRU_BiBWD_FUNC = sru_mod.get_function('sru_bi_bwd')
+        SRU_FWD_FUNC = sru_mod.get_function("sru_fwd")
+        SRU_BWD_FUNC = sru_mod.get_function("sru_bwd")
+        SRU_BiFWD_FUNC = sru_mod.get_function("sru_bi_fwd")
+        SRU_BiBWD_FUNC = sru_mod.get_function("sru_bi_bwd")
 
-        stream = namedtuple('Stream', ['ptr'])
+        stream = namedtuple("Stream", ["ptr"])
         SRU_STREAM = stream(ptr=torch.cuda.current_stream().cuda_stream)
 
 
 class SRU_Compute(Function):
-
     def __init__(self, activation_type, d_out, bidirectional=False):
         SRU_Compute.maybe_load_sru_mod()
         super(SRU_Compute, self).__init__()
         self.activation_type = activation_type
         self.d_out = d_out
         self.bidirectional = bidirectional
 
@@ -407,29 +406,32 @@
 
         init_ = x.new(ncols).zero_() if init is None else init
         size = (length, batch, d * bidir) if x.dim() == 3 else (batch, d * bidir)
         c = x.new(*size)
         h = x.new(*size)
 
         FUNC = SRU_FWD_FUNC if not self.bidirectional else SRU_BiFWD_FUNC
-        FUNC(args=[
-            u.contiguous().data_ptr(),
-            x.contiguous().data_ptr() if k_ == 3 else 0,
-            bias.data_ptr(),
-            init_.contiguous().data_ptr(),
-            mask_h.data_ptr() if mask_h is not None else 0,
-            length,
-            batch,
-            d,
-            k_,
-            h.data_ptr(),
-            c.data_ptr(),
-            self.activation_type],
-            block=(thread_per_block, 1, 1), grid=(num_block, 1, 1),
-            stream=SRU_STREAM
+        FUNC(
+            args=[
+                u.contiguous().data_ptr(),
+                x.contiguous().data_ptr() if k_ == 3 else 0,
+                bias.data_ptr(),
+                init_.contiguous().data_ptr(),
+                mask_h.data_ptr() if mask_h is not None else 0,
+                length,
+                batch,
+                d,
+                k_,
+                h.data_ptr(),
+                c.data_ptr(),
+                self.activation_type,
+            ],
+            block=(thread_per_block, 1, 1),
+            grid=(num_block, 1, 1),
+            stream=SRU_STREAM,
         )
 
         self.save_for_backward(u, x, bias, init, mask_h)
         self.intermediate = c
         if x.dim() == 2:
             last_hidden = c
         elif self.bidirectional:
@@ -465,70 +467,82 @@
         #         if x.dim() == 3 else (batch, x.size(-1))
         # grad_x = x.new(*x.size()) if k_ == 3 else x.new(*size).zero_()
 
         # Normal use
         grad_x = x.new(*x.size()) if k_ == 3 else None
 
         FUNC = SRU_BWD_FUNC if not self.bidirectional else SRU_BiBWD_FUNC
-        FUNC(args=[
-            u.contiguous().data_ptr(),
-            x.contiguous().data_ptr() if k_ == 3 else 0,
-            bias.data_ptr(),
-            init_.contiguous().data_ptr(),
-            mask_h.data_ptr() if mask_h is not None else 0,
-            c.data_ptr(),
-            grad_h.contiguous().data_ptr(),
-            grad_last.contiguous().data_ptr(),
-            length,
-            batch,
-            d,
-            k_,
-            grad_u.data_ptr(),
-            grad_x.data_ptr() if k_ == 3 else 0,
-            grad_bias.data_ptr(),
-            grad_init.data_ptr(),
-            self.activation_type],
-            block=(thread_per_block, 1, 1), grid=(num_block, 1, 1),
-            stream=SRU_STREAM
+        FUNC(
+            args=[
+                u.contiguous().data_ptr(),
+                x.contiguous().data_ptr() if k_ == 3 else 0,
+                bias.data_ptr(),
+                init_.contiguous().data_ptr(),
+                mask_h.data_ptr() if mask_h is not None else 0,
+                c.data_ptr(),
+                grad_h.contiguous().data_ptr(),
+                grad_last.contiguous().data_ptr(),
+                length,
+                batch,
+                d,
+                k_,
+                grad_u.data_ptr(),
+                grad_x.data_ptr() if k_ == 3 else 0,
+                grad_bias.data_ptr(),
+                grad_init.data_ptr(),
+                self.activation_type,
+            ],
+            block=(thread_per_block, 1, 1),
+            grid=(num_block, 1, 1),
+            stream=SRU_STREAM,
         )
         return grad_u, grad_x, grad_bias.sum(1).view(-1), grad_init, None
 
 
 class SRUCell(nn.Module):
-    def __init__(self, n_in, n_out, dropout=0, rnn_dropout=0,
-                 bidirectional=False, use_tanh=1, use_relu=0):
+    def __init__(
+        self,
+        n_in,
+        n_out,
+        dropout=0,
+        rnn_dropout=0,
+        bidirectional=False,
+        use_tanh=1,
+        use_relu=0,
+    ):
         super(SRUCell, self).__init__()
         self.n_in = n_in
         self.n_out = n_out
         self.rnn_dropout = rnn_dropout
         self.dropout = dropout
         self.bidirectional = bidirectional
         self.activation_type = 2 if use_relu else (1 if use_tanh else 0)
 
         out_size = n_out * 2 if bidirectional else n_out
         k = 4 if n_in != out_size else 3
         self.size_per_dir = n_out * k
-        self.weight = nn.Parameter(torch.Tensor(
-            n_in,
-            self.size_per_dir * 2 if bidirectional else self.size_per_dir
-        ))
-        self.bias = nn.Parameter(torch.Tensor(
-            n_out * 4 if bidirectional else n_out * 2
-        ))
+        self.weight = nn.Parameter(
+            torch.Tensor(
+                n_in, self.size_per_dir * 2 if bidirectional else self.size_per_dir
+            )
+        )
+        self.bias = nn.Parameter(
+            torch.Tensor(n_out * 4 if bidirectional else n_out * 2)
+        )
         self.init_weight()
 
     def init_weight(self):
-        val_range = (3.0 / self.n_in)**0.5
+        val_range = (3.0 / self.n_in) ** 0.5
         self.weight.data.uniform_(-val_range, val_range)
         self.bias.data.zero_()
 
     def set_bias(self, bias_val=0):
         n_out = self.n_out
         if self.bidirectional:
-            self.bias.data[n_out * 2:].zero_().add_(bias_val)
+            self.bias.data[n_out * 2 :].zero_().add_(bias_val)
         else:
             self.bias.data[n_out:].zero_().add_(bias_val)
 
     def forward(self, input, c0=None):
         assert input.dim() == 2 or input.dim() == 3
         n_in, n_out = self.n_in, self.n_out
         batch = input.size(-2)
@@ -544,24 +558,21 @@
             x = input
 
         x_2d = x if x.dim() == 2 else x.contiguous().view(-1, n_in)
         u = x_2d.mm(self.weight)
 
         if self.training and (self.dropout > 0):
             bidir = 2 if self.bidirectional else 1
-            mask_h = self.get_dropout_mask_(
-                (batch, n_out * bidir), self.dropout)
-            h, c = SRU_Compute(self.activation_type, n_out,
-                               self.bidirectional)(
-                                   u, input, self.bias, c0, mask_h
+            mask_h = self.get_dropout_mask_((batch, n_out * bidir), self.dropout)
+            h, c = SRU_Compute(self.activation_type, n_out, self.bidirectional)(
+                u, input, self.bias, c0, mask_h
             )
         else:
-            h, c = SRU_Compute(self.activation_type, n_out,
-                               self.bidirectional)(
-                                   u, input, self.bias, c0
+            h, c = SRU_Compute(self.activation_type, n_out, self.bidirectional)(
+                u, input, self.bias, c0
             )
 
         return h, c
 
     def get_dropout_mask_(self, size, p):
         w = self.weight.data
         return w.new(*size).bernoulli_(1 - p).div_(1 - p)
@@ -584,17 +595,25 @@
       dropout (float): dropout to use (stacked)
       rnn_dropout (float): dropout to use (recurrent)
       bidirectional (bool): bidirectional
       use_tanh (bool): activation
       use_relu (bool): activation
     """
 
-    def __init__(self, input_size, hidden_size,
-                 num_layers=2, dropout=0, rnn_dropout=0,
-                 bidirectional=False, use_tanh=1, use_relu=0):
+    def __init__(
+        self,
+        input_size,
+        hidden_size,
+        num_layers=2,
+        dropout=0,
+        rnn_dropout=0,
+        bidirectional=False,
+        use_tanh=1,
+        use_relu=0,
+    ):
         # An entry check here, will catch on train side and translate side
         # if requirements are not satisfied.
         check_sru_requirement(abort=True)
         super(SRU, self).__init__()
         self.n_in = input_size
         self.n_out = hidden_size
         self.depth = num_layers
@@ -620,23 +639,21 @@
         for l in self.rnn_lst:
             l.set_bias(bias_val)
 
     def forward(self, input, c0=None, return_hidden=True):
         assert input.dim() == 3  # (len, batch, n_in)
         dir_ = 2 if self.bidirectional else 1
         if c0 is None:
-            zeros = input.data.new(
-                input.size(1), self.n_out * dir_
-            ).zero_()
+            zeros = input.data.new(input.size(1), self.n_out * dir_).zero_()
             c0 = [zeros for i in range(self.depth)]
         else:
             if isinstance(c0, tuple):
                 # RNNDecoderState wraps hidden as a tuple.
                 c0 = c0[0]
-            assert c0.dim() == 3    # (depth, batch, dir_*n_out)
+            assert c0.dim() == 3  # (depth, batch, dir_*n_out)
             c0 = [h.squeeze(0) for h in c0.chunk(self.depth, 0)]
 
         prevx = input
         lstc = []
         for i, rnn in enumerate(self.rnn_lst):
             h, c = rnn(prevx, c0[i])
             prevx = h
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/stacked_rnn.py` & `OpenNMT-py-3.1.3/onmt/modules/stacked_rnn.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.2/onmt/modules/structured_attention.py` & `OpenNMT-py-3.1.3/onmt/modules/structured_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,25 @@
         super(MatrixTree, self).__init__()
 
     def forward(self, input):
         laplacian = input.exp() + self.eps
         output = input.clone()
         for b in range(input.size(0)):
             lap = laplacian[b].masked_fill(
-                torch.eye(input.size(1), device=input.device).ne(0), 0)
+                torch.eye(input.size(1), device=input.device).ne(0), 0
+            )
             lap = -lap + torch.diag(lap.sum(0))
             # store roots on diagonal
             lap[0] = input[b].diag().exp()
             inv_laplacian = lap.inverse()
 
-            factor = inv_laplacian.diag().unsqueeze(1)\
-                                         .expand_as(input[b]).transpose(0, 1)
+            factor = (
+                inv_laplacian.diag().unsqueeze(1).expand_as(input[b]).transpose(0, 1)
+            )
             term1 = input[b].exp().mul(factor).clone()
             term2 = input[b].exp().mul(inv_laplacian.transpose(0, 1)).clone()
             term1[:, 0] = 0
             term2[0] = 0
             output[b] = term1 - term2
-            roots_output = input[b].diag().exp().mul(
-                inv_laplacian.transpose(0, 1)[0])
+            roots_output = input[b].diag().exp().mul(inv_laplacian.transpose(0, 1)[0])
             output[b] = output[b] + torch.diag(roots_output)
         return output
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/util_class.py` & `OpenNMT-py-3.1.3/onmt/modules/util_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,27 +12,27 @@
     as the list.
     emb_out is the result of applying modules to emb elementwise.
     An optional merge parameter allows the emb_out to be reduced to a
     single Tensor.
     """
 
     def __init__(self, merge=None, *args):
-        assert merge in [None, 'first', 'concat', 'sum', 'mlp']
+        assert merge in [None, "first", "concat", "sum", "mlp"]
         self.merge = merge
         super(Elementwise, self).__init__(*args)
 
     def forward(self, emb):
         emb_ = [feat.squeeze(2) for feat in emb.split(1, dim=2)]
         assert len(self) == len(emb_)
         emb_out = [f(x) for f, x in zip(self, emb_)]
-        if self.merge == 'first':
+        if self.merge == "first":
             return emb_out[0]
-        elif self.merge == 'concat' or self.merge == 'mlp':
+        elif self.merge == "concat" or self.merge == "mlp":
             return torch.cat(emb_out, 2)
-        elif self.merge == 'sum':
+        elif self.merge == "sum":
             return sum(emb_out)
         else:
             return emb_out
 
 
 class Cast(nn.Module):
     """
```

### Comparing `OpenNMT-py-3.1.2/onmt/modules/weight_norm.py` & `OpenNMT-py-3.1.3/onmt/modules/weight_norm.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,33 +2,32 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn import Parameter
 
 
 def get_var_maybe_avg(namespace, var_name, training, polyak_decay):
-    """ utility for retrieving polyak averaged params
-        Update average
+    """utility for retrieving polyak averaged params
+    Update average
     """
     v = getattr(namespace, var_name)
-    v_avg = getattr(namespace, var_name + '_avg')
+    v_avg = getattr(namespace, var_name + "_avg")
     v_avg -= (1 - polyak_decay) * (v_avg - v.data)
 
     if training:
         return v
     else:
         return v_avg
 
 
 def get_vars_maybe_avg(namespace, var_names, training, polyak_decay):
-    """ utility for retrieving polyak averaged params """
+    """utility for retrieving polyak averaged params"""
     vars = []
     for vn in var_names:
-        vars.append(get_var_maybe_avg(
-            namespace, vn, training, polyak_decay))
+        vars.append(get_var_maybe_avg(namespace, vn, training, polyak_decay))
     return vars
 
 
 class WeightNormLinear(nn.Linear):
     """
     Implementation of "Weight Normalization: A Simple Reparameterization
     to Accelerate Training of Deep Neural Networks"
@@ -37,210 +36,249 @@
     As a reparameterization method, weight normalization is same
     as BatchNormalization, but it doesn't depend on minibatch.
 
     NOTE: This is used nowhere in the code at this stage
           Vincent Nguyen 05/18/2018
     """
 
-    def __init__(self, in_features, out_features,
-                 init_scale=1., polyak_decay=0.9995):
-        super(WeightNormLinear, self).__init__(
-            in_features, out_features, bias=True)
+    def __init__(self, in_features, out_features, init_scale=1.0, polyak_decay=0.9995):
+        super(WeightNormLinear, self).__init__(in_features, out_features, bias=True)
 
         self.V = self.weight
         self.g = Parameter(torch.Tensor(out_features))
         self.b = self.bias
 
-        self.register_buffer(
-            'V_avg', torch.zeros(out_features, in_features))
-        self.register_buffer('g_avg', torch.zeros(out_features))
-        self.register_buffer('b_avg', torch.zeros(out_features))
+        self.register_buffer("V_avg", torch.zeros(out_features, in_features))
+        self.register_buffer("g_avg", torch.zeros(out_features))
+        self.register_buffer("b_avg", torch.zeros(out_features))
 
         self.init_scale = init_scale
         self.polyak_decay = polyak_decay
         self.reset_parameters()
 
     def reset_parameters(self):
         return
 
     def forward(self, x, init=False):
         if init is True:
             # out_features * in_features
-            self.V.data.copy_(torch.randn(self.V.data.size()).type_as(
-                self.V.data) * 0.05)
+            self.V.data.copy_(
+                torch.randn(self.V.data.size()).type_as(self.V.data) * 0.05
+            )
             # norm is out_features * 1
-            v_norm = self.V.data / \
-                self.V.data.norm(2, 1).expand_as(self.V.data)
+            v_norm = self.V.data / self.V.data.norm(2, 1).expand_as(self.V.data)
             # batch_size * out_features
             x_init = F.linear(x, v_norm).data
             # out_features
-            m_init, v_init = x_init.mean(0).squeeze(
-                0), x_init.var(0).squeeze(0)
+            m_init, v_init = x_init.mean(0).squeeze(0), x_init.var(0).squeeze(0)
             # out_features
-            scale_init = self.init_scale / \
-                torch.sqrt(v_init + 1e-10)
+            scale_init = self.init_scale / torch.sqrt(v_init + 1e-10)
             self.g.data.copy_(scale_init)
             self.b.data.copy_(-m_init * scale_init)
-            x_init = scale_init.view(1, -1).expand_as(x_init) \
-                * (x_init - m_init.view(1, -1).expand_as(x_init))
+            x_init = scale_init.view(1, -1).expand_as(x_init) * (
+                x_init - m_init.view(1, -1).expand_as(x_init)
+            )
             self.V_avg.copy_(self.V.data)
             self.g_avg.copy_(self.g.data)
             self.b_avg.copy_(self.b.data)
             return x_init
         else:
-            v, g, b = get_vars_maybe_avg(self, ['V', 'g', 'b'],
-                                         self.training,
-                                         polyak_decay=self.polyak_decay)
+            v, g, b = get_vars_maybe_avg(
+                self, ["V", "g", "b"], self.training, polyak_decay=self.polyak_decay
+            )
             # batch_size * out_features
             x = F.linear(x, v)
             scalar = g / torch.norm(v, 2, 1).squeeze(1)
-            x = scalar.view(1, -1).expand_as(x) * x + \
-                b.view(1, -1).expand_as(x)
+            x = scalar.view(1, -1).expand_as(x) * x + b.view(1, -1).expand_as(x)
             return x
 
 
 class WeightNormConv2d(nn.Conv2d):
-    def __init__(self, in_channels, out_channels, kernel_size, stride=1,
-                 padding=0, dilation=1, groups=1, init_scale=1.,
-                 polyak_decay=0.9995):
-        super(WeightNormConv2d, self).__init__(in_channels, out_channels,
-                                               kernel_size, stride, padding,
-                                               dilation, groups)
+    def __init__(
+        self,
+        in_channels,
+        out_channels,
+        kernel_size,
+        stride=1,
+        padding=0,
+        dilation=1,
+        groups=1,
+        init_scale=1.0,
+        polyak_decay=0.9995,
+    ):
+        super(WeightNormConv2d, self).__init__(
+            in_channels, out_channels, kernel_size, stride, padding, dilation, groups
+        )
 
         self.V = self.weight
         self.g = Parameter(torch.Tensor(out_channels))
         self.b = self.bias
 
-        self.register_buffer('V_avg', torch.zeros(self.V.size()))
-        self.register_buffer('g_avg', torch.zeros(out_channels))
-        self.register_buffer('b_avg', torch.zeros(out_channels))
+        self.register_buffer("V_avg", torch.zeros(self.V.size()))
+        self.register_buffer("g_avg", torch.zeros(out_channels))
+        self.register_buffer("b_avg", torch.zeros(out_channels))
 
         self.init_scale = init_scale
         self.polyak_decay = polyak_decay
         self.reset_parameters()
 
     def reset_parameters(self):
         return
 
     def forward(self, x, init=False):
         if init is True:
             # out_channels, in_channels // groups, * kernel_size
-            self.V.data.copy_(torch.randn(self.V.data.size()
-                                          ).type_as(self.V.data) * 0.05)
-            v_norm = self.V.data / self.V.data.view(self.out_channels, -1)\
-                .norm(2, 1).view(self.out_channels, *(
-                    [1] * (len(self.kernel_size) + 1))).expand_as(self.V.data)
-            x_init = F.conv2d(x, v_norm, None, self.stride,
-                              self.padding, self.dilation, self.groups).data
-            t_x_init = x_init.transpose(0, 1).contiguous().view(
-                self.out_channels, -1)
-            m_init, v_init = t_x_init.mean(1).squeeze(
-                1), t_x_init.var(1).squeeze(1)
+            self.V.data.copy_(
+                torch.randn(self.V.data.size()).type_as(self.V.data) * 0.05
+            )
+            v_norm = self.V.data / self.V.data.view(self.out_channels, -1).norm(
+                2, 1
+            ).view(self.out_channels, *([1] * (len(self.kernel_size) + 1))).expand_as(
+                self.V.data
+            )
+            x_init = F.conv2d(
+                x, v_norm, None, self.stride, self.padding, self.dilation, self.groups
+            ).data
+            t_x_init = x_init.transpose(0, 1).contiguous().view(self.out_channels, -1)
+            m_init, v_init = t_x_init.mean(1).squeeze(1), t_x_init.var(1).squeeze(1)
             # out_features
-            scale_init = self.init_scale / \
-                torch.sqrt(v_init + 1e-10)
+            scale_init = self.init_scale / torch.sqrt(v_init + 1e-10)
             self.g.data.copy_(scale_init)
             self.b.data.copy_(-m_init * scale_init)
             scale_init_shape = scale_init.view(
-                1, self.out_channels, *([1] * (len(x_init.size()) - 2)))
+                1, self.out_channels, *([1] * (len(x_init.size()) - 2))
+            )
             m_init_shape = m_init.view(
-                1, self.out_channels, *([1] * (len(x_init.size()) - 2)))
-            x_init = scale_init_shape.expand_as(
-                x_init) * (x_init - m_init_shape.expand_as(x_init))
+                1, self.out_channels, *([1] * (len(x_init.size()) - 2))
+            )
+            x_init = scale_init_shape.expand_as(x_init) * (
+                x_init - m_init_shape.expand_as(x_init)
+            )
             self.V_avg.copy_(self.V.data)
             self.g_avg.copy_(self.g.data)
             self.b_avg.copy_(self.b.data)
             return x_init
         else:
             v, g, b = get_vars_maybe_avg(
-                self, ['V', 'g', 'b'], self.training,
-                polyak_decay=self.polyak_decay)
+                self, ["V", "g", "b"], self.training, polyak_decay=self.polyak_decay
+            )
 
             scalar = torch.norm(v.view(self.out_channels, -1), 2, 1)
             if len(scalar.size()) == 2:
                 scalar = g / scalar.squeeze(1)
             else:
                 scalar = g / scalar
 
-            w = scalar.view(self.out_channels, *
-                            ([1] * (len(v.size()) - 1))).expand_as(v) * v
+            w = (
+                scalar.view(self.out_channels, *([1] * (len(v.size()) - 1))).expand_as(
+                    v
+                )
+                * v
+            )
 
-            x = F.conv2d(x, w, b, self.stride,
-                         self.padding, self.dilation, self.groups)
+            x = F.conv2d(x, w, b, self.stride, self.padding, self.dilation, self.groups)
             return x
 
+
 # This is used nowhere in the code at the moment (Vincent Nguyen 05/18/2018)
 
 
 class WeightNormConvTranspose2d(nn.ConvTranspose2d):
-    def __init__(self, in_channels, out_channels, kernel_size, stride=1,
-                 padding=0, output_padding=0, groups=1, init_scale=1.,
-                 polyak_decay=0.9995):
+    def __init__(
+        self,
+        in_channels,
+        out_channels,
+        kernel_size,
+        stride=1,
+        padding=0,
+        output_padding=0,
+        groups=1,
+        init_scale=1.0,
+        polyak_decay=0.9995,
+    ):
         super(WeightNormConvTranspose2d, self).__init__(
-            in_channels, out_channels,
-            kernel_size, stride,
-            padding, output_padding,
-            groups)
+            in_channels,
+            out_channels,
+            kernel_size,
+            stride,
+            padding,
+            output_padding,
+            groups,
+        )
         # in_channels, out_channels, *kernel_size
         self.V = self.weight
         self.g = Parameter(torch.Tensor(out_channels))
         self.b = self.bias
 
-        self.register_buffer('V_avg', torch.zeros(self.V.size()))
-        self.register_buffer('g_avg', torch.zeros(out_channels))
-        self.register_buffer('b_avg', torch.zeros(out_channels))
+        self.register_buffer("V_avg", torch.zeros(self.V.size()))
+        self.register_buffer("g_avg", torch.zeros(out_channels))
+        self.register_buffer("b_avg", torch.zeros(out_channels))
 
         self.init_scale = init_scale
         self.polyak_decay = polyak_decay
         self.reset_parameters()
 
     def reset_parameters(self):
         return
 
     def forward(self, x, init=False):
         if init is True:
             # in_channels, out_channels, *kernel_size
-            self.V.data.copy_(torch.randn(self.V.data.size()).type_as(
-                self.V.data) * 0.05)
-            v_norm = self.V.data / self.V.data.transpose(0, 1).contiguous() \
-                .view(self.out_channels, -1).norm(2, 1).view(
-                    self.in_channels, self.out_channels,
-                    *([1] * len(self.kernel_size))).expand_as(self.V.data)
+            self.V.data.copy_(
+                torch.randn(self.V.data.size()).type_as(self.V.data) * 0.05
+            )
+            v_norm = self.V.data / self.V.data.transpose(0, 1).contiguous().view(
+                self.out_channels, -1
+            ).norm(2, 1).view(
+                self.in_channels, self.out_channels, *([1] * len(self.kernel_size))
+            ).expand_as(
+                self.V.data
+            )
             x_init = F.conv_transpose2d(
-                x, v_norm, None, self.stride,
-                self.padding, self.output_padding, self.groups).data
+                x,
+                v_norm,
+                None,
+                self.stride,
+                self.padding,
+                self.output_padding,
+                self.groups,
+            ).data
             # self.out_channels, 1
-            t_x_init = x_init.tranpose(0, 1).contiguous().view(
-                self.out_channels, -1)
+            t_x_init = x_init.tranpose(0, 1).contiguous().view(self.out_channels, -1)
             # out_features
-            m_init, v_init = t_x_init.mean(1).squeeze(
-                1), t_x_init.var(1).squeeze(1)
+            m_init, v_init = t_x_init.mean(1).squeeze(1), t_x_init.var(1).squeeze(1)
             # out_features
-            scale_init = self.init_scale / \
-                torch.sqrt(v_init + 1e-10)
+            scale_init = self.init_scale / torch.sqrt(v_init + 1e-10)
             self.g.data.copy_(scale_init)
             self.b.data.copy_(-m_init * scale_init)
             scale_init_shape = scale_init.view(
-                1, self.out_channels, *([1] * (len(x_init.size()) - 2)))
+                1, self.out_channels, *([1] * (len(x_init.size()) - 2))
+            )
             m_init_shape = m_init.view(
-                1, self.out_channels, *([1] * (len(x_init.size()) - 2)))
+                1, self.out_channels, *([1] * (len(x_init.size()) - 2))
+            )
 
-            x_init = scale_init_shape.expand_as(x_init)\
-                * (x_init - m_init_shape.expand_as(x_init))
+            x_init = scale_init_shape.expand_as(x_init) * (
+                x_init - m_init_shape.expand_as(x_init)
+            )
             self.V_avg.copy_(self.V.data)
             self.g_avg.copy_(self.g.data)
             self.b_avg.copy_(self.b.data)
             return x_init
         else:
             v, g, b = get_vars_maybe_avg(
-                self, ['V', 'g', 'b'], self.training,
-                polyak_decay=self.polyak_decay)
-            scalar = g / \
-                torch.norm(v.transpose(0, 1).contiguous().view(
-                    self.out_channels, -1), 2, 1).squeeze(1)
-            w = scalar.view(self.in_channels, self.out_channels,
-                            *([1] * (len(v.size()) - 2))).expand_as(v) * v
-
-            x = F.conv_transpose2d(x, w, b, self.stride,
-                                   self.padding, self.output_padding,
-                                   self.groups)
+                self, ["V", "g", "b"], self.training, polyak_decay=self.polyak_decay
+            )
+            scalar = g / torch.norm(
+                v.transpose(0, 1).contiguous().view(self.out_channels, -1), 2, 1
+            ).squeeze(1)
+            w = (
+                scalar.view(
+                    self.in_channels, self.out_channels, *([1] * (len(v.size()) - 2))
+                ).expand_as(v)
+                * v
+            )
+
+            x = F.conv_transpose2d(
+                x, w, b, self.stride, self.padding, self.output_padding, self.groups
+            )
             return x
```

### Comparing `OpenNMT-py-3.1.2/onmt/scorers/__init__.py` & `OpenNMT-py-3.1.3/onmt/scorers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 """Module for dynamic scoring"""
 import os
 import importlib
 
 from .scorer import Scorer, build_scorers
 
 AVAILABLE_SCORERS = {}
@@ -24,27 +23,30 @@
 
 def register_scorer(metric):
     """Scorer register that can be used to add new scorer class."""
 
     def register_scorer_cls(cls):
         if metric in AVAILABLE_SCORERS.keys():
             raise ValueError(
-                'Cannot register duplicate scorer for metric ({})'.format(
-                    metric))
+                "Cannot register duplicate scorer for metric ({})".format(metric)
+            )
         if not issubclass(cls, Scorer):
-            raise ValueError('scorer ({}: {}) must extend Scorer'.format(
-                metric, cls.__name__))
+            raise ValueError(
+                "scorer ({}: {}) must extend Scorer".format(metric, cls.__name__)
+            )
         AVAILABLE_SCORERS[metric] = cls
         return cls
 
     return register_scorer_cls
 
 
 # Auto import python files in this directory
 scorer_dir = os.path.dirname(__file__)
 for file in os.listdir(scorer_dir):
     path = os.path.join(scorer_dir, file)
-    if not file.startswith('_') and not file.startswith('.') and (
-            file.endswith('.py') or os.path.isdir(path)):
-        file_name = file[:file.find('.py')] if file.endswith('.py') else file
-        module = importlib.import_module(
-            'onmt.scorers.' + file_name)
+    if (
+        not file.startswith("_")
+        and not file.startswith(".")
+        and (file.endswith(".py") or os.path.isdir(path))
+    ):
+        file_name = file[: file.find(".py")] if file.endswith(".py") else file
+        module = importlib.import_module("onmt.scorers." + file_name)
```

### Comparing `OpenNMT-py-3.1.2/onmt/scorers/scorer.py` & `OpenNMT-py-3.1.3/onmt/scorers/scorer.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_attention.py` & `OpenNMT-py-3.1.3/onmt/tests/test_attention.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,32 +5,28 @@
 import torch
 from torch.autograd import Variable
 
 import onmt
 
 
 class TestAttention(unittest.TestCase):
-
     def test_masked_global_attention(self):
-
         src_len = torch.IntTensor([7, 3, 5, 2])
         # illegal_weights_mask = torch.ByteTensor([
         #     [0, 0, 0, 0, 0, 0, 0],
         #     [0, 0, 0, 1, 1, 1, 1],
         #     [0, 0, 0, 0, 0, 1, 1],
         #     [0, 0, 1, 1, 1, 1, 1]])
 
         batch_size = src_len.size(0)
         dim = 20
 
-        enc_out = Variable(torch.randn(batch_size,
-                           src_len.max(), dim))
+        enc_out = Variable(torch.randn(batch_size, src_len.max(), dim))
         enc_final_hs = Variable(torch.randn(batch_size, dim))
 
         attn = onmt.modules.GlobalAttention(dim)
 
-        _, alignments = attn(enc_final_hs, enc_out,
-                             src_len=src_len)
+        _, alignments = attn(enc_final_hs, enc_out, src_len=src_len)
         # TODO: fix for pytorch 0.3
         # illegal_weights = alignments.masked_select(illegal_weights_mask)
 
         # self.assertEqual(0.0, illegal_weights.data.sum())
```

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_beam_search.py` & `OpenNMT-py-3.1.3/onmt/tests/test_beam_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 
 class GlobalScorerStub(object):
     alpha = 0
     beta = 0
 
     def __init__(self):
-        self.length_penalty = lambda x, alpha: 1.
+        self.length_penalty = lambda x, alpha: 1.0
         self.cov_penalty = lambda cov, beta: torch.zeros(
-            (1, cov.shape[-2]), device=cov.device, dtype=torch.float)
+            (1, cov.shape[-2]), device=cov.device, dtype=torch.float
+        )
         self.has_cov_pen = False
         self.has_len_pen = False
 
     def update_global_state(self, beam):
         pass
 
     def score(self, beam, scores):
@@ -33,220 +34,275 @@
         beam_sz = 5
         n_words = 100
         repeat_idx = 47
         ngram_repeat = 3
         device_init = torch.zeros(1, 1)
         for batch_sz in [1, 3]:
             beam = BeamSearch(
-                beam_sz, batch_sz, 0, 1, 2, 3, 1, 2,
-                GlobalScorerStub(), 0, 30,
-                False, ngram_repeat, set(),
-                False, 0., False)
+                beam_sz,
+                batch_sz,
+                0,
+                1,
+                2,
+                3,
+                1,
+                2,
+                GlobalScorerStub(),
+                0,
+                30,
+                False,
+                ngram_repeat,
+                set(),
+                False,
+                0.0,
+                False,
+            )
             beam.initialize(device_init, torch.randint(0, 30, (batch_sz,)))
             for i in range(ngram_repeat + 4):
                 # predict repeat_idx over and over again
-                word_probs = torch.full(
-                    (batch_sz * beam_sz, n_words), -float('inf'))
+                word_probs = torch.full((batch_sz * beam_sz, n_words), -float("inf"))
                 word_probs[0::beam_sz, repeat_idx] = 0
 
-                attns = torch.randn(1, batch_sz * beam_sz, 53)
+                attns = torch.randn(batch_sz * beam_sz, 1, 53)
                 beam.advance(word_probs, attns)
 
                 if i < ngram_repeat:
                     # before repeat, scores are either 0 or -inf
                     expected_scores = torch.tensor(
-                        [0] + [-float('inf')] * (beam_sz - 1))\
-                        .repeat(batch_sz, 1)
+                        [0] + [-float("inf")] * (beam_sz - 1)
+                    ).repeat(batch_sz, 1)
                     self.assertTrue(beam.topk_log_probs.equal(expected_scores))
                 elif i % ngram_repeat == 0:
                     # on repeat, `repeat_idx` score is BLOCKED_SCORE
                     # (but it's still the best score, thus we have
                     # [BLOCKED_SCORE, -inf, -inf, -inf, -inf]
                     expected_scores = torch.tensor(
-                        [self.BLOCKED_SCORE] + [-float('inf')] * (beam_sz - 1)
+                        [self.BLOCKED_SCORE] + [-float("inf")] * (beam_sz - 1)
                     ).repeat(batch_sz, 1)
                     self.assertTrue(beam.topk_log_probs.equal(expected_scores))
                 else:
                     # repetitions keeps maximizing score
                     # index 0 has been blocked, so repeating=>+0.0 score
                     # other indexes are -inf so repeating=>BLOCKED_SCORE
                     # which is higher
                     expected_scores = torch.tensor(
-                        [self.BLOCKED_SCORE] + [-float('inf')] * (beam_sz - 1)
+                        [self.BLOCKED_SCORE] + [-float("inf")] * (beam_sz - 1)
                     ).repeat(batch_sz, 1)
                     self.assertTrue(beam.topk_log_probs.equal(expected_scores))
 
     def test_advance_with_some_repeats_gets_blocked(self):
         # beam 0 and beam >=2 will repeat (beam >= 2 repeat dummy scores)
         beam_sz = 5
         n_words = 100
         repeat_idx = 47
         ngram_repeat = 3
         no_repeat_score = -2.3
         repeat_score = -0.1
         device_init = torch.zeros(1, 1)
         for batch_sz in [1, 3]:
             beam = BeamSearch(
-                beam_sz, batch_sz, 0, 1, 2, 3, 1, 2,
-                GlobalScorerStub(), 0, 30,
-                False, ngram_repeat, set(),
-                False, 0., False)
+                beam_sz,
+                batch_sz,
+                0,
+                1,
+                2,
+                3,
+                1,
+                2,
+                GlobalScorerStub(),
+                0,
+                30,
+                False,
+                ngram_repeat,
+                set(),
+                False,
+                0.0,
+                False,
+            )
             beam.initialize(device_init, torch.randint(0, 30, (batch_sz,)))
             for i in range(ngram_repeat + 4):
                 # non-interesting beams are going to get dummy values
-                word_probs = torch.full(
-                    (batch_sz * beam_sz, n_words), -float('inf'))
+                word_probs = torch.full((batch_sz * beam_sz, n_words), -float("inf"))
                 if i == 0:
                     # on initial round, only predicted scores for beam 0
                     # matter. Make two predictions. Top one will be repeated
                     # in beam zero, second one will live on in beam 1.
                     word_probs[0::beam_sz, repeat_idx] = repeat_score
-                    word_probs[0::beam_sz, repeat_idx +
-                               i + 1] = no_repeat_score
+                    word_probs[0::beam_sz, repeat_idx + i + 1] = no_repeat_score
                 else:
                     # predict the same thing in beam 0
                     word_probs[0::beam_sz, repeat_idx] = 0
                     # continue pushing around what beam 1 predicts
                     word_probs[1::beam_sz, repeat_idx + i + 1] = 0
-                attns = torch.randn(1, batch_sz * beam_sz, 53)
+                attns = torch.randn(batch_sz * beam_sz, 1, 53)
                 beam.advance(word_probs, attns)
                 if i < ngram_repeat:
                     self.assertFalse(
-                        beam.topk_log_probs[0::beam_sz].eq(
-                            self.BLOCKED_SCORE).any())
+                        beam.topk_log_probs[0::beam_sz].eq(self.BLOCKED_SCORE).any()
+                    )
                     self.assertFalse(
-                        beam.topk_log_probs[1::beam_sz].eq(
-                            self.BLOCKED_SCORE).any())
+                        beam.topk_log_probs[1::beam_sz].eq(self.BLOCKED_SCORE).any()
+                    )
                 elif i == ngram_repeat:
                     # now beam 0 dies (along with the others), beam 1 -> beam 0
                     self.assertFalse(
-                        beam.topk_log_probs[:, 0].eq(
-                            self.BLOCKED_SCORE).any())
+                        beam.topk_log_probs[:, 0].eq(self.BLOCKED_SCORE).any()
+                    )
 
                     expected = torch.full([batch_sz, beam_sz], float("-inf"))
                     expected[:, 0] = no_repeat_score
                     expected[:, 1] = self.BLOCKED_SCORE
-                    self.assertTrue(
-                        beam.topk_log_probs[:, :].equal(expected))
+                    self.assertTrue(beam.topk_log_probs[:, :].equal(expected))
                 else:
                     # now beam 0 dies (along with the others), beam 1 -> beam 0
                     self.assertFalse(
-                        beam.topk_log_probs[:, 0].eq(
-                            self.BLOCKED_SCORE).any())
+                        beam.topk_log_probs[:, 0].eq(self.BLOCKED_SCORE).any()
+                    )
 
                     expected = torch.full([batch_sz, beam_sz], float("-inf"))
                     expected[:, 0] = no_repeat_score
                     expected[:, 1:3] = self.BLOCKED_SCORE
                     expected[:, 3:] = float("-inf")
-                    self.assertTrue(
-                        beam.topk_log_probs.equal(expected))
+                    self.assertTrue(beam.topk_log_probs.equal(expected))
 
     def test_repeating_excluded_index_does_not_die(self):
         # beam 0 and beam >= 2 will repeat (beam 2 repeats excluded idx)
         beam_sz = 5
         n_words = 100
         repeat_idx = 47  # will be repeated and should be blocked
         repeat_idx_ignored = 7  # will be repeated and should not be blocked
         ngram_repeat = 3
         device_init = torch.zeros(1, 1)
         for batch_sz in [1, 3]:
             beam = BeamSearch(
-                beam_sz, batch_sz, 0, 1, 2, 3, 1, 2,
-                GlobalScorerStub(), 0, 30,
-                False, ngram_repeat, {repeat_idx_ignored},
-                False, 0., False)
+                beam_sz,
+                batch_sz,
+                0,
+                1,
+                2,
+                3,
+                1,
+                2,
+                GlobalScorerStub(),
+                0,
+                30,
+                False,
+                ngram_repeat,
+                {repeat_idx_ignored},
+                False,
+                0.0,
+                False,
+            )
             beam.initialize(device_init, torch.randint(0, 30, (batch_sz,)))
             for i in range(ngram_repeat + 4):
                 # non-interesting beams are going to get dummy values
-                word_probs = torch.full(
-                    (batch_sz * beam_sz, n_words), -float('inf'))
+                word_probs = torch.full((batch_sz * beam_sz, n_words), -float("inf"))
                 if i == 0:
                     word_probs[0::beam_sz, repeat_idx] = -0.1
                     word_probs[0::beam_sz, repeat_idx + i + 1] = -2.3
                     word_probs[0::beam_sz, repeat_idx_ignored] = -5.0
                 else:
                     # predict the same thing in beam 0
                     word_probs[0::beam_sz, repeat_idx] = 0
                     # continue pushing around what beam 1 predicts
                     word_probs[1::beam_sz, repeat_idx + i + 1] = 0
                     # predict the allowed-repeat again in beam 2
                     word_probs[2::beam_sz, repeat_idx_ignored] = 0
-                attns = torch.randn(1, batch_sz * beam_sz, 53)
+                attns = torch.randn(batch_sz * beam_sz, 1, 53)
                 beam.advance(word_probs, attns)
                 if i < ngram_repeat:
-                    self.assertFalse(beam.topk_log_probs[:, 0].eq(
-                        self.BLOCKED_SCORE).any())
-                    self.assertFalse(beam.topk_log_probs[:, 1].eq(
-                        self.BLOCKED_SCORE).any())
-                    self.assertFalse(beam.topk_log_probs[:, 2].eq(
-                        self.BLOCKED_SCORE).any())
+                    self.assertFalse(
+                        beam.topk_log_probs[:, 0].eq(self.BLOCKED_SCORE).any()
+                    )
+                    self.assertFalse(
+                        beam.topk_log_probs[:, 1].eq(self.BLOCKED_SCORE).any()
+                    )
+                    self.assertFalse(
+                        beam.topk_log_probs[:, 2].eq(self.BLOCKED_SCORE).any()
+                    )
                 else:
                     # now beam 0 dies, beam 1 -> beam 0, beam 2 -> beam 1
                     # and the rest die
-                    self.assertFalse(beam.topk_log_probs[:, 0].eq(
-                        self.BLOCKED_SCORE).any())
+                    self.assertFalse(
+                        beam.topk_log_probs[:, 0].eq(self.BLOCKED_SCORE).any()
+                    )
                     # since all preds after i=0 are 0, we can check
                     # that the beam is the correct idx by checking that
                     # the curr score is the initial score
                     self.assertTrue(beam.topk_log_probs[:, 0].eq(-2.3).all())
-                    self.assertFalse(beam.topk_log_probs[:, 1].eq(
-                        self.BLOCKED_SCORE).all())
+                    self.assertFalse(
+                        beam.topk_log_probs[:, 1].eq(self.BLOCKED_SCORE).all()
+                    )
                     self.assertTrue(beam.topk_log_probs[:, 1].eq(-5.0).all())
 
-                    self.assertTrue(beam.topk_log_probs[:, 2].eq(
-                        self.BLOCKED_SCORE).all())
+                    self.assertTrue(
+                        beam.topk_log_probs[:, 2].eq(self.BLOCKED_SCORE).all()
+                    )
 
     def test_doesnt_predict_eos_if_shorter_than_min_len(self):
         # beam 0 will always predict EOS. The other beams will predict
         # non-eos scores.
         for batch_sz in [1, 3]:
             beam_sz = 5
             n_words = 100
             _non_eos_idxs = [47, 51, 13, 88, 99]
-            valid_score_dist = torch.log_softmax(torch.tensor(
-                [6., 5., 4., 3., 2., 1.]), dim=0)
+            valid_score_dist = torch.log_softmax(
+                torch.tensor([6.0, 5.0, 4.0, 3.0, 2.0, 1.0]), dim=0
+            )
             min_length = 5
             eos_idx = 2
             lengths = torch.randint(0, 30, (batch_sz,))
-            beam = BeamSearch(beam_sz, batch_sz, 0, 1, 2, 3, 1, 2,
-                              GlobalScorerStub(),
-                              min_length, 30, False, 0, set(),
-                              False, 0., False)
+            beam = BeamSearch(
+                beam_sz,
+                batch_sz,
+                0,
+                1,
+                2,
+                3,
+                1,
+                2,
+                GlobalScorerStub(),
+                min_length,
+                30,
+                False,
+                0,
+                set(),
+                False,
+                0.0,
+                False,
+            )
             device_init = torch.zeros(1, 1)
             beam.initialize(device_init, lengths)
             all_attns = []
             for i in range(min_length + 4):
                 # non-interesting beams are going to get dummy values
-                word_probs = torch.full(
-                    (batch_sz * beam_sz, n_words), -float('inf'))
+                word_probs = torch.full((batch_sz * beam_sz, n_words), -float("inf"))
                 if i == 0:
                     # "best" prediction is eos - that should be blocked
                     word_probs[0::beam_sz, eos_idx] = valid_score_dist[0]
                     # include at least beam_sz predictions OTHER than EOS
                     # that are greater than -1e20
                     for j, score in zip(_non_eos_idxs, valid_score_dist[1:]):
                         word_probs[0::beam_sz, j] = score
                 else:
                     # predict eos in beam 0
                     word_probs[0::beam_sz, eos_idx] = valid_score_dist[0]
                     # provide beam_sz other good predictions
                     for k, (j, score) in enumerate(
-                            zip(_non_eos_idxs, valid_score_dist[1:])):
+                        zip(_non_eos_idxs, valid_score_dist[1:])
+                    ):
                         beam_idx = min(beam_sz - 1, k)
                         word_probs[beam_idx::beam_sz, j] = score
 
-                attns = torch.randn(1, batch_sz * beam_sz, 53)
+                attns = torch.randn(batch_sz * beam_sz, 1, 53)
                 all_attns.append(attns)
                 beam.advance(word_probs, attns)
                 if i < min_length:
-                    expected_score_dist = \
-                        (i + 1) * valid_score_dist[1:].unsqueeze(0)
-                    self.assertTrue(
-                        beam.topk_log_probs.allclose(
-                            expected_score_dist))
+                    expected_score_dist = (i + 1) * valid_score_dist[1:].unsqueeze(0)
+                    self.assertTrue(beam.topk_log_probs.allclose(expected_score_dist))
                 elif i == min_length:
                     # now the top beam has ended and no others have
                     self.assertTrue(beam.is_finished[:, 0].eq(1).all())
                     self.assertTrue(beam.is_finished[:, 1:].eq(0).all())
                 else:  # i > min_length
                     # not of interest, but want to make sure it keeps running
                     # since only beam 0 terminates and n_best = 2
@@ -255,49 +311,64 @@
     def test_beam_is_done_when_X_beams_eos_using_min_length(self):
         # this is also a test that when block_ngram_repeat=0,
         # repeating is acceptable
         beam_sz = 5
         batch_sz = 3
         n_words = 100
         _non_eos_idxs = [47, 51, 13, 88, 99]
-        valid_score_dist = torch.log_softmax(torch.tensor(
-            [6., 5., 4., 3., 2., 1.]), dim=0)
+        valid_score_dist = torch.log_softmax(
+            torch.tensor([6.0, 5.0, 4.0, 3.0, 2.0, 1.0]), dim=0
+        )
         min_length = 5
         eos_idx = 2
         beam = BeamSearch(
-            beam_sz, batch_sz, 0, 1, 2, 3, 1, 2,
+            beam_sz,
+            batch_sz,
+            0,
+            1,
+            2,
+            3,
+            1,
+            2,
             GlobalScorerStub(),
-            min_length, 30, False, 0, set(),
-            False, 0., False)
+            min_length,
+            30,
+            False,
+            0,
+            set(),
+            False,
+            0.0,
+            False,
+        )
         device_init = torch.zeros(1, 1)
         beam.initialize(device_init, torch.randint(0, 30, (batch_sz,)))
         for i in range(min_length + 4):
             # non-interesting beams are going to get dummy values
-            word_probs = torch.full(
-                (batch_sz * beam_sz, n_words), -float('inf'))
+            word_probs = torch.full((batch_sz * beam_sz, n_words), -float("inf"))
             if i == 0:
                 # "best" prediction is eos - that should be blocked
                 word_probs[0::beam_sz, eos_idx] = valid_score_dist[0]
                 # include at least beam_sz predictions OTHER than EOS
                 # that are greater than -1e20
                 for j, score in zip(_non_eos_idxs, valid_score_dist[1:]):
                     word_probs[0::beam_sz, j] = score
             elif i <= min_length:
                 # predict eos in beam 1
                 word_probs[1::beam_sz, eos_idx] = valid_score_dist[0]
                 # provide beam_sz other good predictions in other beams
                 for k, (j, score) in enumerate(
-                        zip(_non_eos_idxs, valid_score_dist[1:])):
+                    zip(_non_eos_idxs, valid_score_dist[1:])
+                ):
                     beam_idx = min(beam_sz - 1, k)
                     word_probs[beam_idx::beam_sz, j] = score
             else:
                 for j in range(beam_sz):
                     word_probs[j::beam_sz, eos_idx] = valid_score_dist[0]
 
-            attns = torch.randn(1, batch_sz * beam_sz, 53)
+            attns = torch.randn(batch_sz * beam_sz, 1, 53)
             beam.advance(word_probs, attns)
             if i < min_length:
                 self.assertFalse(beam.done)
             elif i == min_length:
                 # beam 1 dies on min_length
                 self.assertTrue(beam.is_finished[:, 1].all())
                 beam.update_finished()
@@ -309,51 +380,66 @@
                 self.assertTrue(beam.done)
 
     def test_beam_returns_attn_with_correct_length(self):
         beam_sz = 5
         batch_sz = 3
         n_words = 100
         _non_eos_idxs = [47, 51, 13, 88, 99]
-        valid_score_dist = torch.log_softmax(torch.tensor(
-            [6., 5., 4., 3., 2., 1.]), dim=0)
+        valid_score_dist = torch.log_softmax(
+            torch.tensor([6.0, 5.0, 4.0, 3.0, 2.0, 1.0]), dim=0
+        )
         min_length = 5
         eos_idx = 2
         inp_lens = torch.randint(1, 30, (batch_sz,))
         beam = BeamSearch(
-            beam_sz, batch_sz, 0, 1, 2, 3, 1, 2,
+            beam_sz,
+            batch_sz,
+            0,
+            1,
+            2,
+            3,
+            1,
+            2,
             GlobalScorerStub(),
-            min_length, 30, True, 0, set(),
-            False, 0., False)
+            min_length,
+            30,
+            True,
+            0,
+            set(),
+            False,
+            0.0,
+            False,
+        )
         device_init = torch.zeros(1, 1)
         _, _, inp_lens, _ = beam.initialize(device_init, inp_lens)
         # inp_lens is tiled in initialize, reassign to make attn match
         for i in range(min_length + 2):
             # non-interesting beams are going to get dummy values
-            word_probs = torch.full(
-                (batch_sz * beam_sz, n_words), -float('inf'))
+            word_probs = torch.full((batch_sz * beam_sz, n_words), -float("inf"))
             if i == 0:
                 # "best" prediction is eos - that should be blocked
                 word_probs[0::beam_sz, eos_idx] = valid_score_dist[0]
                 # include at least beam_sz predictions OTHER than EOS
                 # that are greater than -1e20
                 for j, score in zip(_non_eos_idxs, valid_score_dist[1:]):
                     word_probs[0::beam_sz, j] = score
             elif i <= min_length:
                 # predict eos in beam 1
                 word_probs[1::beam_sz, eos_idx] = valid_score_dist[0]
                 # provide beam_sz other good predictions in other beams
                 for k, (j, score) in enumerate(
-                        zip(_non_eos_idxs, valid_score_dist[1:])):
+                    zip(_non_eos_idxs, valid_score_dist[1:])
+                ):
                     beam_idx = min(beam_sz - 1, k)
                     word_probs[beam_idx::beam_sz, j] = score
             else:
                 for j in range(beam_sz):
                     word_probs[j::beam_sz, eos_idx] = valid_score_dist[0]
 
-            attns = torch.randn(1, batch_sz * beam_sz, 53)
+            attns = torch.randn(batch_sz * beam_sz, 1, 53)
             beam.advance(word_probs, attns)
             if i < min_length:
                 self.assertFalse(beam.done)
                 # no top beams are finished yet
                 for b in range(batch_sz):
                     self.assertEqual(beam.attention[b], [])
             elif i == min_length:
@@ -371,16 +457,15 @@
                 self.assertTrue(beam.done)
                 # top beam is finished now so there are attentions
                 for b in range(batch_sz):
                     # two beams are finished in each batch
                     self.assertEqual(len(beam.attention[b]), 2)
                     for k in range(2):
                         # second dim is cut down to the non-padded src length
-                        self.assertEqual(beam.attention[b][k].shape[-1],
-                                         inp_lens[b])
+                        self.assertEqual(beam.attention[b][k].shape[-1], inp_lens[b])
                     # first dim is equal to the time of death
                     # (beam 0 died at current step - adjust for SOS)
                     self.assertEqual(beam.attention[b][0].shape[0], i + 1)
                     # (beam 1 died at last step - adjust for SOS)
                     self.assertEqual(beam.attention[b][1].shape[0], i)
                 # behavior gets weird when beam is already done so just stop
                 break
@@ -394,94 +479,108 @@
     N_WORDS = 8  # also don't change for same reason
     N_BEST = 3
     DEAD_SCORE = -1e20
     BATCH_SZ = 3
     INP_SEQ_LEN = 53
 
     def random_attn(self):
-        return torch.randn(1, self.BATCH_SZ * self.BEAM_SZ, self.INP_SEQ_LEN)
+        return torch.randn(self.BATCH_SZ * self.BEAM_SZ, 1, self.INP_SEQ_LEN)
 
     def init_step(self, beam, expected_len_pen):
         # init_preds: [4, 3, 5, 6, 7] - no EOS's
-        init_scores = torch.log_softmax(torch.tensor(
-            [[0, 0, 0, 4, 5, 3, 2, 1]], dtype=torch.float), dim=1)
-        init_scores = deepcopy(init_scores.repeat(
-            self.BATCH_SZ * self.BEAM_SZ, 1))
+        init_scores = torch.log_softmax(
+            torch.tensor([[0, 0, 0, 4, 5, 3, 2, 1]], dtype=torch.float), dim=1
+        )
+        init_scores = deepcopy(init_scores.repeat(self.BATCH_SZ * self.BEAM_SZ, 1))
         new_scores = init_scores + beam.topk_log_probs.view(-1).unsqueeze(1)
-        expected_beam_scores, expected_preds_0 = new_scores \
-            .view(self.BATCH_SZ, self.BEAM_SZ * self.N_WORDS) \
-            .topk(self.BEAM_SZ, dim=-1)
+        expected_beam_scores, expected_preds_0 = new_scores.view(
+            self.BATCH_SZ, self.BEAM_SZ * self.N_WORDS
+        ).topk(self.BEAM_SZ, dim=-1)
         beam.advance(deepcopy(init_scores), self.random_attn())
         self.assertTrue(beam.topk_log_probs.allclose(expected_beam_scores))
         self.assertTrue(beam.topk_ids.equal(expected_preds_0))
         self.assertFalse(beam.is_finished.any())
         self.assertFalse(beam.done)
         return expected_beam_scores
 
     def first_step(self, beam, expected_beam_scores, expected_len_pen):
         # no EOS's yet
         assert beam.is_finished.sum() == 0
-        scores_1 = torch.log_softmax(torch.tensor(
-            [[0, 0, 0, .3, 0, .51, .2, 0],
-             [0, 0, 1.5, 0, 0, 0, 0, 0],
-             [0, 0, 0, 0, .49, .48, 0, 0],
-             [0, 0, 0, .2, .2, .2, .2, .2],
-             [0, 0, 0, .2, .2, .2, .2, .2]]
-        ), dim=1)
+        scores_1 = torch.log_softmax(
+            torch.tensor(
+                [
+                    [0, 0, 0, 0.3, 0, 0.51, 0.2, 0],
+                    [0, 0, 1.5, 0, 0, 0, 0, 0],
+                    [0, 0, 0, 0, 0.49, 0.48, 0, 0],
+                    [0, 0, 0, 0.2, 0.2, 0.2, 0.2, 0.2],
+                    [0, 0, 0, 0.2, 0.2, 0.2, 0.2, 0.2],
+                ]
+            ),
+            dim=1,
+        )
         scores_1 = scores_1.repeat(self.BATCH_SZ, 1)
 
         beam.advance(deepcopy(scores_1), self.random_attn())
 
         new_scores = scores_1 + expected_beam_scores.view(-1).unsqueeze(1)
-        expected_beam_scores, unreduced_preds = new_scores\
-            .view(self.BATCH_SZ, self.BEAM_SZ * self.N_WORDS)\
-            .topk(self.BEAM_SZ, -1)
-        expected_bptr_1 = torch.div(unreduced_preds, self.N_WORDS,
-                                    rounding_mode='trunc')
+        expected_beam_scores, unreduced_preds = new_scores.view(
+            self.BATCH_SZ, self.BEAM_SZ * self.N_WORDS
+        ).topk(self.BEAM_SZ, -1)
+        expected_bptr_1 = torch.div(
+            unreduced_preds, self.N_WORDS, rounding_mode="trunc"
+        )
         # [5, 3, 2, 6, 0], so beam 2 predicts EOS!
         expected_preds_1 = unreduced_preds - expected_bptr_1 * self.N_WORDS
         self.assertTrue(beam.topk_log_probs.allclose(expected_beam_scores))
-        self.assertTrue(beam.topk_scores.allclose(
-            expected_beam_scores / expected_len_pen))
+        self.assertTrue(
+            beam.topk_scores.allclose(expected_beam_scores / expected_len_pen)
+        )
         self.assertTrue(beam.topk_ids.equal(expected_preds_1))
         self.assertTrue(beam.current_backptr.equal(expected_bptr_1))
         self.assertEqual(beam.is_finished.sum(), self.BATCH_SZ)
         self.assertTrue(beam.is_finished[:, 2].all())  # beam 2 finished
         beam.update_finished()
         self.assertFalse(beam.top_beam_finished.any())
         self.assertFalse(beam.done)
         return expected_beam_scores
 
     def second_step(self, beam, expected_beam_scores, expected_len_pen):
         # assumes beam 2 finished on last step
-        scores_2 = torch.log_softmax(torch.tensor(
-            [[0, 0, 0, .3, 0, .51, .2, 0],
-             [0, 0, 0, 0, 0, 0, 0, 0],
-             [0, 0, 0, 0, 5000, .48, 0, 0],  # beam 2 shouldn't continue
-             [0, 0, 50, .2, .2, .2, .2, .2],  # beam 3 -> beam 0 should die
-             [0, 0, 0, .2, .2, .2, .2, .2]]
-        ), dim=1)
+        scores_2 = torch.log_softmax(
+            torch.tensor(
+                [
+                    [0, 0, 0, 0.3, 0, 0.51, 0.2, 0],
+                    [0, 0, 0, 0, 0, 0, 0, 0],
+                    [0, 0, 0, 0, 5000, 0.48, 0, 0],  # beam 2 shouldn't continue
+                    [0, 0, 50, 0.2, 0.2, 0.2, 0.2, 0.2],  # beam 3 -> beam 0 should die
+                    [0, 0, 0, 0.2, 0.2, 0.2, 0.2, 0.2],
+                ]
+            ),
+            dim=1,
+        )
         scores_2 = scores_2.repeat(self.BATCH_SZ, 1)
 
         beam.advance(deepcopy(scores_2), self.random_attn())
 
         # ended beam 2 shouldn't continue
-        expected_beam_scores[:, 2::self.BEAM_SZ] = self.DEAD_SCORE
+        expected_beam_scores[:, 2 :: self.BEAM_SZ] = self.DEAD_SCORE
         new_scores = scores_2 + expected_beam_scores.view(-1).unsqueeze(1)
-        expected_beam_scores, unreduced_preds = new_scores\
-            .view(self.BATCH_SZ, self.BEAM_SZ * self.N_WORDS)\
-            .topk(self.BEAM_SZ, -1)
-        expected_bptr_2 = torch.div(unreduced_preds, self.N_WORDS,
-                                    rounding_mode='trunc')
+        expected_beam_scores, unreduced_preds = new_scores.view(
+            self.BATCH_SZ, self.BEAM_SZ * self.N_WORDS
+        ).topk(self.BEAM_SZ, -1)
+        expected_bptr_2 = torch.div(
+            unreduced_preds, self.N_WORDS, rounding_mode="trunc"
+        )
         # [2, 5, 3, 6, 0] repeat self.BATCH_SZ, so beam 0 predicts EOS!
         expected_preds_2 = unreduced_preds - expected_bptr_2 * self.N_WORDS
         # [-2.4879, -3.8910, -4.1010, -4.2010, -4.4010] repeat self.BATCH_SZ
         self.assertTrue(beam.topk_log_probs.allclose(expected_beam_scores))
-        self.assertTrue(beam.topk_scores.allclose(
-            expected_beam_scores / expected_len_pen))
+        self.assertTrue(
+            beam.topk_scores.allclose(expected_beam_scores / expected_len_pen)
+        )
         self.assertTrue(beam.topk_ids.equal(expected_preds_2))
         self.assertTrue(beam.current_backptr.equal(expected_bptr_2))
         # another beam is finished in all batches
         self.assertEqual(beam.is_finished.sum(), self.BATCH_SZ)
         # new beam 0 finished
         self.assertTrue(beam.is_finished[:, 0].all())
         # new beam 0 is old beam 3
@@ -489,125 +588,190 @@
         beam.update_finished()
         self.assertTrue(beam.top_beam_finished.all())
         self.assertFalse(beam.done)
         return expected_beam_scores
 
     def third_step(self, beam, expected_beam_scores, expected_len_pen):
         # assumes beam 0 finished on last step
-        scores_3 = torch.log_softmax(torch.tensor(
-            [[0, 0, 10000, 0, 5000, .51, .2, 0],  # beam 0 shouldn't cont
-             [0, 0, 0, 0, 0, 0, 0, 0],
-             [0, 0, 10000, 0, 0, 5000, 0, 0],
-             [0, 0, 50, .2, .2, .2, .2, .2],  # beam 3 -> beam 1 should die
-             [0, 0, 50, 0, .2, .2, .2, .2]]
-        ), dim=1)
+        scores_3 = torch.log_softmax(
+            torch.tensor(
+                [
+                    [0, 0, 10000, 0, 5000, 0.51, 0.2, 0],  # beam 0 shouldn't cont
+                    [0, 0, 0, 0, 0, 0, 0, 0],
+                    [0, 0, 10000, 0, 0, 5000, 0, 0],
+                    [0, 0, 50, 0.2, 0.2, 0.2, 0.2, 0.2],  # beam 3 -> beam 1 should die
+                    [0, 0, 50, 0, 0.2, 0.2, 0.2, 0.2],
+                ]
+            ),
+            dim=1,
+        )
         scores_3 = scores_3.repeat(self.BATCH_SZ, 1)
 
         beam.advance(deepcopy(scores_3), self.random_attn())
 
-        expected_beam_scores[:, 0::self.BEAM_SZ] = self.DEAD_SCORE
+        expected_beam_scores[:, 0 :: self.BEAM_SZ] = self.DEAD_SCORE
         new_scores = scores_3 + expected_beam_scores.view(-1).unsqueeze(1)
-        expected_beam_scores, unreduced_preds = new_scores\
-            .view(self.BATCH_SZ, self.BEAM_SZ * self.N_WORDS)\
-            .topk(self.BEAM_SZ, -1)
-        expected_bptr_3 = torch.div(unreduced_preds, self.N_WORDS,
-                                    rounding_mode='trunc')
+        expected_beam_scores, unreduced_preds = new_scores.view(
+            self.BATCH_SZ, self.BEAM_SZ * self.N_WORDS
+        ).topk(self.BEAM_SZ, -1)
+        expected_bptr_3 = torch.div(
+            unreduced_preds, self.N_WORDS, rounding_mode="trunc"
+        )
         # [5, 2, 6, 1, 0] repeat self.BATCH_SZ, so beam 1 predicts EOS!
         expected_preds_3 = unreduced_preds - expected_bptr_3 * self.N_WORDS
-        self.assertTrue(beam.topk_log_probs.allclose(
-            expected_beam_scores))
-        self.assertTrue(beam.topk_scores.allclose(
-            expected_beam_scores / expected_len_pen))
+        self.assertTrue(beam.topk_log_probs.allclose(expected_beam_scores))
+        self.assertTrue(
+            beam.topk_scores.allclose(expected_beam_scores / expected_len_pen)
+        )
         self.assertTrue(beam.topk_ids.equal(expected_preds_3))
         self.assertTrue(beam.current_backptr.equal(expected_bptr_3))
         # we finish 3 hyps per example in this step
         self.assertEqual(beam.is_finished.sum(), self.BATCH_SZ * 3)
         # new beam 1 is old beam 3
         self.assertTrue(expected_bptr_3[:, 1].eq(3).all())
         beam.update_finished()
         self.assertTrue(beam.top_beam_finished.all())
         self.assertTrue(beam.done)
         return expected_beam_scores
 
     def test_beam_advance_against_known_reference(self):
         beam = BeamSearch(
-            self.BEAM_SZ, self.BATCH_SZ, 0, 1, 2, 3, 1, self.N_BEST,
+            self.BEAM_SZ,
+            self.BATCH_SZ,
+            0,
+            1,
+            2,
+            3,
+            1,
+            self.N_BEST,
             GlobalScorerStub(),
-            0, 30, False, 0, set(),
-            False, 0., False)
+            0,
+            30,
+            False,
+            0,
+            set(),
+            False,
+            0.0,
+            False,
+        )
         device_init = torch.zeros(1, 1)
         beam.initialize(device_init, torch.randint(0, 30, (self.BATCH_SZ,)))
         expected_beam_scores = self.init_step(beam, 1)
         expected_beam_scores = self.first_step(beam, expected_beam_scores, 1)
         expected_beam_scores = self.second_step(beam, expected_beam_scores, 1)
         self.third_step(beam, expected_beam_scores, 1)
 
 
 class TestBeamWithLengthPenalty(TestBeamSearchAgainstReferenceCase):
     # this could be considered an integration test because it tests
     # interactions between the GNMT scorer and the beam
 
     def test_beam_advance_against_known_reference(self):
-        scorer = GNMTGlobalScorer(1.0, 0., "avg", "none")
+        scorer = GNMTGlobalScorer(1.0, 0.0, "avg", "none")
         beam = BeamSearch(
-            self.BEAM_SZ, self.BATCH_SZ, 0, 1, 2, 3, 1, self.N_BEST,
+            self.BEAM_SZ,
+            self.BATCH_SZ,
+            0,
+            1,
+            2,
+            3,
+            1,
+            self.N_BEST,
             scorer,
-            0, 30, False, 0, set(),
-            False, 0., False)
+            0,
+            30,
+            False,
+            0,
+            set(),
+            False,
+            0.0,
+            False,
+        )
         device_init = torch.zeros(1, 1)
         beam.initialize(device_init, torch.randint(0, 30, (self.BATCH_SZ,)))
-        expected_beam_scores = self.init_step(beam, 1.)
+        expected_beam_scores = self.init_step(beam, 1.0)
         expected_beam_scores = self.first_step(beam, expected_beam_scores, 3)
         expected_beam_scores = self.second_step(beam, expected_beam_scores, 4)
         self.third_step(beam, expected_beam_scores, 5)
 
 
 class TestBeamSearchLM(TestBeamSearchAgainstReferenceCase):
     def finish_first_beam_step(self, beam):
-        scores_finish = torch.log_softmax(torch.tensor(
-            [[0, 0, 10000, 0, 5000, .51, .2, 0],  # beam 0 shouldn't cont
-             [100000, 100001, 0, 0, 0, 0, 0, 0],
-             [0, 100000, 0, 0, 0, 5000, 0, 0],
-             [0, 0, 0, .2, .2, .2, .2, .2],
-             [0, 0, 0, 0, .2, .2, .2, .2]]  # beam 4 -> beam 1 should die
-        ), dim=1)
+        scores_finish = torch.log_softmax(
+            torch.tensor(
+                [
+                    [0, 0, 10000, 0, 5000, 0.51, 0.2, 0],  # beam 0 shouldn't cont
+                    [100000, 100001, 0, 0, 0, 0, 0, 0],
+                    [0, 100000, 0, 0, 0, 5000, 0, 0],
+                    [0, 0, 0, 0.2, 0.2, 0.2, 0.2, 0.2],
+                    [0, 0, 0, 0, 0.2, 0.2, 0.2, 0.2],
+                ]  # beam 4 -> beam 1 should die
+            ),
+            dim=1,
+        )
         scores_finish = scores_finish.repeat(self.BATCH_SZ, 1)
-        scores_finish[:self.BEAM_SZ, beam.eos] = 100
+        scores_finish[: self.BEAM_SZ, beam.eos] = 100
         beam.advance(scores_finish, None)
 
         any_finished = beam.is_finished.any()
         if any_finished:
             beam.update_finished()
 
     def test_beam_lm_increase_src_len(self):
         beam = BeamSearchLM(
-            self.BEAM_SZ, self.BATCH_SZ, 0, 1, 2, 3, 1, self.N_BEST,
+            self.BEAM_SZ,
+            self.BATCH_SZ,
+            0,
+            1,
+            2,
+            3,
+            1,
+            self.N_BEST,
             GlobalScorerStub(),
-            0, 30, False, 0, set(),
-            False, 0., False)
+            0,
+            30,
+            False,
+            0,
+            set(),
+            False,
+            0.0,
+            False,
+        )
         device_init = torch.zeros(1, 1)
         src_len = torch.randint(0, 30, (self.BATCH_SZ,))
         fn_map_state, _, _, _ = beam.initialize(device_init, src_len)
         expected_beam_scores = self.init_step(beam, 1)
         expected_beam_scores = self.first_step(beam, expected_beam_scores, 1)
         expected_beam_scores = self.second_step(beam, expected_beam_scores, 1)
         self.third_step(beam, expected_beam_scores, 1)
 
         n_steps = beam.alive_seq.shape[-1] - 1
-        self.assertTrue(beam.src_len.equal(
-            n_steps+fn_map_state(src_len, dim=0)))
+        self.assertTrue(beam.src_len.equal(n_steps + fn_map_state(src_len, dim=0)))
 
     def test_beam_lm_update_src_len_when_finished(self):
         beam = BeamSearchLM(
-            self.BEAM_SZ, self.BATCH_SZ, 0, 1, 2, 3, 1, self.N_BEST,
+            self.BEAM_SZ,
+            self.BATCH_SZ,
+            0,
+            1,
+            2,
+            3,
+            1,
+            self.N_BEST,
             GlobalScorerStub(),
-            0, 30, False, 0, set(),
-            False, 0., False)
+            0,
+            30,
+            False,
+            0,
+            set(),
+            False,
+            0.0,
+            False,
+        )
         device_init = torch.zeros(1, 1)
         src_len = torch.randint(0, 30, (self.BATCH_SZ,))
         fn_map_state, _, _, _ = beam.initialize(device_init, src_len)
         self.init_step(beam, 1)
         self.finish_first_beam_step(beam)
 
         n_steps = beam.alive_seq.shape[-1] - 1
-        self.assertTrue(beam.src_len.equal(
-            n_steps+fn_map_state(src_len[1:], dim=0)))
+        self.assertTrue(beam.src_len.equal(n_steps + fn_map_state(src_len[1:], dim=0)))
```

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_copy_generator.py` & `OpenNMT-py-3.1.3/onmt/tests/test_copy_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,131 +7,138 @@
 import torch
 from torch.nn.functional import softmax
 
 from onmt.tests.utils_for_tests import product_dict
 
 
 class TestCopyGenerator(unittest.TestCase):
-    INIT_CASES = list(product_dict(
-        input_size=[172],
-        output_size=[319],
-        pad_idx=[0, 39],
-    ))
-    PARAMS = list(product_dict(
-        batch_size=[1, 14],
-        max_seq_len=[23],
-        tgt_max_len=[50],
-        n_extra_words=[107]
-    ))
+    INIT_CASES = list(
+        product_dict(
+            input_size=[172],
+            output_size=[319],
+            pad_idx=[0, 39],
+        )
+    )
+    PARAMS = list(
+        product_dict(
+            batch_size=[1, 14], max_seq_len=[23], tgt_max_len=[50], n_extra_words=[107]
+        )
+    )
 
     @classmethod
     def dummy_inputs(cls, params, init_case):
-        hidden = torch.randn((params["batch_size"] * params["tgt_max_len"],
-                              init_case["input_size"]))
-        attn = torch.randn((params["batch_size"] * params["tgt_max_len"],
-                            params["max_seq_len"]))
-        src_map = torch.randn((params["batch_size"], params["max_seq_len"],
-                               params["n_extra_words"]))
+        hidden = torch.randn(
+            (params["batch_size"] * params["tgt_max_len"], init_case["input_size"])
+        )
+        attn = torch.randn(
+            (params["batch_size"] * params["tgt_max_len"], params["max_seq_len"])
+        )
+        src_map = torch.randn(
+            (params["batch_size"], params["max_seq_len"], params["n_extra_words"])
+        )
         return hidden, attn, src_map
 
     @classmethod
     def expected_shape(cls, params, init_case):
-        return params["tgt_max_len"] * params["batch_size"], \
-               init_case["output_size"] + params["n_extra_words"]
+        return (
+            params["tgt_max_len"] * params["batch_size"],
+            init_case["output_size"] + params["n_extra_words"],
+        )
 
     def test_copy_gen_forward_shape(self):
-        for params, init_case in itertools.product(
-                self.PARAMS, self.INIT_CASES):
+        for params, init_case in itertools.product(self.PARAMS, self.INIT_CASES):
             cgen = CopyGenerator(**init_case)
             dummy_in = self.dummy_inputs(params, init_case)
             res = cgen(*dummy_in)
             expected_shape = self.expected_shape(params, init_case)
             self.assertEqual(res.shape, expected_shape, init_case.__str__())
 
     def test_copy_gen_outp_has_no_prob_of_pad(self):
-        for params, init_case in itertools.product(
-                self.PARAMS, self.INIT_CASES):
+        for params, init_case in itertools.product(self.PARAMS, self.INIT_CASES):
             cgen = CopyGenerator(**init_case)
             dummy_in = self.dummy_inputs(params, init_case)
             res = cgen(*dummy_in)
-            self.assertTrue(
-                res[:, init_case["pad_idx"]].allclose(torch.tensor(0.0)))
+            self.assertTrue(res[:, init_case["pad_idx"]].allclose(torch.tensor(0.0)))
 
     def test_copy_gen_trainable_params_update(self):
-        for params, init_case in itertools.product(
-                self.PARAMS, self.INIT_CASES):
+        for params, init_case in itertools.product(self.PARAMS, self.INIT_CASES):
             cgen = CopyGenerator(**init_case)
-            trainable_params = {n: p for n, p in cgen.named_parameters()
-                                if p.requires_grad}
+            trainable_params = {
+                n: p for n, p in cgen.named_parameters() if p.requires_grad
+            }
             assert len(trainable_params) > 0  # sanity check
             old_weights = deepcopy(trainable_params)
             dummy_in = self.dummy_inputs(params, init_case)
             res = cgen(*dummy_in)
             pretend_loss = res.sum()
             pretend_loss.backward()
             dummy_optim = torch.optim.SGD(trainable_params.values(), 1)
             dummy_optim.step()
             for param_name in old_weights.keys():
                 self.assertTrue(
-                    trainable_params[param_name]
-                    .ne(old_weights[param_name]).any(),
-                    param_name + " " + init_case.__str__())
+                    trainable_params[param_name].ne(old_weights[param_name]).any(),
+                    param_name + " " + init_case.__str__(),
+                )
 
 
 class TestCopyGeneratorLoss(unittest.TestCase):
-    INIT_CASES = list(product_dict(
-        vocab_size=[172],
-        unk_index=[0, 39],
-        ignore_index=[1, 17],  # pad idx
-        force_copy=[True, False]
-    ))
-    PARAMS = list(product_dict(
-        batch_size=[1, 14],
-        tgt_max_len=[50],
-        n_extra_words=[107]
-    ))
+    INIT_CASES = list(
+        product_dict(
+            vocab_size=[172],
+            unk_index=[0, 39],
+            ignore_index=[1, 17],  # pad idx
+            force_copy=[True, False],
+        )
+    )
+    PARAMS = list(
+        product_dict(batch_size=[1, 14], tgt_max_len=[50], n_extra_words=[107])
+    )
 
     @classmethod
     def dummy_inputs(cls, params, init_case):
         n_unique_src_words = 13
-        scores = torch.randn((params["batch_size"] * params["tgt_max_len"],
-                              init_case["vocab_size"] + n_unique_src_words))
+        scores = torch.randn(
+            (
+                params["batch_size"] * params["tgt_max_len"],
+                init_case["vocab_size"] + n_unique_src_words,
+            )
+        )
         scores = softmax(scores, dim=1)
-        align = torch.randint(0, n_unique_src_words,
-                              (params["batch_size"] * params["tgt_max_len"],))
-        target = torch.randint(0, init_case["vocab_size"],
-                               (params["batch_size"] * params["tgt_max_len"],))
+        align = torch.randint(
+            0, n_unique_src_words, (params["batch_size"] * params["tgt_max_len"],)
+        )
+        target = torch.randint(
+            0, init_case["vocab_size"], (params["batch_size"] * params["tgt_max_len"],)
+        )
         target[0] = init_case["unk_index"]
         target[1] = init_case["ignore_index"]
         return scores, align, target
 
     @classmethod
     def expected_shape(cls, params, init_case):
         return (params["batch_size"] * params["tgt_max_len"],)
 
     def test_copy_loss_forward_shape(self):
-        for params, init_case in itertools.product(
-                self.PARAMS, self.INIT_CASES):
+        for params, init_case in itertools.product(self.PARAMS, self.INIT_CASES):
             loss = CopyGeneratorLoss(**init_case)
             dummy_in = self.dummy_inputs(params, init_case)
             res = loss(*dummy_in)
             expected_shape = self.expected_shape(params, init_case)
             self.assertEqual(res.shape, expected_shape, init_case.__str__())
 
     def test_copy_loss_ignore_index_is_ignored(self):
-        for params, init_case in itertools.product(
-                self.PARAMS, self.INIT_CASES):
+        for params, init_case in itertools.product(self.PARAMS, self.INIT_CASES):
             loss = CopyGeneratorLoss(**init_case)
             scores, align, target = self.dummy_inputs(params, init_case)
             res = loss(scores, align, target)
             should_be_ignored = (target == init_case["ignore_index"]).nonzero(
-                as_tuple=False)
+                as_tuple=False
+            )
             assert len(should_be_ignored) > 0  # otherwise not testing anything
             self.assertTrue(res[should_be_ignored].allclose(torch.tensor(0.0)))
 
     def test_copy_loss_output_range_is_positive(self):
-        for params, init_case in itertools.product(
-                self.PARAMS, self.INIT_CASES):
+        for params, init_case in itertools.product(self.PARAMS, self.INIT_CASES):
             loss = CopyGeneratorLoss(**init_case)
             dummy_in = self.dummy_inputs(params, init_case)
             res = loss(*dummy_in)
             self.assertTrue((res >= 0).all())
```

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_data_prepare.py` & `OpenNMT-py-3.1.3/onmt/tests/test_data_prepare.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 
 from onmt.utils.parse import ArgumentParser
 from onmt.opts import dynamic_prepare_opts
 from onmt.train_single import prepare_transforms_vocabs
 from onmt.constants import CorpusName
 
 
-SAVE_DATA_PREFIX = 'data/test_data_prepare'
+SAVE_DATA_PREFIX = "data/test_data_prepare"
 
 
 def get_default_opts():
-    parser = ArgumentParser(description='data sample prepare')
+    parser = ArgumentParser(description="data sample prepare")
     dynamic_prepare_opts(parser)
 
     default_opts = [
-        '-config', 'data/data.yaml',
-        '-src_vocab', 'data/vocab-train.src',
-        '-tgt_vocab', 'data/vocab-train.tgt'
+        "-config",
+        "data/data.yaml",
+        "-src_vocab",
+        "data/vocab-train.src",
+        "-tgt_vocab",
+        "data/vocab-train.tgt",
     ]
 
     opt = parser.parse_known_args(default_opts)[0]
     # Inject some dummy training options that may needed when build fields
     opt.copy_attn = False
     ArgumentParser.validate_prepare_opts(opt)
     return opt
@@ -42,29 +45,29 @@
 
     def dataset_build(self, opt):
         try:
             prepare_transforms_vocabs(opt)
         except SystemExit as err:
             print(err)
         except IOError as err:
-            if opt.skip_empty_level != 'error':
+            if opt.skip_empty_level != "error":
                 raise err
             else:
                 print(f"Catched IOError: {err}")
         finally:
             # Remove the generated *pt files.
-            for pt in glob.glob(SAVE_DATA_PREFIX + '*.pt'):
+            for pt in glob.glob(SAVE_DATA_PREFIX + "*.pt"):
                 os.remove(pt)
             if self.opt.save_data:
                 # Remove the generated data samples
                 sample_path = os.path.join(
-                    os.path.dirname(self.opt.save_data),
-                    CorpusName.SAMPLE)
+                    os.path.dirname(self.opt.save_data), CorpusName.SAMPLE
+                )
                 if os.path.exists(sample_path):
-                    for f in glob.glob(sample_path + '/*'):
+                    for f in glob.glob(sample_path + "/*"):
                         os.remove(f)
                     os.rmdir(sample_path)
 
 
 def _add_test(param_setting, methodname):
     """
     Adds a Test to TestData according to settings
@@ -78,40 +81,36 @@
         if param_setting:
             opt = copy.deepcopy(self.opt)
             for param, setting in param_setting:
                 setattr(opt, param, setting)
         else:
             opt = self.opt
         getattr(self, methodname)(opt)
+
     if param_setting:
-        name = 'test_' + methodname + "_" + "_".join(
-            str(param_setting).split())
+        name = "test_" + methodname + "_" + "_".join(str(param_setting).split())
     else:
-        name = 'test_' + methodname + '_standard'
+        name = "test_" + methodname + "_standard"
     setattr(TestData, name, test_method)
     test_method.__name__ = name
 
 
-test_databuild = [[],
-                  [('src_vocab_size', 1),
-                   ('tgt_vocab_size', 1)],
-                  [('src_vocab_size', 10000),
-                   ('tgt_vocab_size', 10000)],
-                  [('src_seq_len', 1)],
-                  [('src_seq_len', 5000)],
-                  [('src_seq_length_trunc', 1)],
-                  [('src_seq_length_trunc', 5000)],
-                  [('tgt_seq_len', 1)],
-                  [('tgt_seq_len', 5000)],
-                  [('tgt_seq_length_trunc', 1)],
-                  [('tgt_seq_length_trunc', 5000)],
-                  [('copy_attn', True)],
-                  [('share_vocab', True)],
-                  [('n_sample', 30),
-                   ('save_data', SAVE_DATA_PREFIX)],
-                  [('n_sample', 30),
-                   ('save_data', SAVE_DATA_PREFIX),
-                   ('skip_empty_level', 'error')]
-                  ]
+test_databuild = [
+    [],
+    [("src_vocab_size", 1), ("tgt_vocab_size", 1)],
+    [("src_vocab_size", 10000), ("tgt_vocab_size", 10000)],
+    [("src_seq_len", 1)],
+    [("src_seq_len", 5000)],
+    [("src_seq_length_trunc", 1)],
+    [("src_seq_length_trunc", 5000)],
+    [("tgt_seq_len", 1)],
+    [("tgt_seq_len", 5000)],
+    [("tgt_seq_length_trunc", 1)],
+    [("tgt_seq_length_trunc", 5000)],
+    [("copy_attn", True)],
+    [("share_vocab", True)],
+    [("n_sample", 30), ("save_data", SAVE_DATA_PREFIX)],
+    [("n_sample", 30), ("save_data", SAVE_DATA_PREFIX), ("skip_empty_level", "error")],
+]
 
 for p in test_databuild:
-    _add_test(p, 'dataset_build')
+    _add_test(p, "dataset_build")
```

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_embeddings.py` & `OpenNMT-py-3.1.3/onmt/tests/test_embeddings.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,30 @@
 
 import torch
 
 from onmt.tests.utils_for_tests import product_dict
 
 
 class TestEmbeddings(unittest.TestCase):
-    INIT_CASES = list(product_dict(
-        word_vec_size=[172],
-        word_vocab_size=[319],
-        word_padding_idx=[17],
-        position_encoding=[False, True],
-        feat_merge=["first", "concat", "sum", "mlp"],
-        feat_vec_exponent=[-1, 1.1, 0.7],
-        feat_vec_size=[0, 200],
-        feat_padding_idx=[[], [29], [0, 1]],
-        feat_vocab_sizes=[[], [39], [401, 39]],
-        dropout=[0, 0.5],
-        freeze_word_vecs=[False, True]
-    ))
-    PARAMS = list(product_dict(
-        batch_size=[1, 14],
-        max_seq_len=[23]
-    ))
+    INIT_CASES = list(
+        product_dict(
+            word_vec_size=[172],
+            word_vocab_size=[319],
+            word_padding_idx=[17],
+            position_encoding=[False, True],
+            feat_merge=["first", "concat", "sum", "mlp"],
+            feat_vec_exponent=[-1, 1.1, 0.7],
+            feat_vec_size=[0, 200],
+            feat_padding_idx=[[], [29], [0, 1]],
+            feat_vocab_sizes=[[], [39], [401, 39]],
+            dropout=[0, 0.5],
+            freeze_word_vecs=[False, True],
+        )
+    )
+    PARAMS = list(product_dict(batch_size=[1, 14], max_seq_len=[23]))
 
     @classmethod
     def case_is_degenerate(cls, case):
         no_feats = len(case["feat_vocab_sizes"]) == 0
         if case["feat_merge"] != "first" and no_feats:
             return True
         if case["feat_merge"] == "first" and not no_feats:
@@ -61,23 +60,21 @@
     @classmethod
     def dummy_inputs(cls, params, init_case):
         max_seq_len = params["max_seq_len"]
         batch_size = params["batch_size"]
         fv_sizes = init_case["feat_vocab_sizes"]
         n_words = init_case["word_vocab_size"]
         voc_sizes = [n_words] + fv_sizes
-        pad_idxs = [init_case["word_padding_idx"]] + \
-            init_case["feat_padding_idx"]
+        pad_idxs = [init_case["word_padding_idx"]] + init_case["feat_padding_idx"]
         lengths = torch.randint(0, max_seq_len, (batch_size,))
         lengths[0] = max_seq_len
-        inps = torch.empty((batch_size, max_seq_len, len(voc_sizes)),
-                           dtype=torch.long)
+        inps = torch.empty((batch_size, max_seq_len, len(voc_sizes)), dtype=torch.long)
         for f, (voc_size, pad_idx) in enumerate(zip(voc_sizes, pad_idxs)):
             for b, len_ in enumerate(lengths):
-                inps[b, :len_, f] = torch.randint(0, voc_size-1, (len_,))
+                inps[b, :len_, f] = torch.randint(0, voc_size - 1, (len_,))
                 inps[b, len_:, f] = pad_idx
         return inps
 
     @classmethod
     def expected_shape(cls, params, init_case):
         wvs = init_case["word_vec_size"]
         fvs = init_case["feat_vec_size"]
@@ -92,57 +89,67 @@
             emb = Embeddings(**init_case)
             dummy_in = self.dummy_inputs(params, init_case)
             res = emb(dummy_in)
             expected_shape = self.expected_shape(params, init_case)
             self.assertEqual(res.shape, expected_shape, init_case.__str__())
 
     def test_embeddings_trainable_params(self):
-        for params, init_case in itertools.product(self.PARAMS,
-                                                   self.cases()):
+        for params, init_case in itertools.product(self.PARAMS, self.cases()):
             emb = Embeddings(**init_case)
-            trainable_params = {n: p for n, p in emb.named_parameters()
-                                if p.requires_grad}
+            trainable_params = {
+                n: p for n, p in emb.named_parameters() if p.requires_grad
+            }
             # first check there's nothing unexpectedly not trainable
             for key in emb.state_dict():
                 if key not in trainable_params:
-                    if key.endswith("emb_luts.0.weight") and \
-                            init_case["freeze_word_vecs"]:
+                    if (
+                        key.endswith("emb_luts.0.weight")
+                        and init_case["freeze_word_vecs"]
+                    ):
                         # ok: word embeddings shouldn't be trainable
                         # if word vecs are freezed
                         continue
                     if key.endswith(".pe.pe"):
                         # ok: positional encodings shouldn't be trainable
                         assert init_case["position_encoding"]
                         continue
                     else:
-                        self.fail("Param {:s} is unexpectedly not "
-                                  "trainable.".format(key))
+                        self.fail(
+                            "Param {:s} is unexpectedly not " "trainable.".format(key)
+                        )
             # then check nothing unexpectedly trainable
             if init_case["freeze_word_vecs"]:
                 self.assertFalse(
-                    any(trainable_param.endswith("emb_luts.0.weight")
-                        for trainable_param in trainable_params),
-                    "Word embedding is trainable but word vecs are freezed.")
+                    any(
+                        trainable_param.endswith("emb_luts.0.weight")
+                        for trainable_param in trainable_params
+                    ),
+                    "Word embedding is trainable but word vecs are freezed.",
+                )
             if init_case["position_encoding"]:
                 self.assertFalse(
-                    any(trainable_p.endswith(".pe.pe")
-                        for trainable_p in trainable_params),
-                    "Positional encoding is trainable.")
+                    any(
+                        trainable_p.endswith(".pe.pe")
+                        for trainable_p in trainable_params
+                    ),
+                    "Positional encoding is trainable.",
+                )
 
     def test_embeddings_trainable_params_update(self):
         for params, init_case in itertools.product(self.PARAMS, self.cases()):
             emb = Embeddings(**init_case)
-            trainable_params = {n: p for n, p in emb.named_parameters()
-                                if p.requires_grad}
+            trainable_params = {
+                n: p for n, p in emb.named_parameters() if p.requires_grad
+            }
             if len(trainable_params) > 0:
                 old_weights = deepcopy(trainable_params)
                 dummy_in = self.dummy_inputs(params, init_case)
                 res = emb(dummy_in)
                 pretend_loss = res.sum()
                 pretend_loss.backward()
                 dummy_optim = torch.optim.SGD(trainable_params.values(), 1)
                 dummy_optim.step()
                 for param_name in old_weights.keys():
                     self.assertTrue(
-                        trainable_params[param_name]
-                        .ne(old_weights[param_name]).any(),
-                        param_name + " " + init_case.__str__())
+                        trainable_params[param_name].ne(old_weights[param_name]).any(),
+                        param_name + " " + init_case.__str__(),
+                    )
```

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_events.py` & `OpenNMT-py-3.1.3/onmt/tests/test_events.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,58 @@
-
 from tensorboard.backend.event_processing import event_accumulator
 from argparse import ArgumentParser
 import os
 
 
-class TestEvents():
+class TestEvents:
     def __init__(self):
-        stats = ['xent', 'ppl', 'accuracy', 'tgtper', 'lr']
-        metrics = ['BLEU', 'TER']
+        stats = ["xent", "ppl", "accuracy", "tgtper", "lr"]
+        metrics = ["BLEU", "TER"]
         self.scalars = {}
-        self.scalars["train"] = [('progress/' + stat) for stat in stats]
-        self.scalars["train_valid"] = (self.scalars["train"] +
-                                       [('valid/' + stat) for stat in stats])
-        self.scalars["train_metrics"] = (
-            self.scalars["train"] +
-            [('progress/' + metric) for metric in metrics])
+        self.scalars["train"] = [("progress/" + stat) for stat in stats]
+        self.scalars["train_valid"] = self.scalars["train"] + [
+            ("valid/" + stat) for stat in stats
+        ]
+        self.scalars["train_metrics"] = self.scalars["train"] + [
+            ("progress/" + metric) for metric in metrics
+        ]
         self.scalars["train_valid_metrics"] = (
-            self.scalars["train_metrics"] +
-            [('valid/' + stat) for stat in stats] +
-            [('valid/' + metric) for metric in metrics])
+            self.scalars["train_metrics"]
+            + [("valid/" + stat) for stat in stats]
+            + [("valid/" + metric) for metric in metrics]
+        )
 
     def reload_events(self, path):
         ea = event_accumulator.EventAccumulator(
-            path, size_guidance={event_accumulator.SCALARS: 0},
+            path,
+            size_guidance={event_accumulator.SCALARS: 0},
         )
         ea.Reload()
         return ea
 
     def check_scalars(self, scalars, logdir):
         for event_file in os.listdir(logdir):
             path = os.path.join(logdir, event_file)
             event_accumulator = self.reload_events(path)
             # make sure the scalars are in the event accumulator tags
             assert all(
                 s in event_accumulator.Tags()["scalars"] for s in scalars
             ), "{} some scalars were not found in the event accumulator"
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # required arguments
     parser = ArgumentParser()
-    requiredArgs = parser.add_argument_group('required arguments')
+    requiredArgs = parser.add_argument_group("required arguments")
     requiredArgs.add_argument("-logdir", "--logdir", type=str, required=True)
     requiredArgs.add_argument(
-        "-tensorboard_checks", "--tensorboard_checks", type=str, required=True,
-        choices=["train", "train_metrics",
-                 "train_valid", "train_valid_metrics"])
+        "-tensorboard_checks",
+        "--tensorboard_checks",
+        type=str,
+        required=True,
+        choices=["train", "train_metrics", "train_valid", "train_valid_metrics"],
+    )
     args = parser.parse_args()
     test_event = TestEvents()
     scalars = test_event.scalars[args.tensorboard_checks]
     print("looking for scalars: ", scalars)
     test_event.check_scalars(scalars, args.logdir)
```

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_greedy_search.py` & `OpenNMT-py-3.1.3/onmt/tests/test_greedy_search.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 
 class GlobalScorerStub(object):
     alpha = 0
     beta = 0
 
     def __init__(self):
-        self.length_penalty = lambda x, alpha: 1.
+        self.length_penalty = lambda x, alpha: 1.0
         self.cov_penalty = lambda cov, beta: torch.zeros(
-            (1, cov.shape[-2]), device=cov.device, dtype=torch.float)
+            (1, cov.shape[-2]), device=cov.device, dtype=torch.float
+        )
         self.has_cov_pen = False
         self.has_len_pen = False
 
     def update_global_state(self, beam):
         pass
 
     def score(self, beam, scores):
@@ -31,394 +32,487 @@
 
     def test_doesnt_predict_eos_if_shorter_than_min_len(self):
         # batch 0 will always predict EOS. The other batches will predict
         # non-eos scores.
         for batch_sz in [1, 3]:
             n_words = 100
             _non_eos_idxs = [47]
-            valid_score_dist = torch.log_softmax(torch.tensor(
-                [6., 5.]), dim=0)
+            valid_score_dist = torch.log_softmax(torch.tensor([6.0, 5.0]), dim=0)
             min_length = 5
             eos_idx = 2
             lengths = torch.randint(0, 30, (batch_sz,))
             samp = GreedySearch(
-                0, 1, 2, 3, 1, batch_sz, GlobalScorerStub(), min_length,
-                False, set(), False, 30, 1., 1, 0, 1, False)
+                0,
+                1,
+                2,
+                3,
+                1,
+                batch_sz,
+                GlobalScorerStub(),
+                min_length,
+                False,
+                set(),
+                False,
+                30,
+                1.0,
+                1,
+                0,
+                1,
+                False,
+            )
             samp.initialize(torch.zeros((1, 1)), lengths)
             all_attns = []
             for i in range(min_length + 4):
-                word_probs = torch.full(
-                    (batch_sz, n_words), -float('inf'))
+                word_probs = torch.full((batch_sz, n_words), -float("inf"))
                 # "best" prediction is eos - that should be blocked
                 word_probs[0, eos_idx] = valid_score_dist[0]
                 # include at least one prediction OTHER than EOS
                 # that is greater than -1e20
                 word_probs[0, _non_eos_idxs[0]] = valid_score_dist[1]
                 word_probs[1:, _non_eos_idxs[0] + i] = 0
 
                 attns = torch.randn(1, batch_sz, 53)
                 all_attns.append(attns)
                 samp.advance(word_probs, attns)
                 if i < min_length:
-                    self.assertTrue(
-                        samp.topk_scores[0].allclose(valid_score_dist[1]))
-                    self.assertTrue(
-                        samp.topk_scores[1:].eq(0).all())
+                    self.assertTrue(samp.topk_scores[0].allclose(valid_score_dist[1]))
+                    self.assertTrue(samp.topk_scores[1:].eq(0).all())
                 elif i == min_length:
                     # now batch 0 has ended and no others have
                     self.assertTrue(samp.is_finished[0, :].eq(1).all())
                     self.assertTrue(samp.is_finished[1:, 1:].eq(0).all())
                 else:  # i > min_length
                     break
 
     def test_returns_correct_scores_deterministic(self):
         for batch_sz in [1, 13]:
-            for temp in [1., 3.]:
+            for temp in [1.0, 3.0]:
                 n_words = 100
                 _non_eos_idxs = [47, 51, 13, 88, 99]
-                valid_score_dist_1 = torch.log_softmax(torch.tensor(
-                    [6., 5., 4., 3., 2., 1.]), dim=0)
-                valid_score_dist_2 = torch.log_softmax(torch.tensor(
-                    [6., 1.]), dim=0)
+                valid_score_dist_1 = torch.log_softmax(
+                    torch.tensor([6.0, 5.0, 4.0, 3.0, 2.0, 1.0]), dim=0
+                )
+                valid_score_dist_2 = torch.log_softmax(torch.tensor([6.0, 1.0]), dim=0)
                 eos_idx = 2
                 lengths = torch.randint(0, 30, (batch_sz,))
                 samp = GreedySearch(
-                    0, 1, 2, 3, 1, batch_sz, GlobalScorerStub(), 0,
-                    False, set(), False, 30, temp, 1, 0, 1, False)
+                    0,
+                    1,
+                    2,
+                    3,
+                    1,
+                    batch_sz,
+                    GlobalScorerStub(),
+                    0,
+                    False,
+                    set(),
+                    False,
+                    30,
+                    temp,
+                    1,
+                    0,
+                    1,
+                    False,
+                )
                 samp.initialize(torch.zeros((1, 1)), lengths)
                 # initial step
                 i = 0
-                word_probs = torch.full(
-                    (batch_sz, n_words), -float('inf'))
+                word_probs = torch.full((batch_sz, n_words), -float("inf"))
                 # batch 0 dies on step 0
                 word_probs[0, eos_idx] = valid_score_dist_1[0]
                 # include at least one prediction OTHER than EOS
                 # that is greater than -1e20
                 word_probs[0, _non_eos_idxs] = valid_score_dist_1[1:]
                 word_probs[1:, _non_eos_idxs[0] + i] = 0
 
                 attns = torch.randn(1, batch_sz, 53)
                 samp.advance(word_probs, attns)
                 self.assertTrue(samp.is_finished[0].eq(1).all())
                 samp.update_finished()
                 self.assertEqual(
                     [score for score, _, _ in samp.hypotheses[0]],
-                    [valid_score_dist_1[0] / temp])
+                    [valid_score_dist_1[0] / temp],
+                )
                 if batch_sz == 1:
                     self.assertTrue(samp.done)
                     continue
                 else:
                     self.assertFalse(samp.done)
 
                 # step 2
                 i = 1
-                word_probs = torch.full(
-                    (batch_sz - 1, n_words), -float('inf'))
+                word_probs = torch.full((batch_sz - 1, n_words), -float("inf"))
                 # (old) batch 8 dies on step 1
                 word_probs[7, eos_idx] = valid_score_dist_2[0]
                 word_probs[0:7, _non_eos_idxs[:2]] = valid_score_dist_2
                 word_probs[8:, _non_eos_idxs[:2]] = valid_score_dist_2
 
                 attns = torch.randn(1, batch_sz, 53)
                 samp.advance(word_probs, attns)
 
                 self.assertTrue(samp.is_finished[7].eq(1).all())
                 samp.update_finished()
                 self.assertEqual(
                     [score for score, _, _ in samp.hypotheses[8]],
-                    [valid_score_dist_2[0] / temp])
+                    [valid_score_dist_2[0] / temp],
+                )
 
                 # step 3
                 i = 2
-                word_probs = torch.full(
-                    (batch_sz - 2, n_words), -float('inf'))
+                word_probs = torch.full((batch_sz - 2, n_words), -float("inf"))
                 # everything dies
                 word_probs[:, eos_idx] = 0
 
                 attns = torch.randn(1, batch_sz, 53)
                 samp.advance(word_probs, attns)
 
                 self.assertTrue(samp.is_finished.eq(1).all())
                 samp.update_finished()
                 self.assertTrue(samp.done)
 
     def test_returns_correct_scores_non_deterministic(self):
         for batch_sz in [1, 13]:
-            for temp in [1., 3.]:
+            for temp in [1.0, 3.0]:
                 n_words = 100
                 _non_eos_idxs = [47, 51, 13, 88, 99]
-                valid_score_dist_1 = torch.log_softmax(torch.tensor(
-                    [6., 5., 4., 3., 2., 1.]), dim=0)
-                valid_score_dist_2 = torch.log_softmax(torch.tensor(
-                    [6., 1.]), dim=0)
+                valid_score_dist_1 = torch.log_softmax(
+                    torch.tensor([6.0, 5.0, 4.0, 3.0, 2.0, 1.0]), dim=0
+                )
+                valid_score_dist_2 = torch.log_softmax(torch.tensor([6.0, 1.0]), dim=0)
                 eos_idx = 2
                 lengths = torch.randint(0, 30, (batch_sz,))
                 samp = GreedySearch(
-                    0, 1, 2, 3, 1, batch_sz, GlobalScorerStub(), 0,
-                    False, set(), False, 30, temp, 2, 0, 1, False)
+                    0,
+                    1,
+                    2,
+                    3,
+                    1,
+                    batch_sz,
+                    GlobalScorerStub(),
+                    0,
+                    False,
+                    set(),
+                    False,
+                    30,
+                    temp,
+                    2,
+                    0,
+                    1,
+                    False,
+                )
                 samp.initialize(torch.zeros((1, 1)), lengths)
                 # initial step
                 i = 0
                 for _ in range(100):
-                    word_probs = torch.full(
-                        (batch_sz, n_words), -float('inf'))
+                    word_probs = torch.full((batch_sz, n_words), -float("inf"))
                     # batch 0 dies on step 0
                     word_probs[0, eos_idx] = valid_score_dist_1[0]
                     # include at least one prediction OTHER than EOS
                     # that is greater than -1e20
                     word_probs[0, _non_eos_idxs] = valid_score_dist_1[1:]
                     word_probs[1:, _non_eos_idxs[0] + i] = 0
 
                     attns = torch.randn(1, batch_sz, 53)
                     samp.advance(word_probs, attns)
                     if samp.is_finished[0].eq(1).all():
                         break
                 else:
-                    self.fail("Batch 0 never ended (very unlikely but maybe "
-                              "due to stochasticisty. If so, please increase "
-                              "the range of the for-loop.")
+                    self.fail(
+                        "Batch 0 never ended (very unlikely but maybe "
+                        "due to stochasticisty. If so, please increase "
+                        "the range of the for-loop."
+                    )
                 samp.update_finished()
-                self.assertEqual(
-                    [samp.topk_scores[0]], [valid_score_dist_1[0] / temp])
+                self.assertEqual([samp.topk_scores[0]], [valid_score_dist_1[0] / temp])
                 if batch_sz == 1:
                     self.assertTrue(samp.done)
                     continue
                 else:
                     self.assertFalse(samp.done)
 
                 # step 2
                 i = 1
                 for _ in range(100):
-                    word_probs = torch.full(
-                        (batch_sz - 1, n_words), -float('inf'))
+                    word_probs = torch.full((batch_sz - 1, n_words), -float("inf"))
                     # (old) batch 8 dies on step 1
                     word_probs[7, eos_idx] = valid_score_dist_2[0]
                     word_probs[0:7, _non_eos_idxs[:2]] = valid_score_dist_2
                     word_probs[8:, _non_eos_idxs[:2]] = valid_score_dist_2
 
                     attns = torch.randn(1, batch_sz, 53)
                     samp.advance(word_probs, attns)
                     if samp.is_finished[7].eq(1).all():
                         break
                 else:
-                    self.fail("Batch 8 never ended (very unlikely but maybe "
-                              "due to stochasticisty. If so, please increase "
-                              "the range of the for-loop.")
+                    self.fail(
+                        "Batch 8 never ended (very unlikely but maybe "
+                        "due to stochasticisty. If so, please increase "
+                        "the range of the for-loop."
+                    )
 
                 samp.update_finished()
                 self.assertEqual(
                     [score for score, _, _ in samp.hypotheses[8]],
-                    [valid_score_dist_2[0] / temp])
+                    [valid_score_dist_2[0] / temp],
+                )
 
                 # step 3
                 i = 2
                 for _ in range(250):
                     word_probs = torch.full(
-                        (samp.alive_seq.shape[0], n_words), -float('inf'))
+                        (samp.alive_seq.shape[0], n_words), -float("inf")
+                    )
                     # everything dies
                     word_probs[:, eos_idx] = 0
 
                     attns = torch.randn(1, batch_sz, 53)
                     samp.advance(word_probs, attns)
                     if samp.is_finished.any():
                         samp.update_finished()
                     if samp.is_finished.eq(1).all():
                         break
                 else:
-                    self.fail("All batches never ended (very unlikely but "
-                              "maybe due to stochasticisty. If so, please "
-                              "increase the range of the for-loop.")
+                    self.fail(
+                        "All batches never ended (very unlikely but "
+                        "maybe due to stochasticisty. If so, please "
+                        "increase the range of the for-loop."
+                    )
 
                 self.assertTrue(samp.done)
 
     def test_returns_correct_scores_non_deterministic_beams(self):
         beam_size = 10
         for batch_sz in [1, 13]:
-            for temp in [1., 3.]:
+            for temp in [1.0, 3.0]:
                 n_words = 100
                 _non_eos_idxs = [47, 51, 13, 88, 99]
-                valid_score_dist_1 = torch.log_softmax(torch.tensor(
-                    [6., 5., 4., 3., 2., 1.]), dim=0)
-                valid_score_dist_2 = torch.log_softmax(torch.tensor(
-                    [6., 1.]), dim=0)
+                valid_score_dist_1 = torch.log_softmax(
+                    torch.tensor([6.0, 5.0, 4.0, 3.0, 2.0, 1.0]), dim=0
+                )
+                valid_score_dist_2 = torch.log_softmax(torch.tensor([6.0, 1.0]), dim=0)
                 eos_idx = 2
                 lengths = torch.randint(0, 30, (batch_sz,))
                 samp = GreedySearch(
-                    0, 1, 2, 3, 1, batch_sz, GlobalScorerStub(), 0,
-                    False, set(), False, 30, temp, 50, 0,
-                    beam_size, False)
+                    0,
+                    1,
+                    2,
+                    3,
+                    1,
+                    batch_sz,
+                    GlobalScorerStub(),
+                    0,
+                    False,
+                    set(),
+                    False,
+                    30,
+                    temp,
+                    50,
+                    0,
+                    beam_size,
+                    False,
+                )
                 samp.initialize(torch.zeros((1, 1)), lengths)
                 # initial step
                 # finish one beam
                 i = 0
                 for _ in range(100):
                     word_probs = torch.full(
-                        (batch_sz*beam_size, n_words), -float('inf'))
+                        (batch_sz * beam_size, n_words), -float("inf")
+                    )
 
-                    word_probs[beam_size-2, eos_idx] = valid_score_dist_1[0]
+                    word_probs[beam_size - 2, eos_idx] = valid_score_dist_1[0]
                     # include at least one prediction OTHER than EOS
                     # that is greater than -1e20
-                    word_probs[beam_size-2,
-                               _non_eos_idxs] = valid_score_dist_1[1:]
-                    word_probs[beam_size-2+1:, _non_eos_idxs[0] + i] = 0
-                    word_probs[:beam_size-2, _non_eos_idxs[0] + i] = 0
+                    word_probs[beam_size - 2, _non_eos_idxs] = valid_score_dist_1[1:]
+                    word_probs[beam_size - 2 + 1 :, _non_eos_idxs[0] + i] = 0
+                    word_probs[: beam_size - 2, _non_eos_idxs[0] + i] = 0
 
                     attns = torch.randn(1, batch_sz, 53)
                     samp.advance(word_probs, attns)
-                    if samp.is_finished[beam_size-2].eq(1).all():
+                    if samp.is_finished[beam_size - 2].eq(1).all():
+                        self.assertFalse(samp.is_finished[: beam_size - 2].eq(1).any())
                         self.assertFalse(
-                            samp.is_finished[:beam_size-2].eq(1).any())
-                        self.assertFalse(
-                            samp.is_finished[beam_size-2+1].eq(1).any())
+                            samp.is_finished[beam_size - 2 + 1].eq(1).any()
+                        )
                         break
                 else:
-                    self.fail("Batch 0 never ended (very unlikely but maybe "
-                              "due to stochasticisty. If so, please increase "
-                              "the range of the for-loop.")
+                    self.fail(
+                        "Batch 0 never ended (very unlikely but maybe "
+                        "due to stochasticisty. If so, please increase "
+                        "the range of the for-loop."
+                    )
                 samp.update_finished()
                 self.assertEqual(
-                    [samp.topk_scores[beam_size-2]],
-                    [valid_score_dist_1[0] / temp])
+                    [samp.topk_scores[beam_size - 2]], [valid_score_dist_1[0] / temp]
+                )
 
                 # step 2
                 # finish example in last batch
                 i = 1
                 for _ in range(100):
                     word_probs = torch.full(
-                        (batch_sz*beam_size-1, n_words), -float('inf'))
+                        (batch_sz * beam_size - 1, n_words), -float("inf")
+                    )
                     # (old) batch 8 dies on step 1
-                    word_probs[(batch_sz-1)*beam_size + 7,
-                               eos_idx] = valid_score_dist_2[0]
-                    word_probs[:(batch_sz-1)*beam_size + 7,
-                               _non_eos_idxs[:2]] = valid_score_dist_2
-                    word_probs[(batch_sz-1)*beam_size + 8:,
-                               _non_eos_idxs[:2]] = valid_score_dist_2
+                    word_probs[
+                        (batch_sz - 1) * beam_size + 7, eos_idx
+                    ] = valid_score_dist_2[0]
+                    word_probs[
+                        : (batch_sz - 1) * beam_size + 7, _non_eos_idxs[:2]
+                    ] = valid_score_dist_2
+                    word_probs[
+                        (batch_sz - 1) * beam_size + 8 :, _non_eos_idxs[:2]
+                    ] = valid_score_dist_2
 
                     attns = torch.randn(1, batch_sz, 53)
                     samp.advance(word_probs, attns)
-                    if (
-                        samp.is_finished[(batch_sz - 1) * beam_size + 7]
-                        .eq(1)
-                        .all()
-                    ):
+                    if samp.is_finished[(batch_sz - 1) * beam_size + 7].eq(1).all():
                         break
                 else:
-                    self.fail("Batch 8 never ended (very unlikely but maybe "
-                              "due to stochasticisty. If so, please increase "
-                              "the range of the for-loop.")
+                    self.fail(
+                        "Batch 8 never ended (very unlikely but maybe "
+                        "due to stochasticisty. If so, please increase "
+                        "the range of the for-loop."
+                    )
 
                 samp.update_finished()
                 self.assertEqual(
-                    [score for score, _, _ in samp.hypotheses[
-                        batch_sz-1][-1:]],
-                    [valid_score_dist_2[0] / temp])
+                    [score for score, _, _ in samp.hypotheses[batch_sz - 1][-1:]],
+                    [valid_score_dist_2[0] / temp],
+                )
 
                 # step 3
                 i = 2
                 for _ in range(250):
                     word_probs = torch.full(
-                        (samp.alive_seq.shape[0], n_words), -float('inf'))
+                        (samp.alive_seq.shape[0], n_words), -float("inf")
+                    )
                     # everything dies
                     word_probs[:, eos_idx] = 0
 
                     attns = torch.randn(1, batch_sz, 53)
                     samp.advance(word_probs, attns)
                     if samp.is_finished.any():
                         samp.update_finished()
                     if samp.is_finished.eq(1).all():
                         break
                 else:
-                    self.fail("All batches never ended (very unlikely but "
-                              "maybe due to stochasticisty. If so, please "
-                              "increase the range of the for-loop.")
+                    self.fail(
+                        "All batches never ended (very unlikely but "
+                        "maybe due to stochasticisty. If so, please "
+                        "increase the range of the for-loop."
+                    )
 
                 self.assertTrue(samp.done)
 
     def test_returns_correct_scores_non_deterministic_topp(self):
         for batch_sz in [1, 13]:
-            for temp in [1., 0.3]:
+            for temp in [1.0, 0.3]:
                 n_words = 100
                 _non_eos_idxs = [47, 51, 13, 88, 99]
-                valid_score_dist_1 = torch.log_softmax(torch.tensor(
-                    [6., 5., 4., 3., 2., 1.]), dim=0)
-                valid_score_dist_2 = torch.log_softmax(torch.tensor(
-                    [6., 1.]), dim=0)
+                valid_score_dist_1 = torch.log_softmax(
+                    torch.tensor([6.0, 5.0, 4.0, 3.0, 2.0, 1.0]), dim=0
+                )
+                valid_score_dist_2 = torch.log_softmax(torch.tensor([6.0, 1.0]), dim=0)
                 eos_idx = 2
                 lengths = torch.randint(0, 30, (batch_sz,))
                 samp = GreedySearch(
-                    0, 1, 2, 3, 1, batch_sz, GlobalScorerStub(), 0,
-                    False, set(), False, -1, temp, 50, 0.5, 1, False)
+                    0,
+                    1,
+                    2,
+                    3,
+                    1,
+                    batch_sz,
+                    GlobalScorerStub(),
+                    0,
+                    False,
+                    set(),
+                    False,
+                    -1,
+                    temp,
+                    50,
+                    0.5,
+                    1,
+                    False,
+                )
                 samp.initialize(torch.zeros((1, 1)), lengths)
                 # initial step
                 i = 0
                 for _ in range(100):
-                    word_probs = torch.full(
-                        (batch_sz, n_words), -float('inf'))
+                    word_probs = torch.full((batch_sz, n_words), -float("inf"))
                     # batch 0 dies on step 0
                     word_probs[0, eos_idx] = valid_score_dist_1[0]
                     # include at least one prediction OTHER than EOS
                     # that is greater than -1e20
                     word_probs[0, _non_eos_idxs] = valid_score_dist_1[1:]
                     word_probs[1:, _non_eos_idxs[0] + i] = 0
 
                     attns = torch.randn(1, batch_sz, 53)
                     samp.advance(word_probs, attns)
                     if samp.is_finished[0].eq(1).all():
                         break
                 else:
-                    self.fail("Batch 0 never ended (very unlikely but maybe "
-                              "due to stochasticisty. If so, please increase "
-                              "the range of the for-loop.")
+                    self.fail(
+                        "Batch 0 never ended (very unlikely but maybe "
+                        "due to stochasticisty. If so, please increase "
+                        "the range of the for-loop."
+                    )
                 samp.update_finished()
                 self.assertEqual(
                     [score for score, _, _ in samp.hypotheses[0]],
-                    [valid_score_dist_1[0] / temp])
+                    [valid_score_dist_1[0] / temp],
+                )
                 if batch_sz == 1:
                     self.assertTrue(samp.done)
                     continue
                 else:
                     self.assertFalse(samp.done)
 
                 # step 2
                 i = 1
                 for _ in range(200):
-                    word_probs = torch.full(
-                        (batch_sz - 1, n_words), -float('inf'))
+                    word_probs = torch.full((batch_sz - 1, n_words), -float("inf"))
                     # (old) batch 8 dies on step 1
                     word_probs[7, eos_idx] = valid_score_dist_2[0]
                     word_probs[0:7, _non_eos_idxs[:2]] = valid_score_dist_2
                     word_probs[8:, _non_eos_idxs[:2]] = valid_score_dist_2
 
                     attns = torch.randn(1, batch_sz, 53)
                     samp.advance(word_probs, attns)
                     if samp.is_finished[7].eq(1).all():
                         break
                 else:
-                    self.fail("Batch 8 never ended (very unlikely but maybe "
-                              "due to stochasticisty. If so, please increase "
-                              "the range of the for-loop.")
+                    self.fail(
+                        "Batch 8 never ended (very unlikely but maybe "
+                        "due to stochasticisty. If so, please increase "
+                        "the range of the for-loop."
+                    )
 
                 samp.update_finished()
                 self.assertEqual(
                     [score for score, _, _ in samp.hypotheses[8]],
-                    [valid_score_dist_2[0] / temp])
+                    [valid_score_dist_2[0] / temp],
+                )
 
                 # step 3
                 i = 2
                 for _ in range(250):
                     word_probs = torch.full(
-                        (samp.alive_seq.shape[0], n_words), -float('inf'))
+                        (samp.alive_seq.shape[0], n_words), -float("inf")
+                    )
                     # everything dies
                     word_probs[:, eos_idx] = 0
 
                     attns = torch.randn(1, batch_sz, 53)
                     samp.advance(word_probs, attns)
                     if samp.is_finished.any():
                         samp.update_finished()
                     if samp.is_finished.eq(1).all():
                         break
                 else:
-                    self.fail("All batches never ended (very unlikely but "
-                              "maybe due to stochasticisty. If so, please "
-                              "increase the range of the for-loop.")
+                    self.fail(
+                        "All batches never ended (very unlikely but "
+                        "maybe due to stochasticisty. If so, please "
+                        "increase the range of the for-loop."
+                    )
 
                 self.assertTrue(samp.done)
```

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_models.py` & `OpenNMT-py-3.1.3/onmt/tests/test_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,112 +3,112 @@
 import torch
 import pyonmttok
 from onmt.constants import DefaultTokens
 from collections import Counter
 import onmt
 import onmt.inputters
 import onmt.opts
-from onmt.model_builder import build_embeddings, \
-    build_encoder, build_decoder
+from onmt.model_builder import build_embeddings, build_encoder, build_decoder
 from onmt.utils.parse import ArgumentParser
 
-parser = ArgumentParser(description='train.py')
+parser = ArgumentParser(description="train.py")
 onmt.opts.model_opts(parser)
 onmt.opts._add_train_general_opts(parser)
 
 # -data option is required, but not used in this test, so dummy.
-opt = parser.parse_known_args(['-data', 'dummy'])[0]
+opt = parser.parse_known_args(["-data", "dummy"])[0]
 
 
 class TestModel(unittest.TestCase):
-
     def __init__(self, *args, **kwargs):
         super(TestModel, self).__init__(*args, **kwargs)
         self.opt = opt
 
     def get_vocabs(self):
         src_vocab = pyonmttok.build_vocab_from_tokens(
             Counter(),
             maximum_size=0,
             minimum_frequency=1,
-            special_tokens=[DefaultTokens.UNK,
-                            DefaultTokens.PAD,
-                            DefaultTokens.BOS,
-                            DefaultTokens.EOS])
+            special_tokens=[
+                DefaultTokens.UNK,
+                DefaultTokens.PAD,
+                DefaultTokens.BOS,
+                DefaultTokens.EOS,
+            ],
+        )
 
         tgt_vocab = pyonmttok.build_vocab_from_tokens(
             Counter(),
             maximum_size=0,
             minimum_frequency=1,
-            special_tokens=[DefaultTokens.UNK,
-                            DefaultTokens.PAD,
-                            DefaultTokens.BOS,
-                            DefaultTokens.EOS])
+            special_tokens=[
+                DefaultTokens.UNK,
+                DefaultTokens.PAD,
+                DefaultTokens.BOS,
+                DefaultTokens.EOS,
+            ],
+        )
 
-        vocabs = {'src': src_vocab, 'tgt': tgt_vocab}
+        vocabs = {"src": src_vocab, "tgt": tgt_vocab}
         return vocabs
 
     def get_batch(self, source_l=3, bsize=1):
         # len x batch x nfeat
         test_src = torch.ones(bsize, source_l, 1).long()
         test_tgt = torch.ones(bsize, source_l, 1).long()
         test_length = torch.ones(bsize).fill_(source_l).long()
         return test_src, test_tgt, test_length
 
     def embeddings_forward(self, opt, source_l=3, bsize=1):
-        '''
+        """
         Tests if the embeddings works as expected
 
         args:
             opt: set of options
             source_l: Length of generated input sentence
             bsize: Batchsize of generated input
-        '''
+        """
         vocabs = self.get_vocabs()
         emb = build_embeddings(opt, vocabs)
         test_src, _, __ = self.get_batch(source_l=source_l, bsize=bsize)
-        if opt.decoder_type == 'transformer':
+        if opt.decoder_type == "transformer":
             input = torch.cat([test_src, test_src], 1)
             res = emb(input)
-            compare_to = torch.zeros(bsize, source_l * 2,
-                                     opt.src_word_vec_size)
+            compare_to = torch.zeros(bsize, source_l * 2, opt.src_word_vec_size)
         else:
             res = emb(test_src)
             compare_to = torch.zeros(bsize, source_l, opt.src_word_vec_size)
 
         self.assertEqual(res.size(), compare_to.size())
 
     def encoder_forward(self, opt, source_l=3, bsize=1):
-        '''
+        """
         Tests if the encoder works as expected
 
         args:
             opt: set of options
             source_l: Length of generated input sentence
             bsize: Batchsize of generated input
-        '''
+        """
         if opt.hidden_size > 0:
             opt.enc_hid_size = opt.hidden_size
         vocabs = self.get_vocabs()
         embeddings = build_embeddings(opt, vocabs)
         enc = build_encoder(opt, embeddings)
 
-        test_src, test_tgt, test_length = self.get_batch(source_l=source_l,
-                                                         bsize=bsize)
+        test_src, test_tgt, test_length = self.get_batch(source_l=source_l, bsize=bsize)
 
         enc_out, hidden_t, test_length = enc(test_src, test_length)
 
         # Initialize vectors to compare size with
         test_hid = torch.zeros(self.opt.enc_layers, bsize, opt.enc_hid_size)
         test_out = torch.zeros(bsize, source_l, opt.dec_hid_size)
 
         # Ensure correct sizes and types
-        self.assertEqual(test_hid.size(),
-                         hidden_t[0].size(),
-                         hidden_t[1].size())
+        self.assertEqual(test_hid.size(), hidden_t[0].size(), hidden_t[1].size())
         self.assertEqual(test_out.size(), enc_out.size())
         self.assertEqual(type(enc_out), torch.Tensor)
 
     def nmtmodel_forward(self, opt, source_l=3, bsize=1):
         """
         Creates a nmtmodel with a custom opt function.
         Forwards a testbatch and checks output size.
@@ -127,16 +127,15 @@
         enc = build_encoder(opt, embeddings)
 
         embeddings = build_embeddings(opt, vocabs, for_encoder=False)
         dec = build_decoder(opt, embeddings)
 
         model = onmt.models.model.NMTModel(enc, dec)
 
-        test_src, test_tgt, test_length = self.get_batch(source_l=source_l,
-                                                         bsize=bsize)
+        test_src, test_tgt, test_length = self.get_batch(source_l=source_l, bsize=bsize)
         output, attn = model(test_src, test_tgt, test_length)
         outputsize = torch.zeros(bsize, source_l - 1, opt.dec_hid_size)
         # Make sure that output has the correct size and type
         self.assertEqual(output.size(), outputsize.size())
         self.assertEqual(type(output), torch.Tensor)
 
 
@@ -152,83 +151,88 @@
     def test_method(self):
         opt = copy.deepcopy(self.opt)
         if param_setting:
             for param, setting in param_setting:
                 setattr(opt, param, setting)
         ArgumentParser.update_model_opts(opt)
         getattr(self, methodname)(opt)
+
     if param_setting:
-        name = 'test_' + methodname + "_" + "_".join(
-            str(param_setting).split())
+        name = "test_" + methodname + "_" + "_".join(str(param_setting).split())
     else:
-        name = 'test_' + methodname + '_standard'
+        name = "test_" + methodname + "_standard"
     setattr(TestModel, name, test_method)
     test_method.__name__ = name
 
 
-'''
+"""
 TEST PARAMETERS
-'''
+"""
 opt.brnn = False
 
-test_embeddings = [[],
-                   [('decoder_type', 'transformer')]
-                   ]
+test_embeddings = [[], [("decoder_type", "transformer")]]
 
 for p in test_embeddings:
-    _add_test(p, 'embeddings_forward')
+    _add_test(p, "embeddings_forward")
 
-tests_encoder = [[],
-                 [('encoder_type', 'mean')],
-                 # [('encoder_type', 'transformer'),
-                 # ('word_vec_size', 16), ('hidden_size', 16)],
-                 []
-                 ]
+tests_encoder = [
+    [],
+    [("encoder_type", "mean")],
+    # [('encoder_type', 'transformer'),
+    # ('word_vec_size', 16), ('hidden_size', 16)],
+    [],
+]
 
 for p in tests_encoder:
-    _add_test(p, 'encoder_forward')
+    _add_test(p, "encoder_forward")
 
-tests_nmtmodel = [[('rnn_type', 'GRU')],
-                  [('layers', 10)],
-                  [('input_feed', 0)],
-                  [('decoder_type', 'transformer'),
-                   ('encoder_type', 'transformer'),
-                   ('src_word_vec_size', 16),
-                   ('tgt_word_vec_size', 16),
-                   ('hidden_size', 16)],
-                  [('decoder_type', 'transformer'),
-                   ('encoder_type', 'transformer'),
-                   ('src_word_vec_size', 16),
-                   ('tgt_word_vec_size', 16),
-                   ('hidden_size', 16),
-                   ('position_encoding', True)],
-                  [('coverage_attn', True)],
-                  [('copy_attn', True)],
-                  [('global_attention', 'mlp')],
-                  [('context_gate', 'both')],
-                  [('context_gate', 'target')],
-                  [('context_gate', 'source')],
-                  [('encoder_type', "brnn"),
-                   ('brnn_merge', 'sum')],
-                  [('encoder_type', "brnn")],
-                  [('decoder_type', 'cnn'),
-                   ('encoder_type', 'cnn')],
-                  [('encoder_type', 'rnn'),
-                   ('global_attention', None)],
-                  [('encoder_type', 'rnn'),
-                   ('global_attention', None),
-                   ('copy_attn', True),
-                   ('copy_attn_type', 'general')],
-                  [('encoder_type', 'rnn'),
-                   ('global_attention', 'mlp'),
-                   ('copy_attn', True),
-                   ('copy_attn_type', 'general')],
-                  [],
-                  ]
+tests_nmtmodel = [
+    [("rnn_type", "GRU")],
+    [("layers", 10)],
+    [("input_feed", 0)],
+    [
+        ("decoder_type", "transformer"),
+        ("encoder_type", "transformer"),
+        ("src_word_vec_size", 16),
+        ("tgt_word_vec_size", 16),
+        ("hidden_size", 16),
+    ],
+    [
+        ("decoder_type", "transformer"),
+        ("encoder_type", "transformer"),
+        ("src_word_vec_size", 16),
+        ("tgt_word_vec_size", 16),
+        ("hidden_size", 16),
+        ("position_encoding", True),
+    ],
+    [("coverage_attn", True)],
+    [("copy_attn", True)],
+    [("global_attention", "mlp")],
+    [("context_gate", "both")],
+    [("context_gate", "target")],
+    [("context_gate", "source")],
+    [("encoder_type", "brnn"), ("brnn_merge", "sum")],
+    [("encoder_type", "brnn")],
+    [("decoder_type", "cnn"), ("encoder_type", "cnn")],
+    [("encoder_type", "rnn"), ("global_attention", None)],
+    [
+        ("encoder_type", "rnn"),
+        ("global_attention", None),
+        ("copy_attn", True),
+        ("copy_attn_type", "general"),
+    ],
+    [
+        ("encoder_type", "rnn"),
+        ("global_attention", "mlp"),
+        ("copy_attn", True),
+        ("copy_attn_type", "general"),
+    ],
+    [],
+]
 
 if onmt.modules.sru.check_sru_requirement():
     #   """ Only do SRU test if requirment is safisfied. """
     # SRU doesn't support input_feed.
-    tests_nmtmodel.append([('rnn_type', 'SRU'), ('input_feed', 0)])
+    tests_nmtmodel.append([("rnn_type", "SRU"), ("input_feed", 0)])
 
 for p in tests_nmtmodel:
-    _add_test(p, 'nmtmodel_forward')
+    _add_test(p, "nmtmodel_forward")
```

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_text_utils.py` & `OpenNMT-py-3.1.3/onmt/tests/test_text_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 import unittest
 from onmt.inputters.text_utils import parse_features
 
 
 class TestTextUtils(unittest.TestCase):
-
     def test_parse_features(self):
         input_data = "this is a test"
         text, feats = parse_features(input_data)
         self.assertEqual(text, "this is a test")
         self.assertEqual(feats, None)
 
         input_data = "this is a test"
         text, feats = parse_features(input_data, 0, "0")
         self.assertEqual(text, "this is a test")
         self.assertEqual(feats, None)
 
         input_data = "this is a test"
         n_src_feats = 1
         src_feats_defaults = "0"
-        text, feats = parse_features(input_data, n_src_feats,
-                                     src_feats_defaults)
+        text, feats = parse_features(input_data, n_src_feats, src_feats_defaults)
         self.assertEqual(text, "this is a test")
         self.assertEqual(feats, ["0 0 0 0"])
 
         input_data = "this is a test"
         n_src_feats = 2
         src_feats_defaults = "0￨1"
-        text, feats = parse_features(input_data, n_src_feats,
-                                     src_feats_defaults)
+        text, feats = parse_features(input_data, n_src_feats, src_feats_defaults)
         self.assertEqual(text, "this is a test")
         self.assertEqual(feats, ["0 0 0 0", "1 1 1 1"])
 
         input_data = "this￨0 is￨0 a￨0 test￨1"
         n_src_feats = 1
         src_feats_defaults = "0￨0"
-        text, feats = parse_features(input_data, n_src_feats,
-                                     src_feats_defaults)
+        text, feats = parse_features(input_data, n_src_feats, src_feats_defaults)
         self.assertEqual(text, "this is a test")
         self.assertEqual(feats, ["0 0 0 1"])
 
         input_data = "this￨0￨1 is￨0￨2 a￨0￨3 test￨1￨4"
         n_src_feats = 2
-        text, feats = parse_features(input_data, n_src_feats,
-                                     src_feats_defaults)
+        text, feats = parse_features(input_data, n_src_feats, src_feats_defaults)
         self.assertEqual(text, "this is a test")
         self.assertEqual(feats, ["0 0 0 1", "1 2 3 4"])
 
     def test_invalid_combinations(self):
         # One source feature expected but none given and no default provided
         input_data = "this is a test"
         n_src_feats = 1
```

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_transform.py` & `OpenNMT-py-3.1.3/onmt/tests/test_transform.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,81 +37,83 @@
         self.assertEqual(len(transforms), 0)
         with self.assertRaises(ValueError):
             transforms_cls["switchout"](opt).warm_up(vocabs=None)
             transforms_cls["bart"](opt).warm_up(vocabs=None)
 
     def test_transform_specials(self):
         transforms_cls = get_transforms_cls(["prefix"])
-        corpora = yaml.safe_load("""
+        corpora = yaml.safe_load(
+            """
             trainset:
                 path_src: data/src-train.txt
                 path_tgt: data/tgt-train.txt
                 transforms: ["prefix"]
                 weight: 1
                 src_prefix: "｟_pf_src｠"
                 tgt_prefix: "｟_pf_tgt｠"
-        """)
+        """
+        )
         opt = Namespace(data=corpora)
         specials = get_specials(opt, transforms_cls)
         specials_expected = {"src": ["｟_pf_src｠"], "tgt": ["｟_pf_tgt｠"]}
         self.assertEqual(specials, specials_expected)
 
     def test_transform_pipe(self):
         # 1. Init first transform in the pipe
         prefix_cls = get_transforms_cls(["prefix"])["prefix"]
-        corpora = yaml.safe_load("""
+        corpora = yaml.safe_load(
+            """
             trainset:
                 path_src: data/src-train.txt
                 path_tgt: data/tgt-train.txt
                 transforms: [prefix, filtertoolong]
                 weight: 1
                 src_prefix: "｟_pf_src｠"
                 tgt_prefix: "｟_pf_tgt｠"
-        """)
+        """
+        )
         opt = Namespace(data=corpora, seed=-1)
         prefix_transform = prefix_cls(opt)
         prefix_transform.warm_up()
         # 2. Init second transform in the pipe
         filter_cls = get_transforms_cls(["filtertoolong"])["filtertoolong"]
         opt = Namespace(src_seq_length=4, tgt_seq_length=4)
         filter_transform = filter_cls(opt)
         # 3. Sequential combine them into a transform pipe
-        transform_pipe = TransformPipe.build_from(
-            [prefix_transform, filter_transform]
-        )
+        transform_pipe = TransformPipe.build_from([prefix_transform, filter_transform])
         ex = {
             "src": ["Hello", ",", "world", "."],
             "tgt": ["Bonjour", "le", "monde", "."],
         }
         # 4. apply transform pipe for example
-        ex_after = transform_pipe.apply(
-            copy.deepcopy(ex), corpus_name="trainset"
-        )
+        ex_after = transform_pipe.apply(copy.deepcopy(ex), corpus_name="trainset")
         # 5. example after the pipe exceed the length limit, thus filtered
         self.assertIsNone(ex_after)
         # 6. Transform statistics registed (here for filtertoolong)
         self.assertTrue(len(transform_pipe.statistics.observables) > 0)
         msg = transform_pipe.statistics.report()
         self.assertIsNotNone(msg)
         # 7. after report, statistics become empty as a fresh start
         self.assertTrue(len(transform_pipe.statistics.observables) == 0)
 
 
 class TestMiscTransform(unittest.TestCase):
     def test_prefix(self):
         prefix_cls = get_transforms_cls(["prefix"])["prefix"]
-        corpora = yaml.safe_load("""
+        corpora = yaml.safe_load(
+            """
             trainset:
                 path_src: data/src-train.txt
                 path_tgt: data/tgt-train.txt
                 transforms: [prefix]
                 weight: 1
                 src_prefix: "｟_pf_src｠"
                 tgt_prefix: "｟_pf_tgt｠"
-        """)
+        """
+        )
         opt = Namespace(data=corpora, seed=-1)
         prefix_transform = prefix_cls(opt)
         prefix_transform.warm_up()
         self.assertIn("trainset", prefix_transform.prefix_dict)
 
         ex_in = {
             "src": ["Hello", "world", "."],
@@ -175,16 +177,27 @@
         }
         self.assertEqual(ex, ex_gold)
         # test BPE-dropout:
         bpe_transform.dropout["src"] = 1.0
         tokens = ["Another", "world", "."]
         gold_bpe = ["A@@", "no@@", "ther", "world", "."]
         gold_dropout = [
-            "A@@", "n@@", "o@@", "t@@", "h@@", "e@@", "r",
-            "w@@", "o@@", "r@@", "l@@", "d", ".",
+            "A@@",
+            "n@@",
+            "o@@",
+            "t@@",
+            "h@@",
+            "e@@",
+            "r",
+            "w@@",
+            "o@@",
+            "r@@",
+            "l@@",
+            "d",
+            ".",
         ]
         # 1. disable bpe dropout for not training example
         after_bpe = bpe_transform._tokenize(tokens, is_train=False)
         self.assertEqual(after_bpe, gold_bpe)
         # 2. enable bpe dropout for training example
         after_bpe = bpe_transform._tokenize(tokens, is_train=True)
         self.assertEqual(after_bpe, gold_dropout)
@@ -228,14 +241,15 @@
         onmttok_cls = get_transforms_cls(["onmt_tokenize"])["onmt_tokenize"]
         base_opt = copy.copy(self.base_opts)
         base_opt["src_subword_type"] = "bpe"
         base_opt["tgt_subword_type"] = "bpe"
         onmt_args = "{'mode': 'space', 'joiner_annotate': True}"
         base_opt["src_onmttok_kwargs"] = onmt_args
         base_opt["tgt_onmttok_kwargs"] = onmt_args
+        base_opt["gpt2_pretok"] = False
         opt = Namespace(**base_opt)
         onmttok_cls._validate_options(opt)
         onmttok_transform = onmttok_cls(opt)
         onmttok_transform.warm_up()
         ex = {
             "src": ["Hello", "world", "."],
             "tgt": ["Bonjour", "le", "monde", "."],
@@ -253,14 +267,15 @@
         base_opt["src_subword_type"] = "sentencepiece"
         base_opt["tgt_subword_type"] = "sentencepiece"
         base_opt["src_subword_model"] = "data/sample.sp.model"
         base_opt["tgt_subword_model"] = "data/sample.sp.model"
         onmt_args = "{'mode': 'none', 'spacer_annotate': True}"
         base_opt["src_onmttok_kwargs"] = onmt_args
         base_opt["tgt_onmttok_kwargs"] = onmt_args
+        base_opt["gpt2_pretok"] = False
         opt = Namespace(**base_opt)
         onmttok_cls._validate_options(opt)
         onmttok_transform = onmttok_cls(opt)
         onmttok_transform.warm_up()
         ex = {
             "src": ["Hello", "world", "."],
             "tgt": ["Bonjour", "le", "monde", "."],
@@ -513,47 +528,121 @@
 class TestFeaturesTransform(unittest.TestCase):
     def test_inferfeats(self):
         inferfeats_cls = get_transforms_cls(["inferfeats"])["inferfeats"]
         opt = Namespace(reversible_tokenization="joiner")
         inferfeats_transform = inferfeats_cls(opt)
 
         ex_in = {
-            "src": ['however', '￭,', 'according', 'to', 'the', 'logs',
-                    '￭,', 'she', 'is', 'hard', '￭-￭', 'working', '￭.'],
-            "src_original": ['however,', 'according', 'to', 'the',
-                             'logs,', 'she', 'is', 'hard-working.']
+            "src": [
+                "however",
+                "￭,",
+                "according",
+                "to",
+                "the",
+                "logs",
+                "￭,",
+                "she",
+                "is",
+                "hard",
+                "￭-￭",
+                "working",
+                "￭.",
+            ],
+            "src_original": [
+                "however,",
+                "according",
+                "to",
+                "the",
+                "logs,",
+                "she",
+                "is",
+                "hard-working.",
+            ],
         }
         ex_out = inferfeats_transform.apply(ex_in)
         self.assertIs(ex_out, ex_in)
 
         ex_in["src_feats"] = [["1", "2", "3", "4", "5", "6", "7", "8"]]
         ex_out = inferfeats_transform.apply(ex_in)
         self.assertEqual(
             ex_out["src_feats"][0],
-            ["1", "1", "2", "3", "4", "5", "5", "6", "7", "8", "8",
-             "8", "8"])
+            ["1", "1", "2", "3", "4", "5", "5", "6", "7", "8", "8", "8", "8"],
+        )
 
-        ex_in["src"] = ['｟mrk_case_modifier_C｠', 'however', '￭,',
-                        'according', 'to', 'the', 'logs', '￭,',
-                        '｟mrk_begin_case_region_U｠', 'she', 'is', 'hard',
-                        '￭-￭', 'working', '｟mrk_end_case_region_U｠', '￭.']
+        ex_in["src"] = [
+            "｟mrk_case_modifier_C｠",
+            "however",
+            "￭,",
+            "according",
+            "to",
+            "the",
+            "logs",
+            "￭,",
+            "｟mrk_begin_case_region_U｠",
+            "she",
+            "is",
+            "hard",
+            "￭-￭",
+            "working",
+            "｟mrk_end_case_region_U｠",
+            "￭.",
+        ]
         ex_in["src_feats"] = [["1", "2", "3", "4", "5", "6", "7", "8"]]
         ex_out = inferfeats_transform.apply(ex_in)
         self.assertEqual(
             ex_out["src_feats"][0],
-            ["1", "1", "1", "2", "3", "4", "5", "5",
-             "6", "6", "7", "8", "8", "8", "8", "8"])
+            [
+                "1",
+                "1",
+                "1",
+                "2",
+                "3",
+                "4",
+                "5",
+                "5",
+                "6",
+                "6",
+                "7",
+                "8",
+                "8",
+                "8",
+                "8",
+                "8",
+            ],
+        )
 
         ex_in = {
-            "src": ['however', '￭,', 'according', 'to', 'the', 'logs',
-                    '￭,', 'she', 'is', 'hard', '￭-￭', 'working', '￭.'],
-            "src_original": ['however', '￭,', 'according', 'to', 'the',
-                             'logs', '￭,', 'she', 'is', 'hard-working',
-                             '￭.'],
-            "src_feats": [["1", "2", "3", "4", "5", "6", "7", "8",
-                           "9", "10", "11"]]
+            "src": [
+                "however",
+                "￭,",
+                "according",
+                "to",
+                "the",
+                "logs",
+                "￭,",
+                "she",
+                "is",
+                "hard",
+                "￭-￭",
+                "working",
+                "￭.",
+            ],
+            "src_original": [
+                "however",
+                "￭,",
+                "according",
+                "to",
+                "the",
+                "logs",
+                "￭,",
+                "she",
+                "is",
+                "hard-working",
+                "￭.",
+            ],
+            "src_feats": [["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"]],
         }
         ex_out = inferfeats_transform.apply(ex_in)
         self.assertEqual(
             ex_out["src_feats"][0],
-            ["1", "2", "3", "4", "5", "6", "7", "8",
-             "9", "10", "10", "10", "11"])
+            ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "10", "10", "11"],
+        )
```

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_translation_server.py` & `OpenNMT-py-3.1.3/onmt/tests/test_translation_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,42 +51,54 @@
         with self.assertRaises(ValueError):
             sm.detokenize("hello world")
 
     def test_source_features(self):
         model_id = 0
         opt = {"models": ["test_model.pt"]}
         model_root = TEST_DIR
-        sm = ServerModel(opt, model_id, model_root=model_root, load=True,
-                         features_opt={
-                            "n_src_feats": 1,
-                            "src_feats_defaults": "0",
-                            "reversible_tokenization": "joiner"})
-        feats = sm.maybe_transform_feats("hello world.", "hello world ￭.",
-                                         ["0 1"])
+        sm = ServerModel(
+            opt,
+            model_id,
+            model_root=model_root,
+            load=True,
+            features_opt={
+                "n_src_feats": 1,
+                "src_feats_defaults": "0",
+                "reversible_tokenization": "joiner",
+            },
+        )
+        feats = sm.maybe_transform_feats("hello world.", "hello world ￭.", ["0 1"])
         self.assertEqual(feats, ["0 1 1"])
         preprocessed = sm.maybe_preprocess({"src": "hello￨0 world￨1"})
         self.assertEqual(preprocessed["seg"], ["hello world"])
         self.assertEqual(preprocessed["src_feats"], [["0 1"]])
 
     def test_passing_source_features_without_proper_configuration(self):
         model_id = 0
         opt = {"models": ["test_model.pt"]}
         model_root = TEST_DIR
         sm = ServerModel(opt, model_id, model_root=model_root, load=True)
         with self.assertRaises(AssertionError):
             sm.maybe_preprocess({"src": "hello￨0 world￨1"})
-        sm = ServerModel(opt, model_id, model_root=model_root, load=True,
-                         features_opt={
-                            "n_src_feats": 2,
-                            "src_feats_defaults": "0￨0",
-                            "reversible_tokenization": "joiner"})
+        sm = ServerModel(
+            opt,
+            model_id,
+            model_root=model_root,
+            load=True,
+            features_opt={
+                "n_src_feats": 2,
+                "src_feats_defaults": "0￨0",
+                "reversible_tokenization": "joiner",
+            },
+        )
         with self.assertRaises(AssertionError):
             sm.maybe_preprocess({"src": "hello￨0 world￨1"})
 
     if torch.cuda.is_available():
+
         def test_moving_to_gpu_and_back(self):
             torch.cuda.set_device(torch.device("cuda", 0))
             model_id = 0
             opt = {"models": ["test_model.pt"]}
             model_root = TEST_DIR
             sm = ServerModel(opt, model_id, model_root=model_root, load=True)
             for p in sm.translator.model.parameters():
@@ -113,21 +125,21 @@
                 self.assertEqual(p.device.type, "cuda")
                 self.assertEqual(p.device.index, 0)
             sm.to_cpu()
             for p in sm.translator.model.parameters():
                 self.assertEqual(p.device.type, "cpu")
 
         if torch.cuda.device_count() > 1:
+
             def test_initialize_on_nonzero_gpu_and_back(self):
                 torch.cuda.set_device(torch.device("cuda", 1))
                 model_id = 0
                 opt = {"models": ["test_model.pt"], "gpu": 1}
                 model_root = TEST_DIR
-                sm = ServerModel(opt, model_id, model_root=model_root,
-                                 load=True)
+                sm = ServerModel(opt, model_id, model_root=model_root, load=True)
                 for p in sm.translator.model.parameters():
                     self.assertEqual(p.device.type, "cuda")
                     self.assertEqual(p.device.index, 1)
                 sm.to_gpu()
                 for p in sm.translator.model.parameters():
                     self.assertEqual(p.device.type, "cuda")
                     self.assertEqual(p.device.index, 1)
@@ -136,16 +148,15 @@
                     self.assertEqual(p.device.type, "cpu")
 
     def test_run(self):
         model_id = 0
         opt = {"models": ["test_model.pt"]}
         model_root = TEST_DIR
         sm = ServerModel(opt, model_id, model_root=model_root, load=True)
-        inp = [{"src": "hello how are you today"},
-               {"src": "good morning to you ."}]
+        inp = [{"src": "hello how are you today"}, {"src": "good morning to you ."}]
         results, scores, n_best, time, aligns, align_scores = sm.run(inp)
         self.assertIsInstance(results, list)
         for sentence_string in results:
             self.assertIsInstance(sentence_string, str)
         self.assertIsInstance(scores, list)
         for elem in scores:
             self.assertIsInstance(elem, float)
@@ -165,26 +176,26 @@
         self.assertIn("translation", time)
 
 
 class TestTranslationServer(unittest.TestCase):
     # this could be considered an integration test because it touches
     # the filesystem for the config file (and the models)
 
-    CFG_F = os.path.join(
-        TEST_DIR, "test_translation_server_config_file.json")
+    CFG_F = os.path.join(TEST_DIR, "test_translation_server_config_file.json")
 
     def tearDown(self):
         if os.path.exists(self.CFG_F):
             os.remove(self.CFG_F)
 
     def write(self, cfg):
         with open(self.CFG_F, "w") as f:
             f.write(cfg)
 
-    CFG_NO_LOAD = dedent("""\
+    CFG_NO_LOAD = dedent(
+        """\
         {
             "models_root": "%s",
             "models": [
                 {
                     "id": 100,
                     "model": "test_model.pt",
                     "timeout": -1,
@@ -192,24 +203,27 @@
                     "load": false,
                     "opt": {
                         "beam_size": 5
                     }
                 }
             ]
         }
-        """ % TEST_DIR)
+        """
+        % TEST_DIR
+    )
 
     def test_start_without_initial_loading(self):
         self.write(self.CFG_NO_LOAD)
         sv = TranslationServer()
         sv.start(self.CFG_F)
         self.assertFalse(sv.models[100].loaded)
         self.assertEqual(set(sv.models.keys()), {100})
 
-    CFG_LOAD = dedent("""\
+    CFG_LOAD = dedent(
+        """\
         {
             "models_root": "%s",
             "models": [
                 {
                     "id": 100,
                     "model": "test_model.pt",
                     "timeout": -1,
@@ -217,24 +231,27 @@
                     "load": true,
                     "opt": {
                         "beam_size": 5
                     }
                 }
             ]
         }
-        """ % TEST_DIR)
+        """
+        % TEST_DIR
+    )
 
     def test_start_with_initial_loading(self):
         self.write(self.CFG_LOAD)
         sv = TranslationServer()
         sv.start(self.CFG_F)
         self.assertTrue(sv.models[100].loaded)
         self.assertEqual(set(sv.models.keys()), {100})
 
-    CFG_2_MODELS = dedent("""\
+    CFG_2_MODELS = dedent(
+        """\
         {
             "models_root": "%s",
             "models": [
                 {
                     "id": 100,
                     "model": "test_model.pt",
                     "timeout": -1,
@@ -252,15 +269,17 @@
                     "load": false,
                     "opt": {
                         "beam_size": 5
                     }
                 }
             ]
         }
-        """ % TEST_DIR)
+        """
+        % TEST_DIR
+    )
 
     def test_start_with_two_models(self):
         self.write(self.CFG_2_MODELS)
         sv = TranslationServer()
         sv.start(self.CFG_F)
         self.assertTrue(sv.models[100].loaded)
         self.assertFalse(sv.models[1000].loaded)
```

### Comparing `OpenNMT-py-3.1.2/onmt/tests/test_translator.py` & `OpenNMT-py-3.1.3/onmt/tests/test_translator.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,10 +27,8 @@
         (
             src,
             src_len,
             target_prefix,
         ) = GeneratorLM.split_src_to_prevent_padding(src, src_len)
         self.assertTupleEqual(src.shape, (6, new_length, 1))
         self.assertTupleEqual(target_prefix.shape, (6, 1, 1))
-        self.assertTrue(
-            src_len.equal(new_length * torch.ones(6, dtype=torch.int))
-        )
+        self.assertTrue(src_len.equal(new_length * torch.ones(6, dtype=torch.int)))
```

### Comparing `OpenNMT-py-3.1.2/onmt/train_single.py` & `OpenNMT-py-3.1.3/onmt/train_single.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 """Training on a single process."""
 import torch
 import sys
 
 from onmt.utils.logging import init_logger, logger
 from onmt.utils.parse import ArgumentParser
 from onmt.constants import CorpusTask
-from onmt.transforms import make_transforms, save_transforms, \
-    get_specials, get_transforms_cls
+from onmt.transforms import (
+    make_transforms,
+    save_transforms,
+    get_specials,
+    get_transforms_cls,
+)
 from onmt.inputters import build_vocab, IterOnDevice
-from onmt.inputters.inputter import dict_to_vocabs
+from onmt.inputters.inputter import dict_to_vocabs, vocabs_to_dict
 from onmt.inputters.dynamic_iterator import build_dynamic_dataset_iter
 from onmt.inputters.text_corpus import save_transformed_sample
 from onmt.model_builder import build_model
 from onmt.models.model_saver import load_checkpoint
 from onmt.utils.optimizers import Optimizer
 from onmt.utils.misc import set_random_seed
 from onmt.trainer import build_trainer
@@ -48,39 +52,48 @@
     if opt.dump_transforms or opt.n_sample != 0:
         transforms = make_transforms(opt, transforms_cls, vocabs)
     if opt.dump_transforms:
         save_transforms(transforms, opt.save_data, overwrite=opt.overwrite)
     if opt.n_sample != 0:
         logger.warning(
             "`-n_sample` != 0: Training will not be started. "
-            f"Stop after saving {opt.n_sample} samples/corpus.")
+            f"Stop after saving {opt.n_sample} samples/corpus."
+        )
         save_transformed_sample(opt, transforms, n_sample=opt.n_sample)
-        logger.info(
-            "Sample saved, please check it before restart training.")
+        logger.info("Sample saved, please check it before restart training.")
         sys.exit()
+    logger.info(
+        "The first 10 tokens of the vocabs are:"
+        f"{vocabs_to_dict(vocabs)['src'][0:10]}"
+    )
+    logger.info(f"The decoder start token is: {opt.decoder_start_token}")
     return vocabs, transforms_cls
 
 
 def _init_train(opt):
     """Common initilization stuff for all training process."""
     ArgumentParser.validate_prepare_opts(opt)
 
     if opt.train_from:
         # Load checkpoint if we resume from a previous training.
         checkpoint = load_checkpoint(ckpt_path=opt.train_from)
-        vocabs = dict_to_vocabs(checkpoint['vocab'])
+        vocabs = dict_to_vocabs(checkpoint["vocab"])
         transforms_cls = get_transforms_cls(opt._all_transform)
-        if (hasattr(checkpoint["opt"], '_all_transform') and
-                len(opt._all_transform.symmetric_difference(
-                    checkpoint["opt"]._all_transform)) != 0):
+        if (
+            hasattr(checkpoint["opt"], "_all_transform")
+            and len(
+                opt._all_transform.symmetric_difference(
+                    checkpoint["opt"]._all_transform
+                )
+            )
+            != 0
+        ):
             _msg = "configured transforms is different from checkpoint:"
-            new_transf = opt._all_transform.difference(
-                checkpoint["opt"]._all_transform)
-            old_transf = checkpoint["opt"]._all_transform.difference(
-                opt._all_transform)
+            new_transf = opt._all_transform.difference(checkpoint["opt"]._all_transform)
+            old_transf = checkpoint["opt"]._all_transform.difference(opt._all_transform)
             if len(new_transf) != 0:
                 _msg += f" +{new_transf}"
             if len(old_transf) != 0:
                 _msg += f" -{old_transf}."
             logger.warning(_msg)
             vocabs, transforms_cls = prepare_transforms_vocabs(opt)
         if opt.update_vocab:
@@ -104,52 +117,61 @@
     if checkpoint is not None:
         model_opt = ArgumentParser.ckpt_model_opts(checkpoint["opt"])
         if opt.override_opts:
             logger.info("Over-ride model option set to true - use with care")
             args = list(opt.__dict__.keys())
             model_args = list(model_opt.__dict__.keys())
             for arg in args:
-                if arg in model_args and \
-                        getattr(opt, arg) != getattr(model_opt, arg):
-                    logger.info("Option: %s , value: %s overiding model: %s"
-                                % (arg, getattr(opt, arg),
-                                   getattr(model_opt, arg)))
+                if arg in model_args and getattr(opt, arg) != getattr(model_opt, arg):
+                    logger.info(
+                        "Option: %s , value: %s overiding model: %s"
+                        % (arg, getattr(opt, arg), getattr(model_opt, arg))
+                    )
             model_opt = opt
         else:
             model_opt = ArgumentParser.ckpt_model_opts(checkpoint["opt"])
             ArgumentParser.update_model_opts(model_opt)
             ArgumentParser.validate_model_opts(model_opt)
-            if (opt.tensorboard_log_dir == model_opt.tensorboard_log_dir and
-                    hasattr(model_opt, 'tensorboard_log_dir_dated')):
+            if opt.tensorboard_log_dir == model_opt.tensorboard_log_dir and hasattr(
+                model_opt, "tensorboard_log_dir_dated"
+            ):
                 # ensure tensorboard output is written in the directory
                 # of previous checkpoints
-                opt.tensorboard_log_dir_dated = model_opt.tensorboard_log_dir_dated  # noqa: E501
+                opt.tensorboard_log_dir_dated = (
+                    model_opt.tensorboard_log_dir_dated
+                )  # noqa: E501
             # Override checkpoint's update_embeddings as it defaults to false
             model_opt.update_vocab = opt.update_vocab
             # Override checkpoint's freezing settings as it defaults to false
             model_opt.freeze_encoder = opt.freeze_encoder
             model_opt.freeze_decoder = opt.freeze_decoder
     else:
         model_opt = opt
     return model_opt
 
 
 def _build_valid_iter(opt, transforms_cls, vocabs):
     """Build iterator used for validation."""
     valid_iter = build_dynamic_dataset_iter(
-        opt, transforms_cls, vocabs, task=CorpusTask.VALID,
-        copy=opt.copy_attn)
+        opt, transforms_cls, vocabs, task=CorpusTask.VALID, copy=opt.copy_attn
+    )
     return valid_iter
 
 
 def _build_train_iter(opt, transforms_cls, vocabs, stride=1, offset=0):
     """Build training iterator."""
     train_iter = build_dynamic_dataset_iter(
-        opt, transforms_cls, vocabs, task=CorpusTask.TRAIN,
-        copy=opt.copy_attn, stride=stride, offset=offset)
+        opt,
+        transforms_cls,
+        vocabs,
+        task=CorpusTask.TRAIN,
+        copy=opt.copy_attn,
+        stride=stride,
+        offset=offset,
+    )
     return train_iter
 
 
 def main(opt, device_id):
     """Start training on `device_id`."""
     # NOTE: It's important that ``opt`` has been validated and updated
     # at this point.
@@ -160,49 +182,55 @@
     checkpoint, vocabs, transforms_cls = _init_train(opt)
     model_opt = _get_model_opts(opt, checkpoint=checkpoint)
 
     # Build model.
     model = build_model(model_opt, opt, vocabs, checkpoint)
 
     model.count_parameters(log=logger.info)
-    logger.info(' * src vocab size = %d' % len(vocabs['src']))
-    logger.info(' * tgt vocab size = %d' % len(vocabs['tgt']))
+    logger.info(" * src vocab size = %d" % len(vocabs["src"]))
+    logger.info(" * tgt vocab size = %d" % len(vocabs["tgt"]))
     if "src_feats" in vocabs:
         for i, feat_vocab in enumerate(vocabs["src_feats"]):
-            logger.info(f'* src_feat {i} vocab size = {len(feat_vocab)}')
+            logger.info(f"* src_feat {i} vocab size = {len(feat_vocab)}")
 
     # Build optimizer.
     optim = Optimizer.from_opt(model, opt, checkpoint=checkpoint)
 
     # Build model saver
     model_saver = build_model_saver(model_opt, opt, model, vocabs, optim)
 
     trainer = build_trainer(
-        opt, device_id, model, vocabs, optim, model_saver=model_saver)
+        opt, device_id, model, vocabs, optim, model_saver=model_saver
+    )
 
-    _train_iter = _build_train_iter(opt, transforms_cls, vocabs,
-                                    stride=max(1, len(opt.gpu_ranks)),
-                                    offset=max(0, device_id))
+    _train_iter = _build_train_iter(
+        opt,
+        transforms_cls,
+        vocabs,
+        stride=max(1, len(opt.gpu_ranks)),
+        offset=max(0, device_id),
+    )
     train_iter = IterOnDevice(_train_iter, device_id)
 
     valid_iter = _build_valid_iter(opt, transforms_cls, vocabs)
     if valid_iter is not None:
         valid_iter = IterOnDevice(valid_iter, device_id)
 
     if len(opt.gpu_ranks):
-        logger.info('Starting training on GPU: %s' % opt.gpu_ranks)
+        logger.info("Starting training on GPU: %s" % opt.gpu_ranks)
     else:
-        logger.info('Starting training on CPU, could be very slow')
+        logger.info("Starting training on CPU, could be very slow")
     train_steps = opt.train_steps
     if opt.single_pass and train_steps > 0:
         logger.warning("Option single_pass is enabled, ignoring train_steps.")
         train_steps = 0
 
     trainer.train(
         train_iter,
         train_steps,
         save_checkpoint_steps=opt.save_checkpoint_steps,
         valid_iter=valid_iter,
-        valid_steps=opt.valid_steps)
+        valid_steps=opt.valid_steps,
+    )
 
     if trainer.report_manager.tensorboard_writer is not None:
         trainer.report_manager.tensorboard_writer.close()
```

### Comparing `OpenNMT-py-3.1.2/onmt/trainer.py` & `OpenNMT-py-3.1.3/onmt/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 """
     This is the loadable seq2seq trainer library that is
     in charge of training details, loss compute, and statistics.
     See train.py for a use case of this library.
 
     Note: To make this a general library, we implement *only*
           mechanism things here(i.e. what to do), and leave the strategy
@@ -31,16 +30,16 @@
         optim (:obj:`onmt.utils.Optimizer`): optimizer used during training
         data_type (str): string describing the type of data
             e.g. "text"
         model_saver(:obj:`onmt.models.ModelSaverBase`): the utility object
             used to save the model
     """
 
-    train_loss = LossCompute.from_opts(opt, model, vocabs['tgt'])
-    valid_loss = LossCompute.from_opts(opt, model, vocabs['tgt'], train=False)
+    train_loss = LossCompute.from_opts(opt, model, vocabs["tgt"])
+    valid_loss = LossCompute.from_opts(opt, model, vocabs["tgt"], train=False)
 
     scoring_preparator = ScoringPreparator(vocabs=vocabs, opt=opt)
     validset_transforms = opt.data.get("valid", {}).get("transforms", None)
     if validset_transforms:
         scoring_preparator.warm_up(validset_transforms)
     scorers_cls = get_scorers_cls(opt.train_metrics)
     train_scorers = build_scorers(opt, scorers_cls)
@@ -59,35 +58,49 @@
     dropout_steps = opt.dropout_steps
     if device_id >= 0:
         gpu_rank = opt.gpu_ranks[device_id]
     else:
         gpu_rank = -1
         n_gpu = 0
 
-    earlystopper = onmt.utils.EarlyStopping(
-        opt.early_stopping, scorers=onmt.utils.scorers_from_opts(opt)) \
-        if opt.early_stopping > 0 else None
+    earlystopper = (
+        onmt.utils.EarlyStopping(
+            opt.early_stopping, scorers=onmt.utils.scorers_from_opts(opt)
+        )
+        if opt.early_stopping > 0
+        else None
+    )
 
     report_manager = onmt.utils.build_report_manager(opt, gpu_rank)
-    trainer = onmt.Trainer(model,
-                           train_loss, valid_loss,
-                           scoring_preparator, train_scorers, valid_scorers,
-                           optim, trunc_size, norm_method,
-                           accum_count, accum_steps,
-                           n_gpu, gpu_rank,
-                           opt.train_eval_steps, report_manager,
-                           with_align=True if opt.lambda_align > 0 else False,
-                           model_saver=model_saver if gpu_rank <= 0 else None,
-                           average_decay=average_decay,
-                           average_every=average_every,
-                           model_dtype=opt.model_dtype,
-                           earlystopper=earlystopper,
-                           dropout=dropout,
-                           attention_dropout=attention_dropout,
-                           dropout_steps=dropout_steps)
+    trainer = onmt.Trainer(
+        model,
+        train_loss,
+        valid_loss,
+        scoring_preparator,
+        train_scorers,
+        valid_scorers,
+        optim,
+        trunc_size,
+        norm_method,
+        accum_count,
+        accum_steps,
+        n_gpu,
+        gpu_rank,
+        opt.train_eval_steps,
+        report_manager,
+        with_align=True if opt.lambda_align > 0 else False,
+        model_saver=model_saver if gpu_rank <= 0 else None,
+        average_decay=average_decay,
+        average_every=average_every,
+        model_dtype=opt.model_dtype,
+        earlystopper=earlystopper,
+        dropout=dropout,
+        attention_dropout=attention_dropout,
+        dropout_steps=dropout_steps,
+    )
     return trainer
 
 
 class Trainer(object):
     """Class that controls the training process.
 
     Args:
@@ -124,27 +137,41 @@
         model_dtype (str): fp32 or fp16.
         earlystopper (:obj:`onmt.utils.EarlyStopping`): add early
           stopping mecanism
         dropout (float): dropout value in RNN or FF layers.
         attention_dropout (float): dropaout in attention layers.
         dropout_steps (list): dropout values scheduling in steps."""
 
-    def __init__(self, model, train_loss, valid_loss,
-                 scoring_preparator, train_scorers, valid_scorers,
-                 optim,
-                 trunc_size=0,
-                 norm_method='sents',
-                 accum_count=[1],
-                 accum_steps=[0],
-                 n_gpu=1, gpu_rank=1,
-                 train_eval_steps=200,
-                 report_manager=None, with_align=False, model_saver=None,
-                 average_decay=0, average_every=1, model_dtype='fp32',
-                 earlystopper=None, dropout=[0.3], attention_dropout=[0.1],
-                 dropout_steps=[0]):
+    def __init__(
+        self,
+        model,
+        train_loss,
+        valid_loss,
+        scoring_preparator,
+        train_scorers,
+        valid_scorers,
+        optim,
+        trunc_size=0,
+        norm_method="sents",
+        accum_count=[1],
+        accum_steps=[0],
+        n_gpu=1,
+        gpu_rank=1,
+        train_eval_steps=200,
+        report_manager=None,
+        with_align=False,
+        model_saver=None,
+        average_decay=0,
+        average_every=1,
+        model_dtype="fp32",
+        earlystopper=None,
+        dropout=[0.3],
+        attention_dropout=[0.1],
+        dropout_steps=[0],
+    ):
         # Basic attributes.
 
         self.model = model
         self.train_loss = train_loss
         self.valid_loss = valid_loss
 
         self.scoring_preparator = scoring_preparator
@@ -194,61 +221,65 @@
             if step > self.accum_steps[i]:
                 _accum = self.accum_count_l[i]
         return _accum
 
     def _maybe_update_dropout(self, step):
         for i in range(len(self.dropout_steps)):
             if step > 1 and step == self.dropout_steps[i] + 1:
-                self.model.update_dropout(self.dropout[i],
-                                          self.attention_dropout[i])
-                logger.info("Updated dropout/attn dropout to %f %f at step %d"
-                            % (self.dropout[i],
-                               self.attention_dropout[i], step))
+                self.model.update_dropout(self.dropout[i], self.attention_dropout[i])
+                logger.info(
+                    "Updated dropout/attn dropout to %f %f at step %d"
+                    % (self.dropout[i], self.attention_dropout[i], step)
+                )
 
     def _accum_batches(self, iterator):
         batches = []
         normalization = 0
         self.accum_count = self._accum_count(self.optim.training_step)
         for batch in iterator:
             batches.append(batch)
             if self.norm_method == "tokens":
-                num_tokens = batch['tgt'][:, 1:, 0].ne(
-                    self.train_loss.padding_idx).sum()
+                num_tokens = (
+                    batch["tgt"][:, 1:, 0].ne(self.train_loss.padding_idx).sum()
+                )
                 normalization += num_tokens.item()
-                normalization -= len(batch['tgt'])  # don't count for EOS
+                normalization -= len(batch["tgt"])  # don't count for EOS
             else:
-                normalization += len(batch['tgt'])
+                normalization += len(batch["tgt"])
             if len(batches) == self.accum_count:
                 yield batches, normalization
                 self.accum_count = self._accum_count(self.optim.training_step)
                 batches = []
                 normalization = 0
         if batches:
             yield batches, normalization
 
     def _update_average(self, step):
         if self.moving_average is None:
-            copy_params = [params.detach().float()
-                           for params in self.model.parameters()]
+            copy_params = [
+                params.detach().float() for params in self.model.parameters()
+            ]
             self.moving_average = copy_params
         else:
-            average_decay = max(self.average_decay,
-                                1 - (step + 1) / (step + 10))
-            for (i, avg), cpt in zip(enumerate(self.moving_average),
-                                     self.model.parameters()):
-                self.moving_average[i] = \
-                    (1 - average_decay) * avg + \
-                    cpt.detach().float() * average_decay
-
-    def train(self,
-              train_iter,
-              train_steps,
-              save_checkpoint_steps=5000,
-              valid_iter=None,
-              valid_steps=10000):
+            average_decay = max(self.average_decay, 1 - (step + 1) / (step + 10))
+            for (i, avg), cpt in zip(
+                enumerate(self.moving_average), self.model.parameters()
+            ):
+                self.moving_average[i] = (
+                    1 - average_decay
+                ) * avg + cpt.detach().float() * average_decay
+
+    def train(
+        self,
+        train_iter,
+        train_steps,
+        save_checkpoint_steps=5000,
+        valid_iter=None,
+        valid_steps=10000,
+    ):
         """The main training loop by iterating over ``train_iter`` and possibly
         running validation on ``valid_iter``.
 
         Args:
             train_iter: An iterator that returns the next training batch.
             train_steps: Run training for this many iterations.
             save_checkpoint_steps: Save a checkpoint every this many
@@ -256,72 +287,77 @@
             valid_iter: A generator that returns the next validation batch.
             valid_steps: Run evaluation every this many iterations.
 
         Returns:
             :obj:``nmt.Statistics``: training loss statistics"""
 
         if valid_iter is None:
-            logger.info('Start training loop without validation...')
+            logger.info("Start training loop without validation...")
             valid_stats = None
         else:
-            logger.info('Start training loop and validate every %d steps...',
-                        valid_steps)
-        logger.info(
-            "Scoring with: {}".format(self.scoring_preparator.transform))
+            logger.info(
+                "Start training loop and validate every %d steps...", valid_steps
+            )
+        logger.info("Scoring with: {}".format(self.scoring_preparator.transform))
 
         total_stats = onmt.utils.Statistics()
         report_stats = onmt.utils.Statistics()
         self._start_report_manager(start_time=total_stats.start_time)
         # Let's clean the GPUs before training loop
         torch.cuda.empty_cache()
 
-        for i, (batches, normalization) in enumerate(
-                self._accum_batches(train_iter)):
+        for i, (batches, normalization) in enumerate(self._accum_batches(train_iter)):
             step = self.optim.training_step
             # UPDATE DROPOUT
             self._maybe_update_dropout(step)
 
             if self.n_gpu > 1:
-                normalization = sum(onmt.utils.distributed
-                                    .all_gather_list
-                                    (normalization))
+                normalization = sum(
+                    onmt.utils.distributed.all_gather_list(normalization)
+                )
 
             self._gradient_accumulation(
-                batches, normalization, total_stats,
-                report_stats)
+                batches, normalization, total_stats, report_stats
+            )
 
             if self.average_decay > 0 and i % self.average_every == 0:
                 self._update_average(step)
 
             report_stats = self._maybe_report_training(
-                step, train_steps,
-                self.optim.learning_rate(),
-                report_stats)
+                step, train_steps, self.optim.learning_rate(), report_stats
+            )
 
-            if (valid_iter is not None and step % valid_steps == 0 and
-                    self.gpu_rank <= 0):
+            if (
+                valid_iter is not None
+                and step % valid_steps == 0
+                and self.gpu_rank <= 0
+            ):
                 valid_stats = self.validate(
-                    valid_iter, moving_average=self.moving_average)
+                    valid_iter, moving_average=self.moving_average
+                )
 
             if step % valid_steps == 0 and self.gpu_rank <= 0:
-                self._report_step(self.optim.learning_rate(),
-                                  step, valid_stats=valid_stats,
-                                  train_stats=total_stats)
+                self._report_step(
+                    self.optim.learning_rate(),
+                    step,
+                    valid_stats=valid_stats,
+                    train_stats=total_stats,
+                )
 
                 # Run patience mechanism
                 if self.earlystopper is not None:
                     self.earlystopper(valid_stats, step)
                     # If the patience has reached the limit, stop training
                     if self.earlystopper.has_stopped():
                         logger.info("earlystopper has_stopped!")
                         break
 
-            if (self.model_saver is not None
-                    and (save_checkpoint_steps != 0
-                         and step % save_checkpoint_steps == 0)):
+            if self.model_saver is not None and (
+                save_checkpoint_steps != 0 and step % save_checkpoint_steps == 0
+            ):
                 self.model_saver.save(step, moving_average=self.moving_average)
 
             if train_steps > 0 and step >= train_steps:
                 break
 
         if self.model_saver is not None:
             self.model_saver.save(step, moving_average=self.moving_average)
@@ -337,231 +373,252 @@
             :obj:``nmt.Statistics``: validation loss statistics"""
 
         valid_model = self.model
         if moving_average:
             # swap model params w/ moving average
             # (and keep the original parameters)
             model_params_data = []
-            for avg, param in zip(self.moving_average,
-                                  valid_model.parameters()):
+            for avg, param in zip(self.moving_average, valid_model.parameters()):
                 model_params_data.append(param.data)
-                param.data = avg.data.half() if param.dtype == torch.float16 \
-                    else avg.data
+                param.data = (
+                    avg.data.half() if param.dtype == torch.float16 else avg.data
+                )
 
         # Set model in validating mode.
         valid_model.eval()
 
         transformed_batches = []
         with torch.no_grad():
             stats = onmt.utils.Statistics()
             start = time.time()
             for batch in valid_iter:
-                src = batch['src']
-                src_len = batch['srclen']
-                tgt = batch['tgt']
+                src = batch["src"]
+                src_len = batch["srclen"]
+                tgt = batch["tgt"]
                 if self.valid_scorers:
-                    transformed_batch = self.scoring_preparator.\
-                        ids_to_tokens_batch(batch)
+                    transformed_batch = self.scoring_preparator.ids_to_tokens_batch(
+                        batch
+                    )
                     transformed_batches.append(transformed_batch)
                 with torch.cuda.amp.autocast(enabled=self.optim.amp):
                     # F-prop through the model.
-                    model_out, attns = valid_model(src, tgt, src_len,
-                                                   with_align=self.with_align)
+                    model_out, attns = valid_model(
+                        src, tgt, src_len, with_align=self.with_align
+                    )
 
                     # Compute loss.
                     _, batch_stats = self.valid_loss(batch, model_out, attns)
 
                     stats.update(batch_stats)
-            logger.info("""valid stats calculation and sentences rebuilding
-                           took: {} s.""".format(time.time() - start))
+            logger.info(
+                """valid stats calculation and sentences rebuilding
+                           took: {} s.""".format(
+                    time.time() - start
+                )
+            )
 
             # Compute validation metrics (at batch.dataset level)
             if len(self.valid_scorers) > 0:
                 computed_metrics = {}
                 start = time.time()
                 preds, texts_ref = self.scoring_preparator.translate(
                     model=self.model,
                     transformed_batches=transformed_batches,
                     gpu_rank=self.gpu_rank,
                     step=self.optim.training_step,
-                    mode="valid")
-                logger.info("""The translation of the valid dataset
-                               took : {} s.""".format(time.time() - start))
+                    mode="valid",
+                )
+                logger.info(
+                    """The translation of the valid dataset
+                               took : {} s.""".format(
+                        time.time() - start
+                    )
+                )
             for i, metric in enumerate(self.valid_scorers):
                 logger.info("UPDATING VALIDATION {}".format(metric))
-                self.valid_scorers[
-                    metric]["value"] = self._training_eval_handler(
-                        scorer=self.valid_scorers[metric]["scorer"],
-                        preds=preds,
-                        texts_ref=texts_ref)
-                computed_metrics[
-                    metric] = self.valid_scorers[metric]["value"]
+                self.valid_scorers[metric]["value"] = self._training_eval_handler(
+                    scorer=self.valid_scorers[metric]["scorer"],
+                    preds=preds,
+                    texts_ref=texts_ref,
+                )
+                computed_metrics[metric] = self.valid_scorers[metric]["value"]
                 logger.info(
                     "validation {}: {}".format(
-                        metric, self.valid_scorers[metric]["value"])
-                        )
+                        metric, self.valid_scorers[metric]["value"]
+                    )
+                )
                 # Compute stats
-                metric_stats = onmt.utils.Statistics(
-                    0, 0, 0, 0, 0,
-                    computed_metrics)
+                metric_stats = onmt.utils.Statistics(0, 0, 0, 0, 0, computed_metrics)
 
                 # Update statistics.
                 stats.update(metric_stats)
 
         if moving_average:
-            for param_data, param in zip(model_params_data,
-                                         self.model.parameters()):
+            for param_data, param in zip(model_params_data, self.model.parameters()):
                 param.data = param_data
 
         # Set model back to training mode.
         valid_model.train()
 
         return stats
 
-    def _gradient_accumulation(self, true_batches, normalization, total_stats,
-                               report_stats):
+    def _gradient_accumulation(
+        self, true_batches, normalization, total_stats, report_stats
+    ):
         """Function that iterates over big batches = ``true_batches``
 
         Perform a backward on the loss of each sub_batch and
         finally update the params at the end of the big batch."""
 
         if self.accum_count > 1:
             self.optim.zero_grad(set_to_none=True)
 
         for k, batch in enumerate(true_batches):
-            target_size = batch['tgt'].size(1)
+            target_size = batch["tgt"].size(1)
             # Truncated BPTT: reminder not compatible with accum > 1
             if self.trunc_size:
                 trunc_size = self.trunc_size
             else:
                 trunc_size = target_size
 
-            src = batch['src']
-            src_len = batch['srclen']
+            src = batch["src"]
+            src_len = batch["srclen"]
             if src_len is not None:
                 report_stats.n_src_words += src_len.sum().item()
                 total_stats.n_src_words += src_len.sum().item()
 
-            tgt_outer = batch['tgt']
+            tgt_outer = batch["tgt"]
 
             bptt = False
             for j in range(0, target_size - 1, trunc_size):
                 # 1. Create truncated target.
 
-                tgt = tgt_outer[:, j: j + trunc_size, :]
+                tgt = tgt_outer[:, j : j + trunc_size, :]
 
                 # 2. F-prop all but generator.
                 if self.accum_count == 1:
                     self.optim.zero_grad(set_to_none=True)
 
                 try:
                     with torch.cuda.amp.autocast(enabled=self.optim.amp):
                         model_out, attns = self.model(
-                            src, tgt, src_len, bptt=bptt,
-                            with_align=self.with_align)
+                            src, tgt, src_len, bptt=bptt, with_align=self.with_align
+                        )
                         bptt = True
 
                         # 3. Compute loss.
                         loss, batch_stats = self.train_loss(
                             batch,
                             model_out,
                             attns,
                             trunc_start=j,
-                            trunc_size=trunc_size)
+                            trunc_size=trunc_size,
+                        )
 
                     step = self.optim.training_step
-                    if (
-                           self.train_scorers != {} and
-                           step % self.train_eval_steps == 0
-                    ):
+                    if self.train_scorers != {} and step % self.train_eval_steps == 0:
                         # Compute and save stats
                         computed_metrics = {}
-                        transformed_batch = self.scoring_preparator.\
-                            ids_to_tokens_batch(batch)
+                        transformed_batch = self.scoring_preparator.ids_to_tokens_batch(
+                            batch
+                        )
                         preds, texts_ref = self.scoring_preparator.translate(
                             model=self.model,
                             transformed_batches=[transformed_batch],
                             gpu_rank=self.gpu_rank,
                             step=self.optim.training_step,
-                            mode="train")
+                            mode="train",
+                        )
                         for i, metric in enumerate(self.train_scorers):
                             logger.info("UPDATING TRAINING {}".format(metric))
-                            self.train_scorers[
-                                metric]["value"] = self._training_eval_handler(
-                                scorer=self.train_scorers[
-                                    metric]["scorer"],
+                            self.train_scorers[metric][
+                                "value"
+                            ] = self._training_eval_handler(
+                                scorer=self.train_scorers[metric]["scorer"],
                                 preds=preds,
-                                texts_ref=texts_ref)
+                                texts_ref=texts_ref,
+                            )
                             logger.info(
                                 "training {}: {}".format(
-                                    metric, self.train_scorers[
-                                        metric]["value"]))
-                            computed_metrics[
-                                metric] = self.train_scorers[metric]["value"]
+                                    metric, self.train_scorers[metric]["value"]
+                                )
+                            )
+                            computed_metrics[metric] = self.train_scorers[metric][
+                                "value"
+                            ]
                         batch_stats.computed_metrics = computed_metrics
 
                     if loss is not None:
                         loss /= normalization
                         self.optim.backward(loss)
 
                     total_stats.update(batch_stats)
                     report_stats.update(batch_stats)
 
                 except Exception as exc:
                     trace_content = traceback.format_exc()
                     if "CUDA out of memory" in trace_content:
-                        logger.info("Step %d, cuda OOM - batch removed",
-                                    self.optim.training_step)
+                        logger.info(
+                            "Step %d, cuda OOM - batch removed",
+                            self.optim.training_step,
+                        )
                         torch.cuda.empty_cache()
                     else:
                         traceback.print_exc()
                         raise exc
 
                 # If truncated, don't backprop fully.
                 if self.model.decoder.state != {}:
                     self.model.decoder.detach_state()
 
         # in case of multi step gradient accumulation,
         # update only after accum batches
         if self.n_gpu > 1:
-            grads = [p.grad.data for p in self.model.parameters()
-                     if p.requires_grad
-                     and p.grad is not None]
+            grads = [
+                p.grad.data
+                for p in self.model.parameters()
+                if p.requires_grad and p.grad is not None
+            ]
             onmt.utils.distributed.all_reduce_and_rescale_tensors(
-                grads, float(self.n_gpu))
+                grads, float(self.n_gpu)
+            )
         self.optim.step()
 
     def _start_report_manager(self, start_time=None):
         """Simple function to start report manager (if any)"""
 
         if self.report_manager is not None:
             if start_time is None:
                 self.report_manager.start()
             else:
                 self.report_manager.start_time = start_time
 
-    def _maybe_report_training(self, step, num_steps, learning_rate,
-                               report_stats):
+    def _maybe_report_training(self, step, num_steps, learning_rate, report_stats):
         """Simple function to report training stats (if report_manager is set)
         see ``onmt.utils.ReportManagerBase.report_training`` for doc"""
 
         if self.report_manager is not None:
             return self.report_manager.report_training(
                 step,
                 num_steps,
                 learning_rate,
-                None if self.earlystopper is None
+                None
+                if self.earlystopper is None
                 else self.earlystopper.current_tolerance,
                 report_stats,
-                multigpu=self.n_gpu > 1)
+                multigpu=self.n_gpu > 1,
+            )
 
-    def _report_step(self, learning_rate, step,
-                     valid_stats=None, train_stats=None):
+    def _report_step(self, learning_rate, step, valid_stats=None, train_stats=None):
         """Simple function to report stats (if report_manager is set)
         see ``onmt.utils.ReportManagerBase.report_step`` for doc"""
 
         if self.report_manager is not None:
             return self.report_manager.report_step(
                 learning_rate,
-                None if self.earlystopper is None
+                None
+                if self.earlystopper is None
                 else self.earlystopper.current_tolerance,
-                step, valid_stats=valid_stats, train_stats=train_stats)
+                step,
+                valid_stats=valid_stats,
+                train_stats=train_stats,
+            )
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/__init__.py` & `OpenNMT-py-3.1.3/onmt/transforms/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Module for dynamic data transfrom."""
 import os
 import importlib
 
-from .transform import make_transforms, get_specials,\
-    save_transforms, load_transforms, TransformPipe,\
-    Transform
+from .transform import (
+    make_transforms,
+    get_specials,
+    save_transforms,
+    load_transforms,
+    TransformPipe,
+    Transform,
+)
 
 
 AVAILABLE_TRANSFORMS = {}
 
 
 def get_transforms_cls(transform_names):
     """Return valid transform class indicated in `transform_names`."""
@@ -16,37 +21,45 @@
     for name in transform_names:
         if name not in AVAILABLE_TRANSFORMS:
             raise ValueError("%s transform not supported!" % name)
         transforms_cls[name] = AVAILABLE_TRANSFORMS[name]
     return transforms_cls
 
 
-__all__ = ["get_transforms_cls", "get_specials", "make_transforms",
-           "load_transforms", "save_transforms", "TransformPipe",
-           "prepare_transforms"]
+__all__ = [
+    "get_transforms_cls",
+    "get_specials",
+    "make_transforms",
+    "load_transforms",
+    "save_transforms",
+    "TransformPipe",
+    "prepare_transforms",
+]
 
 
 def register_transform(name):
     """Transform register that can be used to add new transform class."""
 
     def register_transfrom_cls(cls):
         if name in AVAILABLE_TRANSFORMS:
-            raise ValueError(
-                'Cannot register duplicate transform ({})'.format(name))
+            raise ValueError("Cannot register duplicate transform ({})".format(name))
         if not issubclass(cls, Transform):
-            raise ValueError('transform ({}: {}) must extend Transform'.format(
-                name, cls.__name__))
+            raise ValueError(
+                "transform ({}: {}) must extend Transform".format(name, cls.__name__)
+            )
         AVAILABLE_TRANSFORMS[name] = cls
         return cls
 
     return register_transfrom_cls
 
 
 # Auto import python files in this directory
 transform_dir = os.path.dirname(__file__)
 for file in os.listdir(transform_dir):
     path = os.path.join(transform_dir, file)
-    if not file.startswith('_') and not file.startswith('.') and (
-            file.endswith('.py') or os.path.isdir(path)):
-        file_name = file[:file.find('.py')] if file.endswith('.py') else file
-        module = importlib.import_module(
-            'onmt.transforms.' + file_name)
+    if (
+        not file.startswith("_")
+        and not file.startswith(".")
+        and (file.endswith(".py") or os.path.isdir(path))
+    ):
+        file_name = file[: file.find(".py")] if file.endswith(".py") else file
+        module = importlib.import_module("onmt.transforms." + file_name)
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/bart.py` & `OpenNMT-py-3.1.3/onmt/transforms/bart.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """Find word start in a subword list marked by joiner."""
     flag = [True] * len(tokens)
     for i, token in enumerate(tokens):
         if token.startswith(SubwordMarker.JOINER) and i != 0:
             flag[i] = False
         if token.endswith(SubwordMarker.JOINER):
             try:
-                flag[i+1] = False
+                flag[i + 1] = False
             except IndexError:
                 print("Sentence `{}` not correct!".format(" ".join(token)))
                 raise
     return flag
 
 
 def _subword_start_by_spacer(tokens: Sequence[str]) -> Sequence[bool]:
@@ -41,19 +41,29 @@
     else:
         return lambda tokens: [True] * len(tokens)
 
 
 class BARTNoising(object):
     """Noise from BART."""
 
-    def __init__(self, vocab, mask_tok=DefaultTokens.MASK, mask_ratio=0.0,
-                 insert_ratio=0.0, permute_sent_ratio=0.0, poisson_lambda=3.0,
-                 replace_length=-1, rotate_ratio=0.0, mask_length='subword',
-                 random_ratio=0.0, is_joiner=False,
-                 full_stop_token=DefaultTokens.SENT_FULL_STOPS):
+    def __init__(
+        self,
+        vocab,
+        mask_tok=DefaultTokens.MASK,
+        mask_ratio=0.0,
+        insert_ratio=0.0,
+        permute_sent_ratio=0.0,
+        poisson_lambda=3.0,
+        replace_length=-1,
+        rotate_ratio=0.0,
+        mask_length="subword",
+        random_ratio=0.0,
+        is_joiner=False,
+        full_stop_token=DefaultTokens.SENT_FULL_STOPS,
+    ):
         if vocab is None:
             raise ValueError("Inject BART noise requires a valid vocabulary.")
         self.vocab = vocab
 
         self.mask_tok = mask_tok
 
         self.mask_ratio = mask_ratio
@@ -64,30 +74,30 @@
 
         self.full_stop_token = full_stop_token
 
         # -1: keep everything (i.e. 1 mask per token)
         #  0: replace everything (i.e. no mask)
         #  1: 1 mask per span
         if replace_length not in [-1, 0, 1]:
-            raise ValueError(f'invalid arg: replace_length={replace_length}')
+            raise ValueError(f"invalid arg: replace_length={replace_length}")
         self.replace_length = replace_length
 
-        if mask_length not in ['subword', 'word', 'span-poisson']:
-            raise ValueError(f'invalid arg: mask-length={mask_length}')
-        if mask_length == 'subword' and replace_length not in [0, 1]:
-            raise ValueError('if using subwords, use replace-length=1 or 0')
+        if mask_length not in ["subword", "word", "span-poisson"]:
+            raise ValueError(f"invalid arg: mask-length={mask_length}")
+        if mask_length == "subword" and replace_length not in [0, 1]:
+            raise ValueError("if using subwords, use replace-length=1 or 0")
 
-        if mask_length == 'subword' or is_joiner is None:
+        if mask_length == "subword" or is_joiner is None:
             # view each subword as word start / input is word level token
             self._is_word_start = word_start_finder(ignore_subword=True)
         else:
             self._is_word_start = word_start_finder(is_joiner=is_joiner)
 
         self.mask_span_distribution = None
-        if mask_length == 'span-poisson':
+        if mask_length == "span-poisson":
             self.mask_span_distribution = self._make_poisson(poisson_lambda)
         self.mask_length = mask_length
         self.poisson_lambda = poisson_lambda
 
     @staticmethod
     def set_random_seed(seed):
         """Call this before use to ensure reproducibility."""
@@ -98,27 +108,24 @@
         lambda_to_the_k = 1
         e_to_the_minus_lambda = math.exp(-poisson_lambda)
         k_factorial = 1
         ps = []
         for k in range(0, 128):
             ps.append(e_to_the_minus_lambda * lambda_to_the_k / k_factorial)
             lambda_to_the_k *= poisson_lambda
-            k_factorial *= (k + 1)
+            k_factorial *= k + 1
             if ps[-1] < 0.0000001:
                 break
         ps = torch.FloatTensor(ps)
         return torch.distributions.Categorical(ps)
 
     def _get_sentence_borders(self, tokens):
         """Return lengths of each sentence in the token sequence."""
         full_stops = np.array(
-            [
-                True if token in self.full_stop_token else False
-                for token in tokens
-            ]
+            [True if token in self.full_stop_token else False for token in tokens]
         )
         # Pretend it ends with a full stop so last span is a sentence
         full_stops[-1] = True
         # Tokens that are full stops, where the previous token is not
         sentence_lens = (full_stops[1:] * ~full_stops[:-1]).nonzero()[0] + 2
         return sentence_lens
 
@@ -130,46 +137,45 @@
         if n_sentences == 1:
             return tokens
 
         n_to_permute = math.ceil((n_sentences * 2 * p) / 2.0)
 
         substitutions = np.random.permutation(n_sentences)[:n_to_permute]
         ordering = np.arange(0, n_sentences)
-        ordering[substitutions] = substitutions[np.random.permutation(
-            n_to_permute)]
+        ordering[substitutions] = substitutions[np.random.permutation(n_to_permute)]
 
         result = [tok for tok in tokens]
         index = 0
         for i in ordering:
-            sentence = tokens[(sentence_lens[i - 1] if i > 0 else 0):
-                              sentence_lens[i]]
-            result[index:index + len(sentence)] = sentence
+            sentence = tokens[(sentence_lens[i - 1] if i > 0 else 0) : sentence_lens[i]]
+            result[index : index + len(sentence)] = sentence
             index += len(sentence)
         assert len(result) == len(tokens), "Error when permute sentences."
         return result
 
     def whole_word_mask(self, tokens, p=1.0):  # text span mask/infilling
         is_word_start = torch.tensor(self._is_word_start(tokens)).int()
         n_mask = int(math.ceil(is_word_start.sum() * p))
         n_insert = 0
         if n_mask == 0:
             return tokens
 
         if self.mask_span_distribution is not None:  # Text (span) Infilling
-            lengths = self.mask_span_distribution.sample(
-                sample_shape=(n_mask,))
+            lengths = self.mask_span_distribution.sample(sample_shape=(n_mask,))
 
             # Make sure we have enough to mask
             cum_length = torch.cumsum(lengths, 0)
             while cum_length[-1] < n_mask:
-                lengths = torch.cat([
-                    lengths,
-                    self.mask_span_distribution.sample(
-                        sample_shape=(n_mask,))
-                ], dim=0)
+                lengths = torch.cat(
+                    [
+                        lengths,
+                        self.mask_span_distribution.sample(sample_shape=(n_mask,)),
+                    ],
+                    dim=0,
+                )
                 cum_length = torch.cumsum(lengths, 0)
 
             # Trim to masking budget
             i = 0
             while cum_length[i] < n_mask:
                 i += 1
             lengths[i] = n_mask - (0 if i == 0 else cum_length[i - 1])
@@ -184,36 +190,35 @@
                 return self.insertion_noise(tokens, n_insert / len(tokens))
 
             assert (lengths > 0).all()
         else:  # Token Masking
             lengths = torch.ones((n_mask,)).long()
         # assert is_word_start[-1] == 0
         word_starts = is_word_start.nonzero(as_tuple=False)
-        indices = word_starts[
-            torch.randperm(word_starts.size(0))[:n_mask]
-        ].squeeze(1)
+        indices = word_starts[torch.randperm(word_starts.size(0))[:n_mask]].squeeze(1)
         mask_random = torch.FloatTensor(n_mask).uniform_() < self.random_ratio
 
         tokens_length = len(tokens)
         # assert tokens_length - 1 not in indices
         to_keep = torch.ones(tokens_length, dtype=torch.bool)
 
         if self.replace_length == 0:
             to_keep[indices] = 0
         else:
             # keep index, but replace it with [MASK]
             for i in indices.tolist():
                 tokens[i] = self.mask_tok
             random_tok_ids = torch.randint(
-                0, len(self.vocab), size=(mask_random.sum(),)).tolist()
+                0, len(self.vocab), size=(mask_random.sum(),)
+            ).tolist()
             for i, rid in zip(indices[mask_random].tolist(), random_tok_ids):
                 tokens[i] = self.vocab[rid]
 
         if tokens_length - 1 in indices:
-            uncompleted = (indices != tokens_length - 1)
+            uncompleted = indices != tokens_length - 1
             indices = indices[uncompleted]
             mask_random = mask_random[uncompleted]
             lengths = lengths[uncompleted]
 
         # acts as a long length, so spans don't go over the end of doc
         is_word_start[-1] = 255
 
@@ -233,17 +238,17 @@
                     # delete token: 1 mask/remove per span
                     to_keep[indices] = 0
                 else:
                     # keep index, but replace it with [MASK]: 1 mask per token
                     for i in indices.tolist():
                         tokens[i] = self.mask_tok
                     random_tok_ids = torch.randint(
-                        0, len(self.vocab), size=(mask_random.sum(),)).tolist()
-                    for i, rid in zip(
-                            indices[mask_random].tolist(), random_tok_ids):
+                        0, len(self.vocab), size=(mask_random.sum(),)
+                    ).tolist()
+                    for i, rid in zip(indices[mask_random].tolist(), random_tok_ids):
                         tokens[i] = self.vocab[rid]
         else:
             # A bit faster when all lengths are 1
             while indices.size(0) > 0:
                 # to cover whole token
                 uncompleted = is_word_start[indices + 1] == 0
                 indices = indices[uncompleted] + 1
@@ -252,23 +257,22 @@
                     # delete token
                     to_keep[indices] = 0
                 else:
                     # keep index, but replace it with [MASK]
                     for i in indices.tolist():
                         tokens[i] = self.mask_tok
                     random_tok_ids = torch.randint(
-                        0, len(self.vocab), size=(mask_random.sum(),)).tolist()
-                    for i, rid in zip(
-                            indices[mask_random].tolist(), random_tok_ids):
+                        0, len(self.vocab), size=(mask_random.sum(),)
+                    ).tolist()
+                    for i, rid in zip(indices[mask_random].tolist(), random_tok_ids):
                         tokens[i] = self.vocab[rid]
 
                 # assert tokens_length - 1 not in indices
 
-        tokens = [tok for tok, keep in zip(tokens, to_keep.tolist())
-                  if keep is True]
+        tokens = [tok for tok, keep in zip(tokens, to_keep.tolist()) if keep is True]
 
         if n_insert > 0:
             tokens = self.insertion_noise(tokens, n_insert / len(tokens))
 
         return tokens
 
     def insertion_noise(self, tokens, p=1.0):
@@ -282,19 +286,19 @@
         noise_mask = np.zeros(shape=(n_tokens + n_insert,), dtype=bool)
         noise_mask[noise_indices] = 1
 
         result = np.empty(shape=(n_tokens + n_insert,), dtype=object)
         result[noise_indices[n_random:]] = self.mask_tok
         if n_random > 0:
             result[noise_indices[:n_random]] = np.random.choice(
-                self.vocab, size=n_random)
+                self.vocab, size=n_random
+            )
         result[~noise_mask] = tokens
 
-        assert all([item is not None for item in result]),\
-            "Error when inserting noise."
+        assert all([item is not None for item in result]), "Error when inserting noise."
         return result.tolist()
 
     def rolling_noise(self, tokens, p=1.0):
         if np.random.random() >= p:
             return tokens
         offset = np.random.randint(0, max(1, len(tokens) - 1) + 1)
         return tokens[offset:] + tokens[0:offset]
@@ -313,104 +317,143 @@
             tokens = self.rolling_noise(tokens, self.rotate_ratio)
         return tokens
 
     def __repr__(self):
         cls_name = type(self).__name__
         kwargs = {}
         if self.permute_sent_ratio > 0.0:
-            kwargs['permute_sent_ratio'] = self.permute_sent_ratio
-            kwargs['full_stop_token'] = self.full_stop_token
+            kwargs["permute_sent_ratio"] = self.permute_sent_ratio
+            kwargs["full_stop_token"] = self.full_stop_token
         if self.insert_ratio > 0.0:
-            kwargs['insert_ratio'] = self.insert_ratio
+            kwargs["insert_ratio"] = self.insert_ratio
         if self.rotate_ratio > 0.0:
-            kwargs['rotate_ratio'] = self.rotate_ratio
+            kwargs["rotate_ratio"] = self.rotate_ratio
         if self.random_ratio > 0.0:
-            kwargs['random_ratio'] = self.random_ratio
+            kwargs["random_ratio"] = self.random_ratio
         if self.mask_ratio > 0.0:
-            kwargs['mask_ratio'] = self.mask_ratio
-            kwargs['mask_length'] = self.mask_length
-            kwargs['poisson_lambda'] = self.poisson_lambda
-            kwargs['replace_length'] = self.replace_length
-        cls_args = ', '.join(
-            [f'{kw}={arg}' for kw, arg in kwargs.items()])
-        return '{}({})'.format(cls_name, cls_args)
+            kwargs["mask_ratio"] = self.mask_ratio
+            kwargs["mask_length"] = self.mask_length
+            kwargs["poisson_lambda"] = self.poisson_lambda
+            kwargs["replace_length"] = self.replace_length
+        cls_args = ", ".join([f"{kw}={arg}" for kw, arg in kwargs.items()])
+        return "{}({})".format(cls_name, cls_args)
 
 
-@register_transform(name='bart')
+@register_transform(name="bart")
 class BARTNoiseTransform(Transform):
     def __init__(self, opts):
         super().__init__(opts)
 
     def _set_seed(self, seed):
         """set seed to ensure reproducibility."""
         BARTNoising.set_random_seed(seed)
 
     @classmethod
     def add_options(cls, parser):
         """Avalilable options relate to BART."""
         group = parser.add_argument_group("Transform/BART")
-        group.add("--permute_sent_ratio", "-permute_sent_ratio",
-                  type=float, default=0.0,
-                  help="Permute this proportion of sentences "
-                       "(boundaries defined by {}) in all inputs.".format(
-                        DefaultTokens.SENT_FULL_STOPS))
-        group.add("--rotate_ratio", "-rotate_ratio", type=float, default=0.0,
-                  help="Rotate this proportion of inputs.")
-        group.add("--insert_ratio", "-insert_ratio", type=float, default=0.0,
-                  help="Insert this percentage of additional random tokens.")
-        group.add("--random_ratio", "-random_ratio", type=float, default=0.0,
-                  help="Instead of using {}, use random token "
-                       "this often.".format(DefaultTokens.MASK))
-
-        group.add("--mask_ratio", "-mask_ratio", type=float, default=0.0,
-                  help="Fraction of words/subwords that will be masked.")
-        group.add("--mask_length", "-mask_length", type=str, default="subword",
-                  choices=["subword", "word", "span-poisson"],
-                  help="Length of masking window to apply.")
-        group.add("--poisson_lambda", "-poisson_lambda",
-                  type=float, default=3.0,
-                  help="Lambda for Poisson distribution to sample span length "
-                       "if `-mask_length` set to span-poisson.")
-        group.add("--replace_length", "-replace_length",
-                  type=int, default=-1, choices=[-1, 0, 1],
-                  help="When masking N tokens, replace with 0, 1, "
-                       "or N tokens. (use -1 for N)")
+        group.add(
+            "--permute_sent_ratio",
+            "-permute_sent_ratio",
+            type=float,
+            default=0.0,
+            help="Permute this proportion of sentences "
+            "(boundaries defined by {}) in all inputs.".format(
+                DefaultTokens.SENT_FULL_STOPS
+            ),
+        )
+        group.add(
+            "--rotate_ratio",
+            "-rotate_ratio",
+            type=float,
+            default=0.0,
+            help="Rotate this proportion of inputs.",
+        )
+        group.add(
+            "--insert_ratio",
+            "-insert_ratio",
+            type=float,
+            default=0.0,
+            help="Insert this percentage of additional random tokens.",
+        )
+        group.add(
+            "--random_ratio",
+            "-random_ratio",
+            type=float,
+            default=0.0,
+            help="Instead of using {}, use random token "
+            "this often.".format(DefaultTokens.MASK),
+        )
+
+        group.add(
+            "--mask_ratio",
+            "-mask_ratio",
+            type=float,
+            default=0.0,
+            help="Fraction of words/subwords that will be masked.",
+        )
+        group.add(
+            "--mask_length",
+            "-mask_length",
+            type=str,
+            default="subword",
+            choices=["subword", "word", "span-poisson"],
+            help="Length of masking window to apply.",
+        )
+        group.add(
+            "--poisson_lambda",
+            "-poisson_lambda",
+            type=float,
+            default=3.0,
+            help="Lambda for Poisson distribution to sample span length "
+            "if `-mask_length` set to span-poisson.",
+        )
+        group.add(
+            "--replace_length",
+            "-replace_length",
+            type=int,
+            default=-1,
+            choices=[-1, 0, 1],
+            help="When masking N tokens, replace with 0, 1, "
+            "or N tokens. (use -1 for N)",
+        )
 
     @classmethod
     def require_vocab(cls):
         """Override this method to inform it need vocab to start."""
         return True
 
     def warm_up(self, vocabs):
         super().warm_up(vocabs)
 
         subword_type = self.opts.src_subword_type
-        if self.opts.mask_length == 'subword':
-            if subword_type == 'none':
+        if self.opts.mask_length == "subword":
+            if subword_type == "none":
                 raise ValueError(
-                    f'src_subword_type={subword_type} incompatible with '
-                    f'mask_length={self.opts.mask_length}!')
-        is_joiner = (subword_type == 'bpe') if subword_type != 'none' else None
+                    f"src_subword_type={subword_type} incompatible with "
+                    f"mask_length={self.opts.mask_length}!"
+                )
+        is_joiner = (subword_type == "bpe") if subword_type != "none" else None
         self.bart_noise = BARTNoising(
-            self.vocabs['src'].ids_to_tokens,
+            self.vocabs["src"].ids_to_tokens,
             mask_tok=DefaultTokens.MASK,
             mask_ratio=self.opts.mask_ratio,
             insert_ratio=self.opts.insert_ratio,
             permute_sent_ratio=self.opts.permute_sent_ratio,
             poisson_lambda=self.opts.poisson_lambda,
             replace_length=self.opts.replace_length,
             rotate_ratio=self.opts.rotate_ratio,
             mask_length=self.opts.mask_length,
             random_ratio=self.opts.random_ratio,
-            is_joiner=is_joiner
+            is_joiner=is_joiner,
         )
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Apply BART noise to src side tokens."""
         if is_train:
-            src = self.bart_noise.apply(example['src'])
-            example['src'] = src
+            src = self.bart_noise.apply(example["src"])
+            example["src"] = src
         return example
 
     def _repr_args(self):
         """Return str represent key arguments for BART."""
         return repr(self.bart_noise)
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/clean.py` & `OpenNMT-py-3.1.3/onmt/transforms/clean.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,193 +1,253 @@
 from onmt.transforms import register_transform
 from .transform import Transform
 from onmt.utils.logging import logger
-import gcld3
+import fasttext
+import os
+import urllib.request
 import regex as re
 
 
-@register_transform(name='clean')
+@register_transform(name="clean")
 class CleanTransform(Transform):
     """
     Clean examples according to rules
 
     """
 
     def __init__(self, opts):
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """Add an option for the corpus ratio to apply this transform."""
 
         group = parser.add_argument_group("Transform/Clean")
-        group.add("--src_eq_tgt", "-src_eq_tgt", action="store_true",
-                  help="Remove ex src==tgt")
-        group.add("--same_char", "-same_char", action="store_true",
-                  help="Remove ex with same char more than 4 times")
-        group.add("--same_word", "-same_word", action="store_true",
-                  help="Remove ex with same word more than 3 times")
-        group.add('--scripts_ok', '-scripts_ok', default=['Latin', 'Common'],
-                  nargs='*', type=str,
-                  help="list of unicodata scripts accepted")
-        group.add('--scripts_nok', '-scripts_nok', default=[],
-                  nargs='*', type=str,
-                  help="list of unicodata scripts not accepted")
-
-        group.add("--src_tgt_ratio", "-src_tgt_ratio", type=float,
-                  default=2, help="ratio between src and tgt")
-        group.add("--avg_tok_min", "-avg_tok_min", type=float,
-                  default=3, help="average length of tokens min")
-        group.add("--avg_tok_max", "-avg_tok_max", type=float,
-                  default=20, help="average length of tokens max")
-        group.add('--langid', '-langid', default=[],
-                  nargs='*', type=str,
-                  help="list of languages accepted")
+        group.add(
+            "--src_eq_tgt",
+            "-src_eq_tgt",
+            action="store_true",
+            help="Remove ex src==tgt",
+        )
+        group.add(
+            "--same_char",
+            "-same_char",
+            action="store_true",
+            help="Remove ex with same char more than 4 times",
+        )
+        group.add(
+            "--same_word",
+            "-same_word",
+            action="store_true",
+            help="Remove ex with same word more than 3 times",
+        )
+        group.add(
+            "--scripts_ok",
+            "-scripts_ok",
+            default=["Latin", "Common"],
+            nargs="*",
+            type=str,
+            help="list of unicodata scripts accepted",
+        )
+        group.add(
+            "--scripts_nok",
+            "-scripts_nok",
+            default=[],
+            nargs="*",
+            type=str,
+            help="list of unicodata scripts not accepted",
+        )
+
+        group.add(
+            "--src_tgt_ratio",
+            "-src_tgt_ratio",
+            type=float,
+            default=2,
+            help="ratio between src and tgt",
+        )
+        group.add(
+            "--avg_tok_min",
+            "-avg_tok_min",
+            type=float,
+            default=3,
+            help="average length of tokens min",
+        )
+        group.add(
+            "--avg_tok_max",
+            "-avg_tok_max",
+            type=float,
+            default=20,
+            help="average length of tokens max",
+        )
+        group.add(
+            "--langid",
+            "-langid",
+            default=[],
+            nargs="*",
+            type=str,
+            help="list of languages accepted",
+        )
 
     def _parse_opts(self):
         self.src_eq_tgt = self.opts.src_eq_tgt
         self.same_char = self.opts.same_char
         self.same_word = self.opts.same_word
         self.scripts_ok = self.opts.scripts_ok
         self.scripts_nok = self.opts.scripts_nok
         self.src_tgt_ratio = self.opts.src_tgt_ratio
         self.avg_tok_min = self.opts.avg_tok_min
         self.avg_tok_max = self.opts.avg_tok_max
         self.langid = self.opts.langid
-        assert (self.scripts_ok == [] or self.scripts_nok == []), \
-            "Choose either scripts to be included or excluded"
+        assert (
+            self.scripts_ok == [] or self.scripts_nok == []
+        ), "Choose either scripts to be included or excluded"
 
     @staticmethod
     def _get_opt(corpus, opt, def_val):
         """Get opt string of a `corpus`."""
-        if 'clean' in corpus['transforms']:
+        if "clean" in corpus["transforms"]:
             value = corpus.get(opt, def_val)
             clean = value
         else:
             clean = None
         return clean
 
     @classmethod
     def get_opt_dict(cls, opts, opt, def_val):
         """Get clean settings correspond to corpus in `opts`."""
         clean_dict = {}
         # normalize dict src/tgt for each dataset
-        if hasattr(opts, 'data'):
+        if hasattr(opts, "data"):
             for c_name, corpus in opts.data.items():
                 clean = cls._get_opt(corpus, opt, def_val)
                 if clean is not None:
                     logger.debug(f"Get {opt} for {c_name}: {clean}")
                     clean_dict[c_name] = clean
 
         return clean_dict
 
     def warm_up(self, vocabs=None):
         super().warm_up(None)
-        self.src_eq_tgt_dict = self.get_opt_dict(self.opts, 'src_eq_tgt', True)
-        self.same_char_dict = self.get_opt_dict(self.opts, 'same_char', True)
-        self.same_word_dict = self.get_opt_dict(self.opts, 'same_word', True)
-        self.scripts_ok_dict = self.get_opt_dict(self.opts, 'scripts_ok',
-                                                 ['Latin', 'Common'])
-        self.scripts_nok_dict = self.get_opt_dict(self.opts, 'scripts_nok', [])
-        self.src_tgt_ratio_dict = self.get_opt_dict(self.opts, 'src_tgt_ratio',
-                                                    2)
-        self.avg_tok_min_dict = self.get_opt_dict(self.opts, 'avg_tok_min', 3)
-        self.avg_tok_max_dict = self.get_opt_dict(self.opts, 'avg_tok_max', 20)
-        self.langid_dict = self.get_opt_dict(self.opts, 'langid', [])
-
-        self.id_func = gcld3.NNetLanguageIdentifier(min_num_bytes=0,
-                                                    max_num_bytes=200)
+        self.src_eq_tgt_dict = self.get_opt_dict(self.opts, "src_eq_tgt", True)
+        self.same_char_dict = self.get_opt_dict(self.opts, "same_char", True)
+        self.same_word_dict = self.get_opt_dict(self.opts, "same_word", True)
+        self.scripts_ok_dict = self.get_opt_dict(
+            self.opts, "scripts_ok", ["Latin", "Common"]
+        )
+        self.scripts_nok_dict = self.get_opt_dict(self.opts, "scripts_nok", [])
+        self.src_tgt_ratio_dict = self.get_opt_dict(self.opts, "src_tgt_ratio", 2)
+        self.avg_tok_min_dict = self.get_opt_dict(self.opts, "avg_tok_min", 3)
+        self.avg_tok_max_dict = self.get_opt_dict(self.opts, "avg_tok_max", 20)
+        self.langid_dict = self.get_opt_dict(self.opts, "langid", [])
+        fasttext_loc = f"{os.path.dirname(os.path.abspath(__file__))}/lid.176.ftz"
+
+        if not os.path.exists(fasttext_loc):
+            urllib.request.urlretrieve(
+                "https://dl.fbaipublicfiles.com/"
+                + "fasttext/supervised-models/lid.176.ftz",
+                fasttext_loc,
+            )
+        self.id_func = fasttext.load_model(fasttext_loc)
 
     def batch_apply(self, batch, is_train=False, stats=None, **kwargs):
         """Convert source and target examples to doc level segments."""
+
         def _id(string):
-            res = self.id_func.FindLanguage(text=string)
-            return res.language
+            res = self.id_func.predict(string, k=1)
+            res = res[0][0].replace("__label__", "")
+            return res
 
         trf_batch = []
 
-        for (ex, _, cid) in batch:
-
+        for ex, _, cid in batch:
             if self.scripts_ok_dict[cid]:
-                ok_regex = "[^" + "".join(r"\p{%s}" % sc for sc in
-                                          self.scripts_ok_dict[cid]) + "]"
+                ok_regex = (
+                    "[^"
+                    + "".join(r"\p{%s}" % sc for sc in self.scripts_ok_dict[cid])
+                    + "]"
+                )
 
             if self.scripts_nok_dict[cid]:
-                nok_regex = "[" + "".join(r"\p{%s}" % sc for sc in
-                                          self.scripts_nok_dict[cid]) + "]"
+                nok_regex = (
+                    "["
+                    + "".join(r"\p{%s}" % sc for sc in self.scripts_nok_dict[cid])
+                    + "]"
+                )
 
-            src_str = ' '.join(ex['src'])
+            src_str = " ".join(ex["src"])
             if len(src_str) == 0:
                 # print("src empty")
                 continue
-            if self.same_char_dict[cid] and re.search(r'([^0-9])\1{3}',
-                                                      src_str):
+            if self.same_char_dict[cid] and re.search(r"([^0-9])\1{3}", src_str):
                 # print("too many same char in src")
                 continue
-            if self.same_word_dict[cid] and re.search(r'(\ .*|.*\ )\1{2}',
-                                                      src_str):
+            if self.same_word_dict[cid] and re.search(r"(\ .*|.*\ )\1{2}", src_str):
                 # print("too many same word in src")
                 continue
-            if len(src_str) / len(ex['src']) < self.avg_tok_min_dict[cid]:
+            if len(src_str) / len(ex["src"]) < self.avg_tok_min_dict[cid]:
                 # print("avg token min", len(src_str) / len(ex['src']))
                 continue
-            if len(src_str) / len(ex['src']) > self.avg_tok_max_dict[cid]:
+            if len(src_str) / len(ex["src"]) > self.avg_tok_max_dict[cid]:
                 # print("avg token max", len(src_str) / len(ex['src']))
                 continue
 
             if self.scripts_ok_dict[cid] and re.search(ok_regex, src_str):
                 # print("text does not fully belong to wanted script")
                 continue
             if self.scripts_nok_dict[cid] and re.search(nok_regex, src_str):
                 # print("Some text belong to unwanted scripts")
                 continue
 
-            if self.langid_dict[cid] != [] and \
-                    _id(src_str) not in self.langid_dict[cid]:
+            if (
+                self.langid_dict[cid] != []
+                and _id(src_str) not in self.langid_dict[cid]
+            ):
                 # print("langid does not match", _id(src_str))
                 continue
 
-            if ex['tgt'] is not None:
-                tgt_str = ' '.join(ex['tgt'])
+            if ex["tgt"] is not None:
+                tgt_str = " ".join(ex["tgt"])
                 if self.src_eq_tgt_dict[cid] and src_str == tgt_str:
                     # print("src = tgt")
                     continue
                 if len(tgt_str) == 0:
                     # print("tgt empty")
                     continue
-                if (len(ex['src']) + 1) / (len(ex['tgt']) + 1) > \
-                        self.src_tgt_ratio_dict[cid] or \
-                        (len(ex['src']) + 1) / (len(ex['tgt']) + 1) < \
-                        (1 / self.src_tgt_ratio_dict[cid]):
+                if (len(ex["src"]) + 1) / (
+                    len(ex["tgt"]) + 1
+                ) > self.src_tgt_ratio_dict[cid] or (len(ex["src"]) + 1) / (
+                    len(ex["tgt"]) + 1
+                ) < (
+                    1 / self.src_tgt_ratio_dict[cid]
+                ):
                     # print("src / tgt ratio ", len(src_str) / len(tgt_str))
                     continue
-                if self.same_char_dict[cid] and re.search(r'([^0-9])\1{3}',
-                                                          tgt_str):
+                if self.same_char_dict[cid] and re.search(r"([^0-9])\1{3}", tgt_str):
                     # print("too many same char in tgt")
                     continue
-                if self.same_word_dict[cid] and re.search(r'(\ .*|.*\ )\1{2}',
-                                                          tgt_str):
+                if self.same_word_dict[cid] and re.search(r"(\ .*|.*\ )\1{2}", tgt_str):
                     # print("too many same word in tgt")
                     continue
-                if len(tgt_str) / len(ex['tgt']) < self.avg_tok_min_dict[cid]:
+                if len(tgt_str) / len(ex["tgt"]) < self.avg_tok_min_dict[cid]:
                     # print("avg token min", len(tgt_str) / len(ex['tgt']))
                     continue
-                if len(tgt_str) / len(ex['tgt']) > self.avg_tok_max_dict[cid]:
+                if len(tgt_str) / len(ex["tgt"]) > self.avg_tok_max_dict[cid]:
                     # print("avg token max", len(tgt_str) / len(ex['tgt']))
                     continue
 
                 if self.scripts_ok_dict[cid] and re.search(ok_regex, tgt_str):
                     # print("text does not fully belong to wanted script")
                     continue
-                if self.scripts_nok_dict[cid] and re.search(nok_regex,
-                                                            tgt_str):
+                if self.scripts_nok_dict[cid] and re.search(nok_regex, tgt_str):
                     # print("Some text belong to unwanted scripts")
                     continue
 
-                if self.langid_dict[cid] != [] and \
-                        _id(tgt_str) not in self.langid_dict[cid]:
+                if (
+                    self.langid_dict[cid] != []
+                    and _id(tgt_str) not in self.langid_dict[cid]
+                ):
                     # print("langid does not match", _id(tgt_str))
                     continue
 
             trf_batch.append((ex, self, cid))
 
         return trf_batch
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/docify.py` & `OpenNMT-py-3.1.3/onmt/transforms/docify.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from onmt.constants import DefaultTokens
 from onmt.transforms import register_transform
 from .transform import Transform
 import copy
 
 
-@register_transform(name='docify')
+@register_transform(name="docify")
 class DocifyTransform(Transform):
     """
     Convert source and target examples to doc level segments.
 
     It concatenates segments with a DefaultTokens.SEP
     until it reaches --doc_length tokens
 
@@ -18,120 +18,126 @@
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """Add an option for the corpus ratio to apply this transform."""
 
         group = parser.add_argument_group("Transform/Docify")
-        group.add("--doc_length", "-doc_length", type=int,
-                  default=200, help="Number of tokens per doc.")
-        group.add("--max_context", "-max_context", type=int,
-                  default=1, help="Max context segments.")
+        group.add(
+            "--doc_length",
+            "-doc_length",
+            type=int,
+            default=200,
+            help="Number of tokens per doc.",
+        )
+        group.add(
+            "--max_context",
+            "-max_context",
+            type=int,
+            default=1,
+            help="Max context segments.",
+        )
 
     def _parse_opts(self):
-        if (hasattr(self.opts, 'num_workers') and
-                hasattr(self.opts, 'world_size')):
+        if hasattr(self.opts, "num_workers") and hasattr(self.opts, "world_size"):
             self.stride = self.opts.num_workers * self.opts.world_size
         else:
             self.stride = 1
         self.doc_length = self.opts.doc_length
         self.max_context = self.opts.max_context
 
     @classmethod
     def get_specials(cls, opts):
         """Add newline tag to src and tgt vocabs."""
 
-        src_specials, tgt_specials = ['｟newline｠'], ['｟newline｠']
+        src_specials, tgt_specials = [DefaultTokens.SEP], [DefaultTokens.SEP]
         return (src_specials, tgt_specials)
 
     def warm_up(self, vocabs=None):
         super().warm_up(None)
         if self.stride != 1:
-            assert (self.stride % (self.max_context + 1) == 0), \
-                "(max_context+1) must be a multiple \
+            assert (
+                self.stride % (self.max_context + 1) == 0
+            ), "(max_context+1) must be a multiple \
                  of num_workers * world_size"
 
     def batch_apply(self, batch, is_train=False, stats=None, **kwargs):
         """Convert source and target examples to doc level segments."""
         if self.max_context == 0:
             return batch
         trf_batch = []
         doc = {}
-        doc['src'] = []
-        doc['tgt'] = []
-        doc['indices'] = 0
-
-        for (ex, _, cid) in batch:
-            if ex['tgt'] is not None:
-                cur_len = max(len(doc['src'] + ex['src']),
-                              len(doc['tgt'] + ex['tgt']))
+        doc["src"] = []
+        doc["tgt"] = []
+        doc["indices"] = 0
+
+        for ex, _, cid in batch:
+            if ex["tgt"] is not None:
+                cur_len = max(len(doc["src"] + ex["src"]), len(doc["tgt"] + ex["tgt"]))
 
-                if len(ex['src']) == 0 and len(ex['tgt']) == 0:
+                if len(ex["src"]) == 0 and len(ex["tgt"]) == 0:
                     # doc break we add it, restart new doc
                     trf_batch.append((doc, self, cid))
                     doc = {}
-                    doc['src'] = []
-                    doc['tgt'] = []
-                    doc['indices'] = ex['indices']
+                    doc["src"] = []
+                    doc["tgt"] = []
+                    doc["indices"] = ex["indices"]
                 elif cur_len > self.doc_length:
-                    if len(doc['src']) == 0:
+                    if len(doc["src"]) == 0:
                         # case 1st ex is already longer
                         trf_batch.append((ex, self, cid))
                     else:
                         # adding cur ex is too long we add cur doc
                         # and reset doc to cur ex
                         trf_batch.append((doc, self, cid))
                         doc = copy.deepcopy(ex)
                 else:
-                    if len(doc['src']) == 0:
+                    if len(doc["src"]) == 0:
                         # we start the new doc with cur ex
                         doc = copy.deepcopy(ex)
                     else:
                         # we cumulate cur ex to cur doc
-                        doc['src'] += [DefaultTokens.SEP] + ex['src']
-                        doc['src_original'] += ([DefaultTokens.SEP] +
-                                                ex['src_original'])
-                        doc['tgt'] += [DefaultTokens.SEP] + ex['tgt']
-                        doc['tgt_original'] += ([DefaultTokens.SEP] +
-                                                ex['tgt_original'])
-                        nb_ctx = doc['src'].count(DefaultTokens.SEP)
+                        doc["src"] += [DefaultTokens.SEP] + ex["src"]
+                        doc["src_original"] += [DefaultTokens.SEP] + ex["src_original"]
+                        doc["tgt"] += [DefaultTokens.SEP] + ex["tgt"]
+                        doc["tgt_original"] += [DefaultTokens.SEP] + ex["tgt_original"]
+                        nb_ctx = doc["src"].count(DefaultTokens.SEP)
                         if nb_ctx >= self.max_context:
                             trf_batch.append((doc, self, cid))
                             doc = {}
-                            doc['src'] = []
-                            doc['tgt'] = []
-                            doc['indices'] = ex['indices']
+                            doc["src"] = []
+                            doc["tgt"] = []
+                            doc["indices"] = ex["indices"]
             else:
-                cur_len = len(doc['src'] + ex['src'])
-                doc['tgt'] = None
-                if len(ex['src']) == 0:
+                cur_len = len(doc["src"] + ex["src"])
+                doc["tgt"] = None
+                if len(ex["src"]) == 0:
                     trf_batch.append((doc, self, cid))
                     doc = {}
-                    doc['src'] = []
-                    doc['indices'] = ex['indices']
+                    doc["src"] = []
+                    doc["indices"] = ex["indices"]
                 elif cur_len > self.doc_length:
-                    if len(doc['src']) == 0:
+                    if len(doc["src"]) == 0:
                         trf_batch.append((ex, self, cid))
                     else:
                         trf_batch.append((doc, self, cid))
                         doc = copy.deepcopy(ex)
                 else:
-                    if len(doc['src']) == 0:
+                    if len(doc["src"]) == 0:
                         doc = copy.deepcopy(ex)
                     else:
-                        doc['src'] += [DefaultTokens.SEP] + ex['src']
-                        doc['src_original'] += ([DefaultTokens.SEP] +
-                                                ex['src_original'])
-                        nb_ctx = doc['src'].count(DefaultTokens.SEP)
+                        doc["src"] += [DefaultTokens.SEP] + ex["src"]
+                        doc["src_original"] += [DefaultTokens.SEP] + ex["src_original"]
+                        nb_ctx = doc["src"].count(DefaultTokens.SEP)
                         if nb_ctx >= self.max_context:
                             trf_batch.append((doc, self, cid))
                             doc = {}
-                            doc['src'] = []
-                            doc['indices'] = ex['indices']
-        if len(doc['src']) > 0:
+                            doc["src"] = []
+                            doc["indices"] = ex["indices"]
+        if len(doc["src"]) > 0:
             trf_batch.append((doc, self, cid))
         return trf_batch
 
     def apply_reverse(self, translated):
         segments = translated.split(DefaultTokens.SEP)
-        segments = [segment.strip(' ') for segment in segments]
+        segments = [segment.strip(" ") for segment in segments]
         return segments
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/features.py` & `OpenNMT-py-3.1.3/onmt/transforms/features.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 from onmt.transforms import register_transform
 from .transform import Transform
 from onmt.utils.alignment import subword_map_by_joiner, subword_map_by_spacer
 
 
-@register_transform(name='inferfeats')
+@register_transform(name="inferfeats")
 class InferFeatsTransform(Transform):
     """Infer features for subword tokenization."""
 
     def __init__(self, opts):
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """Avalilable options related to this Transform."""
         group = parser.add_argument_group("Transform/InferFeats")
-        group.add("--reversible_tokenization", "-reversible_tokenization",
-                  default="joiner", choices=["joiner", "spacer"],
-                  help="Type of reversible tokenization "
-                       "applied on the tokenizer.")
+        group.add(
+            "--reversible_tokenization",
+            "-reversible_tokenization",
+            default="joiner",
+            choices=["joiner", "spacer"],
+            help="Type of reversible tokenization " "applied on the tokenizer.",
+        )
 
     def _parse_opts(self):
         super()._parse_opts()
         self.reversible_tokenization = self.opts.reversible_tokenization
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
-
         if "src_feats" not in example:
             # Do nothing
             return example
 
         if self.reversible_tokenization == "joiner":
             original_src = example["src_original"]
             word_to_subword_mapping = subword_map_by_joiner(
-                example["src"], original_subwords=original_src)
+                example["src"], original_subwords=original_src
+            )
         else:  # Spacer
             word_to_subword_mapping = subword_map_by_spacer(example["src"])
 
         new_src_feats = [[] for _ in range(len(example["src_feats"]))]
         for subword, word_id in zip(example["src"], word_to_subword_mapping):
             for i, feat_values in enumerate(example["src_feats"]):
                 inferred_feat = feat_values[word_id]
                 new_src_feats[i].append(inferred_feat)
         example["src_feats"] = new_src_feats
 
         return example
 
     def _repr_args(self):
-        return ''
+        return ""
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/fuzzymatch.py` & `OpenNMT-py-3.1.3/onmt/transforms/fuzzymatch.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 import numpy as np
 import time
 
 
 class FuzzyMatcher(object):
     """Class for creating and setting up fuzzy matchers."""
 
-    def __init__(self, tm_path,
-                 corpus_ratio,
-                 threshold=70,
-                 tm_delimiter='\t',
-                 fuzzy_token='｟fuzzy｠',
-                 tm_unit_min_lentgh=4,
-                 tm_unit_max_length=70):
+    def __init__(
+        self,
+        tm_path,
+        corpus_ratio,
+        threshold=70,
+        tm_delimiter="\t",
+        fuzzy_token="｟fuzzy｠",
+        tm_unit_min_lentgh=4,
+        tm_unit_max_length=70,
+    ):
         self.threshold = threshold
         self.corpus_ratio = corpus_ratio
         self.tm_delimiter = tm_delimiter
         self.fuzzy_token = fuzzy_token
         self.tm_unit_min_length = tm_unit_min_lentgh
         self.tm_unit_max_length = tm_unit_max_length
         self.internal_tm = self._create_tm(tm_path)
@@ -30,115 +33,144 @@
         containing a source sentence and its translation, separated
         by the `self.tm_delimiter`. A TM size of 200k-250k pairs should
         provide enough matches and good performance, but this may
         depend on overall system specs (RAM, CPU)
         """
 
         src_segments, tgt_segments = list(), list()
-        with open(tm_path, mode='r', encoding='utf-8') as file:
+        with open(tm_path, mode="r", encoding="utf-8") as file:
             pairs = file.readlines()
             for pair in pairs:
                 source, target = map(str, pair.split(self.tm_delimiter))
 
                 # Filter out very short or very long sentences
                 # from the TM for better performance
-                if len(source) < self.tm_unit_min_length or \
-                        len(source) > self.tm_unit_max_length:
+                if (
+                    len(source) < self.tm_unit_min_length
+                    or len(source) > self.tm_unit_max_length
+                ):
                     continue
                 src_segments.append(source.strip())
                 tgt_segments.append(target.strip())
-        logger.debug(f'Translation Memory size for FuzzyMatch transform: '
-                     f'{len(src_segments)}')
+        logger.debug(
+            f"Translation Memory size for FuzzyMatch transform: " f"{len(src_segments)}"
+        )
         return [src_segments, tgt_segments]
 
     def _get_batch_matches(self, batch):
-        logger.debug(f'Starting fuzzy matching on {len(batch)} examples')
+        logger.debug(f"Starting fuzzy matching on {len(batch)} examples")
         fuzzy_count = 0
         start = time.time()
         augmented = list()
 
         # We split the `batch` and perform fuzzy matching
         # in smaller chunks of 10.000 examples in order to
         # reduce memory usage.
         # Perfomance is not affected.
         chunk_size = 10000
-        mini_batches = np.array_split(batch, len(batch) // chunk_size
-                                      if len(batch) > chunk_size else 1)
+        mini_batches = np.array_split(
+            batch, len(batch) // chunk_size if len(batch) > chunk_size else 1
+        )
         for mini_batch in mini_batches:
             plist = list(mini_batch)
             if fuzzy_count >= len(batch) * self.corpus_ratio:
                 augmented.extend(plist)
                 continue
 
-            results = process.cdist(plist,
-                                    self.internal_tm[0],
-                                    scorer=fuzz.ratio,
-                                    dtype=np.uint8,
-                                    score_cutoff=self.threshold,
-                                    workers=-1)
+            results = process.cdist(
+                plist,
+                self.internal_tm[0],
+                scorer=fuzz.ratio,
+                dtype=np.uint8,
+                score_cutoff=self.threshold,
+                workers=-1,
+            )
 
             matches = np.any(results, 1)
             argmax = np.argmax(results, axis=1)
             for idx, s in enumerate(plist):
                 # Probably redundant but let's be safe
                 # in case some examples are already fuzzied
                 # (e.g. from another pipeline or workflow)
                 if self.fuzzy_token in s:
                     continue
                 # We don't want exact matches
                 if matches[idx] and results[idx][argmax[idx]] < 100:
                     if fuzzy_count >= len(batch) * self.corpus_ratio:
                         break
-                    plist[idx] = s + self.fuzzy_token + \
-                        self.internal_tm[1][argmax[idx]]
+                    plist[idx] = s + self.fuzzy_token + self.internal_tm[1][argmax[idx]]
                     fuzzy_count += 1
             augmented.extend(plist)
 
         end = time.time()
-        logger.debug(f'FuzzyMatch Transform: Added {fuzzy_count} '
-                     f'fuzzies in {end-start} secs')
+        logger.debug(
+            f"FuzzyMatch Transform: Added {fuzzy_count} " f"fuzzies in {end-start} secs"
+        )
 
         return augmented
 
 
-@register_transform(name='fuzzymatch')
+@register_transform(name="fuzzymatch")
 class FuzzyMatchTransform(Transform):
     """Perform fuzzy matching against a translation memory and
     augment source examples with target matches for Neural Fuzzy Repair.
     :cite:`bulte-tezcan-2019-neural`
     """
 
     def __init__(self, opts):
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """Options for fuzzy matching."""
 
         group = parser.add_argument_group("Transform/FuzzyMatching")
-        group.add("--tm_path", "-tm_path",
-                  type=str, help="Path to a flat text TM.")
-        group.add("--fuzzy_corpus_ratio", "-fuzzy_corpus_ratio",
-                  type=float, default=0.1,
-                  help="Ratio of corpus to augment with fuzzy matches.")
-        group.add("--fuzzy_threshold", "-fuzzy_threshold",
-                  type=int, default=70,
-                  help="The fuzzy matching threshold.")
-        group.add("--tm_delimiter", "-tm_delimiter",
-                  type=str, default="\t",
-                  help="The delimiter used in the flat text TM.")
-        group.add("--fuzzy_token", "-fuzzy_token",
-                  type=str, default="｟fuzzy｠",
-                  help="The fuzzy token to be added with the matches.")
-        group.add("--fuzzymatch_min_length", "-fuzzymatch_min_length",
-                  type=int, default=4,
-                  help="Min length for TM entries and examples to match.")
-        group.add("--fuzzymatch_max_length", "-fuzzymatch_max_length",
-                  type=int, default=70,
-                  help="Max length for TM entries and examples to match.")
+        group.add("--tm_path", "-tm_path", type=str, help="Path to a flat text TM.")
+        group.add(
+            "--fuzzy_corpus_ratio",
+            "-fuzzy_corpus_ratio",
+            type=float,
+            default=0.1,
+            help="Ratio of corpus to augment with fuzzy matches.",
+        )
+        group.add(
+            "--fuzzy_threshold",
+            "-fuzzy_threshold",
+            type=int,
+            default=70,
+            help="The fuzzy matching threshold.",
+        )
+        group.add(
+            "--tm_delimiter",
+            "-tm_delimiter",
+            type=str,
+            default="\t",
+            help="The delimiter used in the flat text TM.",
+        )
+        group.add(
+            "--fuzzy_token",
+            "-fuzzy_token",
+            type=str,
+            default="｟fuzzy｠",
+            help="The fuzzy token to be added with the matches.",
+        )
+        group.add(
+            "--fuzzymatch_min_length",
+            "-fuzzymatch_min_length",
+            type=int,
+            default=4,
+            help="Min length for TM entries and examples to match.",
+        )
+        group.add(
+            "--fuzzymatch_max_length",
+            "-fuzzymatch_max_length",
+            type=int,
+            default=70,
+            help="Max length for TM entries and examples to match.",
+        )
 
     def _parse_opts(self):
         self.tm_path = self.opts.tm_path
         self.fuzzy_corpus_ratio = self.opts.fuzzy_corpus_ratio
         self.fuzzy_threshold = self.opts.fuzzy_threshold
         self.tm_delimiter = self.opts.tm_delimiter
         self.fuzzy_token = self.opts.fuzzy_token
@@ -151,35 +183,39 @@
 
         return ([opts.fuzzy_token], list())
 
     def warm_up(self, vocabs=None):
         """Create the fuzzy matcher."""
 
         super().warm_up(None)
-        self.matcher = FuzzyMatcher(self.tm_path,
-                                    self.fuzzy_corpus_ratio,
-                                    self.fuzzy_threshold,
-                                    self.tm_delimiter,
-                                    self.fuzzy_token,
-                                    self.fuzzymatch_min_length,
-                                    self.fuzzymatch_max_length)
+        self.matcher = FuzzyMatcher(
+            self.tm_path,
+            self.fuzzy_corpus_ratio,
+            self.fuzzy_threshold,
+            self.tm_delimiter,
+            self.fuzzy_token,
+            self.fuzzymatch_min_length,
+            self.fuzzymatch_max_length,
+        )
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         return example
 
     def batch_apply(self, batch, is_train=False, stats=None, **kwargs):
         src_segments = list()
-        for (ex, _, _) in batch:
+        for ex, _, _ in batch:
             # Apply a basic filtering to leave out very short or very long
             # sentences and speed up things a bit during fuzzy matching
-            if len(' '.join(ex['src'])) > self.fuzzymatch_min_length and \
-                    len(' '.join(ex['src'])) < self.fuzzymatch_max_length:
-                src_segments.append(' '.join(ex['src']))
+            if (
+                len(" ".join(ex["src"])) > self.fuzzymatch_min_length
+                and len(" ".join(ex["src"])) < self.fuzzymatch_max_length
+            ):
+                src_segments.append(" ".join(ex["src"]))
             else:
-                src_segments.append('')
+                src_segments.append("")
         fuzzied_src = self.matcher._get_batch_matches(src_segments)
-        assert (len(src_segments) == len(fuzzied_src))
+        assert len(src_segments) == len(fuzzied_src)
         for idx, (example, _, _) in enumerate(batch):
-            if fuzzied_src[idx] != '':
-                example['src'] = fuzzied_src[idx].split()
+            if fuzzied_src[idx] != "":
+                example["src"] = fuzzied_src[idx].split()
 
         return batch
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/inlinetags.py` & `OpenNMT-py-3.1.3/onmt/transforms/inlinetags.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,44 +14,51 @@
     It requires a prepared tab-delimited dictionary of source-target
     words and phrases. A dictionary can be created with
     tools such as fastalign and it should ideally contain enough long
     phrases (of 3-4 words or more) for more realistic applications
     of start and end tags. A dictionary with 20.000-30.000 entries
     should give sufficient number of matches."""
 
-    def __init__(self, tags_dictionary_path, max_tags,
-                 paired_start_tag,
-                 paired_end_tag,
-                 isolated_tag,
-                 src_delimiter,
-                 tag_corpus_ratio=0.1):
+    def __init__(
+        self,
+        tags_dictionary_path,
+        max_tags,
+        paired_start_tag,
+        paired_end_tag,
+        isolated_tag,
+        src_delimiter,
+        tag_corpus_ratio=0.1,
+    ):
         self.max_tags = max_tags
         self.tag_corpus_ratio = tag_corpus_ratio
         self.src_delimiter = src_delimiter
         self.internal_dictionary = self._create_internal_dictionary(
             tags_dictionary_path
         )
-        self.paired_stag_prefix, self.paired_stag_suffix = \
-            map(str, paired_start_tag.split("#"))
-        self.paired_etag_prefix, self.paired_etag_suffix = \
-            map(str, paired_end_tag.split("#"))
-        self.isolated_tag_prefix, self.isolated_tag_suffix = \
-            map(str, isolated_tag.split("#"))
+        self.paired_stag_prefix, self.paired_stag_suffix = map(
+            str, paired_start_tag.split("#")
+        )
+        self.paired_etag_prefix, self.paired_etag_suffix = map(
+            str, paired_end_tag.split("#")
+        )
+        self.isolated_tag_prefix, self.isolated_tag_suffix = map(
+            str, isolated_tag.split("#")
+        )
 
         self.automaton = self._create_automaton()
 
     def _create_internal_dictionary(self, tags_dictionary_path):
-        logger.debug('Creating tag dictionary for tagging transform...')
+        logger.debug("Creating tag dictionary for tagging transform...")
         dictionary = list()
-        with open(tags_dictionary_path, mode='r', encoding='utf-8') as file:
+        with open(tags_dictionary_path, mode="r", encoding="utf-8") as file:
             pairs = file.readlines()
             for pair in pairs:
-                src_term, tgt_term = map(str, pair.split('\t'))
+                src_term, tgt_term = map(str, pair.split("\t"))
                 dictionary.append((src_term.strip(), tgt_term.strip()))
-        logger.debug(f'Created tag dictionary with {len(dictionary)} entries.')
+        logger.debug(f"Created tag dictionary with {len(dictionary)} entries.")
         return dictionary
 
     def _create_automaton(self):
         automaton = ahocorasick.Automaton()
         for entry in self.internal_dictionary:
             automaton.add_word(entry[0], (entry[0], entry[1]))
 
@@ -61,16 +68,17 @@
     def _tagged_src_tgt(self, src_example, tgt_example):
         """Uses the dictionary to find exact source matches with corresponding
         target matches and adds both paired tags and standalone tags."""
 
         maybe_augmented = src_example.split(self.src_delimiter)
         source_only = maybe_augmented[0].strip()
 
-        augmented_part = maybe_augmented[1].strip() \
-            if len(maybe_augmented) > 1 else None
+        augmented_part = (
+            maybe_augmented[1].strip() if len(maybe_augmented) > 1 else None
+        )
 
         tokenized_source_string = source_only.split()
         tokenized_target_string = tgt_example.split()
 
         src_offset, tgt_offset = 0, 0
         src_with_tags, tgt_with_tags = list(), list()
 
@@ -78,20 +86,18 @@
         # to 12 + the number of subsequent tags that
         # will be added. We also apply weights to this choice so tags
         # are more probable to start from 1, then from 2, etc.
         # This way we cover most scenarios met in real usage and
         # the system will learn to handle a fairly large number of
         # numbered tags (but not an excessively large number)
         paired_tag_start_num = random.choices(
-            range(1, self.max_tags + 1),
-            weights=range(self.max_tags, 0, -1), k=1
+            range(1, self.max_tags + 1), weights=range(self.max_tags, 0, -1), k=1
         )[0]
         single_tag_start_num = random.choices(
-            range(1, self.max_tags + 1),
-            weights=range(self.max_tags, 0, -1), k=1
+            range(1, self.max_tags + 1), weights=range(self.max_tags, 0, -1), k=1
         )[0]
 
         is_match = False
         tag_counter = 0
 
         for src_match_end, pair in self.automaton.iter_long(source_only):
             if tag_counter == self.max_tags:
@@ -100,15 +106,15 @@
             src_match_start = src_match_end - len(pair[0]) + 1
             tgt_match_start = tgt_example.find(pair[1], tgt_offset)
             tgt_match_end = tgt_match_start + len(pair[1])
 
             # Make sure we only search for exact matches (we don't want
             # to match part of words) and perform some bound checking
             if (
-                (pair[1] not in ' '.join(tokenized_target_string))
+                (pair[1] not in " ".join(tokenized_target_string))
                 or (
                     len(source_only) != src_match_end + 1
                     and not (
                         source_only[src_match_end + 1].isspace()
                         or source_only[src_match_end + 1] in string.punctuation
                     )
                 )
@@ -131,53 +137,53 @@
                 for i, w in enumerate(tokenized_target_string):
                     if target_index == tgt_match_start:
                         target_index = i
                         break
                     else:
                         target_index += len(w) + 1
 
-                src_term = ' '.join(
+                src_term = " ".join(
                     tokenized_source_string[
-                        source_index: source_index + len(pair[0].split())
+                        source_index : source_index + len(pair[0].split())
                     ]
                 )
-                tgt_term = ' '.join(
+                tgt_term = " ".join(
                     tokenized_target_string[
-                        target_index: target_index + len(pair[1].split())
+                        target_index : target_index + len(pair[1].split())
                     ]
                 )
 
                 # Create all possible tag forms. We inject a special
                 # unicode char (∥) as a placeholder for whitespace in order
                 # to keep the indices unaltered. This char is replaced with
                 # spaces before we return the augmented examples.
                 src_single_tags = (
-                    f'{source_only[src_offset: src_match_start]}'
-                    f'{self.isolated_tag_prefix}{single_tag_start_num}'
-                    f'{self.isolated_tag_suffix}∥{src_term}∥'
+                    f"{source_only[src_offset: src_match_start]}"
+                    f"{self.isolated_tag_prefix}{single_tag_start_num}"
+                    f"{self.isolated_tag_suffix}∥{src_term}∥"
                 )
                 src_paired_tags = (
-                    f'{source_only[src_offset: src_match_start]}'
-                    f'{self.paired_stag_prefix}{paired_tag_start_num}'
-                    f'{self.paired_stag_suffix}∥{src_term}∥'
-                    f'{self.paired_etag_prefix}{paired_tag_start_num}'
-                    f'{self.paired_etag_suffix}'
+                    f"{source_only[src_offset: src_match_start]}"
+                    f"{self.paired_stag_prefix}{paired_tag_start_num}"
+                    f"{self.paired_stag_suffix}∥{src_term}∥"
+                    f"{self.paired_etag_prefix}{paired_tag_start_num}"
+                    f"{self.paired_etag_suffix}"
                 )
 
                 tgt_single_tags = (
-                    f'{tgt_example[tgt_offset: tgt_match_start]}'
-                    f'{self.isolated_tag_prefix}{single_tag_start_num}'
-                    f'{self.isolated_tag_suffix}∥{tgt_term}∥'
+                    f"{tgt_example[tgt_offset: tgt_match_start]}"
+                    f"{self.isolated_tag_prefix}{single_tag_start_num}"
+                    f"{self.isolated_tag_suffix}∥{tgt_term}∥"
                 )
                 tgt_paired_tags = (
-                    f'{tgt_example[tgt_offset: tgt_match_start]}'
-                    f'{self.paired_stag_prefix}{paired_tag_start_num}'
-                    f'{self.paired_stag_suffix}∥{tgt_term}∥'
-                    f'{self.paired_etag_prefix}{paired_tag_start_num}'
-                    f'{self.paired_etag_suffix}'
+                    f"{tgt_example[tgt_offset: tgt_match_start]}"
+                    f"{self.paired_stag_prefix}{paired_tag_start_num}"
+                    f"{self.paired_stag_suffix}∥{tgt_term}∥"
+                    f"{self.paired_etag_prefix}{paired_tag_start_num}"
+                    f"{self.paired_etag_suffix}"
                 )
 
                 # Make a weighted choice between paired tags or single tags.
                 # We usually encounter, and thus here we favor, paired tags
                 # with a ratio 1/3.
                 choice = random.choices(
                     [src_single_tags, src_paired_tags], weights=(1, 3), k=1
@@ -194,126 +200,160 @@
                     paired_tag_start_num += 1
 
                 tgt_offset = tgt_match_end + 1
                 tag_counter += 1
                 is_match = True
         if is_match:
             if augmented_part is not None:
-                src_with_tags.append(source_only[src_offset:] +
-                                     self.src_delimiter +
-                                     augmented_part)
+                src_with_tags.append(
+                    source_only[src_offset:] + self.src_delimiter + augmented_part
+                )
             else:
                 src_with_tags.append(source_only[src_offset:])
 
             tgt_with_tags.append(tgt_example[tgt_offset:])
 
             return (
-                ''.join(src_with_tags).replace('∥', ' ').split(),
-                ''.join(tgt_with_tags).replace('∥', ' ').split(),
+                "".join(src_with_tags).replace("∥", " ").split(),
+                "".join(tgt_with_tags).replace("∥", " ").split(),
             )
         else:
             return (src_example.split(), tgt_example.split())
 
 
-@register_transform(name='inlinetags')
+@register_transform(name="inlinetags")
 class InlineTagsTransform(Transform):
     def __init__(self, opts):
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """Available options for adding inline tags."""
 
         group = parser.add_argument_group("Transform/InlineTags")
-        group.add("--tags_dictionary_path", "-tags_dictionary_path",
-                  type=str, help="Path to a flat term dictionary.")
-        group.add("--tags_corpus_ratio", "-tags_corpus_ratio", type=float,
-                  default=0.1, help="Ratio of corpus to augment with tags.")
-        group.add("--max_tags", "-max_tags", type=int,
-                  default=12,
-                  help="Maximum number of tags that can be added to "
-                  "a single sentence.")
-        group.add("--paired_stag", "-paired_stag",
-                  type=str, default='｟ph_#_beg｠',
-                  help="The format of an opening paired inline tag. "
-                  "Must include the character #.")
-        group.add("--paired_etag", "-paired_etag",
-                  type=str, default='｟ph_#_end｠',
-                  help="The format of a closing paired inline tag. "
-                  "Must include the character #.")
-        group.add("--isolated_tag", "-isolated_tag",
-                  type=str, default='｟ph_#_std｠',
-                  help="The format of an isolated inline tag. "
-                  "Must include the character #.")
-        group.add("--src_delimiter", "-src_delimiter", type=str,
-                  default='｟fuzzy｠',
-                  help="Any special token used for augmented src sentences. "
-                  "The default is the fuzzy token used in the "
-                  "FuzzyMatch transform.")
+        group.add(
+            "--tags_dictionary_path",
+            "-tags_dictionary_path",
+            type=str,
+            help="Path to a flat term dictionary.",
+        )
+        group.add(
+            "--tags_corpus_ratio",
+            "-tags_corpus_ratio",
+            type=float,
+            default=0.1,
+            help="Ratio of corpus to augment with tags.",
+        )
+        group.add(
+            "--max_tags",
+            "-max_tags",
+            type=int,
+            default=12,
+            help="Maximum number of tags that can be added to " "a single sentence.",
+        )
+        group.add(
+            "--paired_stag",
+            "-paired_stag",
+            type=str,
+            default="｟ph_#_beg｠",
+            help="The format of an opening paired inline tag. "
+            "Must include the character #.",
+        )
+        group.add(
+            "--paired_etag",
+            "-paired_etag",
+            type=str,
+            default="｟ph_#_end｠",
+            help="The format of a closing paired inline tag. "
+            "Must include the character #.",
+        )
+        group.add(
+            "--isolated_tag",
+            "-isolated_tag",
+            type=str,
+            default="｟ph_#_std｠",
+            help="The format of an isolated inline tag. "
+            "Must include the character #.",
+        )
+        group.add(
+            "--src_delimiter",
+            "-src_delimiter",
+            type=str,
+            default="｟fuzzy｠",
+            help="Any special token used for augmented src sentences. "
+            "The default is the fuzzy token used in the "
+            "FuzzyMatch transform.",
+        )
 
     def _parse_opts(self):
         self.tags_dictionary_path = self.opts.tags_dictionary_path
         self.tags_corpus_ratio = self.opts.tags_corpus_ratio
         self.max_tags = self.opts.max_tags
         self.src_delimiter = self.opts.src_delimiter
-        self.paired_stag = self.opts.paired_stag,
-        self.paired_etag = self.opts.paired_etag,
-        self.isolated_tag = self.opts.isolated_tag,
+        self.paired_stag = (self.opts.paired_stag,)
+        self.paired_etag = (self.opts.paired_etag,)
+        self.isolated_tag = (self.opts.isolated_tag,)
 
     @classmethod
     def get_specials(cls, opts):
         """Add up to self.max_tags * 2 placeholders to src and tgt vocabs."""
 
         # Check if the tags include the
         # mandatory "#" number placeholder"
-        if "#" not in opts.paired_stag or \
-           "#" not in opts.paired_etag or \
-           "#" not in opts.isolated_tag:
-            logger.error('Inline tags must include the number '
-                         'placeholder \"#\"')
+        if (
+            "#" not in opts.paired_stag
+            or "#" not in opts.paired_etag
+            or "#" not in opts.isolated_tag
+        ):
+            logger.error("Inline tags must include the number " 'placeholder "#"')
 
         # We split the user-defined tags in the # placeholder
         # in order to number them
-        paired_stag_prefix, paired_stag_suffix = \
-            map(str, opts.paired_stag.split('#'))
-        paired_etag_prefix, paired_etag_suffix = \
-            map(str, opts.paired_etag.split('#'))
-        isolated_tag_prefix, isolated_tag_suffix = \
-            map(str, opts.isolated_tag.split('#'))
+        paired_stag_prefix, paired_stag_suffix = map(str, opts.paired_stag.split("#"))
+        paired_etag_prefix, paired_etag_suffix = map(str, opts.paired_etag.split("#"))
+        isolated_tag_prefix, isolated_tag_suffix = map(
+            str, opts.isolated_tag.split("#")
+        )
 
         src_specials, tgt_specials = list(), list()
         tags = list()
         for i in range(1, opts.max_tags * 2):
-            tags.extend([paired_stag_prefix + str(i) + paired_stag_suffix,
-                         paired_etag_prefix + str(i) + paired_etag_suffix,
-                         isolated_tag_prefix + str(i) + isolated_tag_suffix])
+            tags.extend(
+                [
+                    paired_stag_prefix + str(i) + paired_stag_suffix,
+                    paired_etag_prefix + str(i) + paired_etag_suffix,
+                    isolated_tag_prefix + str(i) + isolated_tag_suffix,
+                ]
+            )
 
         src_specials.extend(tags)
         tgt_specials.extend(tags)
 
         return (src_specials, tgt_specials)
 
     def warm_up(self, vocabs=None):
         """Create the tagger."""
 
         super().warm_up(None)
-        self.tagger = InlineTagger(self.tags_dictionary_path,
-                                   self.max_tags,
-                                   self.paired_stag,
-                                   self.paired_etag,
-                                   self.isolated_tag,
-                                   self.src_delimiter,
-                                   self.tags_corpus_ratio)
+        self.tagger = InlineTagger(
+            self.tags_dictionary_path,
+            self.max_tags,
+            self.paired_stag,
+            self.paired_etag,
+            self.isolated_tag,
+            self.src_delimiter,
+            self.tags_corpus_ratio,
+        )
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Add tags (placeholders) to source and target segments."""
 
         if random.random() > self.tags_corpus_ratio:
             return example
 
         src_tgt_pair = self.tagger._tagged_src_tgt(
-            ' '.join(example['src']), ' '.join(example['tgt'])
+            " ".join(example["src"]), " ".join(example["tgt"])
         )
-        example['src'] = src_tgt_pair[0]
-        example['tgt'] = src_tgt_pair[1]
+        example["src"] = src_tgt_pair[0]
+        example["tgt"] = src_tgt_pair[1]
 
         return example
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/misc.py` & `OpenNMT-py-3.1.3/onmt/transforms/misc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,128 +1,147 @@
 from onmt.utils.logging import logger
 from onmt.transforms import register_transform
 from .transform import Transform, ObservableStats
 
 
 class FilterTooLongStats(ObservableStats):
     """Runing statistics for FilterTooLongTransform."""
+
     __slots__ = ["filtered"]
 
     def __init__(self):
         self.filtered = 1
 
     def update(self, other: "FilterTooLongStats"):
         self.filtered += other.filtered
 
 
-@register_transform(name='filtertoolong')
+@register_transform(name="filtertoolong")
 class FilterTooLongTransform(Transform):
     """Filter out sentence that are too long."""
 
     def __init__(self, opts):
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """
         Available options relate to this Transform.
         For performance it is better to use multiple of 8
         On target side, since we'll add BOS/EOS, we filter with minus 2
         """
         group = parser.add_argument_group("Transform/Filter")
-        group.add("--src_seq_length", "-src_seq_length", type=int, default=192,
-                  help="Maximum source sequence length.")
-        group.add("--tgt_seq_length", "-tgt_seq_length", type=int, default=192,
-                  help="Maximum target sequence length.")
+        group.add(
+            "--src_seq_length",
+            "-src_seq_length",
+            type=int,
+            default=192,
+            help="Maximum source sequence length.",
+        )
+        group.add(
+            "--tgt_seq_length",
+            "-tgt_seq_length",
+            type=int,
+            default=192,
+            help="Maximum target sequence length.",
+        )
 
     def _parse_opts(self):
         self.src_seq_length = self.opts.src_seq_length
         self.tgt_seq_length = self.opts.tgt_seq_length
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Return None if too long else return as is."""
-        if (len(example['src']) > self.src_seq_length or
-                len(example['tgt']) > self.tgt_seq_length - 2):
+        if (
+            len(example["src"]) > self.src_seq_length
+            or len(example["tgt"]) > self.tgt_seq_length - 2
+        ):
             if stats is not None:
                 stats.update(FilterTooLongStats())
             return None
         else:
             return example
 
     def _repr_args(self):
         """Return str represent key arguments for class."""
-        return '{}={}, {}={}'.format(
-            'src_seq_length', self.src_seq_length,
-            'tgt_seq_length', self.tgt_seq_length
+        return "{}={}, {}={}".format(
+            "src_seq_length", self.src_seq_length, "tgt_seq_length", self.tgt_seq_length
         )
 
 
-@register_transform(name='prefix')
+@register_transform(name="prefix")
 class PrefixTransform(Transform):
     """Add Prefix to src (& tgt) sentence."""
 
     def __init__(self, opts):
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """Avalailable options relate to this Transform."""
         group = parser.add_argument_group("Transform/Prefix")
-        group.add("--src_prefix", "-src_prefix", type=str, default="",
-                  help="String to prepend to all source example.")
-        group.add("--tgt_prefix", "-tgt_prefix", type=str, default="",
-                  help="String to prepend to all target example.")
+        group.add(
+            "--src_prefix",
+            "-src_prefix",
+            type=str,
+            default="",
+            help="String to prepend to all source example.",
+        )
+        group.add(
+            "--tgt_prefix",
+            "-tgt_prefix",
+            type=str,
+            default="",
+            help="String to prepend to all target example.",
+        )
 
     @staticmethod
     def _get_prefix(corpus):
         """Get prefix string of a `corpus`."""
-        if 'prefix' in corpus['transforms']:
-            src_prefix = corpus.get('src_prefix', "")
-            tgt_prefix = corpus.get('tgt_prefix', "")
-            prefix = {
-                'src': src_prefix,
-                'tgt': tgt_prefix
-            }
+        if "prefix" in corpus["transforms"]:
+            src_prefix = corpus.get("src_prefix", "")
+            tgt_prefix = corpus.get("tgt_prefix", "")
+            prefix = {"src": src_prefix, "tgt": tgt_prefix}
         else:
             prefix = None
         return prefix
 
     @classmethod
     def get_prefix_dict(cls, opts):
         """Get all needed prefix correspond to corpus in `opts`."""
         prefix_dict = {}
         # prefix src/tgt for each dataset
-        if hasattr(opts, 'data'):
+        if hasattr(opts, "data"):
             for c_name, corpus in opts.data.items():
                 prefix = cls._get_prefix(corpus)
                 if prefix is not None:
                     logger.debug(f"Get prefix for {c_name}: {prefix}")
                     prefix_dict[c_name] = prefix
         # prefix as general option for inference
-        if hasattr(opts, 'src_prefix'):
-            if 'infer' not in prefix_dict.keys():
-                prefix_dict['infer'] = {}
-            prefix_dict['infer']['src'] = opts.src_prefix
+        if hasattr(opts, "src_prefix"):
+            if "infer" not in prefix_dict.keys():
+                prefix_dict["infer"] = {}
+            prefix_dict["infer"]["src"] = opts.src_prefix
             logger.debug(f"Get prefix for src infer: {opts.src_prefix}")
-        if hasattr(opts, 'tgt_prefix'):
-            if 'infer' not in prefix_dict.keys():
-                prefix_dict['infer'] = {}
-            prefix_dict['infer']['tgt'] = opts.tgt_prefix
+        if hasattr(opts, "tgt_prefix"):
+            if "infer" not in prefix_dict.keys():
+                prefix_dict["infer"] = {}
+            prefix_dict["infer"]["tgt"] = opts.tgt_prefix
             logger.debug(f"Get prefix for tgt infer: {opts.tgt_prefix}")
 
         return prefix_dict
 
     @classmethod
     def get_specials(cls, opts):
         """Get special vocabs added by prefix transform."""
         prefix_dict = cls.get_prefix_dict(opts)
         src_specials, tgt_specials = set(), set()
         for _, prefix in prefix_dict.items():
-            src_specials.update(prefix['src'].split())
-            tgt_specials.update(prefix['tgt'].split())
+            src_specials.update(prefix["src"].split())
+            tgt_specials.update(prefix["tgt"].split())
         return (src_specials, tgt_specials)
 
     def warm_up(self, vocabs=None):
         """Warm up to get prefix dictionary."""
         super().warm_up(None)
         self.prefix_dict = self.get_prefix_dict(self.opts)
 
@@ -136,99 +155,107 @@
         return example
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Apply prefix prepend to example.
 
         Should provide `corpus_name` to get correspond prefix.
         """
-        corpus_name = kwargs.get('corpus_name', None)
+        corpus_name = kwargs.get("corpus_name", None)
         if corpus_name is None:
-            raise ValueError('corpus_name is required.')
+            raise ValueError("corpus_name is required.")
         corpus_prefix = self.prefix_dict.get(corpus_name, None)
         if corpus_prefix is None:
-            raise ValueError(f'prefix for {corpus_name} does not exist.')
+            raise ValueError(f"prefix for {corpus_name} does not exist.")
         return self._prepend(example, corpus_prefix)
 
     def apply_reverse(self, translated):
         def _removeprefix(s, prefix):
             if s.startswith(prefix) and len(prefix) > 0:
-                return s[len(prefix) + 1:]
+                return s[len(prefix) + 1 :]
             else:
                 return s
-        corpus_prefix = self.prefix_dict.get('infer', None)
-        return _removeprefix(translated, corpus_prefix['tgt'])
+
+        corpus_prefix = self.prefix_dict.get("infer", None)
+        return _removeprefix(translated, corpus_prefix["tgt"])
 
     def _repr_args(self):
         """Return str represent key arguments for class."""
-        return '{}={}'.format('prefix_dict', self.prefix_dict)
+        return "{}={}".format("prefix_dict", self.prefix_dict)
 
 
-@register_transform(name='suffix')
+@register_transform(name="suffix")
 class SuffixTransform(Transform):
     """Add Suffix to src (& tgt) sentence."""
 
     def __init__(self, opts):
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """Avalailable options relate to this Transform."""
         group = parser.add_argument_group("Transform/Suffix")
-        group.add("--src_suffix", "-src_suffix", type=str, default="",
-                  help="String to append to all source example.")
-        group.add("--tgt_suffix", "-tgt_suffix", type=str, default="",
-                  help="String to append to all target example.")
+        group.add(
+            "--src_suffix",
+            "-src_suffix",
+            type=str,
+            default="",
+            help="String to append to all source example.",
+        )
+        group.add(
+            "--tgt_suffix",
+            "-tgt_suffix",
+            type=str,
+            default="",
+            help="String to append to all target example.",
+        )
 
     @staticmethod
     def _get_suffix(corpus):
         """Get suffix string of a `corpus`."""
-        if 'suffix' in corpus['transforms']:
-            src_suffix = corpus.get('src_suffix', "")
-            tgt_suffix = corpus.get('tgt_suffix', "")
-            suffix = {
-                'src': src_suffix,
-                'tgt': tgt_suffix
-            }
+        if "suffix" in corpus["transforms"]:
+            src_suffix = corpus.get("src_suffix", "")
+            tgt_suffix = corpus.get("tgt_suffix", "")
+            suffix = {"src": src_suffix, "tgt": tgt_suffix}
         else:
             suffix = None
         return suffix
 
     @classmethod
     def get_suffix_dict(cls, opts):
         """Get all needed suffix correspond to corpus in `opts`."""
         suffix_dict = {}
         # suffix src/tgt for each dataset
-        if hasattr(opts, 'data'):
+        if hasattr(opts, "data"):
             for c_name, corpus in opts.data.items():
                 suffix = cls._get_suffix(corpus)
                 if suffix is not None:
                     logger.debug(f"Get suffix for {c_name}: {suffix}")
                     suffix_dict[c_name] = suffix
         # suffix as general option for inference
-        if hasattr(opts, 'src_suffix'):
-            if 'infer' not in suffix_dict.keys():
-                suffix_dict['infer'] = {}
-            suffix_dict['infer']['src'] = opts.src_suffix
+        if hasattr(opts, "src_suffix"):
+            if "infer" not in suffix_dict.keys():
+                suffix_dict["infer"] = {}
+            suffix_dict["infer"]["src"] = opts.src_suffix
             logger.debug(f"Get suffix for src infer: {opts.src_suffix}")
-        if hasattr(opts, 'tgt_suffix'):
-            if 'infer' not in suffix_dict.keys():
-                suffix_dict['infer'] = {}
-            suffix_dict['infer']['tgt'] = opts.tgt_suffix
+        if hasattr(opts, "tgt_suffix"):
+            if "infer" not in suffix_dict.keys():
+                suffix_dict["infer"] = {}
+            suffix_dict["infer"]["tgt"] = opts.tgt_suffix
             logger.debug(f"Get suffix for tgt infer: {opts.tgt_suffix}")
 
         return suffix_dict
 
     @classmethod
     def get_specials(cls, opts):
         """Get special vocabs added by suffix transform."""
         suffix_dict = cls.get_suffix_dict(opts)
         src_specials, tgt_specials = set(), set()
         for _, suffix in suffix_dict.items():
-            src_specials.update(suffix['src'].split())
-            tgt_specials.update(suffix['tgt'].split())
+            src_specials.update(suffix["src"].split())
+            tgt_specials.update(suffix["tgt"].split())
         return (src_specials, tgt_specials)
 
     def warm_up(self, vocabs=None):
         """Warm up to get suffix dictionary."""
         super().warm_up(None)
         self.suffix_dict = self.get_suffix_dict(self.opts)
 
@@ -242,18 +269,18 @@
         return example
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Apply suffix append to example.
 
         Should provide `corpus_name` to get correspond suffix.
         """
-        corpus_name = kwargs.get('corpus_name', None)
+        corpus_name = kwargs.get("corpus_name", None)
         if corpus_name is None:
-            raise ValueError('corpus_name is required.')
+            raise ValueError("corpus_name is required.")
         corpus_suffix = self.suffix_dict.get(corpus_name, None)
         if corpus_suffix is None:
-            raise ValueError(f'suffix for {corpus_name} does not exist.')
+            raise ValueError(f"suffix for {corpus_name} does not exist.")
         return self._append(example, corpus_suffix)
 
     def _repr_args(self):
         """Return str represent key arguments for class."""
-        return '{}={}'.format('suffix_dict', self.suffix_dict)
+        return "{}={}".format("suffix_dict", self.suffix_dict)
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/normalize.py` & `OpenNMT-py-3.1.3/onmt/transforms/normalize.py`

 * *Files 7% similar despite different names*

```diff
@@ -132,25 +132,26 @@
         ("〉", ">"),
         ("【", "["),
         ("】", "]"),
         ("％", "%"),
     ]
 
     def __init__(self):
-        """
-        """
+        """ """
 
-    def normalize(self,
-                  text,
-                  lang="en",
-                  penn=True,
-                  norm_quote_commas=True,
-                  norm_numbers=True,
-                  pre_replace_unicode_punct=False,
-                  post_remove_control_chars=False):
+    def normalize(
+        self,
+        text,
+        lang="en",
+        penn=True,
+        norm_quote_commas=True,
+        norm_numbers=True,
+        pre_replace_unicode_punct=False,
+        post_remove_control_chars=False,
+    ):
         """
         Returns a string with normalized punctuation.
         :param language: The two-letter language code.
         :type lang: str
         :param penn: Normalize Penn Treebank style quotations.
         :type penn: bool
         :param norm_quote_commas: Normalize quotations and commas
@@ -169,16 +170,15 @@
             # Adds the penn substitutions after extra_whitespace regexes.
             self.substitutions.insert(1, self.NORMALIZE_UNICODE_IF_NOT_PENN)
 
         if norm_quote_commas:
             if lang == "en":
                 self.substitutions.append(self.EN_QUOTATION_FOLLOWED_BY_COMMA)
             elif lang in ["de", "es", "fr"]:
-                self.substitutions.append(
-                    self.DE_ES_FR_QUOTATION_FOLLOWED_BY_COMMA)
+                self.substitutions.append(self.DE_ES_FR_QUOTATION_FOLLOWED_BY_COMMA)
 
         if norm_numbers:
             if lang in ["de", "es", "cz", "cs", "fr"]:
                 self.substitutions.append(self.DE_ES_CZ_CS_FR)
             else:
                 self.substitutions.append(self.OTHER)
 
@@ -203,125 +203,144 @@
             text = re.sub(regexp, substitution, str(text))
         return text
 
     def remove_control_chars(self, text):
         return regex.sub(r"\p{C}", "", text)
 
 
-@register_transform(name='normalize')
+@register_transform(name="normalize")
 class NormalizeTransform(Transform):
     """
     Normalize source and target based on Moses script.
     """
 
     def __init__(self, opts):
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """Add an option for the corpus ratio to apply this transform."""
 
         group = parser.add_argument_group("Transform/Normalize")
-        group.add("--src_lang", "-src_lang", type=str,
-                  default="", help="Source language code")
-        group.add("--tgt_lang", "-tgt_lang", type=str,
-                  default="", help="Target language code")
-        group.add("--penn", "-penn", type=bool,
-                  default=True, help="Penn substitution")
-        group.add("--norm_quote_commas", "-norm_quote_commas", type=bool,
-                  default=True, help="Normalize quotations and commas")
-        group.add("--norm_numbers", "-norm_numbers", type=bool,
-                  default=True, help="Normalize numbers")
-        group.add("--pre_replace_unicode_punct", "-pre_replace_unicode_punct",
-                  type=bool, default=False, help="Replace unicode punct")
-        group.add("--post_remove_control_chars", "-post_remove_control_chars",
-                  type=bool, default=False, help="Remove control chars")
+        group.add(
+            "--src_lang", "-src_lang", type=str, default="", help="Source language code"
+        )
+        group.add(
+            "--tgt_lang", "-tgt_lang", type=str, default="", help="Target language code"
+        )
+        group.add("--penn", "-penn", type=bool, default=True, help="Penn substitution")
+        group.add(
+            "--norm_quote_commas",
+            "-norm_quote_commas",
+            type=bool,
+            default=True,
+            help="Normalize quotations and commas",
+        )
+        group.add(
+            "--norm_numbers",
+            "-norm_numbers",
+            type=bool,
+            default=True,
+            help="Normalize numbers",
+        )
+        group.add(
+            "--pre_replace_unicode_punct",
+            "-pre_replace_unicode_punct",
+            type=bool,
+            default=False,
+            help="Replace unicode punct",
+        )
+        group.add(
+            "--post_remove_control_chars",
+            "-post_remove_control_chars",
+            type=bool,
+            default=False,
+            help="Remove control chars",
+        )
 
     def _parse_opts(self):
         self.src_lang = self.opts.src_lang
         self.tgt_lang = self.opts.tgt_lang
         self.penn = self.opts.penn
         self.norm_quote_commas = self.opts.norm_quote_commas
         self.norm_numbers = self.opts.norm_numbers
         self.pre_replace_unicode_punct = self.opts.pre_replace_unicode_punct
         self.post_remove_control_chars = self.opts.post_remove_control_chars
 
     @staticmethod
     def _get_opt(corpus, opt, def_val):
         """Get opt string of a `corpus`."""
-        if 'normalize' in corpus['transforms']:
+        if "normalize" in corpus["transforms"]:
             value = corpus.get(opt, def_val)
             normalize = value
         else:
             normalize = None
         return normalize
 
     @classmethod
     def get_opt_dict(cls, opts, opt, def_val):
         """Get normalize settings correspond to corpus in `opts`."""
         normalize_dict = {}
         # normalize dict src/tgt for each dataset
-        if hasattr(opts, 'data'):
+        if hasattr(opts, "data"):
             for c_name, corpus in opts.data.items():
                 normalize = cls._get_opt(corpus, opt, def_val)
                 if normalize is not None:
                     logger.debug(f"Get {opt} for {c_name}: {normalize}")
                     normalize_dict[c_name] = normalize
 
         return normalize_dict
 
     def warm_up(self, vocabs=None):
         """Set options for each dataset."""
         super().warm_up(None)
-        self.src_lang_dict = self.get_opt_dict(self.opts, 'src_lang', '')
-        self.tgt_lang_dict = self.get_opt_dict(self.opts, 'tgt_lang', '')
-        self.penn_dict = self.get_opt_dict(self.opts, 'penn', True)
-        self.norm_quote_commas_dict = self.get_opt_dict(self.opts,
-                                                        'norm_quote_commas',
-                                                        True)
-        self.norm_numbers_dict = self.get_opt_dict(self.opts, 'norm_numbers',
-                                                   True)
-        self.pre_dict = self.get_opt_dict(self.opts,
-                                          'pre_replace_unicode_punct',
-                                          False)
-        self.post_dict = self.get_opt_dict(self.opts,
-                                           'post_remove_control_chars',
-                                           False)
-        self.src_lang_dict['infer'] = self.src_lang
-        self.tgt_lang_dict['infer'] = self.tgt_lang
-        self.penn_dict['infer'] = self.penn
-        self.norm_quote_commas_dict['infer'] = self.norm_quote_commas
-        self.norm_numbers_dict['infer'] = self.norm_numbers
-        self.pre_dict['infer'] = self.pre_replace_unicode_punct
-        self.post_dict['infer'] = self.post_remove_control_chars
+        self.src_lang_dict = self.get_opt_dict(self.opts, "src_lang", "")
+        self.tgt_lang_dict = self.get_opt_dict(self.opts, "tgt_lang", "")
+        self.penn_dict = self.get_opt_dict(self.opts, "penn", True)
+        self.norm_quote_commas_dict = self.get_opt_dict(
+            self.opts, "norm_quote_commas", True
+        )
+        self.norm_numbers_dict = self.get_opt_dict(self.opts, "norm_numbers", True)
+        self.pre_dict = self.get_opt_dict(self.opts, "pre_replace_unicode_punct", False)
+        self.post_dict = self.get_opt_dict(
+            self.opts, "post_remove_control_chars", False
+        )
+        self.src_lang_dict["infer"] = self.src_lang
+        self.tgt_lang_dict["infer"] = self.tgt_lang
+        self.penn_dict["infer"] = self.penn
+        self.norm_quote_commas_dict["infer"] = self.norm_quote_commas
+        self.norm_numbers_dict["infer"] = self.norm_numbers
+        self.pre_dict["infer"] = self.pre_replace_unicode_punct
+        self.post_dict["infer"] = self.post_remove_control_chars
 
-        self.mpn =\
-            MosesPunctNormalizer()
+        self.mpn = MosesPunctNormalizer()
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Normalize source and target examples."""
-        corpus_name = kwargs.get('corpus_name', None)
+        corpus_name = kwargs.get("corpus_name", None)
         if corpus_name is None:
-            raise ValueError('corpus_name is required.')
+            raise ValueError("corpus_name is required.")
 
         src_str = self.mpn.normalize(
-            ' '.join(example['src']),
+            " ".join(example["src"]),
             self.src_lang_dict[corpus_name],
             self.penn_dict[corpus_name],
             self.norm_quote_commas_dict[corpus_name],
             self.norm_numbers_dict[corpus_name],
             self.pre_dict[corpus_name],
-            self.post_dict[corpus_name])
-        example['src'] = src_str.split()
+            self.post_dict[corpus_name],
+        )
+        example["src"] = src_str.split()
 
-        if example['tgt'] is not None:
+        if example["tgt"] is not None:
             tgt_str = self.mpn.normalize(
-                ' '.join(example['tgt']),
+                " ".join(example["tgt"]),
                 self.tgt_lang_dict[corpus_name],
                 self.penn_dict[corpus_name],
                 self.norm_quote_commas_dict[corpus_name],
                 self.norm_numbers_dict[corpus_name],
                 self.pre_dict[corpus_name],
-                self.post_dict[corpus_name])
-            example['tgt'] = tgt_str.split()
+                self.post_dict[corpus_name],
+            )
+            example["tgt"] = tgt_str.split()
 
         return example
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/sampling.py` & `OpenNMT-py-3.1.3/onmt/transforms/sampling.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .transform import Transform, ObservableStats
 
 
 class HammingDistanceSampling(object):
     """Functions related to (negative) Hamming Distance Sampling."""
 
     def _softmax(self, x):
-        softmax = np.exp(x)/sum(np.exp(x))
+        softmax = np.exp(x) / sum(np.exp(x))
         return softmax
 
     def _sample_replace(self, vocab, reject):
         """Sample a token from `vocab` other than `reject`."""
         token = reject
         while token == reject:
             token = random.choice(vocab)
@@ -54,15 +54,15 @@
         self.total = total
 
     def update(self, other: "SwitchOutStats"):
         self.changed += other.changed
         self.total += other.total
 
 
-@register_transform(name='switchout')
+@register_transform(name="switchout")
 class SwitchOutTransform(HammingDistanceSamplingTransform):
     """
     SwitchOut.
     :cite:`DBLP:journals/corr/abs-1808-07512`
     """
 
     def __init__(self, opts):
@@ -73,19 +73,23 @@
         """Override this method to inform it need vocab to start."""
         return True
 
     @classmethod
     def add_options(cls, parser):
         """Avalilable options relate to this Transform."""
         group = parser.add_argument_group("Transform/SwitchOut")
-        group.add("-switchout_temperature", "--switchout_temperature",
-                  type=float, default=1.0,
-                  help="Sampling temperature for SwitchOut. :math:`\\tau^{-1}`"
-                       " in :cite:`DBLP:journals/corr/abs-1808-07512`. "
-                       "Smaller value makes data more diverse.")
+        group.add(
+            "-switchout_temperature",
+            "--switchout_temperature",
+            type=float,
+            default=1.0,
+            help="Sampling temperature for SwitchOut. :math:`\\tau^{-1}`"
+            " in :cite:`DBLP:journals/corr/abs-1808-07512`. "
+            "Smaller value makes data more diverse.",
+        )
 
     def _parse_opts(self):
         self.temperature = self.opts.switchout_temperature
 
     def _switchout(self, tokens, vocab, stats=None):
         # 1. sample number of tokens to corrupt
         n_chosen = self._sample_distance(tokens, self.temperature)
@@ -97,23 +101,25 @@
         if stats is not None:
             stats.update(SwitchOutStats(n_chosen, len(tokens)))
         return tokens
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Apply switchout to both src and tgt side tokens."""
         if is_train:
-            example['src'] = self._switchout(
-                example['src'], self.vocabs['src'].ids_to_tokens, stats)
-            example['tgt'] = self._switchout(
-                example['tgt'], self.vocabs['tgt'].ids_to_tokens, stats)
+            example["src"] = self._switchout(
+                example["src"], self.vocabs["src"].ids_to_tokens, stats
+            )
+            example["tgt"] = self._switchout(
+                example["tgt"], self.vocabs["tgt"].ids_to_tokens, stats
+            )
         return example
 
     def _repr_args(self):
         """Return str represent key arguments for class."""
-        return '{}={}'.format('switchout_temperature', self.temperature)
+        return "{}={}".format("switchout_temperature", self.temperature)
 
 
 class TokenDropStats(ObservableStats):
     """Runing statistics for counting tokens being switched out."""
 
     __slots__ = ["dropped", "total"]
 
@@ -122,55 +128,58 @@
         self.total = total
 
     def update(self, other: "TokenDropStats"):
         self.dropped += other.dropped
         self.total += other.total
 
 
-@register_transform(name='tokendrop')
+@register_transform(name="tokendrop")
 class TokenDropTransform(HammingDistanceSamplingTransform):
     """Random drop tokens from sentence."""
 
     def __init__(self, opts):
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """Avalilable options relate to this Transform."""
         group = parser.add_argument_group("Transform/Token_Drop")
-        group.add("-tokendrop_temperature", "--tokendrop_temperature",
-                  type=float, default=1.0,
-                  help="Sampling temperature for token deletion.")
+        group.add(
+            "-tokendrop_temperature",
+            "--tokendrop_temperature",
+            type=float,
+            default=1.0,
+            help="Sampling temperature for token deletion.",
+        )
 
     def _parse_opts(self):
         self.temperature = self.opts.tokendrop_temperature
 
     def _token_drop(self, tokens, stats=None):
         n_items = len(tokens)
         # 1. sample number of tokens to corrupt
         n_chosen = self._sample_distance(tokens, self.temperature)
         # 2. sample positions to corrput
         chosen_indices = self._sample_position(tokens, distance=n_chosen)
         # 3. Drop token on chosen position
-        out = [tok for (i, tok) in enumerate(tokens)
-               if i not in chosen_indices]
+        out = [tok for (i, tok) in enumerate(tokens) if i not in chosen_indices]
         if stats is not None:
             stats.update(TokenDropStats(n_chosen, n_items))
         return out
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Apply token drop to both src and tgt side tokens."""
         if is_train:
-            example['src'] = self._token_drop(example['src'], stats)
-            example['tgt'] = self._token_drop(example['tgt'], stats)
+            example["src"] = self._token_drop(example["src"], stats)
+            example["tgt"] = self._token_drop(example["tgt"], stats)
         return example
 
     def _repr_args(self):
         """Return str represent key arguments for class."""
-        return '{}={}'.format('tokendrop_temperature', self.temperature)
+        return "{}={}".format("tokendrop_temperature", self.temperature)
 
 
 class TokenMaskStats(ObservableStats):
     """Runing statistics for counting tokens being switched out."""
 
     __slots__ = ["masked", "total"]
 
@@ -179,30 +188,34 @@
         self.total = total
 
     def update(self, other: "TokenMaskStats"):
         self.masked += other.masked
         self.total += other.total
 
 
-@register_transform(name='tokenmask')
+@register_transform(name="tokenmask")
 class TokenMaskTransform(HammingDistanceSamplingTransform):
     """Random mask tokens from src sentence."""
 
     MASK_TOK = DefaultTokens.MASK
 
     def __init__(self, opts):
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """Avalilable options relate to this Transform."""
         group = parser.add_argument_group("Transform/Token_Mask")
-        group.add('-tokenmask_temperature', '--tokenmask_temperature',
-                  type=float, default=1.0,
-                  help="Sampling temperature for token masking.")
+        group.add(
+            "-tokenmask_temperature",
+            "--tokenmask_temperature",
+            type=float,
+            default=1.0,
+            help="Sampling temperature for token masking.",
+        )
 
     def _parse_opts(self):
         self.temperature = self.opts.tokenmask_temperature
 
     @classmethod
     def get_specials(cls, opts):
         """Get special vocabs added by prefix transform."""
@@ -219,13 +232,13 @@
         if stats is not None:
             stats.update(TokenDropStats(n_chosen, len(tokens)))
         return tokens
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Apply word drop to both src and tgt side tokens."""
         if is_train:
-            example['src'] = self._token_mask(example['src'], stats)
+            example["src"] = self._token_mask(example["src"], stats)
         return example
 
     def _repr_args(self):
         """Return str represent key arguments for class."""
-        return '{}={}'.format('tokenmask_temperature', self.temperature)
+        return "{}={}".format("tokenmask_temperature", self.temperature)
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/tokenize.py` & `OpenNMT-py-3.1.3/onmt/transforms/tokenize.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,74 +15,116 @@
 
     @classmethod
     def add_options(cls, parser):
         """Available options relate to Subword."""
         # Sharing options among `TokenizerTransform`s, same name conflict in
         # this scope will be resolved by remove previous occurrence in parser
         group = parser.add_argument_group(
-            'Transform/Subword/Common', conflict_handler='resolve',
+            "Transform/Subword/Common",
+            conflict_handler="resolve",
             description=".. Attention:: Common options shared by all subword transforms. "  # noqa: E501
             "Including options for indicate subword model path, "
             "`Subword Regularization <https://arxiv.org/abs/1804.10959>`_"
             "/`BPE-Dropout <https://arxiv.org/abs/1910.13267>`_, "
-            "and `Vocabulary Restriction <https://github.com/rsennrich/subword-nmt#best-practice-advice-for-byte-pair-encoding-in-nmt>`__.")  # noqa: E501
-        group.add('-src_subword_model', '--src_subword_model',
-                  help="Path of subword model for src (or shared).")
-        group.add("-tgt_subword_model", "--tgt_subword_model",
-                  help="Path of subword model for tgt.")
+            "and `Vocabulary Restriction <https://github.com/rsennrich/subword-nmt#best-practice-advice-for-byte-pair-encoding-in-nmt>`__.",  # noqa: E501
+        )  # noqa: E501
+        group.add(
+            "-src_subword_model",
+            "--src_subword_model",
+            help="Path of subword model for src (or shared).",
+        )
+        group.add(
+            "-tgt_subword_model",
+            "--tgt_subword_model",
+            help="Path of subword model for tgt.",
+        )
 
         # subword regularization(or BPE dropout) options:
-        group.add('-src_subword_nbest', '--src_subword_nbest',
-                  type=int, default=1,
-                  help="Number of candidates in subword regularization. "
-                       "Valid for unigram sampling, "
-                       "invalid for BPE-dropout. "
-                       "(source side)")
-        group.add('-tgt_subword_nbest', '--tgt_subword_nbest',
-                  type=int, default=1,
-                  help="Number of candidates in subword regularization. "
-                       "Valid for unigram sampling, "
-                       "invalid for BPE-dropout. "
-                       "(target side)")
-        group.add('-src_subword_alpha', '--src_subword_alpha',
-                  type=float, default=0,
-                  help="Smoothing parameter for sentencepiece unigram "
-                       "sampling, and dropout probability for BPE-dropout. "
-                       "(source side)")
-        group.add('-tgt_subword_alpha', '--tgt_subword_alpha',
-                  type=float, default=0,
-                  help="Smoothing parameter for sentencepiece unigram "
-                       "sampling, and dropout probability for BPE-dropout. "
-                       "(target side)")
+        group.add(
+            "-src_subword_nbest",
+            "--src_subword_nbest",
+            type=int,
+            default=1,
+            help="Number of candidates in subword regularization. "
+            "Valid for unigram sampling, "
+            "invalid for BPE-dropout. "
+            "(source side)",
+        )
+        group.add(
+            "-tgt_subword_nbest",
+            "--tgt_subword_nbest",
+            type=int,
+            default=1,
+            help="Number of candidates in subword regularization. "
+            "Valid for unigram sampling, "
+            "invalid for BPE-dropout. "
+            "(target side)",
+        )
+        group.add(
+            "-src_subword_alpha",
+            "--src_subword_alpha",
+            type=float,
+            default=0,
+            help="Smoothing parameter for sentencepiece unigram "
+            "sampling, and dropout probability for BPE-dropout. "
+            "(source side)",
+        )
+        group.add(
+            "-tgt_subword_alpha",
+            "--tgt_subword_alpha",
+            type=float,
+            default=0,
+            help="Smoothing parameter for sentencepiece unigram "
+            "sampling, and dropout probability for BPE-dropout. "
+            "(target side)",
+        )
 
         # subword vocabulary restriction options:
-        group.add('-src_subword_vocab', '--src_subword_vocab',
-                  type=str, default="",
-                  help="Path to the vocabulary file for src subword. "
-                  "Format: <word>\t<count> per line.")
-        group.add("-tgt_subword_vocab", "--tgt_subword_vocab",
-                  type=str, default="",
-                  help="Path to the vocabulary file for tgt subword. "
-                  "Format: <word>\t<count> per line.")
-        group.add('-src_vocab_threshold', '--src_vocab_threshold',
-                  type=int, default=0,
-                  help="Only produce src subword in src_subword_vocab with "
-                  " frequency >= src_vocab_threshold.")
-        group.add("-tgt_vocab_threshold", "--tgt_vocab_threshold",
-                  type=int, default=0,
-                  help="Only produce tgt subword in tgt_subword_vocab with "
-                  " frequency >= tgt_vocab_threshold.")
+        group.add(
+            "-src_subword_vocab",
+            "--src_subword_vocab",
+            type=str,
+            default="",
+            help="Path to the vocabulary file for src subword. "
+            "Format: <word>\t<count> per line.",
+        )
+        group.add(
+            "-tgt_subword_vocab",
+            "--tgt_subword_vocab",
+            type=str,
+            default="",
+            help="Path to the vocabulary file for tgt subword. "
+            "Format: <word>\t<count> per line.",
+        )
+        group.add(
+            "-src_vocab_threshold",
+            "--src_vocab_threshold",
+            type=int,
+            default=0,
+            help="Only produce src subword in src_subword_vocab with "
+            " frequency >= src_vocab_threshold.",
+        )
+        group.add(
+            "-tgt_vocab_threshold",
+            "--tgt_vocab_threshold",
+            type=int,
+            default=0,
+            help="Only produce tgt subword in tgt_subword_vocab with "
+            " frequency >= tgt_vocab_threshold.",
+        )
 
     @classmethod
     def _validate_options(cls, opts):
         """Extra checks for Subword options."""
-        assert 0 <= opts.src_subword_alpha <= 1, \
-            "src_subword_alpha should be in the range [0, 1]"
-        assert 0 <= opts.tgt_subword_alpha <= 1, \
-            "tgt_subword_alpha should be in the range [0, 1]"
+        assert (
+            0 <= opts.src_subword_alpha <= 1
+        ), "src_subword_alpha should be in the range [0, 1]"
+        assert (
+            0 <= opts.tgt_subword_alpha <= 1
+        ), "tgt_subword_alpha should be in the range [0, 1]"
 
     def _parse_opts(self):
         self.share_vocab = self.opts.share_vocab
         self.src_subword_model = self.opts.src_subword_model
         self.tgt_subword_model = self.opts.tgt_subword_model
         self.src_subword_nbest = self.opts.src_subword_nbest
         self.tgt_subword_nbest = self.opts.tgt_subword_nbest
@@ -92,25 +134,25 @@
         self.tgt_subword_vocab = self.opts.tgt_subword_vocab
         self.src_vocab_threshold = self.opts.src_vocab_threshold
         self.tgt_vocab_threshold = self.opts.tgt_vocab_threshold
 
     def _repr_args(self):
         """Return str represent key arguments for TokenizerTransform."""
         kwargs = {
-            'share_vocab': self.share_vocab,
-            'src_subword_model': self.src_subword_model,
-            'tgt_subword_model': self.tgt_subword_model,
-            'src_subword_alpha': self.src_subword_alpha,
-            'tgt_subword_alpha': self.tgt_subword_alpha,
-            'src_subword_vocab': self.src_subword_vocab,
-            'tgt_subword_vocab': self.tgt_subword_vocab,
-            'src_vocab_threshold': self.src_vocab_threshold,
-            'tgt_vocab_threshold': self.tgt_vocab_threshold
+            "share_vocab": self.share_vocab,
+            "src_subword_model": self.src_subword_model,
+            "tgt_subword_model": self.tgt_subword_model,
+            "src_subword_alpha": self.src_subword_alpha,
+            "tgt_subword_alpha": self.tgt_subword_alpha,
+            "src_subword_vocab": self.src_subword_vocab,
+            "tgt_subword_vocab": self.tgt_subword_vocab,
+            "src_vocab_threshold": self.src_vocab_threshold,
+            "tgt_vocab_threshold": self.tgt_vocab_threshold,
         }
-        return ', '.join([f'{kw}={arg}' for kw, arg in kwargs.items()])
+        return ", ".join([f"{kw}={arg}" for kw, arg in kwargs.items()])
 
 
 class SubwordStats(ObservableStats):
     """Runing statistics for counting tokens before/after subword transform."""
 
     __slots__ = ["subwords", "words"]
 
@@ -119,241 +161,263 @@
         self.words = words
 
     def update(self, other: "SubwordStats"):
         self.subwords += other.subwords
         self.words += other.words
 
     def __str__(self) -> str:
-        return "{}: {} -> {} tokens".format(
-            self.name(), self.words, self.subwords
-        )
+        return "{}: {} -> {} tokens".format(self.name(), self.words, self.subwords)
 
 
-@register_transform(name='sentencepiece')
+@register_transform(name="sentencepiece")
 class SentencePieceTransform(TokenizerTransform):
     """SentencePiece subword transform class."""
 
     def __init__(self, opts):
         """Initialize necessary options for sentencepiece."""
         super().__init__(opts)
 
     def _set_seed(self, seed):
         """set seed to ensure reproducibility."""
         import sentencepiece as spm
+
         spm.set_random_generator_seed(seed)
 
     def warm_up(self, vocabs=None):
         """Load subword models."""
         super().warm_up(None)
         import sentencepiece as spm
+
         load_src_model = spm.SentencePieceProcessor()
         load_src_model.Load(self.src_subword_model)
-        _diff_vocab = self.src_subword_vocab != self.tgt_subword_vocab or \
-            self.src_vocab_threshold != self.tgt_vocab_threshold
+        _diff_vocab = (
+            self.src_subword_vocab != self.tgt_subword_vocab
+            or self.src_vocab_threshold != self.tgt_vocab_threshold
+        )
         if self.src_subword_vocab != "" and self.src_vocab_threshold > 0:
             load_src_model.LoadVocabulary(
-                self.src_subword_vocab, self.src_vocab_threshold)
+                self.src_subword_vocab, self.src_vocab_threshold
+            )
         if self.share_vocab and not _diff_vocab:
-            self.load_models = {
-                'src': load_src_model,
-                'tgt': load_src_model
-            }
+            self.load_models = {"src": load_src_model, "tgt": load_src_model}
         else:
             load_tgt_model = spm.SentencePieceProcessor()
             load_tgt_model.Load(self.tgt_subword_model)
             if self.tgt_subword_vocab != "" and self.tgt_vocab_threshold > 0:
                 load_tgt_model.LoadVocabulary(
-                    self.tgt_subword_vocab, self.tgt_vocab_threshold)
-            self.load_models = {
-                'src': load_src_model,
-                'tgt': load_tgt_model
-            }
+                    self.tgt_subword_vocab, self.tgt_vocab_threshold
+                )
+            self.load_models = {"src": load_src_model, "tgt": load_tgt_model}
 
-    def _tokenize(self, tokens, side='src', is_train=False):
+    def _tokenize(self, tokens, side="src", is_train=False):
         """Do sentencepiece subword tokenize."""
         sp_model = self.load_models[side]
-        sentence = ' '.join(tokens).replace(DefaultTokens.SEP, '\n')
+        sentence = " ".join(tokens).replace(DefaultTokens.SEP, "\n")
         sent_list = sentence.split(DefaultTokens.EOS)
         segmented = []
         for sentence in sent_list:
-            nbest_size = self.tgt_subword_nbest if side == 'tgt' else \
-                self.src_subword_nbest
+            nbest_size = (
+                self.tgt_subword_nbest if side == "tgt" else self.src_subword_nbest
+            )
             if is_train is False or nbest_size in [0, 1]:
                 # derterministic subwording
                 segmented += sp_model.encode(sentence, out_type=str)
             else:
                 # subword sampling when nbest_size > 1 or -1
                 # alpha should be 0.0 < alpha < 1.0
-                alpha = self.tgt_subword_alpha if side == 'tgt' else \
-                    self.src_subword_alpha
+                alpha = (
+                    self.tgt_subword_alpha if side == "tgt" else self.src_subword_alpha
+                )
                 segmented += sp_model.encode(
-                    sentence, out_type=str, enable_sampling=True,
-                    alpha=alpha, nbest_size=nbest_size)
+                    sentence,
+                    out_type=str,
+                    enable_sampling=True,
+                    alpha=alpha,
+                    nbest_size=nbest_size,
+                )
             segmented += [DefaultTokens.EOS]
 
         return segmented[:-1]
 
     def _detokenize(self, tokens, side="src"):
         """Apply SentencePiece Detokenizer"""
         sp_model = self.load_models[side]
-        return sp_model.DecodePieces(tokens).replace('\n', DefaultTokens.SEP)
+        return sp_model.DecodePieces(tokens).replace("\n", DefaultTokens.SEP)
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Apply sentencepiece subword encode to src & tgt."""
-        src_out = self._tokenize(example['src'], 'src', is_train)
-        if example['tgt'] is not None:
-            tgt_out = self._tokenize(example['tgt'], 'tgt', is_train)
+        src_out = self._tokenize(example["src"], "src", is_train)
+        if example["tgt"] is not None:
+            tgt_out = self._tokenize(example["tgt"], "tgt", is_train)
             if stats is not None:
-                n_words = len(example['src']) + len(example['tgt'])
+                n_words = len(example["src"]) + len(example["tgt"])
                 n_subwords = len(src_out) + len(tgt_out)
                 stats.update(SubwordStats(n_subwords, n_words))
         else:
             tgt_out = None
             if stats is not None:
-                n_words = len(example['src'])
+                n_words = len(example["src"])
                 n_subwords = len(src_out)
                 stats.update(SubwordStats(n_subwords, n_words))
-        example['src'], example['tgt'] = src_out, tgt_out
+        example["src"], example["tgt"] = src_out, tgt_out
         return example
 
     def apply_reverse(self, translated):
         """Apply SentencePiece Detokenizer."""
         if isinstance(translated, list):
             return self._detokenize(translated, "tgt")
         else:
             return self._detokenize(translated.split(), "tgt")
 
     def _repr_args(self):
         """Return str represent key arguments for class."""
         kwargs_str = super()._repr_args()
-        additional_str = 'src_subword_nbest={}, tgt_subword_nbest={}'.format(
+        additional_str = "src_subword_nbest={}, tgt_subword_nbest={}".format(
             self.src_subword_nbest, self.tgt_subword_nbest
         )
-        return kwargs_str + ', ' + additional_str
+        return kwargs_str + ", " + additional_str
 
 
-@register_transform(name='bpe')
+@register_transform(name="bpe")
 class BPETransform(TokenizerTransform):
     """subword_nmt: official BPE subword transform class."""
 
     def __init__(self, opts):
         """Initialize necessary options for subword_nmt."""
         super().__init__(opts)
 
     def _parse_opts(self):
         super()._parse_opts()
-        self.dropout = {'src': self.src_subword_alpha,
-                        'tgt': self.tgt_subword_alpha}
+        self.dropout = {"src": self.src_subword_alpha, "tgt": self.tgt_subword_alpha}
 
     def _set_seed(self, seed):
         """set seed to ensure reproducibility."""
         import random
+
         random.seed(seed)
 
     def warm_up(self, vocabs=None):
         """Load subword models."""
         super().warm_up(None)
         from subword_nmt.apply_bpe import BPE, read_vocabulary
+
         # Load vocabulary file if provided and set threshold
         src_vocabulary, tgt_vocabulary = None, None
         if self.src_subword_vocab != "" and self.src_vocab_threshold > 0:
-            with open(self.src_subword_vocab, encoding='utf-8') as _sv:
+            with open(self.src_subword_vocab, encoding="utf-8") as _sv:
                 src_vocabulary = read_vocabulary(_sv, self.src_vocab_threshold)
         if self.tgt_subword_vocab != "" and self.tgt_vocab_threshold > 0:
-            with open(self.tgt_subword_vocab, encoding='utf-8') as _tv:
+            with open(self.tgt_subword_vocab, encoding="utf-8") as _tv:
                 tgt_vocabulary = read_vocabulary(_tv, self.tgt_vocab_threshold)
         # Load Subword Model
-        with open(self.src_subword_model, encoding='utf-8') as src_codes:
+        with open(self.src_subword_model, encoding="utf-8") as src_codes:
             load_src_model = BPE(codes=src_codes, vocab=src_vocabulary)
         if self.share_vocab and (src_vocabulary == tgt_vocabulary):
-            self.load_models = {
-                'src': load_src_model,
-                'tgt': load_src_model
-            }
+            self.load_models = {"src": load_src_model, "tgt": load_src_model}
         else:
-            with open(self.tgt_subword_model, encoding='utf-8') as tgt_codes:
+            with open(self.tgt_subword_model, encoding="utf-8") as tgt_codes:
                 load_tgt_model = BPE(codes=tgt_codes, vocab=tgt_vocabulary)
-            self.load_models = {
-                'src': load_src_model,
-                'tgt': load_tgt_model
-            }
+            self.load_models = {"src": load_src_model, "tgt": load_tgt_model}
 
-    def _tokenize(self, tokens, side='src', is_train=False):
+    def _tokenize(self, tokens, side="src", is_train=False):
         """Do bpe subword tokenize."""
         bpe_model = self.load_models[side]
         dropout = self.dropout[side] if is_train else 0.0
         segmented = bpe_model.segment_tokens(tokens, dropout=dropout)
         return segmented
 
     def _detokenize(self, tokens, side="src", is_train=False):
-        """"Apply bpe subword detokenizer"""
-        detokenized = re.sub(r"(@@ )|(@@ ?$)", r'', " ".join(tokens))
+        """ "Apply bpe subword detokenizer"""
+        detokenized = re.sub(r"(@@ )|(@@ ?$)", r"", " ".join(tokens))
         return detokenized
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Apply bpe subword encode to src & tgt."""
-        src_out = self._tokenize(example['src'], 'src', is_train)
-        if example['tgt'] is not None:
-            tgt_out = self._tokenize(example['tgt'], 'tgt', is_train)
+        src_out = self._tokenize(example["src"], "src", is_train)
+        if example["tgt"] is not None:
+            tgt_out = self._tokenize(example["tgt"], "tgt", is_train)
             if stats is not None:
-                n_words = len(example['src']) + len(example['tgt'])
+                n_words = len(example["src"]) + len(example["tgt"])
                 n_subwords = len(src_out) + len(tgt_out)
                 stats.update(SubwordStats(n_subwords, n_words))
         else:
             tgt_out = None
             if stats is not None:
-                n_words = len(example['src'])
+                n_words = len(example["src"])
                 n_subwords = len(src_out)
                 stats.update(SubwordStats(n_subwords, n_words))
-        example['src'], example['tgt'] = src_out, tgt_out
+        example["src"], example["tgt"] = src_out, tgt_out
         return example
 
     def apply_reverse(self, translated):
         """Apply bpe subword detokenizer"""
         if isinstance(translated, list):
             return self._detokenize(translated, "tgt")
         else:
             return self._detokenize(translated.split(), "tgt")
 
 
-@register_transform(name='onmt_tokenize')
+@register_transform(name="onmt_tokenize")
 class ONMTTokenizerTransform(TokenizerTransform):
     """OpenNMT Tokenizer transform class."""
 
     def __init__(self, opts):
         """Initialize necessary options for OpenNMT Tokenizer."""
         super().__init__(opts)
 
     def _set_seed(self, seed):
         """set seed to ensure reproducibility."""
         import pyonmttok
+
         pyonmttok.set_random_seed(seed)
 
     @classmethod
     def add_options(cls, parser):
         """Available options relate to Subword."""
         super().add_options(parser)
-        group = parser.add_argument_group('Transform/Subword/ONMTTOK')
-        group.add('-src_subword_type', '--src_subword_type',
-                  type=str, default='none',
-                  choices=['none', 'sentencepiece', 'bpe'],
-                  help="Type of subword model for src (or shared) "
-                       "in pyonmttok.")
-        group.add('-tgt_subword_type', '--tgt_subword_type',
-                  type=str, default='none',
-                  choices=['none', 'sentencepiece', 'bpe'],
-                  help="Type of subword model for tgt in  pyonmttok.")
-        group.add('-src_onmttok_kwargs', '--src_onmttok_kwargs', type=str,
-                  default="{'mode': 'none'}",
-                  help="Other pyonmttok options for src in dict string, "
-                  "except subword related options listed earlier.")
-        group.add('-tgt_onmttok_kwargs', '--tgt_onmttok_kwargs', type=str,
-                  default="{'mode': 'none'}",
-                  help="Other pyonmttok options for tgt in dict string, "
-                  "except subword related options listed earlier.")
+        group = parser.add_argument_group("Transform/Subword/ONMTTOK")
+        group.add(
+            "-src_subword_type",
+            "--src_subword_type",
+            type=str,
+            default="none",
+            choices=["none", "sentencepiece", "bpe"],
+            help="Type of subword model for src (or shared) " "in pyonmttok.",
+        )
+        group.add(
+            "-tgt_subword_type",
+            "--tgt_subword_type",
+            type=str,
+            default="none",
+            choices=["none", "sentencepiece", "bpe"],
+            help="Type of subword model for tgt in  pyonmttok.",
+        )
+        group.add(
+            "-src_onmttok_kwargs",
+            "--src_onmttok_kwargs",
+            type=str,
+            default="{'mode': 'none'}",
+            help="Other pyonmttok options for src in dict string, "
+            "except subword related options listed earlier.",
+        )
+        group.add(
+            "-tgt_onmttok_kwargs",
+            "--tgt_onmttok_kwargs",
+            type=str,
+            default="{'mode': 'none'}",
+            help="Other pyonmttok options for tgt in dict string, "
+            "except subword related options listed earlier.",
+        )
+        group.add(
+            "--gpt2_pretok",
+            "-gpt2_pretok",
+            action="store_true",
+            default=False,
+            help="Preprocess sentence with byte-level mapping",
+        )
 
     @classmethod
     def _validate_options(cls, opts):
         """Extra checks for OpenNMT Tokenizer options."""
         super()._validate_options(opts)
         src_kwargs_dict = eval(opts.src_onmttok_kwargs)
         tgt_kwargs_dict = eval(opts.tgt_onmttok_kwargs)
@@ -364,137 +428,181 @@
         opts.src_onmttok_kwargs = src_kwargs_dict
         opts.tgt_onmttok_kwargs = tgt_kwargs_dict
 
     def _parse_opts(self):
         super()._parse_opts()
         self.src_subword_type = self.opts.src_subword_type
         self.tgt_subword_type = self.opts.tgt_subword_type
-        logger.debug("Parsed pyonmttok kwargs for src: {}".format(
-            self.opts.src_onmttok_kwargs))
-        logger.debug("Parsed pyonmttok kwargs for tgt: {}".format(
-            self.opts.tgt_onmttok_kwargs))
+        logger.debug(
+            "Parsed pyonmttok kwargs for src: {}".format(self.opts.src_onmttok_kwargs)
+        )
+        logger.debug(
+            "Parsed pyonmttok kwargs for tgt: {}".format(self.opts.tgt_onmttok_kwargs)
+        )
         self.src_other_kwargs = self.opts.src_onmttok_kwargs
         self.tgt_other_kwargs = self.opts.tgt_onmttok_kwargs
+        self.gpt2_pretok = self.opts.gpt2_pretok
 
     @classmethod
     def get_specials(cls, opts):
         src_specials, tgt_specials = [], []
         if opts.src_onmttok_kwargs.get("case_markup", False):
-            _case_specials = ['｟mrk_case_modifier_C｠',
-                              '｟mrk_begin_case_region_U｠',
-                              '｟mrk_end_case_region_U｠']
+            _case_specials = [
+                "｟mrk_case_modifier_C｠",
+                "｟mrk_begin_case_region_U｠",
+                "｟mrk_end_case_region_U｠",
+            ]
             for src_spec in _case_specials:
                 src_specials.append(src_spec)
         if opts.tgt_onmttok_kwargs.get("case_markup", False):
-            _case_specials = ['｟mrk_case_modifier_C｠',
-                              '｟mrk_begin_case_region_U｠',
-                              '｟mrk_end_case_region_U｠']
+            _case_specials = [
+                "｟mrk_case_modifier_C｠",
+                "｟mrk_begin_case_region_U｠",
+                "｟mrk_end_case_region_U｠",
+            ]
             for tgt_spec in _case_specials:
                 tgt_specials.append(tgt_spec)
         return (src_specials, tgt_specials)
 
-    def _get_subword_kwargs(self, side='src'):
+    def _get_subword_kwargs(self, side="src"):
         """Return a dict containing kwargs relate to `side` subwords."""
-        subword_type = self.tgt_subword_type if side == 'tgt' \
-            else self.src_subword_type
-        subword_model = self.tgt_subword_model if side == 'tgt' \
-            else self.src_subword_model
-        subword_nbest = self.tgt_subword_nbest if side == 'tgt' \
-            else self.src_subword_nbest
-        subword_alpha = self.tgt_subword_alpha if side == 'tgt' \
-            else self.src_subword_alpha
+        subword_type = self.tgt_subword_type if side == "tgt" else self.src_subword_type
+        subword_model = (
+            self.tgt_subword_model if side == "tgt" else self.src_subword_model
+        )
+        subword_nbest = (
+            self.tgt_subword_nbest if side == "tgt" else self.src_subword_nbest
+        )
+        subword_alpha = (
+            self.tgt_subword_alpha if side == "tgt" else self.src_subword_alpha
+        )
         kwopts = dict()
-        if subword_type == 'bpe':
-            kwopts['bpe_model_path'] = subword_model
-            kwopts['bpe_dropout'] = subword_alpha
-        elif subword_type == 'sentencepiece':
-            kwopts['sp_model_path'] = subword_model
-            kwopts['sp_nbest_size'] = subword_nbest
-            kwopts['sp_alpha'] = subword_alpha
-        else:
-            logger.debug('No subword method will be applied.')
-        vocabulary_threshold = self.tgt_vocab_threshold if side == 'tgt' \
-            else self.src_vocab_threshold
-        vocabulary_path = self.tgt_subword_vocab if side == 'tgt' \
-            else self.src_subword_vocab
+        if subword_type == "bpe":
+            kwopts["bpe_model_path"] = subword_model
+            kwopts["bpe_dropout"] = subword_alpha
+        elif subword_type == "sentencepiece":
+            kwopts["sp_model_path"] = subword_model
+            kwopts["sp_nbest_size"] = subword_nbest
+            kwopts["sp_alpha"] = subword_alpha
+        else:
+            logger.debug("No subword method will be applied.")
+        vocabulary_threshold = (
+            self.tgt_vocab_threshold if side == "tgt" else self.src_vocab_threshold
+        )
+        vocabulary_path = (
+            self.tgt_subword_vocab if side == "tgt" else self.src_subword_vocab
+        )
         if vocabulary_threshold > 0 and vocabulary_path != "":
-            kwopts['vocabulary_path'] = vocabulary_path
-            kwopts['vocabulary_threshold'] = vocabulary_threshold
+            kwopts["vocabulary_path"] = vocabulary_path
+            kwopts["vocabulary_threshold"] = vocabulary_threshold
         return kwopts
 
     def warm_up(self, vocabs=None):
         """Initialize Tokenizer models."""
         super().warm_up(None)
         import pyonmttok
-        src_subword_kwargs = self._get_subword_kwargs(side='src')
+
+        src_subword_kwargs = self._get_subword_kwargs(side="src")
         src_tokenizer = pyonmttok.Tokenizer(
             **src_subword_kwargs, **self.src_other_kwargs
         )
-        tgt_subword_kwargs = self._get_subword_kwargs(side='tgt')
-        _diff_vocab = (
-            src_subword_kwargs.get('vocabulary_path', '') !=
-            tgt_subword_kwargs.get('vocabulary_path', '') or
-            src_subword_kwargs.get('vocabulary_threshold', 0) !=
-            tgt_subword_kwargs.get('vocabulary_threshold', 0))
+        tgt_subword_kwargs = self._get_subword_kwargs(side="tgt")
+        _diff_vocab = src_subword_kwargs.get(
+            "vocabulary_path", ""
+        ) != tgt_subword_kwargs.get("vocabulary_path", "") or src_subword_kwargs.get(
+            "vocabulary_threshold", 0
+        ) != tgt_subword_kwargs.get(
+            "vocabulary_threshold", 0
+        )
         if self.share_vocab and not _diff_vocab:
-            self.load_models = {
-                'src': src_tokenizer,
-                'tgt': src_tokenizer
-            }
+            self.load_models = {"src": src_tokenizer, "tgt": src_tokenizer}
         else:
-            tgt_subword_kwargs = self._get_subword_kwargs(side='tgt')
+            tgt_subword_kwargs = self._get_subword_kwargs(side="tgt")
             tgt_tokenizer = pyonmttok.Tokenizer(
                 **tgt_subword_kwargs, **self.tgt_other_kwargs
             )
-            self.load_models = {
-                'src': src_tokenizer,
-                'tgt': tgt_tokenizer
-            }
+            self.load_models = {"src": src_tokenizer, "tgt": tgt_tokenizer}
+        if self.gpt2_pretok:
+            """
+            Returns list of utf-8 byte and a corresponding list of unicode
+            strings. The reversible bpe codes work on unicode strings.
+            code taken from openai/gpt2
+            """
+            bs = (
+                list(range(ord("!"), ord("~") + 1))
+                + list(range(ord("¡"), ord("¬") + 1))
+                + list(range(ord("®"), ord("ÿ") + 1))
+            )
+            cs = bs[:]
+            n = 0
+            for b in range(2**8):
+                if b not in bs:
+                    bs.append(b)
+                    cs.append(2**8 + n)
+                    n += 1
+            cs = [chr(n) for n in cs]
+            self.maptable = dict(zip(bs, cs))
+            self.revtable = {v: k for k, v in self.maptable.items()}
 
-    def _tokenize(self, tokens, side='src', is_train=False):
+    def _tokenize(self, tokens, side="src", is_train=False):
         """Do OpenNMT Tokenizer's tokenize."""
         tokenizer = self.load_models[side]
-        sentence = ' '.join(tokens)
-        segmented, _ = tokenizer.tokenize(sentence)
+        sentence = " ".join(tokens)
+        if self.gpt2_pretok:
+            sentence = "".join(
+                self.maptable[b]
+                for b in sentence.replace(DefaultTokens.SEP, "\n").encode("utf-8")
+            )
+            segmented = tokenizer(sentence)
+        else:
+            segmented = tokenizer(sentence)
         return segmented
 
-    def _detokenize(self, tokens, side='src', is_train=False):
+    def _detokenize(self, tokens, side="src", is_train=False):
         """Do OpenNMT Tokenizer's detokenize."""
         tokenizer = self.load_models[side]
-        detokenized = tokenizer.detokenize(tokens)
-        return detokenized
+        if self.gpt2_pretok:
+            sentence = "".join(tokens)
+            detokenized = bytearray([self.revtable[c] for c in sentence]).decode(
+                "utf-8", errors="replace"
+            )
+        else:
+            detokenized = tokenizer.detokenize(tokens)
+        return detokenized.replace("\n", DefaultTokens.SEP)
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Apply OpenNMT Tokenizer to src & tgt."""
-        src_out = self._tokenize(example['src'], 'src')
-        if example['tgt'] is not None:
-            tgt_out = self._tokenize(example['tgt'], 'tgt')
+        src_out = self._tokenize(example["src"], "src")
+        if example["tgt"] is not None:
+            tgt_out = self._tokenize(example["tgt"], "tgt")
             if stats is not None:
-                n_words = len(example['src']) + len(example['tgt'])
+                n_words = len(example["src"]) + len(example["tgt"])
                 n_subwords = len(src_out) + len(tgt_out)
                 stats.update(SubwordStats(n_subwords, n_words))
         else:
             tgt_out = None
             if stats is not None:
-                n_words = len(example['src'])
+                n_words = len(example["src"])
                 n_subwords = len(src_out)
                 stats.update(SubwordStats(n_subwords, n_words))
-        example['src'], example['tgt'] = src_out, tgt_out
+        example["src"], example["tgt"] = src_out, tgt_out
         return example
 
     def apply_reverse(self, translated):
         """Apply OpenNMT Tokenizer to src & tgt."""
         if isinstance(translated, list):
             return self._detokenize(translated, "tgt")
         else:
             return self._detokenize(translated.split(), "tgt")
 
     def _repr_args(self):
         """Return str represent key arguments for class."""
-        repr_str = '{}={}'.format('share_vocab', self.share_vocab)
-        repr_str += ', src_subword_kwargs={}'.format(
-            self._get_subword_kwargs(side='src'))
-        repr_str += ', src_onmttok_kwargs={}'.format(self.src_other_kwargs)
-        repr_str += ', tgt_subword_kwargs={}'.format(
-            self._get_subword_kwargs(side='tgt'))
-        repr_str += ', tgt_onmttok_kwargs={}'.format(self.tgt_other_kwargs)
+        repr_str = "{}={}".format("share_vocab", self.share_vocab)
+        repr_str += ", src_subword_kwargs={}".format(
+            self._get_subword_kwargs(side="src")
+        )
+        repr_str += ", src_onmttok_kwargs={}".format(self.src_other_kwargs)
+        repr_str += ", tgt_subword_kwargs={}".format(
+            self._get_subword_kwargs(side="tgt")
+        )
+        repr_str += ", tgt_onmttok_kwargs={}".format(self.tgt_other_kwargs)
         return repr_str
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/transform.py` & `OpenNMT-py-3.1.3/onmt/transforms/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def batch_apply(self, batch, is_train=False, **kwargs):
         """Apply transform to `batch`.
         Args:
             batch (list): a list of examples;
             is_train (bool): Indicate if src/tgt is training data;bject.
         """
         transformed_batch = []
-        for (example, _, cid) in batch:
+        for example, _, cid in batch:
             example = self.apply(example, is_train=is_train, **kwargs)
             if example is not None:
                 transformed_batch.append((example, self, cid))
         return transformed_batch
 
     def apply_reverse(self, translated):
         return translated
@@ -84,16 +84,16 @@
             elif reversed is not None:
                 transformed_batch.append(reversed)
         return transformed_batch
 
     def __getstate__(self):
         """Pickling following for rebuild."""
         state = {"opts": self.opts}
-        if hasattr(self, 'vocabs'):
-            state['vocabs'] = self.vocabs
+        if hasattr(self, "vocabs"):
+            state["vocabs"] = self.vocabs
         return state
 
     def _parse_opts(self):
         """Parse opts to set/reset instance's attributes.
 
         This should be override if there are attributes other than self.opts.
         To make sure we recover from picked state.
@@ -102,29 +102,29 @@
         """
         pass
 
     def __setstate__(self, state):
         """Reload when unpickling from save file."""
         self.opts = state["opts"]
         self._parse_opts()
-        vocabs = state.get('vocabs', None)
+        vocabs = state.get("vocabs", None)
         self.warm_up(vocabs=vocabs)
 
     def stats(self):
         """Return statistic message."""
-        return ''
+        return ""
 
     def _repr_args(self):
         """Return str represent key arguments for class."""
-        return ''
+        return ""
 
     def __repr__(self):
         cls_name = type(self).__name__
         cls_args = self._repr_args()
-        return '{}({})'.format(cls_name, cls_args)
+        return "{}({})".format(cls_name, cls_args)
 
 
 class ObservableStats:
     """A running observable statistics."""
 
     __slots__ = []
 
@@ -135,22 +135,21 @@
     def update(self, other: "ObservableStats"):
         """Update current statistics with others."""
         raise NotImplementedError
 
     def __str__(self) -> str:
         return "{}({})".format(
             self.name(),
-            ", ".join(
-                f"{name}={getattr(self, name)}" for name in self.__slots__
-            )
+            ", ".join(f"{name}={getattr(self, name)}" for name in self.__slots__),
         )
 
 
 class TransformStatistics:
     """A observer containing runing statistics."""
+
     def __init__(self):
         self.observables = {}
 
     def update(self, observable: ObservableStats):
         """Adding observable to observe/updating existing observable."""
         name = observable.name()
         if name not in self.observables:
@@ -180,16 +179,17 @@
         self.transforms = transform_list
         self.statistics = TransformStatistics()
 
     @classmethod
     def build_from(cls, transform_list):
         """Return a `TransformPipe` instance build from `transform_list`."""
         for transform in transform_list:
-            assert isinstance(transform, Transform), \
-                "transform should be a instance of Transform."
+            assert isinstance(
+                transform, Transform
+            ), "transform should be a instance of Transform."
         transform_pipe = cls(None, transform_list)
         return transform_pipe
 
     def warm_up(self, vocabs):
         """Warm up Pipeline by iterate over all transfroms."""
         for transform in self.transforms:
             transform.warm_up(vocabs)
@@ -211,29 +211,31 @@
 
         Args:
             example (dict): a dict of field value, ex. src, tgt.
 
         """
         for transform in self.transforms:
             example = transform.apply(
-                example, is_train=is_train, stats=self.statistics, **kwargs)
+                example, is_train=is_train, stats=self.statistics, **kwargs
+            )
             if example is None:
                 break
         return example
 
     def batch_apply(self, batch, is_train=False, **kwargs):
         """Apply transform pipe to `example`.
 
         Args:
             example (dict): a dict of field value, ex. src, tgt.
 
         """
         for transform in self.transforms:
             batch = transform.batch_apply(
-                batch, is_train=is_train, stats=self.statistics, **kwargs)
+                batch, is_train=is_train, stats=self.statistics, **kwargs
+            )
             if batch is None:
                 break
         return batch
 
     def apply_reverse(self, translated):
         for transform in self.transforms:
             translated = transform.apply_reverse(translated)
@@ -252,41 +254,39 @@
         return self.statistics.report()
 
     def _repr_args(self):
         """Return str represent key arguments for class."""
         info_args = []
         for transform in self.transforms:
             info_args.append(repr(transform))
-        return ', '.join(info_args)
+        return ", ".join(info_args)
 
 
 def make_transforms(opts, transforms_cls, vocabs):
     """Build transforms in `transforms_cls` with vocab of `fields`."""
     transforms = {}
     for name, transform_cls in transforms_cls.items():
         if transform_cls.require_vocab() and vocabs is None:
-            logger.warning(
-                f"{transform_cls.__name__} require vocab to apply, skip it."
-            )
+            logger.warning(f"{transform_cls.__name__} require vocab to apply, skip it.")
             continue
         transform_obj = transform_cls(opts)
         transform_obj.warm_up(vocabs)
         transforms[name] = transform_obj
     return transforms
 
 
 def get_specials(opts, transforms_cls_dict):
     """Get specials of transforms that should be registed in Vocab."""
-    all_specials = {'src': [], 'tgt': []}
+    all_specials = {"src": [], "tgt": []}
     for name, transform_cls in transforms_cls_dict.items():
         src_specials, tgt_specials = transform_cls.get_specials(opts)
         for src_spec in src_specials:
-            all_specials['src'].append(src_spec)
+            all_specials["src"].append(src_spec)
         for tgt_spec in tgt_specials:
-            all_specials['tgt'].append(tgt_spec)
+            all_specials["tgt"].append(tgt_spec)
     logger.info(f"Get special vocabs from Transforms: {all_specials}.")
     return all_specials
 
 
 def save_transforms(transforms, save_data, overwrite=True):
     """Dump `transforms` object."""
     transforms_path = "{}.transforms.pt".format(save_data)
```

### Comparing `OpenNMT-py-3.1.2/onmt/transforms/uppercase.py` & `OpenNMT-py-3.1.3/onmt/transforms/uppercase.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from onmt.transforms import register_transform
 from .transform import Transform
 import unicodedata
 import random
 
 
-@register_transform(name='uppercase')
+@register_transform(name="uppercase")
 class UpperCaseTransform(Transform):
     """
     Convert source and target examples to uppercase.
 
     This transform uses `unicodedata` to normalize the converted
     uppercase strings as this is needed for some languages (e.g. Greek).
     One issue is that the normalization removes all diacritics and
@@ -20,32 +20,42 @@
         super().__init__(opts)
 
     @classmethod
     def add_options(cls, parser):
         """Add an option for the corpus ratio to apply this transform."""
 
         group = parser.add_argument_group("Transform/Uppercase")
-        group.add("--upper_corpus_ratio", "-upper_corpus_ratio", type=float,
-                  default=0.01, help="Corpus ratio to apply uppercasing.")
+        group.add(
+            "--upper_corpus_ratio",
+            "-upper_corpus_ratio",
+            type=float,
+            default=0.01,
+            help="Corpus ratio to apply uppercasing.",
+        )
 
     def _parse_opts(self):
         self.upper_corpus_ratio = self.opts.upper_corpus_ratio
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Convert source and target examples to uppercase."""
 
         if random.random() > self.upper_corpus_ratio:
             return example
 
-        src_str = ' '.join(example['src'])
-        src_str = ''.join(c for c in unicodedata.normalize('NFD',
-                          src_str.upper()) if unicodedata.category(c) != 'Mn')
-        example['src'] = src_str.split()
-
-        if example['tgt'] is not None:
-            tgt_str = ' '.join(example['tgt'])
-            tgt_str = ''.join(c for c in unicodedata.normalize('NFD',
-                              tgt_str.upper()) if unicodedata.category(c) !=
-                              'Mn')
-            example['tgt'] = tgt_str.split()
+        src_str = " ".join(example["src"])
+        src_str = "".join(
+            c
+            for c in unicodedata.normalize("NFD", src_str.upper())
+            if unicodedata.category(c) != "Mn"
+        )
+        example["src"] = src_str.split()
+
+        if example["tgt"] is not None:
+            tgt_str = " ".join(example["tgt"])
+            tgt_str = "".join(
+                c
+                for c in unicodedata.normalize("NFD", tgt_str.upper())
+                if unicodedata.category(c) != "Mn"
+            )
+            example["tgt"] = tgt_str.split()
 
         return example
```

### Comparing `OpenNMT-py-3.1.2/onmt/translate/__init__.py` & `OpenNMT-py-3.1.3/onmt/translate/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,24 @@
 from onmt.translate.translator import Translator, GeneratorLM
 from onmt.translate.translation import Translation, TranslationBuilder
 from onmt.translate.beam_search import BeamSearch, GNMTGlobalScorer
 from onmt.translate.beam_search import BeamSearchLM
 from onmt.translate.decode_strategy import DecodeStrategy
 from onmt.translate.greedy_search import GreedySearch, GreedySearchLM
 from onmt.translate.penalties import PenaltyBuilder
-from onmt.translate.translation_server import TranslationServer, \
-    ServerModelError
+from onmt.translate.translation_server import TranslationServer, ServerModelError
 
-__all__ = ['Translator', 'Translation', 'BeamSearch',
-           'GNMTGlobalScorer', 'TranslationBuilder',
-           'PenaltyBuilder', 'TranslationServer', 'ServerModelError',
-           "DecodeStrategy", "GreedySearch", "GreedySearchLM",
-           "BeamSearchLM", "GeneratorLM"]
+__all__ = [
+    "Translator",
+    "Translation",
+    "BeamSearch",
+    "GNMTGlobalScorer",
+    "TranslationBuilder",
+    "PenaltyBuilder",
+    "TranslationServer",
+    "ServerModelError",
+    "DecodeStrategy",
+    "GreedySearch",
+    "GreedySearchLM",
+    "BeamSearchLM",
+    "GeneratorLM",
+]
```

### Comparing `OpenNMT-py-3.1.2/onmt/translate/beam_search.py` & `OpenNMT-py-3.1.3/onmt/translate/beam_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,22 +51,51 @@
         _prev_penalty (FloatTensor or NoneType): Shape
             ``(B, beam_size)``. Initialized to ``None``.
         _coverage (FloatTensor or NoneType): Shape
             ``(1, B x beam_size, inp_seq_len)``.
         hypotheses (list[list[Tuple[Tensor]]]): Contains a tuple
             of score (float), sequence (long), and attention (float or None).
     """
-    def __init__(self, beam_size, batch_size, pad, bos, eos, unk, start,
-                 n_best, global_scorer, min_length, max_length,
-                 return_attention, block_ngram_repeat, exclusion_tokens,
-                 stepwise_penalty, ratio, ban_unk_token):
+
+    def __init__(
+        self,
+        beam_size,
+        batch_size,
+        pad,
+        bos,
+        eos,
+        unk,
+        start,
+        n_best,
+        global_scorer,
+        min_length,
+        max_length,
+        return_attention,
+        block_ngram_repeat,
+        exclusion_tokens,
+        stepwise_penalty,
+        ratio,
+        ban_unk_token,
+    ):
         super(BeamSearchBase, self).__init__(
-            pad, bos, eos, unk, start, batch_size, beam_size, global_scorer,
-            min_length, block_ngram_repeat, exclusion_tokens,
-            return_attention, max_length, ban_unk_token)
+            pad,
+            bos,
+            eos,
+            unk,
+            start,
+            batch_size,
+            beam_size,
+            global_scorer,
+            min_length,
+            block_ngram_repeat,
+            exclusion_tokens,
+            return_attention,
+            max_length,
+            ban_unk_token,
+        )
         # beam parameters
         self.beam_size = beam_size
         self.n_best = n_best
         self.ratio = ratio
 
         # beam state
         self.top_beam_finished = torch.zeros([batch_size], dtype=torch.uint8)
@@ -79,55 +108,64 @@
 
         self.select_indices = None
         self.done = False
         # "global state" of the old beam
         self._prev_penalty = None
         self._coverage = None
 
-        self._stepwise_cov_pen = (
-            stepwise_penalty and self.global_scorer.has_cov_pen)
-        self._vanilla_cov_pen = (
-            not stepwise_penalty and self.global_scorer.has_cov_pen)
+        self._stepwise_cov_pen = stepwise_penalty and self.global_scorer.has_cov_pen
+        self._vanilla_cov_pen = not stepwise_penalty and self.global_scorer.has_cov_pen
         self._cov_pen = self.global_scorer.has_cov_pen
 
         self.src_len = None
 
     def initialize(self, *args, **kwargs):
         raise NotImplementedError
 
-    def initialize_(self, enc_out, src_len, src_map, device,
-                    target_prefix):
+    def initialize_(self, enc_out, src_len, src_map, device, target_prefix):
         super(BeamSearchBase, self).initialize(
-            enc_out, src_len, src_map, device, target_prefix)
+            enc_out, src_len, src_map, device, target_prefix
+        )
 
         self.best_scores = torch.full(
-            [self.batch_size], -1e10, dtype=torch.float, device=device)
+            [self.batch_size], -1e10, dtype=torch.float, device=device
+        )
         self._beam_offset = torch.arange(
-            0, self.batch_size * self.beam_size, step=self.beam_size,
-            dtype=torch.long, device=device)
-        self.topk_log_probs = torch.tensor(
-            [0.0] + [float("-inf")] * (self.beam_size - 1), device=device
-        ).repeat(self.batch_size).reshape(self.batch_size, self.beam_size)
+            0,
+            self.batch_size * self.beam_size,
+            step=self.beam_size,
+            dtype=torch.long,
+            device=device,
+        )
+        self.topk_log_probs = (
+            torch.tensor([0.0] + [float("-inf")] * (self.beam_size - 1), device=device)
+            .repeat(self.batch_size)
+            .reshape(self.batch_size, self.beam_size)
+        )
         # buffers for the topk scores and 'backpointer'
-        self.topk_scores = torch.empty((self.batch_size, self.beam_size),
-                                       dtype=torch.float, device=device)
-        self.topk_ids = torch.empty((self.batch_size, self.beam_size),
-                                    dtype=torch.long, device=device)
-        self._batch_index = torch.empty([self.batch_size, self.beam_size],
-                                        dtype=torch.long, device=device)
+        self.topk_scores = torch.empty(
+            (self.batch_size, self.beam_size), dtype=torch.float, device=device
+        )
+        self.topk_ids = torch.empty(
+            (self.batch_size, self.beam_size), dtype=torch.long, device=device
+        )
+        self._batch_index = torch.empty(
+            [self.batch_size, self.beam_size], dtype=torch.long, device=device
+        )
 
     @property
     def current_predictions(self):
         return self.alive_seq[:, -1]
 
     @property
     def current_backptr(self):
         # for testing
-        return self.select_indices.view(self.batch_size, self.beam_size)\
-            .fmod(self.beam_size)
+        return self.select_indices.view(self.batch_size, self.beam_size).fmod(
+            self.beam_size
+        )
 
     @property
     def batch_offset(self):
         return self._batch_offset
 
     def _pick(self, log_probs, out=None):
         """Take a token pick decision for a step.
@@ -155,119 +193,130 @@
     def update_finished(self):
         # Penalize beams that finished.
         _B_old = self.topk_log_probs.shape[0]
         step = self.alive_seq.shape[-1]  # 1 greater than the step in advance
         self.topk_log_probs.masked_fill_(self.is_finished, -1e10)
         # on real data (newstest2017) with the pretrained transformer,
         # it's faster to not move this back to the original device
-        self.is_finished = self.is_finished.to('cpu')
+        self.is_finished = self.is_finished.to("cpu")
         self.top_beam_finished |= self.is_finished[:, 0].eq(1)
         predictions = self.alive_seq.view(_B_old, self.beam_size, step)
         attention = (
             self.alive_attn.view(
-                step - 1, _B_old, self.beam_size, self.alive_attn.size(-1))
-            if self.alive_attn is not None else None)
+                _B_old, self.beam_size, step - 1, self.alive_attn.size(-1)
+            )
+            if self.alive_attn is not None
+            else None
+        )
         non_finished_batch = []
         for i in range(self.is_finished.size(0)):  # Batch level
             b = self._batch_offset[i]
             finished_hyp = self.is_finished[i].nonzero(as_tuple=False).view(-1)
             # Store finished hypotheses for this batch.
             for j in finished_hyp:  # Beam level: finished beam j in batch i
                 if self.ratio > 0:
                     s = self.topk_scores[i, j] / (step + 1)
                     if self.best_scores[b] < s:
                         self.best_scores[b] = s
-                self.hypotheses[b].append((
-                    self.topk_scores[i, j],
-                    predictions[i, j, 1:],  # Ignore start_token.
-                    attention[:, i, j, :self.src_len[i]]
-                    if attention is not None else None))
+                self.hypotheses[b].append(
+                    (
+                        self.topk_scores[i, j],
+                        predictions[i, j, 1:],  # Ignore start_token.
+                        attention[i, j, :, : self.src_len[i]]
+                        if attention is not None
+                        else None,
+                    )
+                )
             # End condition is the top beam finished and we can return
             # n_best hypotheses.
             if self.ratio > 0:
                 pred_len = self.src_len[i] * self.ratio
-                finish_flag = ((self.topk_scores[i, 0] / pred_len)
-                               <= self.best_scores[b]) or \
-                    self.is_finished[i].all()
+                finish_flag = (
+                    (self.topk_scores[i, 0] / pred_len) <= self.best_scores[b]
+                ) or self.is_finished[i].all()
             else:
                 finish_flag = self.top_beam_finished[i] != 0
             if finish_flag and len(self.hypotheses[b]) >= self.beam_size:
-                best_hyp = sorted(
-                    self.hypotheses[b], key=lambda x: x[0],
-                    reverse=True)[:self.n_best]
+                best_hyp = sorted(self.hypotheses[b], key=lambda x: x[0], reverse=True)[
+                    : self.n_best
+                ]
                 for n, (score, pred, attn) in enumerate(best_hyp):
                     self.scores[b].append(score)
                     self.predictions[b].append(pred)  # ``(batch, n_best,)``
-                    self.attention[b].append(
-                        attn if attn is not None else [])
+                    self.attention[b].append(attn if attn is not None else [])
             else:
                 non_finished_batch.append(i)
 
         non_finished = torch.tensor(non_finished_batch)
         # If all sentences are translated, no need to go further.
         if len(non_finished) == 0:
             self.done = True
             return
 
         _B_new = non_finished.shape[0]
-        self.remove_finished_batches(_B_new, _B_old, non_finished,
-                                     predictions, attention, step)
-
-    def remove_finished_batches(self, _B_new, _B_old, non_finished,
-                                predictions, attention, step):
+        self.remove_finished_batches(
+            _B_new, _B_old, non_finished, predictions, attention, step
+        )
+
+    def remove_finished_batches(
+        self, _B_new, _B_old, non_finished, predictions, attention, step
+    ):
         # Remove finished batches for the next step.
-        self.top_beam_finished = self.top_beam_finished.index_select(
-            0, non_finished)
+        self.top_beam_finished = self.top_beam_finished.index_select(0, non_finished)
         self._batch_offset = self._batch_offset.index_select(0, non_finished)
         non_finished = non_finished.to(self.topk_ids.device)
-        self.topk_log_probs = self.topk_log_probs.index_select(0,
-                                                               non_finished)
+        self.topk_log_probs = self.topk_log_probs.index_select(0, non_finished)
         self._batch_index = self._batch_index.index_select(0, non_finished)
         self.select_indices = self._batch_index.view(_B_new * self.beam_size)
-        self.alive_seq = predictions.index_select(0, non_finished) \
-            .view(-1, self.alive_seq.size(-1))
+        self.alive_seq = predictions.index_select(0, non_finished).view(
+            -1, self.alive_seq.size(-1)
+        )
         self.topk_scores = self.topk_scores.index_select(0, non_finished)
         self.topk_ids = self.topk_ids.index_select(0, non_finished)
         self.maybe_update_target_prefix(self.select_indices)
         if self.alive_attn is not None:
             inp_seq_len = self.alive_attn.size(-1)
-            self.alive_attn = attention.index_select(1, non_finished) \
-                .view(step - 1, _B_new * self.beam_size, inp_seq_len)
+            self.alive_attn = attention.index_select(0, non_finished).view(
+                _B_new * self.beam_size, step - 1, inp_seq_len
+            )
             if self._cov_pen:
-                self._coverage = self._coverage \
-                    .view(1, _B_old, self.beam_size, inp_seq_len) \
-                    .index_select(1, non_finished) \
-                    .view(1, _B_new * self.beam_size, inp_seq_len)
+                self._coverage = (
+                    self._coverage.view(_B_old, self.beam_size, 1, inp_seq_len)
+                    .index_select(0, non_finished)
+                    .view(_B_new * self.beam_size, 1, inp_seq_len)
+                )
                 if self._stepwise_cov_pen:
                     self._prev_penalty = self._prev_penalty.index_select(
-                        0, non_finished)
+                        0, non_finished
+                    )
 
     def advance(self, log_probs, attn):
         vocab_size = log_probs.size(-1)
 
         # using integer division to get an integer _B without casting
         _B = log_probs.shape[0] // self.beam_size
 
         if self._stepwise_cov_pen and self._prev_penalty is not None:
             self.topk_log_probs += self._prev_penalty
             self.topk_log_probs -= self.global_scorer.cov_penalty(
-                self._coverage + attn, self.global_scorer.beta).view(
-                _B, self.beam_size)
+                self._coverage + attn, self.global_scorer.beta
+            ).view(_B, self.beam_size)
 
         # force the output to be longer than self.min_length
         step = len(self)
         self.ensure_min_length(log_probs)
         self.ensure_unk_removed(log_probs)
         # Multiply probs by the beam probability.
         log_probs += self.topk_log_probs.view(_B * self.beam_size, 1)
 
         # if the sequence ends now, then the penalty is the current
         # length + 1, to include the EOS token
         length_penalty = self.global_scorer.length_penalty(
-            step + 1, alpha=self.global_scorer.alpha)
+            step + 1, alpha=self.global_scorer.alpha
+        )
 
         curr_scores = log_probs / length_penalty
 
         # Avoid any direction that would repeat unwanted ngrams
         self.block_ngram_repeats(curr_scores)
 
         # Pick up candidate token by curr_scores
@@ -275,121 +324,132 @@
 
         # Recover log probs.
         # Length penalty is just a scalar. It doesn't matter if it's applied
         # before or after the topk.
         torch.mul(self.topk_scores, length_penalty, out=self.topk_log_probs)
 
         # Resolve beam origin and map to batch index flat representation.
-        self._batch_index = torch.div(self.topk_ids, vocab_size,
-                                      rounding_mode='trunc')
+        self._batch_index = torch.div(self.topk_ids, vocab_size, rounding_mode="trunc")
         self._batch_index += self._beam_offset[:_B].unsqueeze(1)
         self.select_indices = self._batch_index.view(_B * self.beam_size)
         self.topk_ids.fmod_(vocab_size)  # resolve true word ids
 
         # Append last prediction.
         self.alive_seq = torch.cat(
-            [self.alive_seq.index_select(0, self.select_indices),
-             self.topk_ids.view(_B * self.beam_size, 1)], -1)
+            [
+                self.alive_seq.index_select(0, self.select_indices),
+                self.topk_ids.view(_B * self.beam_size, 1),
+            ],
+            -1,
+        )
 
         self.maybe_update_forbidden_tokens()
 
         if self.return_attention or self._cov_pen:
-            current_attn = attn.index_select(1, self.select_indices)
+            current_attn = attn.index_select(0, self.select_indices)
             if step == 1:
                 self.alive_attn = current_attn
                 # update global state (step == 1)
                 if self._cov_pen:  # coverage penalty
                     self._prev_penalty = torch.zeros_like(self.topk_log_probs)
                     self._coverage = current_attn
             else:
-                self.alive_attn = self.alive_attn.index_select(
-                    1, self.select_indices)
-                self.alive_attn = torch.cat([self.alive_attn, current_attn], 0)
+                self.alive_attn = self.alive_attn.index_select(0, self.select_indices)
+                self.alive_attn = torch.cat([self.alive_attn, current_attn], 1)
                 # update global state (step > 1)
                 if self._cov_pen:
-                    self._coverage = self._coverage.index_select(
-                        1, self.select_indices)
+                    self._coverage = self._coverage.index_select(0, self.select_indices)
                     self._coverage += current_attn
                     self._prev_penalty = self.global_scorer.cov_penalty(
-                        self._coverage, beta=self.global_scorer.beta).view(
-                            _B, self.beam_size)
+                        self._coverage, beta=self.global_scorer.beta
+                    ).view(_B, self.beam_size)
 
         if self._vanilla_cov_pen:
             # shape: (batch_size x beam_size, 1)
             cov_penalty = self.global_scorer.cov_penalty(
-                self._coverage,
-                beta=self.global_scorer.beta)
+                self._coverage, beta=self.global_scorer.beta
+            )
             self.topk_scores -= cov_penalty.view(_B, self.beam_size).float()
 
         self.is_finished = self.topk_ids.eq(self.eos)
         self.ensure_max_length()
 
 
 class BeamSearch(BeamSearchBase):
     """
-        Beam search for seq2seq/encoder-decoder models
+    Beam search for seq2seq/encoder-decoder models
     """
-    def initialize(self, enc_out, src_len, src_map=None, device=None,
-                   target_prefix=None):
+
+    def initialize(
+        self, enc_out, src_len, src_map=None, device=None, target_prefix=None
+    ):
         """Initialize for decoding.
         Repeat src objects `beam_size` times.
         """
 
-        (fn_map_state, enc_out, src_map,
-            target_prefix) = self.initialize_tile(
-                enc_out, src_len, src_map, target_prefix)
+        (fn_map_state, enc_out, src_map, target_prefix) = self.initialize_tile(
+            enc_out, src_len, src_map, target_prefix
+        )
         if device is None:
             device = self.get_device_from_enc_out(enc_out)
 
         super(BeamSearch, self).initialize_(
-            enc_out, self.src_len, src_map, device, target_prefix)
+            enc_out, self.src_len, src_map, device, target_prefix
+        )
 
         return fn_map_state, enc_out, self.src_len, src_map
 
 
 class BeamSearchLM(BeamSearchBase):
     """
-        Beam search for language/decoder only models
+    Beam search for language/decoder only models
     """
-    def initialize(self, src, src_len, src_map=None, device=None,
-                   target_prefix=None):
+
+    def initialize(self, src, src_len, src_map=None, device=None, target_prefix=None):
         """Initialize for decoding.
         Repeat src objects `beam_size` times.
         """
-        (fn_map_state, _, src_map,
-            target_prefix) = self.initialize_tile(
-                None, src_len, src_map, target_prefix)
+        (fn_map_state, _, src_map, target_prefix) = self.initialize_tile(
+            None, src_len, src_map, target_prefix
+        )
         if device is None:
             device = src.device
 
         super(BeamSearchLM, self).initialize_(
-            None, self.src_len, src_map=src_map, device=device,
-            target_prefix=target_prefix)
+            None,
+            self.src_len,
+            src_map=src_map,
+            device=device,
+            target_prefix=target_prefix,
+        )
 
         return fn_map_state, src, self.src_len, src_map
 
     def advance(self, log_probs, attn):
         super(BeamSearchLM, self).advance(log_probs, attn)
 
         # in LM task src_len is associated with currently generated src
         # and therefore needs to follow the generation
         self.src_len += 1
 
-    def remove_finished_batches(self, _B_new, _B_old, non_finished,
-                                predictions, attention, step):
+    def remove_finished_batches(
+        self, _B_new, _B_old, non_finished, predictions, attention, step
+    ):
         super(BeamSearchLM, self).remove_finished_batches(
-            _B_new, _B_old, non_finished, predictions, attention, step)
+            _B_new, _B_old, non_finished, predictions, attention, step
+        )
 
         # in LM task src_len is associated with currently generated src
         # and therefore needs to follow the generation
         non_finished = non_finished.to(self.topk_ids.device)
-        self.src_len = self.src_len.view(
-            _B_old, self.beam_size) \
-            .index_select(0, non_finished) \
+        self.src_len = (
+            self.src_len.view(_B_old, self.beam_size)
+            .index_select(0, non_finished)
             .view(_B_new * self.beam_size)
+        )
 
 
 class GNMTGlobalScorer(object):
     """NMT re-ranking.
 
     Args:
        alpha (float): Length parameter.
@@ -404,44 +464,45 @@
         coverage_penalty (callable): See :class:`penalties.PenaltyBuilder`.
         has_cov_pen (bool): See :class:`penalties.PenaltyBuilder`.
         has_len_pen (bool): See :class:`penalties.PenaltyBuilder`.
     """
 
     @classmethod
     def from_opt(cls, opt):
-        return cls(
-            opt.alpha,
-            opt.beta,
-            opt.length_penalty,
-            opt.coverage_penalty)
+        return cls(opt.alpha, opt.beta, opt.length_penalty, opt.coverage_penalty)
 
     def __init__(self, alpha, beta, length_penalty, coverage_penalty):
         self._validate(alpha, beta, length_penalty, coverage_penalty)
         self.alpha = alpha
         self.beta = beta
-        penalty_builder = penalties.PenaltyBuilder(coverage_penalty,
-                                                   length_penalty)
+        penalty_builder = penalties.PenaltyBuilder(coverage_penalty, length_penalty)
         self.has_cov_pen = penalty_builder.has_cov_pen
         # Term will be subtracted from probability
         self.cov_penalty = penalty_builder.coverage_penalty
 
         self.has_len_pen = penalty_builder.has_len_pen
         # Probability will be divided by this
         self.length_penalty = penalty_builder.length_penalty
 
     @classmethod
     def _validate(cls, alpha, beta, length_penalty, coverage_penalty):
         # these warnings indicate that either the alpha/beta
         # forces a penalty to be a no-op, or a penalty is a no-op but
         # the alpha/beta would suggest otherwise.
-        if length_penalty is not None and alpha == 0.:
-            warnings.warn("Using length penalty with alpha==0 "
-                          "is equivalent to using length penalty none.")
+        if length_penalty is not None and alpha == 0.0:
+            warnings.warn(
+                "Using length penalty with alpha==0 "
+                "is equivalent to using length penalty none."
+            )
         if coverage_penalty is None or coverage_penalty == "none":
             if beta != 0:
-                warnings.warn("Non-default `beta` with no coverage penalty. "
-                              "`beta` has no effect.")
+                warnings.warn(
+                    "Non-default `beta` with no coverage penalty. "
+                    "`beta` has no effect."
+                )
         else:
             # using some coverage penalty
-            if beta == 0.:
-                warnings.warn("Non-default coverage penalty with beta==0 "
-                              "is equivalent to using coverage penalty none.")
+            if beta == 0.0:
+                warnings.warn(
+                    "Non-default coverage penalty with beta==0 "
+                    "is equivalent to using coverage penalty none."
+                )
```

### Comparing `OpenNMT-py-3.1.2/onmt/translate/decode_strategy.py` & `OpenNMT-py-3.1.3/onmt/translate/decode_strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,19 +60,31 @@
       max_length (int): See above.
       ban_unk_token (Boolean): See above.
       block_ngram_repeat (int): See above.
       exclusion_tokens (set[int]): See above.
       return_attention (bool): See above.
       done (bool): See above."""
 
-    def __init__(self, pad, bos, eos, unk, start, batch_size, parallel_paths,
-                 global_scorer, min_length, block_ngram_repeat,
-                 exclusion_tokens, return_attention, max_length,
-                 ban_unk_token):
-
+    def __init__(
+        self,
+        pad,
+        bos,
+        eos,
+        unk,
+        start,
+        batch_size,
+        parallel_paths,
+        global_scorer,
+        min_length,
+        block_ngram_repeat,
+        exclusion_tokens,
+        return_attention,
+        max_length,
+        ban_unk_token,
+    ):
         # magic indices
         self.pad = pad
         self.bos = bos
         self.eos = eos
         self.unk = unk
         self.start = start
 
@@ -104,61 +116,64 @@
     def get_device_from_enc_out(self, enc_out):
         if isinstance(enc_out, tuple):
             mb_device = enc_out[0].device
         else:
             mb_device = enc_out.device
         return mb_device
 
-    def initialize_tile(self, enc_out, src_len, src_map=None,
-                        target_prefix=None):
+    def initialize_tile(self, enc_out, src_len, src_map=None, target_prefix=None):
         def fn_map_state(state, dim):
             return tile(state, self.beam_size, dim=dim)
 
         if isinstance(enc_out, tuple):
-            enc_out = tuple(tile(x, self.beam_size, dim=0)
-                            for x in enc_out)
+            enc_out = tuple(tile(x, self.beam_size, dim=0) for x in enc_out)
         elif enc_out is not None:
             enc_out = tile(enc_out, self.beam_size, dim=0)
 
         if src_map is not None:
             src_map = tile(src_map, self.beam_size, dim=0)
 
         self.src_len = tile(src_len, self.beam_size)
         if target_prefix is not None:
             target_prefix = tile(target_prefix, self.beam_size, dim=0)
 
         return fn_map_state, enc_out, src_map, target_prefix
 
-    def initialize(self, enc_out, src_len, src_map=None, device=None,
-                   target_prefix=None):
+    def initialize(
+        self, enc_out, src_len, src_map=None, device=None, target_prefix=None
+    ):
         """DecodeStrategy subclasses should override :func:`initialize()`.
 
         `initialize` should be called before all actions.
         used to prepare necessary ingredients for decode."""
 
         if device is None:
-            device = torch.device('cpu')
+            device = torch.device("cpu")
         # Here we set the decoder to start with self.start (BOS or EOS)
         self.alive_seq = torch.full(
-            [self.batch_size * self.parallel_paths, 1], self.start,
-            dtype=torch.long, device=device)
+            [self.batch_size * self.parallel_paths, 1],
+            self.start,
+            dtype=torch.long,
+            device=device,
+        )
         self.is_finished = torch.zeros(
-            [self.batch_size, self.parallel_paths],
-            dtype=torch.uint8, device=device)
+            [self.batch_size, self.parallel_paths], dtype=torch.uint8, device=device
+        )
         if target_prefix is not None:
             batch_size, seq_len, n_feats = target_prefix.size()
-            assert batch_size == self.batch_size * self.parallel_paths,\
-                "forced target_prefix should've extend to same number of path!"
+            assert (
+                batch_size == self.batch_size * self.parallel_paths
+            ), "forced target_prefix should've extend to same number of path!"
             target_prefix_words = target_prefix[:, :, 0]  # no features
             target_prefix = target_prefix_words[:, 1:]  # remove bos
 
             # fix length constraint and remove eos from count
             prefix_non_pad = target_prefix.ne(self.pad).sum(dim=-1).tolist()
-            self.max_length += max(prefix_non_pad)-1
-            self.min_length += min(prefix_non_pad)-1
+            self.max_length += max(prefix_non_pad) - 1
+            self.min_length += min(prefix_non_pad) - 1
 
         self.target_prefix = target_prefix  # NOTE: forced prefix words
         return None, enc_out, src_len, src_map
 
     def __len__(self):
         return self.alive_seq.shape[1]
 
@@ -203,16 +218,15 @@
             return
 
         n = self.block_ngram_repeat - 1
         for path_idx in range(self.alive_seq.shape[0]):
             # we check paths one by one
 
             current_ngram = tuple(self.alive_seq[path_idx, -n:].tolist())
-            forbidden_tokens = self.forbidden_tokens[path_idx].get(
-                current_ngram, None)
+            forbidden_tokens = self.forbidden_tokens[path_idx].get(current_ngram, None)
             if forbidden_tokens is not None:
                 log_probs[path_idx, list(forbidden_tokens)] = -10e20
 
     def maybe_update_forbidden_tokens(self):
         """We complete and reorder the list of forbidden_tokens"""
 
         # we don't forbid nothing if the user doesn't want it
@@ -223,19 +237,17 @@
         if len(self) < self.block_ngram_repeat:
             return
 
         n = self.block_ngram_repeat
 
         forbidden_tokens = list()
         for path_idx, seq in zip(self.select_indices, self.alive_seq):
-
             # Reordering forbidden_tokens following beam selection
             # We rebuild a dict to ensure we get the value and not the pointer
-            forbidden_tokens.append(
-                deepcopy(self.forbidden_tokens[path_idx]))
+            forbidden_tokens.append(deepcopy(self.forbidden_tokens[path_idx]))
 
             # Grabing the newly selected tokens and associated ngram
             current_ngram = tuple(seq[-n:].tolist())
 
             # skip the blocking if any token in current_ngram is excluded
             if set(current_ngram) & self.exclusion_tokens:
                 continue
@@ -252,39 +264,46 @@
         log_probs (FloatTensor): logits of size ``(B, vocab_size)``.
 
         Returns:
         log_probs (FloatTensor): modified logits in ``(B, vocab_size)``.
         """
         _B, vocab_size = log_probs.size()
         step = len(self)
-        if (self.target_prefix is not None and
-                step <= self.target_prefix.size(1)):
+        if self.target_prefix is not None and step <= self.target_prefix.size(1):
             pick_idx = self.target_prefix[:, step - 1].tolist()  # (B)
-            pick_coo = [[path_i, pick] for path_i, pick in enumerate(pick_idx)
-                        if pick not in [self.eos, self.pad]]
-            mask_pathid = [path_i for path_i, pick in enumerate(pick_idx)
-                           if pick in [self.eos, self.pad]]
+            pick_coo = [
+                [path_i, pick]
+                for path_i, pick in enumerate(pick_idx)
+                if pick not in [self.eos, self.pad]
+            ]
+            mask_pathid = [
+                path_i
+                for path_i, pick in enumerate(pick_idx)
+                if pick in [self.eos, self.pad]
+            ]
             if len(pick_coo) > 0:
                 pick_coo = torch.tensor(pick_coo).to(self.target_prefix)
-                pick_fill_value = torch.ones(
-                    [pick_coo.size(0)], dtype=log_probs.dtype)
+                pick_fill_value = torch.ones([pick_coo.size(0)], dtype=log_probs.dtype)
                 # pickups: Tensor where specified index were set to 1, others 0
                 pickups = torch.sparse_coo_tensor(
-                    pick_coo.t(), pick_fill_value,
-                    size=log_probs.size(), device=log_probs.device).to_dense()
+                    pick_coo.t(),
+                    pick_fill_value,
+                    size=log_probs.size(),
+                    device=log_probs.device,
+                ).to_dense()
                 # dropdowns: opposite of pickups, 1 for those shouldn't pick
                 dropdowns = torch.ones_like(pickups) - pickups
                 if len(mask_pathid) > 0:
                     path_mask = torch.zeros(_B).to(self.target_prefix)
                     path_mask[mask_pathid] = 1
                     path_mask = path_mask.unsqueeze(1).to(dtype=bool)
                     dropdowns = dropdowns.masked_fill(path_mask, 0)
                 # Minus dropdowns to log_probs making probabilities of
                 # unspecified index close to 0
-                log_probs -= 10000*dropdowns
+                log_probs -= 10000 * dropdowns
         return log_probs
 
     def maybe_update_target_prefix(self, select_index):
         """We update / reorder `target_prefix` for alive path."""
         if self.target_prefix is None:
             return
         # prediction step have surpass length of given target_prefix,
```

### Comparing `OpenNMT-py-3.1.2/onmt/translate/greedy_search.py` & `OpenNMT-py-3.1.3/onmt/translate/greedy_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import torch
 import torch.nn.functional as F
 
 from onmt.translate.decode_strategy import DecodeStrategy
 
 
 def sample_topp(logits, keep_topp):
-    sorted_logits, sorted_indices = torch.sort(logits,
-                                               descending=True,
-                                               dim=1)
+    sorted_logits, sorted_indices = torch.sort(logits, descending=True, dim=1)
 
-    cumulative_probs = torch.cumsum(F.softmax(sorted_logits,
-                                              dim=-1), dim=-1)
+    cumulative_probs = torch.cumsum(F.softmax(sorted_logits, dim=-1), dim=-1)
     sorted_indices_to_keep = cumulative_probs.lt(keep_topp)
 
     # keep indices until overflowing p
     cumsum_mask = sorted_indices_to_keep.cumsum(dim=1)
     last_included = cumsum_mask[:, -1:]
     last_included.clamp_(0, sorted_indices_to_keep.size()[1] - 1)
-    sorted_indices_to_keep = sorted_indices_to_keep.scatter_(
-        1, last_included, 1)
+    sorted_indices_to_keep = sorted_indices_to_keep.scatter_(1, last_included, 1)
 
     # Set all logits that are not in the top-p to -10000.
     # This puts the probabilities close to 0.
     keep_indices = sorted_indices_to_keep.scatter(
-                                1,
-                                sorted_indices,
-                                sorted_indices_to_keep,
-                                )
+        1,
+        sorted_indices,
+        sorted_indices_to_keep,
+    )
     return logits.masked_fill(~keep_indices, -10000)
 
 
 def sample_topk(logits, keep_topk):
     top_values, _ = torch.topk(logits, keep_topk, dim=1)
     kth_best = top_values[:, -1].view([-1, 1])
     kth_best = kth_best.repeat([1, logits.shape[1]]).float()
@@ -116,45 +112,78 @@
         keep_topk (int): See
             :func:`~onmt.translate.greedy_search.sample_with_temperature()`.
         keep_topp (float): See
             :func:`~onmt.translate.greedy_search.sample_with_temperature()`.
         beam_size (int): Number of beams to use.
     """
 
-    def __init__(self, pad, bos, eos, unk, start, batch_size, global_scorer,
-                 min_length, block_ngram_repeat, exclusion_tokens,
-                 return_attention, max_length, sampling_temp, keep_topk,
-                 keep_topp, beam_size, ban_unk_token):
+    def __init__(
+        self,
+        pad,
+        bos,
+        eos,
+        unk,
+        start,
+        batch_size,
+        global_scorer,
+        min_length,
+        block_ngram_repeat,
+        exclusion_tokens,
+        return_attention,
+        max_length,
+        sampling_temp,
+        keep_topk,
+        keep_topp,
+        beam_size,
+        ban_unk_token,
+    ):
         super(GreedySearch, self).__init__(
-            pad, bos, eos, unk, start, batch_size, beam_size, global_scorer,
-            min_length, block_ngram_repeat, exclusion_tokens,
-            return_attention, max_length, ban_unk_token)
+            pad,
+            bos,
+            eos,
+            unk,
+            start,
+            batch_size,
+            beam_size,
+            global_scorer,
+            min_length,
+            block_ngram_repeat,
+            exclusion_tokens,
+            return_attention,
+            max_length,
+            ban_unk_token,
+        )
         self.sampling_temp = sampling_temp
         self.keep_topk = keep_topk
         self.keep_topp = keep_topp
         self.topk_scores = None
         self.beam_size = beam_size
 
-    def initialize(self, enc_out, src_len, src_map=None, device=None,
-                   target_prefix=None):
+    def initialize(
+        self, enc_out, src_len, src_map=None, device=None, target_prefix=None
+    ):
         """Initialize for decoding."""
-        (fn_map_state, enc_out,
-            src_map, target_prefix) = self.initialize_tile(
-                enc_out, src_len, src_map, target_prefix)
+        (fn_map_state, enc_out, src_map, target_prefix) = self.initialize_tile(
+            enc_out, src_len, src_map, target_prefix
+        )
         if device is None:
             device = self.get_device_from_enc_out(enc_out)
 
         super(GreedySearch, self).initialize(
-            enc_out, src_len, src_map, device, target_prefix)
+            enc_out, src_len, src_map, device, target_prefix
+        )
         self.select_indices = torch.arange(
-            self.batch_size*self.beam_size, dtype=torch.long, device=device)
-        self.original_batch_idx = fn_map_state(torch.arange(
-            self.batch_size, dtype=torch.long, device=device), dim=0)
-        self.beams_scores = torch.zeros((self.batch_size*self.beam_size, 1),
-                                        dtype=torch.float, device=device)
+            self.batch_size * self.beam_size, dtype=torch.long, device=device
+        )
+        self.original_batch_idx = fn_map_state(
+            torch.arange(self.batch_size, dtype=torch.long, device=device), dim=0
+        )
+        self.beams_scores = torch.zeros(
+            (self.batch_size * self.beam_size, 1), dtype=torch.float, device=device
+        )
         return fn_map_state, enc_out, self.src_len, src_map
 
     @property
     def current_predictions(self):
         return self.alive_seq[:, -1]
 
     @property
@@ -166,24 +195,28 @@
 
         Args:
             log_probs (FloatTensor): ``(batch_size, vocab_size)``.
         """
         # maybe fix some prediction at this step by modifying log_probs
         log_probs = self.target_prefixing(log_probs)
         topk_ids, topk_scores = sample_with_temperature(
-            log_probs, self.sampling_temp, self.keep_topk, self.keep_topp)
+            log_probs, self.sampling_temp, self.keep_topk, self.keep_topp
+        )
         return topk_ids, topk_scores
 
     def align_select_indices(self):
-        nb_finished_beams = (self.is_finished.view(-1).size(0) -
-                             self.select_indices.size(0))
+        nb_finished_beams = self.is_finished.view(-1).size(
+            0
+        ) - self.select_indices.size(0)
         if nb_finished_beams:
             self.select_indices = torch.arange(
-                self.select_indices.size(0), dtype=torch.long,
-                device=self.select_indices.device)
+                self.select_indices.size(0),
+                dtype=torch.long,
+                device=self.select_indices.device,
+            )
 
     def advance(self, log_probs, attn):
         """Select next tokens randomly from the top k possible next tokens.
 
         Args:
             log_probs (FloatTensor): Shaped ``(batch_size, vocab_size)``.
                 These can be logits (``(-inf, inf)``) or log-probs
@@ -215,29 +248,31 @@
 
     def update_finished(self):
         """Finalize scores and predictions."""
         # shape: (sum(~ self.is_finished), 1)
         finished_batches = self.is_finished.view(-1).nonzero(as_tuple=False)
         step = len(self)
         length_penalty = self.global_scorer.length_penalty(
-            step, alpha=self.global_scorer.alpha)
+            step, alpha=self.global_scorer.alpha
+        )
 
         for b in finished_batches.view(-1):
             b_orig = self.original_batch_idx[b]
-            score = self.beams_scores[b, 0]/length_penalty
+            score = self.beams_scores[b, 0] / length_penalty
             pred = self.alive_seq[b, 1:]
             attention = (
-                self.alive_attn[:, b, :self.src_len[b]]
-                if self.alive_attn is not None else [])
+                self.alive_attn[:, b, : self.src_len[b]]
+                if self.alive_attn is not None
+                else []
+            )
             self.hypotheses[b_orig].append((score, pred, attention))
         self.done = self.is_finished.all()
         if self.done:
             for b in range(self.batch_size):
-                best_hyp = sorted(
-                    self.hypotheses[b], key=lambda x: x[0], reverse=True)
+                best_hyp = sorted(self.hypotheses[b], key=lambda x: x[0], reverse=True)
                 for score, pred, attn in best_hyp:
                     self.scores[b].append(score)
                     self.predictions[b].append(pred)
                     self.attention[b].append(attn)
             return
         is_alive = ~self.is_finished.view(-1)
         self.alive_seq = self.alive_seq[is_alive]
@@ -261,19 +296,18 @@
     def advance(self, log_probs, attn):
         super(GreedySearchLM, self).advance(log_probs, attn)
 
         # in LM task src_len is associated with currently generated src
         # and therefore needs to follow the generation
         self.src_len += 1
 
-    def initialize(self, src, src_len, src_map=None, device=None,
-                   target_prefix=None):
+    def initialize(self, src, src_len, src_map=None, device=None, target_prefix=None):
         """Initialize for decoding."""
 
         if device is None:
             device = src.device
 
-        (fn_map_state, _, self.src_len,
-            src_map) = super(GreedySearchLM, self).initialize(
-                None, src_len, src_map, device, target_prefix)
+        (fn_map_state, _, self.src_len, src_map) = super(
+            GreedySearchLM, self
+        ).initialize(None, src_len, src_map, device, target_prefix)
 
         return fn_map_state, src, self.src_len, src_map
```

### Comparing `OpenNMT-py-3.1.2/onmt/translate/penalties.py` & `OpenNMT-py-3.1.3/onmt/translate/penalties.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,67 +35,64 @@
         if cov_pen == "wu":
             return self.coverage_wu
         elif cov_pen == "summary":
             return self.coverage_summary
         elif self._pen_is_none(cov_pen):
             return self.coverage_none
         else:
-            raise NotImplementedError("No '{:s}' coverage penalty.".format(
-                cov_pen))
+            raise NotImplementedError("No '{:s}' coverage penalty.".format(cov_pen))
 
     def _length_penalty(self, length_pen):
         if length_pen == "wu":
             return self.length_wu
         elif length_pen == "avg":
             return self.length_average
         elif self._pen_is_none(length_pen):
             return self.length_none
         else:
-            raise NotImplementedError("No '{:s}' length penalty.".format(
-                length_pen))
+            raise NotImplementedError("No '{:s}' length penalty.".format(length_pen))
 
     # Below are all the different penalty terms implemented so far.
     # Subtract coverage penalty from topk log probs.
     # Divide topk log probs by length penalty.
 
-    def coverage_wu(self, cov, beta=0.):
+    def coverage_wu(self, cov, beta=0.0):
         """GNMT coverage re-ranking score.
 
         See "Google's Neural Machine Translation System" :cite:`wu2016google`.
         ``cov`` is expected to be sized ``(*, seq_len)``, where ``*`` is
         probably ``batch_size x beam_size`` but could be several
         dimensions like ``(batch_size, beam_size)``. If ``cov`` is attention,
         then the ``seq_len`` axis probably sums to (almost) 1.
         """
 
         penalty = -torch.min(cov, cov.clone().fill_(1.0)).log().sum(-1)
         return beta * penalty
 
-    def coverage_summary(self, cov, beta=0.):
+    def coverage_summary(self, cov, beta=0.0):
         """Our summary penalty."""
         penalty = torch.max(cov, cov.clone().fill_(1.0)).sum(-1)
         penalty -= cov.size(-1)
         return beta * penalty
 
-    def coverage_none(self, cov, beta=0.):
+    def coverage_none(self, cov, beta=0.0):
         """Returns zero as penalty"""
-        none = torch.zeros((1,), device=cov.device,
-                           dtype=torch.float)
+        none = torch.zeros((1,), device=cov.device, dtype=torch.float)
         if cov.dim() == 3:
             none = none.unsqueeze(0)
         return none
 
-    def length_wu(self, cur_len, alpha=0.):
+    def length_wu(self, cur_len, alpha=0.0):
         """GNMT length re-ranking score.
 
         See "Google's Neural Machine Translation System" :cite:`wu2016google`.
         """
 
         return ((5 + cur_len) / 6.0) ** alpha
 
-    def length_average(self, cur_len, alpha=1.):
+    def length_average(self, cur_len, alpha=1.0):
         """Returns the current sequence length."""
-        return cur_len ** alpha
+        return cur_len**alpha
 
-    def length_none(self, cur_len, alpha=0.):
+    def length_none(self, cur_len, alpha=0.0):
         """Returns unmodified scores."""
         return 1.0
```

### Comparing `OpenNMT-py-3.1.2/onmt/translate/process_zh.py` & `OpenNMT-py-3.1.3/onmt/translate/process_zh.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import pkuseg
 
 
 def wrap_str_func(func):
     """
     Wrapper to apply str function to the proper key of return_dict.
     """
+
     def wrapper(some_dict):
         some_dict["seg"] = [func(item) for item in some_dict["seg"]]
         return some_dict
+
     return wrapper
 
 
 # Chinese segmentation
 @wrap_str_func
 def zh_segmentator(line, server_model):
     return " ".join(pkuseg.pkuseg().cut(line))
```

### Comparing `OpenNMT-py-3.1.2/onmt/translate/translation.py` & `OpenNMT-py-3.1.3/onmt/translate/translation.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,111 +16,129 @@
     Args:
        data ():
        vocabs ():
        n_best (int): number of translations produced
        replace_unk (bool): replace unknown words using attention
     """
 
-    def __init__(self, data, vocabs, n_best=1, replace_unk=False,
-                 phrase_table=""):
+    def __init__(self, data, vocabs, n_best=1, replace_unk=False, phrase_table=""):
         self.data = data
         self.vocabs = vocabs
         self.n_best = n_best
         self.replace_unk = replace_unk
         self.phrase_table_dict = {}
         if phrase_table != "" and os.path.exists(phrase_table):
             with open(phrase_table) as phrase_table_fd:
                 for line in phrase_table_fd:
                     phrase_src, phrase_trg = line.rstrip("\n").split(
-                        DefaultTokens.PHRASE_TABLE_SEPARATOR)
+                        DefaultTokens.PHRASE_TABLE_SEPARATOR
+                    )
                     self.phrase_table_dict[phrase_src] = phrase_trg
 
     def _build_source_tokens(self, src):
         tokens = []
         for tok in src:
-            tokens.append(self.vocabs['src'].lookup_index(tok))
+            tokens.append(self.vocabs["src"].lookup_index(tok))
             if tokens[-1] == DefaultTokens.PAD:
                 tokens = tokens[:-1]
                 break
         return tokens
 
     def _build_target_tokens(self, src, src_raw, pred, attn):
         tokens = []
 
         for tok in pred:
-            if tok < len(self.vocabs['tgt']):
-                tokens.append(self.vocabs['tgt'].lookup_index(tok))
+            if tok < len(self.vocabs["tgt"]):
+                tokens.append(self.vocabs["tgt"].lookup_index(tok))
             else:
-                vl = len(self.vocabs['tgt'])
-                tokens.append(self.vocabs['src'].lookup_index(tok - vl))
+                vl = len(self.vocabs["tgt"])
+                tokens.append(self.vocabs["src"].lookup_index(tok - vl))
             if tokens[-1] == DefaultTokens.EOS:
                 tokens = tokens[:-1]
                 break
         if self.replace_unk and attn is not None and src is not None:
             for i in range(len(tokens)):
                 if tokens[i] == DefaultTokens.UNK:
-                    _, max_index = attn[i][:len(src_raw)].max(0)
+                    _, max_index = attn[i][: len(src_raw)].max(0)
                     tokens[i] = src_raw[max_index.item()]
                     if self.phrase_table_dict:
                         src_tok = src_raw[max_index.item()]
                         if src_tok in self.phrase_table_dict:
                             tokens[i] = self.phrase_table_dict[src_tok]
         return tokens
 
     def from_batch(self, translation_batch):
         batch = translation_batch["batch"]
-        assert (len(translation_batch["gold_score"]) ==
-               len(translation_batch["predictions"]))
-        batch_size = len(batch['srclen'])
-
-        preds, pred_score, attn, align, gold_score, indices = list(zip(
-            *sorted(zip(translation_batch["predictions"],
+        assert len(translation_batch["gold_score"]) == len(
+            translation_batch["predictions"]
+        )
+        batch_size = len(batch["srclen"])
+
+        preds, pred_score, attn, align, gold_score, indices = list(
+            zip(
+                *sorted(
+                    zip(
+                        translation_batch["predictions"],
                         translation_batch["scores"],
                         translation_batch["attention"],
                         translation_batch["alignment"],
                         translation_batch["gold_score"],
-                        batch['indices']),
-                    key=lambda x: x[-1])))
+                        batch["indices"],
+                    ),
+                    key=lambda x: x[-1],
+                )
+            )
+        )
 
         if not any(align):  # when align is a empty nested list
             align = [None] * batch_size
 
         # Sorting
-        inds, perm = torch.sort(batch['indices'])
+        inds, perm = torch.sort(batch["indices"])
 
-        src = batch['src'][:, :, 0].index_select(0, perm)
-        if 'tgt' in batch.keys():
-            tgt = batch['tgt'][:, :, 0].index_select(0, perm)
+        src = batch["src"][:, :, 0].index_select(0, perm)
+        if "tgt" in batch.keys():
+            tgt = batch["tgt"][:, :, 0].index_select(0, perm)
         else:
             tgt = None
 
         translations = []
 
         for b in range(batch_size):
             if src is not None:
                 src_raw = self._build_source_tokens(src[b, :])
             else:
                 src_raw = None
-            pred_sents = [self._build_target_tokens(
-                src[b, :] if src is not None else None,
-                src_raw,
-                preds[b][n],
-                align[b][n] if align[b] is not None else attn[b][n])
-                for n in range(self.n_best)]
+            pred_sents = [
+                self._build_target_tokens(
+                    src[b, :] if src is not None else None,
+                    src_raw,
+                    preds[b][n],
+                    align[b][n] if align[b] is not None else attn[b][n],
+                )
+                for n in range(self.n_best)
+            ]
             gold_sent = None
             if tgt is not None:
                 gold_sent = self._build_target_tokens(
                     src[b, :] if src is not None else None,
                     src_raw,
-                    tgt[b, 1:] if tgt is not None else None, None)
+                    tgt[b, 1:] if tgt is not None else None,
+                    None,
+                )
 
             translation = Translation(
                 src[b, :] if src is not None else None,
-                src_raw, pred_sents, attn[b], pred_score[b],
-                gold_sent, gold_score[b], align[b]
+                src_raw,
+                pred_sents,
+                attn[b],
+                pred_score[b],
+                gold_sent,
+                gold_score[b],
+                align[b],
             )
             translations.append(translation)
 
         return translations
 
 
 class Translation(object):
@@ -135,50 +153,67 @@
             translation.
         gold_sent (List[str]): Words from gold translation.
         gold_score (List[float]): Log-prob of gold translation.
         word_aligns (List[FloatTensor]): Words Alignment distribution for
             each translation.
     """
 
-    __slots__ = ["src", "src_raw", "pred_sents", "attns", "pred_scores",
-                 "gold_sent", "gold_score", "word_aligns"]
-
-    def __init__(self, src, src_raw, pred_sents,
-                 attn, pred_scores, tgt_sent, gold_score, word_aligns):
+    __slots__ = [
+        "src",
+        "src_raw",
+        "pred_sents",
+        "attns",
+        "pred_scores",
+        "gold_sent",
+        "gold_score",
+        "word_aligns",
+    ]
+
+    def __init__(
+        self,
+        src,
+        src_raw,
+        pred_sents,
+        attn,
+        pred_scores,
+        tgt_sent,
+        gold_score,
+        word_aligns,
+    ):
         self.src = src
         self.src_raw = src_raw
         self.pred_sents = pred_sents
         self.attns = attn
         self.pred_scores = pred_scores
         self.gold_sent = tgt_sent
         self.gold_score = gold_score
         self.word_aligns = word_aligns
 
     def log(self, sent_number):
         """
         Log translation.
         """
 
-        msg = ['\nSENT {}: {}\n'.format(sent_number, self.src_raw)]
+        msg = ["\nSENT {}: {}\n".format(sent_number, self.src_raw)]
 
         best_pred = self.pred_sents[0]
         best_score = self.pred_scores[0]
-        pred_sent = ' '.join(best_pred)
-        msg.append('PRED {}: {}\n'.format(sent_number, pred_sent))
+        pred_sent = " ".join(best_pred)
+        msg.append("PRED {}: {}\n".format(sent_number, pred_sent))
         msg.append("PRED SCORE: {:.4f}\n".format(best_score))
 
         if self.word_aligns is not None:
             pred_align = self.word_aligns[0]
             pred_align_pharaoh = build_align_pharaoh(pred_align)
-            pred_align_sent = ' '.join(pred_align_pharaoh)
+            pred_align_sent = " ".join(pred_align_pharaoh)
             msg.append("ALIGN: {}\n".format(pred_align_sent))
 
         if self.gold_sent is not None:
-            tgt_sent = ' '.join(self.gold_sent)
-            msg.append('GOLD {}: {}\n'.format(sent_number, tgt_sent))
+            tgt_sent = " ".join(self.gold_sent)
+            msg.append("GOLD {}: {}\n".format(sent_number, tgt_sent))
             msg.append(("GOLD SCORE: {:.4f}\n".format(self.gold_score)))
         if len(self.pred_sents) > 1:
-            msg.append('\nBEST HYP:\n')
+            msg.append("\nBEST HYP:\n")
             for score, sent in zip(self.pred_scores, self.pred_sents):
                 msg.append("[{:.4f}] {}\n".format(score, sent))
 
         return "".join(msg)
```

### Comparing `OpenNMT-py-3.1.2/onmt/translate/translation_server.py` & `OpenNMT-py-3.1.3/onmt/translate/translation_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,39 +20,43 @@
 from onmt.utils.logging import init_logger
 from onmt.utils.misc import set_random_seed
 from onmt.utils.misc import check_model_config
 from onmt.utils.alignment import to_word_align
 from onmt.utils.parse import ArgumentParser
 from onmt.translate.translator import build_translator
 from onmt.transforms.features import InferFeatsTransform
-from onmt.inputters.text_utils import (textbatch_to_tensor,
-                                       parse_features,
-                                       append_features_to_text)
+from onmt.inputters.text_utils import (
+    textbatch_to_tensor,
+    parse_features,
+    append_features_to_text,
+)
 from onmt.inputters.inputter import IterOnDevice
 from onmt.utils.alignment import build_align_pharaoh
 
 
 def critical(func):
     """Decorator for critical section (mutually exclusive code)"""
 
     def wrapper(server_model, *args, **kwargs):
         if sys.version_info[0] == 3:
             if not server_model.running_lock.acquire(True, 120):
-                raise ServerModelError("Model %d running lock timeout"
-                                       % server_model.model_id)
+                raise ServerModelError(
+                    "Model %d running lock timeout" % server_model.model_id
+                )
         else:
             # semaphore doesn't have a timeout arg in Python 2.7
             server_model.running_lock.acquire(True)
         try:
             o = func(server_model, *args, **kwargs)
         except (Exception, RuntimeError):
             server_model.running_lock.release()
             raise
         server_model.running_lock.release()
         return o
+
     return wrapper
 
 
 class Timer:
     def __init__(self, start=False):
         self.stime = -1
         self.prev = -1
@@ -82,41 +86,48 @@
     pass
 
 
 class CTranslate2Translator(object):
     """This class wraps the ``ctranslate2.Translator`` object to
     reproduce the ``onmt.translate.translator`` API."""
 
-    def __init__(self, model_path, ct2_translator_args,
-                 ct2_translate_batch_args, target_prefix=False,
-                 preload=False, report_align=False):
+    def __init__(
+        self,
+        model_path,
+        ct2_translator_args,
+        ct2_translate_batch_args,
+        target_prefix=False,
+        preload=False,
+        report_align=False,
+    ):
         import ctranslate2
-        self.translator = ctranslate2.Translator(
-            model_path,
-            **ct2_translator_args)
+
+        self.translator = ctranslate2.Translator(model_path, **ct2_translator_args)
         self.ct2_translate_batch_args = ct2_translate_batch_args
         self.target_prefix = target_prefix
         self.report_align = report_align
         if preload:
             # perform a first request to initialize everything
             dummy_translation = self.translate([{"src": {"src": "a"}}])
-            print("Performed a dummy translation to initialize the model",
-                  dummy_translation)
+            print(
+                "Performed a dummy translation to initialize the model",
+                dummy_translation,
+            )
             time.sleep(1)
             self.translator.unload_model(to_cpu=True)
 
     @staticmethod
-    def convert_onmt_to_ct2_opts(ct2_translator_args,
-                                 ct2_translate_batch_args, opt):
-
+    def convert_onmt_to_ct2_opts(ct2_translator_args, ct2_translate_batch_args, opt):
         def setdefault_if_exists_must_match(obj, name, value):
             if name in obj:
-                assert value == obj[name], f"{name} is different in"\
-                    " OpenNMT-py config and in CTranslate2 config"\
+                assert value == obj[name], (
+                    f"{name} is different in"
+                    " OpenNMT-py config and in CTranslate2 config"
                     f" ({value} vs {obj[name]})"
+                )
             else:
                 obj.setdefault(name, value)
 
         default_for_translator = {
             "inter_threads": 1,
             "intra_threads": torch.get_num_threads(),
             "compute_type": "default",
@@ -125,85 +136,85 @@
             ct2_translator_args.setdefault(name, value)
 
         onmt_for_translator = {
             "device": "cuda" if opt.cuda else "cpu",
             "device_index": opt.gpu if opt.cuda else 0,
         }
         for name, value in onmt_for_translator.items():
-            setdefault_if_exists_must_match(
-                ct2_translator_args, name, value)
+            setdefault_if_exists_must_match(ct2_translator_args, name, value)
 
         onmt_for_translate_batch_enforce = {
             "beam_size": opt.beam_size,
             "max_batch_size": opt.batch_size,
             "num_hypotheses": opt.n_best,
             "max_decoding_length": opt.max_length,
             "min_decoding_length": opt.min_length,
         }
         for name, value in onmt_for_translate_batch_enforce.items():
-            setdefault_if_exists_must_match(
-                ct2_translate_batch_args, name, value)
+            setdefault_if_exists_must_match(ct2_translate_batch_args, name, value)
 
     def translate(self, examples, batch_size=8, tgt=None):
         if "feats" in examples[0]["src"]:
-            batch = [append_features_to_text(
-                        ex["src"]["src"],
-                        ex["src"]["feats"]).split(" ")
-                     for ex in examples]
+            batch = [
+                append_features_to_text(ex["src"]["src"], ex["src"]["feats"]).split(" ")
+                for ex in examples
+            ]
         else:
             batch = [ex["src"]["src"].split(" ") for ex in examples]
         if tgt is not None:
             tgt = [item.split(" ") for item in tgt]
         if self.report_align:
-            self.ct2_translate_batch_args['return_attention'] = True
+            self.ct2_translate_batch_args["return_attention"] = True
         preds = self.translator.translate_batch(
             batch,
             target_prefix=tgt if self.target_prefix else None,
             return_scores=True,
-            **self.ct2_translate_batch_args
+            **self.ct2_translate_batch_args,
         )
         scores = [[item["score"] for item in ex] for ex in preds]
-        predictions = [[" ".join(item["tokens"]) for item in ex]
-                       for ex in preds]
+        predictions = [[" ".join(item["tokens"]) for item in ex] for ex in preds]
         if self.report_align:
-            attentions = [[torch.Tensor(item["attention"]) for item in ex]
-                          for ex in preds]
-            align_pharaohs = [[build_align_pharaoh(item) for item in ex]
-                              for ex in attentions]
-            aligns = [[' '.join(item[0]) for item in ex]
-                      for ex in align_pharaohs]
-            align_scores = [[' '.join(item[1]) for item in ex]
-                            for ex in align_pharaohs]
+            attentions = [
+                [torch.Tensor(item["attention"]) for item in ex] for ex in preds
+            ]
+            align_pharaohs = [
+                [build_align_pharaoh(item) for item in ex] for ex in attentions
+            ]
+            aligns = [[" ".join(item[0]) for item in ex] for ex in align_pharaohs]
+            align_scores = [[" ".join(item[1]) for item in ex] for ex in align_pharaohs]
             predictions = [
                 [
-                    pred + DefaultTokens.ALIGNMENT_SEPARATOR + align
-                    + DefaultTokens.ALIGNMENT_SEPARATOR + align_score
+                    pred
+                    + DefaultTokens.ALIGNMENT_SEPARATOR
+                    + align
+                    + DefaultTokens.ALIGNMENT_SEPARATOR
+                    + align_score
                     for pred, align, align_score in zip(*item)
                 ]
-                for item in zip(
-                    predictions, aligns, align_scores
-                )
+                for item in zip(predictions, aligns, align_scores)
             ]
         return scores, predictions
 
     def to_cpu(self):
         self.translator.unload_model(to_cpu=True)
 
     def to_gpu(self):
         self.translator.load_model()
 
 
 def parse_features_opts(conf):
     features_opt = conf.get("features", None)
     if features_opt is not None:
         features_opt["n_src_feats"] = features_opt.get("n_src_feats", 0)
-        features_opt["src_feats_defaults"] = \
-            features_opt.get("src_feats_defaults", None)
-        features_opt["reversible_tokenization"] = \
-            features_opt.get("reversible_tokenization", "joiner")
+        features_opt["src_feats_defaults"] = features_opt.get(
+            "src_feats_defaults", None
+        )
+        features_opt["reversible_tokenization"] = features_opt.get(
+            "reversible_tokenization", "joiner"
+        )
     return features_opt
 
 
 class TranslationServer(object):
     def __init__(self):
         self.models = {}
         self.next_id = 0
@@ -211,39 +222,41 @@
     def start(self, config_file):
         """Read the config file and pre-/load the models."""
 
         self.config_file = config_file
         with open(self.config_file) as f:
             self.confs = json.load(f)
 
-        self.models_root = self.confs.get('models_root', './available_models')
+        self.models_root = self.confs.get("models_root", "./available_models")
         for i, conf in enumerate(self.confs["models"]):
             if "models" not in conf:
                 if "model" in conf:
                     # backwards compatibility for confs
                     conf["models"] = [conf["model"]]
                 else:
-                    raise ValueError("""Incorrect config file: missing 'models'
-                                        parameter for model #%d""" % i)
+                    raise ValueError(
+                        """Incorrect config file: missing 'models'
+                                        parameter for model #%d"""
+                        % i
+                    )
             check_model_config(conf, self.models_root)
-            kwargs = {'timeout': conf.get('timeout', None),
-                      'load': conf.get('load', None),
-                      'preprocess_opt': conf.get('preprocess', None),
-                      'tokenizer_opt': conf.get('tokenizer', None),
-                      'postprocess_opt': conf.get('postprocess', None),
-                      'custom_opt': conf.get('custom_opt', None),
-                      'on_timeout': conf.get('on_timeout', None),
-                      'model_root': conf.get('model_root', self.models_root),
-                      'ct2_model': conf.get('ct2_model', None),
-                      'ct2_translator_args': conf.get('ct2_translator_args',
-                                                      {}),
-                      'ct2_translate_batch_args': conf.get(
-                          'ct2_translate_batch_args', {}),
-                      'features_opt': parse_features_opts(conf)
-                      }
+            kwargs = {
+                "timeout": conf.get("timeout", None),
+                "load": conf.get("load", None),
+                "preprocess_opt": conf.get("preprocess", None),
+                "tokenizer_opt": conf.get("tokenizer", None),
+                "postprocess_opt": conf.get("postprocess", None),
+                "custom_opt": conf.get("custom_opt", None),
+                "on_timeout": conf.get("on_timeout", None),
+                "model_root": conf.get("model_root", self.models_root),
+                "ct2_model": conf.get("ct2_model", None),
+                "ct2_translator_args": conf.get("ct2_translator_args", {}),
+                "ct2_translate_batch_args": conf.get("ct2_translate_batch_args", {}),
+                "features_opt": parse_features_opts(conf),
+            }
             kwargs = {k: v for (k, v) in kwargs.items() if v is not None}
             model_id = conf.get("id", None)
             opt = conf["opt"]
             opt["models"] = conf["models"]
             self.preload_model(opt, model_id=model_id, **kwargs)
 
     def clone_model(self, model_id, opt, timeout=-1):
@@ -310,16 +323,15 @@
 
         if model_id in self.models and self.models[model_id] is not None:
             self.models[model_id].unload()
         else:
             raise ServerModelError("No such model '%s'" % str(model_id))
 
     def list_models(self):
-        """Return the list of available models
-        """
+        """Return the list of available models"""
         models = []
         for _, model in self.models.items():
             models += [model.to_dict()]
         return models
 
 
 class ServerModel(object):
@@ -337,47 +349,60 @@
         timeout (int): Seconds before running :func: ``do_timeout()``
           Negative values means no timeout
         on_timeout (str): Options are [to_cpu, unload]. Set what to do on
         timeout (see :func: ``do_timeout()``.)
         model_root (str): Path to the model directory
           it must contain the model and tokenizer file"""
 
-    def __init__(self, opt, model_id, preprocess_opt=None, tokenizer_opt=None,
-                 postprocess_opt=None, custom_opt=None, load=False, timeout=-1,
-                 on_timeout="to_cpu", model_root="./", ct2_model=None,
-                 ct2_translator_args=None, ct2_translate_batch_args=None,
-                 features_opt=None):
+    def __init__(
+        self,
+        opt,
+        model_id,
+        preprocess_opt=None,
+        tokenizer_opt=None,
+        postprocess_opt=None,
+        custom_opt=None,
+        load=False,
+        timeout=-1,
+        on_timeout="to_cpu",
+        model_root="./",
+        ct2_model=None,
+        ct2_translator_args=None,
+        ct2_translate_batch_args=None,
+        features_opt=None,
+    ):
         self.model_root = model_root
         self.opt = self.parse_opt(opt)
         self.custom_opt = custom_opt
 
         self.model_id = model_id
         self.preprocess_opt = preprocess_opt
         self.tokenizers_opt = tokenizer_opt
         self.features_opt = features_opt
         self.postprocess_opt = postprocess_opt
         self.timeout = timeout
         self.on_timeout = on_timeout
 
-        self.ct2_model = os.path.join(model_root, ct2_model) \
-            if ct2_model is not None else None
+        self.ct2_model = (
+            os.path.join(model_root, ct2_model) if ct2_model is not None else None
+        )
         self.ct2_translator_args = ct2_translator_args
         self.ct2_translate_batch_args = ct2_translate_batch_args
 
         self.unload_timer = None
         self.user_opt = opt
         self.tokenizers = None
 
         if len(self.opt.log_file) > 0:
             log_file = os.path.join(model_root, self.opt.log_file)
         else:
             log_file = None
-        self.logger = init_logger(log_file=log_file,
-                                  log_file_level=self.opt.log_file_level,
-                                  rotate=True)
+        self.logger = init_logger(
+            log_file=log_file, log_file_level=self.opt.log_file_level, rotate=True
+        )
 
         self.loading_lock = threading.Event()
         self.loading_lock.set()
         self.running_lock = threading.Semaphore(value=1)
 
         set_random_seed(self.opt.seed, self.opt.cuda)
 
@@ -389,33 +414,26 @@
                 function = get_function_by_path(function_path)
                 self.preprocessor.append(function)
 
         if self.tokenizers_opt is not None:
             if "src" in self.tokenizers_opt and "tgt" in self.tokenizers_opt:
                 self.logger.info("Loading src & tgt tokenizer")
                 self.tokenizers = {
-                    'src': self.build_tokenizer(tokenizer_opt['src']),
-                    'tgt': self.build_tokenizer(tokenizer_opt['tgt'])
+                    "src": self.build_tokenizer(tokenizer_opt["src"]),
+                    "tgt": self.build_tokenizer(tokenizer_opt["tgt"]),
                 }
             else:
                 self.logger.info("Loading tokenizer")
-                self.tokenizers_opt = {
-                    'src': tokenizer_opt,
-                    'tgt': tokenizer_opt
-                }
+                self.tokenizers_opt = {"src": tokenizer_opt, "tgt": tokenizer_opt}
                 tokenizer = self.build_tokenizer(tokenizer_opt)
-                self.tokenizers = {
-                    'src': tokenizer,
-                    'tgt': tokenizer
-                }
+                self.tokenizers = {"src": tokenizer, "tgt": tokenizer}
 
         self.feats_transform = None
         if self.features_opt is not None:
-            self.feats_transform = InferFeatsTransform(
-                Namespace(**self.features_opt))
+            self.feats_transform = InferFeatsTransform(Namespace(**self.features_opt))
 
         if self.postprocess_opt is not None:
             self.logger.info("Loading postprocessor")
             self.postprocessor = []
 
             for function_path in self.postprocess_opt:
                 function = get_function_by_path(function_path)
@@ -436,64 +454,66 @@
         """
 
         prec_argv = sys.argv
         sys.argv = sys.argv[:1]
         parser = ArgumentParser()
         onmt.opts.translate_opts(parser)
 
-        models = opt['models']
+        models = opt["models"]
         if not isinstance(models, (list, tuple)):
             models = [models]
-        opt['models'] = [os.path.join(self.model_root, model)
-                         for model in models]
-        opt['src'] = "dummy_src"
-
-        for (k, v) in opt.items():
-            if k == 'models':
-                sys.argv += ['-model']
+        opt["models"] = [os.path.join(self.model_root, model) for model in models]
+        opt["src"] = "dummy_src"
+
+        for k, v in opt.items():
+            if k == "models":
+                sys.argv += ["-model"]
                 sys.argv += [str(model) for model in v]
             elif type(v) == bool:
-                sys.argv += ['-%s' % k]
+                sys.argv += ["-%s" % k]
             else:
-                sys.argv += ['-%s' % k, str(v)]
+                sys.argv += ["-%s" % k, str(v)]
 
         opt = parser.parse_args()
         ArgumentParser.validate_translate_opts(opt)
         opt.cuda = opt.gpu > -1
 
         sys.argv = prec_argv
         return opt
 
     @property
     def loaded(self):
-        return hasattr(self, 'translator')
+        return hasattr(self, "translator")
 
     def load(self, preload=False):
         self.loading_lock.clear()
 
         timer = Timer()
         self.logger.info("Loading model %d" % self.model_id)
         timer.start()
 
         try:
             if self.ct2_model is not None:
                 CTranslate2Translator.convert_onmt_to_ct2_opts(
-                    self.ct2_translator_args, self.ct2_translate_batch_args,
-                    self.opt)
+                    self.ct2_translator_args, self.ct2_translate_batch_args, self.opt
+                )
                 self.translator = CTranslate2Translator(
                     self.ct2_model,
                     ct2_translator_args=self.ct2_translator_args,
                     ct2_translate_batch_args=self.ct2_translate_batch_args,
                     target_prefix=self.opt.tgt_file_prefix,
                     preload=preload,
-                    report_align=self.opt.report_align)
+                    report_align=self.opt.report_align,
+                )
             else:
                 self.translator = build_translator(
-                    self.opt, report_score=False,
-                    out_file=codecs.open(os.devnull, "w", "utf-8"))
+                    self.opt,
+                    report_score=False,
+                    out_file=codecs.open(os.devnull, "w", "utf-8"),
+                )
         except RuntimeError as e:
             raise ServerModelError("Runtime Error: %s" % str(e))
 
         timer.tick("model_loading")
         self.load_time = timer.tick()
         self.reset_unload_timer()
         self.loading_lock.set()
@@ -514,188 +534,187 @@
         timer = Timer()
         timer.start()
 
         self.logger.info("Running translation using %d" % self.model_id)
 
         if not self.loading_lock.is_set():
             self.logger.info(
-                "Model #%d is being loaded by another thread, waiting"
-                % self.model_id)
+                "Model #%d is being loaded by another thread, waiting" % self.model_id
+            )
             if not self.loading_lock.wait(timeout=30):
-                raise ServerModelError("Model %d loading timeout"
-                                       % self.model_id)
+                raise ServerModelError("Model %d loading timeout" % self.model_id)
 
         else:
             if not self.loaded:
                 self.load()
                 timer.tick(name="load")
             elif self.opt.cuda:
                 self.to_gpu()
                 timer.tick(name="to_gpu")
 
         texts = []
         head_spaces = []
         tail_spaces = []
         all_preprocessed = []
         for i, inp in enumerate(inputs):
-            src = inp['src']
+            src = inp["src"]
             whitespaces_before, whitespaces_after = "", ""
-            match_before = re.search(r'^\s+', src)
-            match_after = re.search(r'\s+$', src)
+            match_before = re.search(r"^\s+", src)
+            match_after = re.search(r"\s+$", src)
             if match_before is not None:
                 whitespaces_before = match_before.group(0)
             if match_after is not None:
                 whitespaces_after = match_after.group(0)
             head_spaces.append(whitespaces_before)
             # every segment becomes a dict for flexibility purposes
             seg_dict = self.maybe_preprocess(inp)
             all_preprocessed.append(seg_dict)
             for seg, ref, feats in zip_longest(
-                    seg_dict["seg"], seg_dict["ref"],
-                    seg_dict["src_feats"]):
+                seg_dict["seg"], seg_dict["ref"], seg_dict["src_feats"]
+            ):
                 tok = self.maybe_tokenize(seg)
                 if ref is not None:
-                    ref = self.maybe_tokenize(ref, side='tgt')
+                    ref = self.maybe_tokenize(ref, side="tgt")
                 feats = self.maybe_transform_feats(seg, tok, feats)
                 texts.append((tok, ref, feats))
             tail_spaces.append(whitespaces_after)
 
         empty_indices = []
         examples = []
         for i, (tok, ref_tok, feats) in enumerate(texts):
             if tok == "":
                 empty_indices.append(i)
             else:
                 ex = {
                     "src": {"src": tok},
-                    "tgt": {"tgt": ref_tok} if ref_tok is not None else None
+                    "tgt": {"tgt": ref_tok} if ref_tok is not None else None,
                 }
                 if feats is not None:
                     ex["src"]["feats"] = feats
                 examples.append(ex)
 
         scores = []
         predictions = []
         if len(examples) > 0:
             try:
                 if isinstance(self.translator, CTranslate2Translator):
-                    scores, predictions = self.translator.translate(
-                        examples)
+                    scores, predictions = self.translator.translate(examples)
                 else:
-                    infer_iter = textbatch_to_tensor(
-                        self.translator.vocabs, examples)
-                    device = (self.translator._dev.index
-                              if self.translator._use_cuda else -1)
+                    infer_iter = textbatch_to_tensor(self.translator.vocabs, examples)
+                    device = (
+                        self.translator._dev.index if self.translator._use_cuda else -1
+                    )
                     infer_iter = IterOnDevice(infer_iter, device)
-                    scores, predictions = \
-                        self.translator._translate(infer_iter)
+                    scores, predictions = self.translator._translate(infer_iter)
             except (RuntimeError, Exception) as e:
                 err = "Error: %s" % str(e)
                 self.logger.error(err)
                 self.logger.error("repr(examples): " + repr(examples))
                 self.logger.error("model: #%s" % self.model_id)
                 self.logger.error("model opt: " + str(self.opt.__dict__))
                 self.logger.error(traceback.format_exc())
 
                 raise ServerModelError(err)
 
         timer.tick(name="translation")
-        self.logger.info("""Using model #%d\t%d inputs
-               \ttranslation time: %f""" % (self.model_id, len(texts),
-                                            timer.times['translation']))
+        self.logger.info(
+            """Using model #%d\t%d inputs
+               \ttranslation time: %f"""
+            % (self.model_id, len(texts), timer.times["translation"])
+        )
         self.reset_unload_timer()
 
         # NOTE: translator returns lists of `n_best` list
-        def flatten_list(_list): return sum(_list, [])
-        tiled_texts = [ex["src"]["src"] for ex in examples
-                       for _ in range(self.opt.n_best)]
+        def flatten_list(_list):
+            return sum(_list, [])
+
+        tiled_texts = [
+            ex["src"]["src"] for ex in examples for _ in range(self.opt.n_best)
+        ]
         results = flatten_list(predictions)
 
-        def maybe_item(x): return x.item() if type(x) is torch.Tensor else x
-        scores = [maybe_item(score_tensor)
-                  for score_tensor in flatten_list(scores)]
-
-        results = [self.maybe_detokenize_with_align(result, src)
-                   for result, src in zip(results, tiled_texts)]
-
-        aligns = [align[0] if align is not None else None
-                  for _, align in results]
-        align_scores = [align[1] if align is not None else None
-                        for _, align in results]
+        def maybe_item(x):
+            return x.item() if type(x) is torch.Tensor else x
+
+        scores = [maybe_item(score_tensor) for score_tensor in flatten_list(scores)]
+
+        results = [
+            self.maybe_detokenize_with_align(result, src)
+            for result, src in zip(results, tiled_texts)
+        ]
+
+        aligns = [align[0] if align is not None else None for _, align in results]
+        align_scores = [align[1] if align is not None else None for _, align in results]
         results = [tokens for tokens, _ in results]
 
         # build back results with empty texts
         for i in empty_indices:
             j = i * self.opt.n_best
             results = results[:j] + [""] * self.opt.n_best + results[j:]
             aligns = aligns[:j] + [None] * self.opt.n_best + aligns[j:]
-            align_scores = (align_scores[:j] + [None] *
-                            self.opt.n_best + align_scores[j:])
+            align_scores = (
+                align_scores[:j] + [None] * self.opt.n_best + align_scores[j:]
+            )
             scores = scores[:j] + [0] * self.opt.n_best + scores[j:]
 
         rebuilt_segs, scores, aligns, align_scores = self.rebuild_seg_packages(
-            all_preprocessed, results, scores,
-            aligns, align_scores, self.opt.n_best)
+            all_preprocessed, results, scores, aligns, align_scores, self.opt.n_best
+        )
 
         results = [self.maybe_postprocess(seg) for seg in rebuilt_segs]
 
         head_spaces = [h for h in head_spaces for i in range(self.opt.n_best)]
         tail_spaces = [h for h in tail_spaces for i in range(self.opt.n_best)]
-        results = ["".join(items)
-                   for items in zip(head_spaces, results, tail_spaces)]
+        results = ["".join(items) for items in zip(head_spaces, results, tail_spaces)]
 
         self.logger.info("Translation Results: %d", len(results))
 
-        return (results, scores, self.opt.n_best, timer.times,
-                aligns, align_scores)
+        return (results, scores, self.opt.n_best, timer.times, aligns, align_scores)
 
-    def rebuild_seg_packages(self, all_preprocessed, results,
-                             scores, aligns, align_scores, n_best):
+    def rebuild_seg_packages(
+        self, all_preprocessed, results, scores, aligns, align_scores, n_best
+    ):
         """Rebuild proper segment packages based on initial n_seg."""
 
         offset = 0
         rebuilt_segs = []
         avg_scores = []
         merged_aligns = []
         merged_align_scores = []
         for i, seg_dict in enumerate(all_preprocessed):
             n_seg = seg_dict["n_seg"]
-            sub_results = results[n_best * offset: (offset + n_seg) * n_best]
-            sub_scores = scores[n_best * offset: (offset + n_seg) * n_best]
-            sub_aligns = aligns[n_best * offset: (offset + n_seg) * n_best]
-            sub_align_scores = align_scores[
-                n_best * offset: (offset + n_seg) * n_best
-            ]
+            sub_results = results[n_best * offset : (offset + n_seg) * n_best]
+            sub_scores = scores[n_best * offset : (offset + n_seg) * n_best]
+            sub_aligns = aligns[n_best * offset : (offset + n_seg) * n_best]
+            sub_align_scores = align_scores[n_best * offset : (offset + n_seg) * n_best]
             for j in range(n_best):
                 _seg_dict = deepcopy(seg_dict)
                 _seg_dict["seg"] = list(islice(sub_results, j, None, n_best))
                 rebuilt_segs.append(_seg_dict)
                 sub_sub_scores = list(islice(sub_scores, j, None, n_best))
-                avg_score = sum(sub_sub_scores)/n_seg if n_seg != 0 else 0
+                avg_score = sum(sub_sub_scores) / n_seg if n_seg != 0 else 0
                 avg_scores.append(avg_score)
                 sub_sub_aligns = list(islice(sub_aligns, j, None, n_best))
                 merged_aligns.append(sub_sub_aligns)
-                sub_sub_align_scores = list(islice(sub_align_scores, j,
-                                                   None, n_best))
+                sub_sub_align_scores = list(islice(sub_align_scores, j, None, n_best))
                 merged_align_scores.append(sub_sub_align_scores)
             offset += n_seg
         return rebuilt_segs, avg_scores, merged_aligns, merged_align_scores
 
     def do_timeout(self):
         """Timeout function that frees GPU memory.
 
         Moves the model to CPU or unloads it; depending on
         attr ``self.on_timemout`` value"""
 
         if self.on_timeout == "unload":
             self.logger.info("Timeout: unloading model %d" % self.model_id)
             self.unload()
         if self.on_timeout == "to_cpu":
-            self.logger.info("Timeout: sending model %d to CPU"
-                             % self.model_id)
+            self.logger.info("Timeout: sending model %d to CPU" % self.model_id)
             self.to_cpu()
 
     @critical
     def unload(self):
         self.logger.info("Unloading model %d" % self.model_id)
         del self.translator
         if self.opt.cuda:
@@ -713,21 +732,23 @@
 
         self.stop_unload_timer()
         self.unload_timer = threading.Timer(self.timeout, self.do_timeout)
         self.unload_timer.start()
 
     def to_dict(self):
         hide_opt = ["models", "src"]
-        d = {"model_id": self.model_id,
-             "opt": {k: self.user_opt[k] for k in self.user_opt.keys()
-                     if k not in hide_opt},
-             "models": self.user_opt["models"],
-             "loaded": self.loaded,
-             "timeout": self.timeout,
-             }
+        d = {
+            "model_id": self.model_id,
+            "opt": {
+                k: self.user_opt[k] for k in self.user_opt.keys() if k not in hide_opt
+            },
+            "models": self.user_opt["models"],
+            "loaded": self.loaded,
+            "timeout": self.timeout,
+        }
         if self.tokenizers_opt is not None:
             d["tokenizer"] = self.tokenizers_opt
         return d
 
     @critical
     def to_cpu(self):
         """Move the model to CPU and clear CUDA cache."""
@@ -751,21 +772,28 @@
     def maybe_preprocess(self, sequence):
         """Preprocess the sequence (or not)"""
 
         if sequence.get("src", None) is not None:
             sequence = deepcopy(sequence)
             src, src_feats = parse_features(
                 sequence["src"].strip(),
-                n_feats=(self.features_opt["n_src_feats"]
-                         if self.features_opt is not None else 0),
-                defaults=(self.features_opt["src_feats_defaults"]
-                          if self.features_opt is not None else None))
+                n_feats=(
+                    self.features_opt["n_src_feats"]
+                    if self.features_opt is not None
+                    else 0
+                ),
+                defaults=(
+                    self.features_opt["src_feats_defaults"]
+                    if self.features_opt is not None
+                    else None
+                ),
+            )
             sequence["seg"] = [src]
             sequence.pop("src")
-            sequence["ref"] = [sequence.get('ref', None)]
+            sequence["ref"] = [sequence.get("ref", None)]
             sequence["src_feats"] = [src_feats]
             sequence["n_seg"] = 1
         if self.preprocess_opt is not None:
             return self.preprocess(sequence)
         return sequence
 
     def preprocess(self, sequence):
@@ -787,68 +815,64 @@
         """Apply InferFeatsTransform to features"""
 
         if self.features_opt is None:
             return feats
         if self.feats_transform is None:
             return feats
         ex = {
-            "src": tok_src.split(' '),
-            "src_original": raw_src.split(' '),
-            "src_feats": [f.split(' ') for f in feats]
+            "src": tok_src.split(" "),
+            "src_original": raw_src.split(" "),
+            "src_feats": [f.split(" ") for f in feats],
         }
         transformed_ex = self.feats_transform.apply(ex)
         return [" ".join(f) for f in transformed_ex["src_feats"]]
 
     def build_tokenizer(self, tokenizer_opt):
         """Build tokenizer described by ``tokenizer_opt``."""
 
         if "type" not in tokenizer_opt:
-            raise ValueError(
-                "Missing mandatory tokenizer option 'type'")
+            raise ValueError("Missing mandatory tokenizer option 'type'")
 
-        if tokenizer_opt['type'] == 'sentencepiece':
+        if tokenizer_opt["type"] == "sentencepiece":
             if "model" not in tokenizer_opt:
-                raise ValueError(
-                    "Missing mandatory tokenizer option 'model'")
+                raise ValueError("Missing mandatory tokenizer option 'model'")
             import sentencepiece as spm
+
             tokenizer = spm.SentencePieceProcessor()
-            model_path = os.path.join(self.model_root,
-                                      tokenizer_opt['model'])
+            model_path = os.path.join(self.model_root, tokenizer_opt["model"])
             tokenizer.Load(model_path)
-        elif tokenizer_opt['type'] == 'pyonmttok':
+        elif tokenizer_opt["type"] == "pyonmttok":
             if "params" not in tokenizer_opt:
-                raise ValueError(
-                    "Missing mandatory tokenizer option 'params'")
+                raise ValueError("Missing mandatory tokenizer option 'params'")
             import pyonmttok
+
             if tokenizer_opt["mode"] is not None:
                 mode = tokenizer_opt["mode"]
             else:
                 mode = None
             # load can be called multiple times: modify copy
             tokenizer_params = dict(tokenizer_opt["params"])
             for key, value in tokenizer_opt["params"].items():
                 if key.endswith("path"):
-                    tokenizer_params[key] = os.path.join(
-                        self.model_root, value)
-            tokenizer = pyonmttok.Tokenizer(mode,
-                                            **tokenizer_params)
+                    tokenizer_params[key] = os.path.join(self.model_root, value)
+            tokenizer = pyonmttok.Tokenizer(mode, **tokenizer_params)
         else:
             raise ValueError("Invalid value for tokenizer type")
         return tokenizer
 
-    def maybe_tokenize(self, sequence, side='src'):
+    def maybe_tokenize(self, sequence, side="src"):
         """Tokenize the sequence (or not).
 
         Same args/returns as ``tokenize``"""
 
         if self.tokenizers_opt is not None:
             return self.tokenize(sequence, side)
         return sequence
 
-    def tokenize(self, sequence, side='src'):
+    def tokenize(self, sequence, side="src"):
         """Tokenize a single sequence.
 
         Args:
             sequence (str): The sequence to tokenize.
 
         Returns:
             tok (str): The tokenized sequence."""
@@ -860,32 +884,32 @@
             tok = self.tokenizers[side].EncodeAsPieces(sequence)
             tok = " ".join(tok)
         elif self.tokenizers_opt[side]["type"] == "pyonmttok":
             tok, _ = self.tokenizers[side].tokenize(sequence)
             tok = " ".join(tok)
         return tok
 
-    def tokenizer_marker(self, side='src'):
+    def tokenizer_marker(self, side="src"):
         """Return marker used in ``side`` tokenizer."""
 
         marker = None
         if self.tokenizers_opt is not None:
-            tokenizer_type = self.tokenizers_opt[side].get('type', None)
+            tokenizer_type = self.tokenizers_opt[side].get("type", None)
             if tokenizer_type == "pyonmttok":
-                params = self.tokenizers_opt[side].get('params', None)
+                params = self.tokenizers_opt[side].get("params", None)
                 if params is not None:
                     if params.get("joiner_annotate", None) is not None:
-                        marker = 'joiner'
+                        marker = "joiner"
                     elif params.get("spacer_annotate", None) is not None:
-                        marker = 'spacer'
+                        marker = "spacer"
             elif tokenizer_type == "sentencepiece":
-                marker = 'spacer'
+                marker = "spacer"
         return marker
 
-    def maybe_detokenize_with_align(self, sequence, src, side='tgt'):
+    def maybe_detokenize_with_align(self, sequence, src, side="tgt"):
         """De-tokenize (or not) the sequence (with alignment).
 
         Args:
             sequence (str): The sequence to detokenize, possible with
             alignment seperate by '|||'
 
         Returns:
@@ -893,30 +917,30 @@
             align (str): The alignment correspand to detokenized src/tgt
             sorted or None if no alignment in output."""
 
         align = None
         if self.opt.report_align:
             # output contain alignment
             sequence, align, align_scores = sequence.split(
-                DefaultTokens.ALIGNMENT_SEPARATOR)
-            if align != '':
-                align = self.maybe_convert_align(src, sequence,
-                                                 align, align_scores)
+                DefaultTokens.ALIGNMENT_SEPARATOR
+            )
+            if align != "":
+                align = self.maybe_convert_align(src, sequence, align, align_scores)
         sequence = self.maybe_detokenize(sequence, side)
         return (sequence, align)
 
-    def maybe_detokenize(self, sequence, side='tgt'):
+    def maybe_detokenize(self, sequence, side="tgt"):
         """De-tokenize the sequence (or not)
         Same args/returns as :func:``tokenize()``"""
 
-        if self.tokenizers_opt is not None and ''.join(sequence.split()) != '':
+        if self.tokenizers_opt is not None and "".join(sequence.split()) != "":
             return self.detokenize(sequence, side)
         return sequence
 
-    def detokenize(self, sequence, side='tgt'):
+    def detokenize(self, sequence, side="tgt"):
         """Detokenize a single sequence
 
         Same args/returns as :func:``tokenize()``"""
 
         if self.tokenizers is None:
             raise ValueError("No tokenizer loaded")
 
@@ -936,22 +960,25 @@
             align (str): The alignment correspand to src/tgt pair.
 
         Returns:
             align (str): The alignment correspand to detokenized src/tgt.
         """
 
         if self.tokenizers_opt is not None:
-            src_marker = self.tokenizer_marker(side='src')
-            tgt_marker = self.tokenizer_marker(side='tgt')
+            src_marker = self.tokenizer_marker(side="src")
+            tgt_marker = self.tokenizer_marker(side="tgt")
             if src_marker is None or tgt_marker is None:
-                raise ValueError("To get decoded alignment, joiner/spacer "
-                                 "should be used in both side's tokenizer.")
-            elif ''.join(tgt.split()) != '':
-                align = to_word_align(src, tgt, align, align_scores,
-                                      src_marker, tgt_marker)
+                raise ValueError(
+                    "To get decoded alignment, joiner/spacer "
+                    "should be used in both side's tokenizer."
+                )
+            elif "".join(tgt.split()) != "":
+                align = to_word_align(
+                    src, tgt, align, align_scores, src_marker, tgt_marker
+                )
         return align
 
     def maybe_postprocess(self, sequence):
         """Postprocess the sequence (or not)"""
 
         if self.postprocess_opt is not None:
             return self.postprocess(sequence)
```

### Comparing `OpenNMT-py-3.1.2/onmt/translate/translator.py` & `OpenNMT-py-3.1.3/onmt/translate/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,30 +131,27 @@
         report_score=True,
         logger=None,
         seed=-1,
         with_score=False,
     ):
         self.model = model
         self.vocabs = vocabs
-        self._tgt_vocab = vocabs['tgt']
-        self._tgt_eos_idx = vocabs['tgt'].lookup_token(DefaultTokens.EOS)
-        self._tgt_pad_idx = vocabs['tgt'].lookup_token(DefaultTokens.PAD)
-        self._tgt_bos_idx = vocabs['tgt'].lookup_token(DefaultTokens.BOS)
-        self._tgt_unk_idx = vocabs['tgt'].lookup_token(DefaultTokens.UNK)
-        self._tgt_sep_idx = vocabs['tgt'].lookup_token(DefaultTokens.SEP)
-        self._tgt_start_with =\
-            vocabs['tgt'].lookup_token(vocabs['decoder_start_token'])
+        self._tgt_vocab = vocabs["tgt"]
+        self._tgt_eos_idx = vocabs["tgt"].lookup_token(DefaultTokens.EOS)
+        self._tgt_pad_idx = vocabs["tgt"].lookup_token(DefaultTokens.PAD)
+        self._tgt_bos_idx = vocabs["tgt"].lookup_token(DefaultTokens.BOS)
+        self._tgt_unk_idx = vocabs["tgt"].lookup_token(DefaultTokens.UNK)
+        self._tgt_sep_idx = vocabs["tgt"].lookup_token(DefaultTokens.SEP)
+        self._tgt_start_with = vocabs["tgt"].lookup_token(vocabs["decoder_start_token"])
         self._tgt_vocab_len = len(self._tgt_vocab)
 
         self._gpu = gpu
         self._use_cuda = gpu > -1
         self._dev = (
-            torch.device("cuda", self._gpu)
-            if self._use_cuda
-            else torch.device("cpu")
+            torch.device("cuda", self._gpu) if self._use_cuda else torch.device("cpu")
         )
 
         self.n_best = n_best
         self.max_length = max_length
 
         self.beam_size = beam_size
         self.random_sampling_temp = random_sampling_temp
@@ -164,36 +161,29 @@
         self.min_length = min_length
         self.ban_unk_token = ban_unk_token
         self.ratio = ratio
         self.stepwise_penalty = stepwise_penalty
         self.dump_beam = dump_beam
         self.block_ngram_repeat = block_ngram_repeat
         self.ignore_when_blocking = ignore_when_blocking
-        self._exclusion_idxs = {
-            self._tgt_vocab[t] for t in self.ignore_when_blocking
-        }
+        self._exclusion_idxs = {self._tgt_vocab[t] for t in self.ignore_when_blocking}
         self.replace_unk = replace_unk
         if self.replace_unk and not self.model.decoder.attentional:
             raise ValueError("replace_unk requires an attentional decoder.")
         self.tgt_file_prefix = tgt_file_prefix
         self.phrase_table = phrase_table
         self.data_type = data_type
         self.verbose = verbose
         self.report_time = report_time
 
         self.copy_attn = copy_attn
 
         self.global_scorer = global_scorer
-        if (
-            self.global_scorer.has_cov_pen
-            and not self.model.decoder.attentional
-        ):
-            raise ValueError(
-                "Coverage penalty requires an attentional decoder."
-            )
+        if self.global_scorer.has_cov_pen and not self.model.decoder.attentional:
+            raise ValueError("Coverage penalty requires an attentional decoder.")
         self.out_file = out_file
         self.report_align = report_align
         self.gold_align = gold_align
         self.report_score = report_score
         self.logger = logger
 
         self.use_filter_pred = False
@@ -292,33 +282,33 @@
         enc_out,
         src_len,
         use_src_map,
         enc_final_hs,
         batch_size,
         src,
     ):
-        if 'tgt' in batch.keys() and not self.tgt_file_prefix:
+        if "tgt" in batch.keys() and not self.tgt_file_prefix:
             gs = self._score_target(
                 batch,
                 enc_out,
                 src_len,
-                batch['src_map'] if use_src_map else None,
+                batch["src_map"] if use_src_map else None,
             )
             self.model.decoder.init_state(src, enc_out, enc_final_hs)
         else:
             gs = [0] * batch_size
         return gs
 
     def _translate(
         self,
         infer_iter,
         transform=None,
         attn_debug=False,
         align_debug=False,
-        phrase_table=""
+        phrase_table="",
     ):
         """Translate content of ``src`` and get gold scores from ``tgt``.
 
         Args:
             infer_iter: tensored batch iterator from DynamicDatasetIter
             attn_debug (bool): enables the attention logging
             align_debug (bool): enables the word alignment logging
@@ -346,83 +336,76 @@
         all_scores = []
         all_predictions = []
 
         start_time = time.time()
 
         def _maybe_retranslate(translations, batch):
             """Here we handle the cases of mismatch in number of segments
-               between source and target. We re-translate seg by seg."""
-            inds, perm = torch.sort(batch['indices'])
+            between source and target. We re-translate seg by seg."""
+            inds, perm = torch.sort(batch["indices"])
             trans_copy = deepcopy(translations)
             inserted_so_far = 0
             for j, trans in enumerate(translations):
-                if (trans.src_raw.count(DefaultTokens.SEP) !=
-                        trans.pred_sents[0].count(DefaultTokens.SEP)):
+                if trans.src_raw.count(DefaultTokens.SEP) != trans.pred_sents[0].count(
+                    DefaultTokens.SEP
+                ):
                     self._log("Mismatch in number of ((newline))")
                     # those two should be the same except feat dim
                     # batch['src'][perm[j], :, :])
                     # trans.src
 
                     # we rebuild a small batch made of the sub-segments
                     # in the long segment.
                     idx = (trans.src == self._tgt_sep_idx).nonzero()
                     sub_src = []
                     start_idx = 0
                     for i in range(len(idx)):
                         end_idx = idx[i]
-                        sub_src.append(batch['src'][perm[j],
-                                                    start_idx:end_idx,
-                                                    :])
+                        sub_src.append(batch["src"][perm[j], start_idx:end_idx, :])
                         start_idx = end_idx + 1
-                    end_idx = batch['src'][perm[j],
-                                           :,
-                                           0].ne(self._tgt_pad_idx).sum() - 1
-                    sub_src.append(batch['src'][perm[j],
-                                                start_idx:end_idx,
-                                                :])
-                    t_sub_src = pad_sequence(sub_src,
-                                             batch_first=True,
-                                             padding_value=self._tgt_pad_idx)
-                    t_sub_src_len = t_sub_src[:,
-                                              :,
-                                              0].ne(self._tgt_pad_idx).sum(1)
-                    t_sub_src_ind = torch.tensor([i for i in
-                                                  range(len(sub_src))],
-                                                 dtype=torch.int16)
-                    device = batch['src'].device
-                    t_sub_batch = {'src': t_sub_src.to(device),
-                                   'srclen': t_sub_src_len.to(device),
-                                   'indices': t_sub_src_ind.to(device)}
+                    end_idx = (
+                        batch["src"][perm[j], :, 0].ne(self._tgt_pad_idx).sum() - 1
+                    )
+                    sub_src.append(batch["src"][perm[j], start_idx:end_idx, :])
+                    t_sub_src = pad_sequence(
+                        sub_src, batch_first=True, padding_value=self._tgt_pad_idx
+                    )
+                    t_sub_src_len = t_sub_src[:, :, 0].ne(self._tgt_pad_idx).sum(1)
+                    t_sub_src_ind = torch.tensor(
+                        [i for i in range(len(sub_src))], dtype=torch.int16
+                    )
+                    device = batch["src"].device
+                    t_sub_batch = {
+                        "src": t_sub_src.to(device),
+                        "srclen": t_sub_src_len.to(device),
+                        "indices": t_sub_src_ind.to(device),
+                    }
                     # new sub-batch ready to be translated
                     sub_data = self.translate_batch(t_sub_batch, attn_debug)
                     sub_trans = xlation_builder.from_batch(sub_data)
 
                     # we re-insert the sub-batch in the initial translations
                     trans_copy[j + inserted_so_far] = sub_trans[0]
                     for i in range(1, len(sub_src)):
-                        trans_copy.insert(j + i + inserted_so_far,
-                                          sub_trans[i])
+                        trans_copy.insert(j + i + inserted_so_far, sub_trans[i])
                     inserted_so_far += len(sub_src) - 1
             return trans_copy
 
         for batch in infer_iter:
-
-            batch_data = self.translate_batch(
-                batch, attn_debug
-            )
+            batch_data = self.translate_batch(batch, attn_debug)
 
             translations = xlation_builder.from_batch(batch_data)
             if not isinstance(self, GeneratorLM):
                 translations = _maybe_retranslate(translations, batch)
 
             for j, trans in enumerate(translations):
                 all_scores += [trans.pred_scores[: self.n_best]]
                 pred_score_total += trans.pred_scores[0]
                 pred_words_total += len(trans.pred_sents[0])
-                if 'tgt' in batch.keys():
+                if "tgt" in batch.keys():
                     gold_score_total += trans.gold_score
                     gold_words_total += len(trans.gold_sent) + 1
 
                 n_best_preds = [
                     " ".join(pred) for pred in trans.pred_sents[: self.n_best]
                 ]
 
@@ -431,32 +414,28 @@
                 ]
 
                 if self.report_align:
                     align_pharaohs = [
                         build_align_pharaoh(align)
                         for align in trans.word_aligns[: self.n_best]
                     ]
-                    n_best_preds_align = [
-                        " ".join(align) for align in align_pharaohs
-                    ]
+                    n_best_preds_align = [" ".join(align) for align in align_pharaohs]
                     n_best_preds = [
                         pred + DefaultTokens.ALIGNMENT_SEPARATOR + align
-                        for pred, align in zip(
-                            n_best_preds, n_best_preds_align
-                        )
+                        for pred, align in zip(n_best_preds, n_best_preds_align)
                     ]
 
                 if transform is not None:
                     n_best_preds = transform.batch_apply_reverse(n_best_preds)
 
                 all_predictions += [n_best_preds]
 
                 out_all = [
-                    pred + "\t" + str(score) for (pred, score) in
-                    zip(n_best_preds, n_best_scores)
+                    pred + "\t" + str(score)
+                    for (pred, score) in zip(n_best_preds, n_best_scores)
                 ]
 
                 if self.with_score:
                     self.out_file.write("\n".join(out_all) + "\n")
                 else:
                     self.out_file.write("\n".join(n_best_preds) + "\n")
                 self.out_file.flush()
@@ -498,34 +477,28 @@
                         self.logger.info(output)
                     else:
                         os.write(1, output.encode("utf-8"))
 
         end_time = time.time()
 
         if self.report_score:
-            msg = self._report_score(
-                "PRED", pred_score_total, len(all_scores)
-            )
+            msg = self._report_score("PRED", pred_score_total, len(all_scores))
             self._log(msg)
-            if 'tgt' in batch.keys() and not self.tgt_file_prefix:
-                msg = self._report_score(
-                    "GOLD", gold_score_total, len(all_scores)
-                )
+            if "tgt" in batch.keys() and not self.tgt_file_prefix:
+                msg = self._report_score("GOLD", gold_score_total, len(all_scores))
                 self._log(msg)
 
         if self.report_time:
             total_time = end_time - start_time
             self._log("Total translation time (s): %.1f" % total_time)
             self._log(
                 "Average translation time (ms): %.1f"
                 % (total_time / len(all_predictions) * 1000)
             )
-            self._log(
-                "Tokens per second: %.1f" % (pred_words_total / total_time)
-            )
+            self._log("Tokens per second: %.1f" % (pred_words_total / total_time))
 
         if self.dump_beam:
             import json
 
             json.dump(
                 self.translator.beam_accum,
                 codecs.open(self.dump_beam, "w", "utf-8"),
@@ -544,25 +517,21 @@
             bos (int): bos index to be used.
             pad (int): pad index to be used.
 
         Return:
             batched_nbest_predict (torch.LongTensor): `(batch, n_best, tgt_l)`
         """
         dtype, device = predictions[0][0].dtype, predictions[0][0].device
-        flatten_tgt = [
-            best.tolist() for bests in predictions for best in bests
-        ]
+        flatten_tgt = [best.tolist() for bests in predictions for best in bests]
         paded_tgt = torch.tensor(
             list(zip_longest(*flatten_tgt, fillvalue=pad)),
             dtype=dtype,
             device=device,
         ).T
-        bos_tensor = torch.full(
-            [paded_tgt.size(0), 1], bos, dtype=dtype, device=device
-        )
+        bos_tensor = torch.full([paded_tgt.size(0), 1], bos, dtype=dtype, device=device)
         full_tgt = torch.cat((bos_tensor, paded_tgt), dim=-1)
         batched_nbest_predict = full_tgt.view(
             len(predictions), -1, full_tgt.size(-1)
         )  # (batch, n_best, tgt_l)
         return batched_nbest_predict
 
     def _report_score(self, name, score_total, nb_sentences):
@@ -578,15 +547,15 @@
             score = score_total / nb_sentences
             ppl = np.exp(-score_total.item() / nb_sentences)
             msg = "%s SCORE: %.4f, %s PPL: %.2f NB SENTENCES: %d" % (
                 name,
                 score,
                 name,
                 ppl,
-                nb_sentences
+                nb_sentences,
             )
         return msg
 
     def _decode_and_generate(
         self,
         decoder_in,
         enc_out,
@@ -627,16 +596,15 @@
             scores = self.model.generator(
                 dec_out.view(-1, dec_out.size(2)),
                 attn.view(-1, attn.size(2)),
                 src_map,
             )
             # here we have scores [tgt_lenxbatch, vocab] or [beamxbatch, vocab]
             if batch_offset is None:
-                scores = scores.view(-1, len(batch['srclen']),
-                                     scores.size(-1))
+                scores = scores.view(-1, len(batch["srclen"]), scores.size(-1))
                 scores = scores.transpose(0, 1).contiguous()
             else:
                 scores = scores.view(-1, self.beam_size, scores.size(-1))
             # at this point scores is batch first (dim=0)
             scores = collapse_copy_scores(
                 scores,
                 batch,
@@ -650,17 +618,15 @@
             # or [batch_size, tgt_len, vocab ] when full sentence
         return log_probs, attn
 
     def translate_batch(self, batch, attn_debug):
         """Translate a batch of sentences."""
         raise NotImplementedError
 
-    def _score_target(
-        self, batch, enc_out, src_len, src_map
-    ):
+    def _score_target(self, batch, enc_out, src_len, src_map):
         raise NotImplementedError
 
     def report_results(
         self,
         gold_score,
         batch,
         batch_size,
@@ -701,20 +667,21 @@
     def _align_forward(self, batch, predictions):
         """
         For a batch of input and its prediction, return a list of batch predict
         alignment src indice Tensor in size ``(batch, n_best,)``.
         """
 
         # (0) add BOS and padding to tgt prediction
-        if 'tgt' in batch.keys() and self.gold_align:
+        if "tgt" in batch.keys() and self.gold_align:
             self._log("Computing alignments with gold target")
-            batch_tgt_idxs = batch['tgt'].transpose(1, 2)
+            batch_tgt_idxs = batch["tgt"].transpose(1, 2)
         else:
             batch_tgt_idxs = self._align_pad_prediction(
-                predictions, bos=self._tgt_bos_idx, pad=self._tgt_pad_idx)
+                predictions, bos=self._tgt_bos_idx, pad=self._tgt_pad_idx
+            )
         tgt_mask = (
             batch_tgt_idxs.eq(self._tgt_pad_idx)
             | batch_tgt_idxs.eq(self._tgt_eos_idx)
             | batch_tgt_idxs.eq(self._tgt_bos_idx)
         )
 
         n_best = batch_tgt_idxs.size(1)
@@ -738,39 +705,35 @@
         # (3) Init decoder with n_best src,
         self.model.decoder.init_state(src, enc_out, enc_states)
         # reshape tgt to ``(len, batch * n_best, nfeat)``
         # it should be done in a better way
         tgt = batch_tgt_idxs.view(-1, batch_tgt_idxs.size(-1)).T.unsqueeze(-1)
         dec_in = tgt[:-1].transpose(0, 1)  # exclude last target from inputs
         # here dec_in is batch first
-        _, attns = self.model.decoder(
-            dec_in, enc_out, src_len=src_len, with_align=True
-        )
+        _, attns = self.model.decoder(dec_in, enc_out, src_len=src_len, with_align=True)
 
         alignment_attn = attns["align"]  # ``(B, tgt_len-1, src_len)``
         # masked_select
         align_tgt_mask = tgt_mask.view(-1, tgt_mask.size(-1))
         prediction_mask = align_tgt_mask[:, 1:]  # exclude bos to match pred
         # get aligned src id for each prediction's valid tgt tokens
-        alignement = extract_alignment(
-            alignment_attn, prediction_mask, src_len, n_best
-        )
+        alignement = extract_alignment(alignment_attn, prediction_mask, src_len, n_best)
         return alignement
 
     def translate_batch(self, batch, attn_debug):
         """Translate a batch of sentences."""
         with torch.no_grad():
             if self.sample_from_topk != 0 or self.sample_from_topp != 0:
                 decode_strategy = GreedySearch(
                     pad=self._tgt_pad_idx,
                     bos=self._tgt_bos_idx,
                     eos=self._tgt_eos_idx,
                     unk=self._tgt_unk_idx,
                     start=self._tgt_start_with,
-                    batch_size=len(batch['srclen']),
+                    batch_size=len(batch["srclen"]),
                     global_scorer=self.global_scorer,
                     min_length=self.min_length,
                     max_length=self.max_length,
                     block_ngram_repeat=self.block_ngram_repeat,
                     exclusion_tokens=self._exclusion_idxs,
                     return_attention=attn_debug or self.replace_unk,
                     sampling_temp=self.random_sampling_temp,
@@ -780,15 +743,15 @@
                     ban_unk_token=self.ban_unk_token,
                 )
             else:
                 # TODO: support these blacklisted features
                 assert not self.dump_beam
                 decode_strategy = BeamSearch(
                     self.beam_size,
-                    batch_size=len(batch['srclen']),
+                    batch_size=len(batch["srclen"]),
                     pad=self._tgt_pad_idx,
                     bos=self._tgt_bos_idx,
                     eos=self._tgt_eos_idx,
                     unk=self._tgt_unk_idx,
                     start=self._tgt_start_with,
                     n_best=self.n_best,
                     global_scorer=self.global_scorer,
@@ -797,57 +760,48 @@
                     return_attention=attn_debug or self.replace_unk,
                     block_ngram_repeat=self.block_ngram_repeat,
                     exclusion_tokens=self._exclusion_idxs,
                     stepwise_penalty=self.stepwise_penalty,
                     ratio=self.ratio,
                     ban_unk_token=self.ban_unk_token,
                 )
-            return self._translate_batch_with_strategy(
-                batch, decode_strategy
-            )
+            return self._translate_batch_with_strategy(batch, decode_strategy)
 
     def _run_encoder(self, batch):
-        src = batch['src']
-        src_len = batch['srclen']
-        batch_size = len(batch['srclen'])
+        src = batch["src"]
+        src_len = batch["srclen"]
+        batch_size = len(batch["srclen"])
 
-        enc_out, enc_final_hs, src_len = self.model.encoder(
-            src, src_len
-        )
+        enc_out, enc_final_hs, src_len = self.model.encoder(src, src_len)
 
         if src_len is None:
             assert not isinstance(
                 enc_out, tuple
             ), "Ensemble decoding only supported for text data"
             src_len = (
-                torch.Tensor(batch_size)
-                .type_as(enc_out)
-                .long()
-                .fill_(enc_out.size(1))
+                torch.Tensor(batch_size).type_as(enc_out).long().fill_(enc_out.size(1))
             )
         return src, enc_final_hs, enc_out, src_len
 
-    def _translate_batch_with_strategy(
-        self, batch, decode_strategy
-    ):
+    def _translate_batch_with_strategy(self, batch, decode_strategy):
         """Translate a batch of sentences step by step using cache.
 
         Args:
             batch: a batch of sentences, yield by data iterator.
             decode_strategy (DecodeStrategy): A decode strategy to use for
                 generate translation step by step.
 
         Returns:
             results (dict): The translation results.
         """
         # (0) Prep the components of the search.
         use_src_map = self.copy_attn
         parallel_paths = decode_strategy.parallel_paths  # beam_size
 
-        batch_size = len(batch['srclen'])
+        batch_size = len(batch["srclen"])
 
         # (1) Run the encoder on the src.
         src, enc_final_hs, enc_out, src_len = self._run_encoder(batch)
 
         self.model.decoder.init_state(src, enc_out, enc_final_hs)
 
         gold_score = self._gold_score(
@@ -857,22 +811,17 @@
             use_src_map,
             enc_final_hs,
             batch_size,
             src,
         )
 
         # (2) prep decode_strategy. Possibly repeat src objects.
-        src_map = batch['src_map'] if use_src_map else None
-        target_prefix = batch['tgt'] if self.tgt_file_prefix else None
-        (
-            fn_map_state,
-            enc_out,
-            src_len_tiled,
-            src_map,
-        ) = decode_strategy.initialize(
+        src_map = batch["src_map"] if use_src_map else None
+        target_prefix = batch["tgt"] if self.tgt_file_prefix else None
+        (fn_map_state, enc_out, src_len_tiled, src_map,) = decode_strategy.initialize(
             enc_out, src_len, src_map, target_prefix=target_prefix
         )
 
         if fn_map_state is not None:
             self.model.decoder.map_state(fn_map_state)
 
         # (3) Begin decoding step by step:
@@ -899,17 +848,15 @@
                     break
 
             select_indices = decode_strategy.select_indices
 
             if any_finished:
                 # Reorder states.
                 if isinstance(enc_out, tuple):
-                    enc_out = tuple(
-                        x.index_select(0, select_indices) for x in enc_out
-                    )
+                    enc_out = tuple(x.index_select(0, select_indices) for x in enc_out)
                 else:
                     enc_out = enc_out.index_select(0, select_indices)
 
                 src_len_tiled = src_len_tiled.index_select(0, select_indices)
 
                 if src_map is not None:
                     src_map = src_map.index_select(0, select_indices)
@@ -925,18 +872,16 @@
             batch_size,
             src,
             src_len,
             use_src_map,
             decode_strategy,
         )
 
-    def _score_target(
-        self, batch, enc_out, src_len, src_map
-    ):
-        tgt = batch['tgt']
+    def _score_target(self, batch, enc_out, src_len, src_map):
+        tgt = batch["tgt"]
         tgt_in = tgt[:, :-1, :]
 
         log_probs, attn = self._decode_and_generate(
             tgt_in,
             enc_out,
             batch,
             src_len=src_len,
@@ -964,34 +909,36 @@
         For a batch of input and its prediction, return a list of batch predict
         alignment src indice Tensor in size ``(batch, n_best,)``.
         """
         raise NotImplementedError
 
     def translate_batch(self, batch, attn_debug):
         """Translate a batch of sentences."""
-        batch_size = len(batch['srclen'])
+        batch_size = len(batch["srclen"])
         if batch_size != 1:
-            warning_msg = ("GeneratorLM does not support batch_size != 1"
-                           " nicely. You can remove this limitation here."
-                           " With batch_size > 1 the end of each input is"
-                           " repeated until the input is finished. Then"
-                           " generation will start.")
+            warning_msg = (
+                "GeneratorLM does not support batch_size != 1"
+                " nicely. You can remove this limitation here."
+                " With batch_size > 1 the end of each input is"
+                " repeated until the input is finished. Then"
+                " generation will start."
+            )
             if self.logger:
                 self.logger.info(warning_msg)
             else:
                 os.write(1, warning_msg.encode("utf-8"))
         with torch.no_grad():
             if self.sample_from_topk != 0 or self.sample_from_topp != 0:
                 decode_strategy = GreedySearchLM(
                     pad=self._tgt_pad_idx,
                     bos=self._tgt_bos_idx,
                     eos=self._tgt_eos_idx,
                     unk=self._tgt_unk_idx,
                     start=self._tgt_start_with,
-                    batch_size=len(batch['srclen']),
+                    batch_size=len(batch["srclen"]),
                     global_scorer=self.global_scorer,
                     min_length=self.min_length,
                     max_length=self.max_length,
                     block_ngram_repeat=self.block_ngram_repeat,
                     exclusion_tokens=self._exclusion_idxs,
                     return_attention=attn_debug or self.replace_unk,
                     sampling_temp=self.random_sampling_temp,
@@ -1001,15 +948,15 @@
                     ban_unk_token=self.ban_unk_token,
                 )
             else:
                 # TODO: support these blacklisted features
                 assert not self.dump_beam
                 decode_strategy = BeamSearchLM(
                     self.beam_size,
-                    batch_size=len(batch['srclen']),
+                    batch_size=len(batch["srclen"]),
                     pad=self._tgt_pad_idx,
                     bos=self._tgt_bos_idx,
                     eos=self._tgt_eos_idx,
                     unk=self._tgt_unk_idx,
                     start=self._tgt_start_with,
                     n_best=self.n_best,
                     global_scorer=self.global_scorer,
@@ -1018,17 +965,15 @@
                     return_attention=attn_debug or self.replace_unk,
                     block_ngram_repeat=self.block_ngram_repeat,
                     exclusion_tokens=self._exclusion_idxs,
                     stepwise_penalty=self.stepwise_penalty,
                     ratio=self.ratio,
                     ban_unk_token=self.ban_unk_token,
                 )
-            return self._translate_batch_with_strategy(
-                batch, decode_strategy
-            )
+            return self._translate_batch_with_strategy(batch, decode_strategy)
 
     @classmethod
     def split_src_to_prevent_padding(cls, src, src_len):
         min_len_batch = torch.min(src_len).item()
         target_prefix = None
         if min_len_batch > 0 and min_len_batch < src.size(1):
             target_prefix = src[:, min_len_batch:, :]
@@ -1039,87 +984,77 @@
     def tile_to_beam_size_after_initial_step(self, fn_map_state, log_probs):
         if fn_map_state is not None:
             log_probs = fn_map_state(log_probs, dim=0)
             self.model.decoder.map_state(fn_map_state)
             log_probs = log_probs[:, -1, :]
         return log_probs
 
-    def _translate_batch_with_strategy(
-        self, batch, decode_strategy
-    ):
+    def _translate_batch_with_strategy(self, batch, decode_strategy):
         """Translate a batch of sentences step by step using cache.
 
         Args:
             batch: a batch of sentences, yield by data iterator.
             decode_strategy (DecodeStrategy): A decode strategy to use for
                 generate translation step by step.
 
         Returns:
             results (dict): The translation results.
         """
         # (0) Prep the components of the search.
         use_src_map = self.copy_attn
         parallel_paths = decode_strategy.parallel_paths  # beam_size
-        batch_size = len(batch['srclen'])
+        batch_size = len(batch["srclen"])
 
         # (1) split src into src and target_prefix to avoid padding.
-        src = batch['src']
-        src_len = batch['srclen']
+        src = batch["src"]
+        src_len = batch["srclen"]
 
-        src, src_len, target_prefix = self.split_src_to_prevent_padding(
-            src, src_len
-        )
+        src, src_len, target_prefix = self.split_src_to_prevent_padding(src, src_len)
 
         # (2) init decoder
         self.model.decoder.init_state(src, None, None)
         gold_score = self._gold_score(
             batch,
             None,
             src_len,
             use_src_map,
             None,
             batch_size,
             src,
         )
 
         # (3) prep decode_strategy. Possibly repeat src objects.
-        src_map = batch['src_map'] if use_src_map else None
-        (
-            fn_map_state,
-            src,
-            src_len_tiled,
-            src_map,
-        ) = decode_strategy.initialize(
+        src_map = batch["src_map"] if use_src_map else None
+        (fn_map_state, src, src_len_tiled, src_map,) = decode_strategy.initialize(
             src,
             src_len,
             src_map,
             target_prefix=target_prefix,
         )
 
         # (4) Begin decoding step by step:
         for step in range(decode_strategy.max_length):
             decoder_input = (
-                src
-                if step == 0
-                else decode_strategy.current_predictions.view(-1, 1, 1)
+                src if step == 0 else decode_strategy.current_predictions.view(-1, 1, 1)
             )
 
             log_probs, attn = self._decode_and_generate(
                 decoder_input,
                 None,
                 batch,
                 src_len=src_len_tiled.clone(),
                 src_map=src_map,
                 step=step if step == 0 else step + src_len[0].item(),
                 batch_offset=decode_strategy.batch_offset,
             )
 
             if step == 0:
                 log_probs = self.tile_to_beam_size_after_initial_step(
-                    fn_map_state, log_probs)
+                    fn_map_state, log_probs
+                )
 
             decode_strategy.advance(log_probs, attn)
             any_finished = decode_strategy.is_finished.any()
             if any_finished:
                 decode_strategy.update_finished()
                 if decode_strategy.done:
                     break
@@ -1145,20 +1080,18 @@
             batch_size,
             src,
             src_len,
             use_src_map,
             decode_strategy,
         )
 
-    def _score_target(
-        self, batch, enc_out, src_len, src_map
-    ):
-        src = batch['src']
-        src_len = batch['srclen']
-        tgt = batch['tgt']
+    def _score_target(self, batch, enc_out, src_len, src_map):
+        src = batch["src"]
+        src_len = batch["srclen"]
+        tgt = batch["tgt"]
 
         log_probs, attn = self._decode_and_generate(
             src,
             None,
             batch,
             src_len=src_len,
             src_map=src_map,
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/__init__.py` & `OpenNMT-py-3.1.3/onmt/utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 """Module defining various utilities."""
 from onmt.utils.misc import use_gpu, set_random_seed
 from onmt.utils.alignment import make_batch_align_matrix
 from onmt.utils.report_manager import ReportMgr, build_report_manager
 from onmt.utils.statistics import Statistics
-from onmt.utils.optimizers import MultipleOptimizer, \
-    Optimizer, AdaFactor, FusedAdam
+from onmt.utils.optimizers import MultipleOptimizer, Optimizer, AdaFactor, FusedAdam
 from onmt.utils.earlystopping import EarlyStopping, scorers_from_opts
 
-__all__ = ["use_gpu", "set_random_seed", "ReportMgr",
-           "build_report_manager", "Statistics",
-           "MultipleOptimizer", "Optimizer", "AdaFactor",
-           "FusedAdam", "EarlyStopping",
-           "scorers_from_opts", "make_batch_align_matrix"]
+__all__ = [
+    "use_gpu",
+    "set_random_seed",
+    "ReportMgr",
+    "build_report_manager",
+    "Statistics",
+    "MultipleOptimizer",
+    "Optimizer",
+    "AdaFactor",
+    "FusedAdam",
+    "EarlyStopping",
+    "scorers_from_opts",
+    "make_batch_align_matrix",
+]
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/alignment.py` & `OpenNMT-py-3.1.3/onmt/utils/alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         index_tensor (LongTensor): ``(N, 3)`` of [batch_id, tgt_id, src_id]
         size (List[int]): Size of the sparse tensor.
         normalize (bool): if normalize the 2nd dim of resulting tensor.
     """
     n_fill, device = index_tensor.size(0), index_tensor.device
     value_tensor = torch.ones([n_fill], dtype=torch.float)
     dense_tensor = torch.sparse_coo_tensor(
-        index_tensor.t(), value_tensor, size=size, device=device).to_dense()
+        index_tensor.t(), value_tensor, size=size, device=device
+    ).to_dense()
     if normalize:
         row_sum = dense_tensor.sum(-1, keepdim=True)  # sum by row(tgt)
         # threshold on 1 to avoid div by 0
         torch.nn.functional.threshold(row_sum, 1, 1, inplace=True)
         dense_tensor.div_(row_sum)
     return dense_tensor
 
@@ -49,52 +50,57 @@
     batch_size_n_best = align_matrix.size(0)
     assert batch_size_n_best % n_best == 0
 
     alignments = [[] for _ in range(batch_size_n_best // n_best)]
 
     # treat alignment matrix one by one as each have different lengths
     for i, (am_b, tgt_mask_b, src_len) in enumerate(
-            zip(align_matrix, tgt_mask, src_len)):
+        zip(align_matrix, tgt_mask, src_len)
+    ):
         valid_tgt = ~tgt_mask_b
         valid_tgt_len = valid_tgt.sum()
         if valid_tgt_len == 0:
             # No alignment if not exist valid tgt token
             valid_alignment = None
         else:
             # get valid alignment (sub-matrix from full paded aligment matrix)
-            am_valid_tgt = am_b.masked_select(valid_tgt.unsqueeze(-1)) \
-                               .view(valid_tgt_len, -1)
+            am_valid_tgt = am_b.masked_select(valid_tgt.unsqueeze(-1)).view(
+                valid_tgt_len, -1
+            )
             valid_alignment = am_valid_tgt[:, :src_len]  # only keep valid src
         alignments[i // n_best].append(valid_alignment)
 
     return alignments
 
 
 def build_align_pharaoh(valid_alignment):
     """Convert valid alignment matrix to i-j (from 0) Pharaoh format pairs,
     or empty list if it's None.
     """
     align_pairs = []
     align_scores = []
     if isinstance(valid_alignment, torch.Tensor):
         tgt_align_src_id = valid_alignment.argmax(dim=-1)
-        align_scores = torch.divide(valid_alignment.max(dim=-1).values,
-                                    valid_alignment.sum(dim=-1))
+        align_scores = torch.divide(
+            valid_alignment.max(dim=-1).values, valid_alignment.sum(dim=-1)
+        )
         for tgt_id, src_id in enumerate(tgt_align_src_id.tolist()):
             align_pairs.append(str(src_id) + "-" + str(tgt_id))
-        align_scores = ["{0}-{1:.5f}".format(i, s)
-                        for i, s in enumerate(align_scores.tolist())]
-        align_pairs.sort(key=lambda x: int(x.split('-')[-1]))  # sort by tgt_id
-        align_pairs.sort(key=lambda x: int(x.split('-')[0]))  # sort by src_id
+        align_scores = [
+            "{0}-{1:.5f}".format(i, s) for i, s in enumerate(align_scores.tolist())
+        ]
+        align_pairs.sort(key=lambda x: int(x.split("-")[-1]))  # sort by tgt_id
+        align_pairs.sort(key=lambda x: int(x.split("-")[0]))  # sort by src_id
         print(align_scores)
     return align_pairs, align_scores
 
 
-def to_word_align(src, tgt, subword_align, subword_align_scores,
-                  m_src='joiner', m_tgt='joiner'):
+def to_word_align(
+    src, tgt, subword_align, subword_align_scores, m_src="joiner", m_tgt="joiner"
+):
     """Convert subword alignment to word alignment.
 
     Args:
         src (string): tokenized sentence in source language.
         tgt (string): tokenized sentence in target language.
         subword_align (string): align_pharaoh correspond to src-tgt.
         m_src (string): tokenization mode used in src,
@@ -106,39 +112,46 @@
         word_align (string): converted alignments correspand to
             detokenized src-tgt.
     """
     assert m_src in ["joiner", "spacer"], "Invalid value for argument m_src!"
     assert m_tgt in ["joiner", "spacer"], "Invalid value for argument m_tgt!"
 
     src, tgt = src.strip().split(), tgt.strip().split()
-    subword_align = {(int(a), int(b)) for a, b in (x.split("-")
-                     for x in subword_align.split())}
-
-    subword_align_scores = dict((int(a), float(b)) for a, b in (x.split("-")
-                                for x in subword_align_scores.split()))
+    subword_align = {
+        (int(a), int(b)) for a, b in (x.split("-") for x in subword_align.split())
+    }
+
+    subword_align_scores = dict(
+        (int(a), float(b))
+        for a, b in (x.split("-") for x in subword_align_scores.split())
+    )
 
-    src_map = (subword_map_by_spacer(src) if m_src == 'spacer'
-               else subword_map_by_joiner(src))
+    src_map = (
+        subword_map_by_spacer(src) if m_src == "spacer" else subword_map_by_joiner(src)
+    )
 
-    tgt_map = (subword_map_by_spacer(tgt) if m_tgt == 'spacer'
-               else subword_map_by_joiner(tgt))
+    tgt_map = (
+        subword_map_by_spacer(tgt) if m_tgt == "spacer" else subword_map_by_joiner(tgt)
+    )
 
-    word_align = list({"{}-{}".format(src_map[a], tgt_map[b])
-                       for a, b in subword_align})
+    word_align = list(
+        {"{}-{}".format(src_map[a], tgt_map[b]) for a, b in subword_align}
+    )
 
     word_align_scores = list(
-        {"{}-{}".format(tgt_map[a],
-                        subword_align_scores[a])
-         for a in subword_align_scores.keys()}
+        {
+            "{}-{}".format(tgt_map[a], subword_align_scores[a])
+            for a in subword_align_scores.keys()
+        }
     )
 
-    word_align.sort(key=lambda x: int(x.split('-')[-1]))  # sort by tgt_id
-    word_align.sort(key=lambda x: int(x.split('-')[0]))  # sort by src_id
+    word_align.sort(key=lambda x: int(x.split("-")[-1]))  # sort by tgt_id
+    word_align.sort(key=lambda x: int(x.split("-")[0]))  # sort by src_id
 
-    word_align_scores.sort(key=lambda x: int(x.split('-')[0]))
+    word_align_scores.sort(key=lambda x: int(x.split("-")[0]))
 
     return " ".join(word_align), " ".join(word_align_scores)
 
 
 # Helper functions
 def begin_uppercase(token):
     return token == SubwordMarker.BEGIN_UPPERCASE
@@ -149,46 +162,51 @@
 
 
 def begin_case(token):
     return token == SubwordMarker.BEGIN_CASED
 
 
 def case_markup(token):
-    return begin_uppercase(token) \
-        or end_uppercase(token) \
-        or begin_case(token)
+    return begin_uppercase(token) or end_uppercase(token) or begin_case(token)
 
 
-def subword_map_by_joiner(subwords,
-                          original_subwords=None,
-                          marker=SubwordMarker.JOINER):
+def subword_map_by_joiner(
+    subwords, original_subwords=None, marker=SubwordMarker.JOINER
+):
     """Return word id for each subword token (annotate by joiner)."""
 
     flags = [1] * len(subwords)
     j = 0
     finished = True
     for i, tok in enumerate(subwords):
-
-        previous_tok = subwords[i-1] if i else ""  # Previous N-1 token
-        previous_tok_2 = subwords[i-2] if i > 1 else ""  # Previous N-2 token
+        previous_tok = subwords[i - 1] if i else ""  # Previous N-1 token
+        previous_tok_2 = subwords[i - 2] if i > 1 else ""  # Previous N-2 token
         # Keeps track of the original words/subwords
         # ('prior_tokenization' option)
-        current_original_subword = "" if not original_subwords \
-            else original_subwords[j] if j < len(original_subwords) else ""
+        current_original_subword = (
+            ""
+            if not original_subwords
+            else original_subwords[j]
+            if j < len(original_subwords)
+            else ""
+        )
 
         if tok.startswith(marker) and tok != current_original_subword:
             flags[i] = 0
-        elif (previous_tok.endswith(marker)
-                or begin_case(previous_tok)
-                or begin_uppercase(previous_tok)) \
-                and not finished:
+        elif (
+            previous_tok.endswith(marker)
+            or begin_case(previous_tok)
+            or begin_uppercase(previous_tok)
+        ) and not finished:
             flags[i] = 0
-        elif previous_tok_2.endswith(marker) \
-                and case_markup(previous_tok) \
-                and not finished:
+        elif (
+            previous_tok_2.endswith(marker)
+            and case_markup(previous_tok)
+            and not finished
+        ):
             flags[i] = 0
         elif end_uppercase(tok) and tok != current_original_subword:
             flags[i] = 0
         else:
             finished = False
             if tok == current_original_subword:
                 finished = True
@@ -204,24 +222,24 @@
 
 def subword_map_by_spacer(subwords, marker=SubwordMarker.SPACER):
     """Return word id for each subword token (annotate by spacer)."""
     flags = [0] * len(subwords)
     for i, tok in enumerate(subwords):
         if marker in tok:
             if case_markup(tok.replace(marker, "")):
-                if i < len(subwords)-1:
+                if i < len(subwords) - 1:
                     flags[i] = 1
             else:
                 if i > 0:
-                    previous = subwords[i-1].replace(marker, "")
+                    previous = subwords[i - 1].replace(marker, "")
                     if not case_markup(previous):
                         flags[i] = 1
 
     # In case there is a final case_markup when new_spacer is on
-    for i in range(1, len(subwords)-1):
+    for i in range(1, len(subwords) - 1):
         if case_markup(subwords[-i]):
             flags[-i] = 0
         elif subwords[-i] == marker:
             flags[-i] = 0
             break
 
     word_group = list(accumulate(flags))
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/cnn_factory.py` & `OpenNMT-py-3.1.3/onmt/utils/cnn_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,53 +3,55 @@
 """
 import torch
 import torch.nn as nn
 import torch.nn.init as init
 
 import onmt.modules
 
-SCALE_WEIGHT = 0.5 ** 0.5
+SCALE_WEIGHT = 0.5**0.5
 
 
 def shape_transform(x):
-    """ Tranform the size of the tensors to fit for conv input. """
+    """Tranform the size of the tensors to fit for conv input."""
     return torch.unsqueeze(torch.transpose(x, 1, 2), 3)
 
 
 class GatedConv(nn.Module):
-    """ Gated convolution for CNN class """
+    """Gated convolution for CNN class"""
 
     def __init__(self, input_size, width=3, dropout=0.2, nopad=False):
         super(GatedConv, self).__init__()
         self.conv = onmt.modules.WeightNormConv2d(
-            input_size, 2 * input_size, kernel_size=(width, 1), stride=(1, 1),
-            padding=(width // 2 * (1 - nopad), 0))
+            input_size,
+            2 * input_size,
+            kernel_size=(width, 1),
+            stride=(1, 1),
+            padding=(width // 2 * (1 - nopad), 0),
+        )
         # this param init is overridden by model_builder, useless then.
-        init.xavier_uniform_(self.conv.weight, gain=(4 * (1 - dropout))**0.5)
+        init.xavier_uniform_(self.conv.weight, gain=(4 * (1 - dropout)) ** 0.5)
         self.dropout = nn.Dropout(dropout)
 
     def forward(self, x_var):
         x_var = self.dropout(x_var)
         x_var = self.conv(x_var)
         out, gate = x_var.split(int(x_var.size(1) / 2), 1)
         out = out * torch.sigmoid(gate)
         return out
 
 
 class StackedCNN(nn.Module):
-    """ Stacked CNN class """
+    """Stacked CNN class"""
 
-    def __init__(self, num_layers, input_size, cnn_kernel_width=3,
-                 dropout=0.2):
+    def __init__(self, num_layers, input_size, cnn_kernel_width=3, dropout=0.2):
         super(StackedCNN, self).__init__()
         self.dropout = dropout
         self.num_layers = num_layers
         self.layers = nn.ModuleList()
         for _ in range(num_layers):
-            self.layers.append(
-                GatedConv(input_size, cnn_kernel_width, dropout))
+            self.layers.append(GatedConv(input_size, cnn_kernel_width, dropout))
 
     def forward(self, x):
         for conv in self.layers:
             x = x + conv(x)
             x *= SCALE_WEIGHT
         return x
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/distributed.py` & `OpenNMT-py-3.1.3/onmt/utils/distributed.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,59 +11,62 @@
 
 
 def is_master(opt, device_id):
     return opt.gpu_ranks[device_id] == 0
 
 
 def multi_init(opt, device_id):
-    dist_init_method = 'tcp://{master_ip}:{master_port}'.format(
-        master_ip=opt.master_ip,
-        master_port=opt.master_port)
+    dist_init_method = "tcp://{master_ip}:{master_port}".format(
+        master_ip=opt.master_ip, master_port=opt.master_port
+    )
     dist_world_size = opt.world_size
     torch.distributed.init_process_group(
-        backend=opt.gpu_backend, init_method=dist_init_method,
-        world_size=dist_world_size, rank=opt.gpu_ranks[device_id])
+        backend=opt.gpu_backend,
+        init_method=dist_init_method,
+        world_size=dist_world_size,
+        rank=opt.gpu_ranks[device_id],
+    )
     gpu_rank = torch.distributed.get_rank()
     if not is_master(opt, device_id):
         logger.disabled = True
 
     return gpu_rank
 
 
-def all_reduce_and_rescale_tensors(tensors, rescale_denom,
-                                   buffer_size=104857600):
+def all_reduce_and_rescale_tensors(tensors, rescale_denom, buffer_size=104857600):
     """All-reduce and rescale tensors in chunks of the specified size.
 
     Args:
         tensors: list of Tensors to all-reduce
         rescale_denom: denominator for rescaling summed Tensors
         buffer_size: all-reduce chunk size in bytes
     """
     # buffer size in bytes, determine equiv. # of elements based on data type
-    buffer_t = tensors[0].new(
-        math.ceil(buffer_size / tensors[0].element_size())).zero_()
+    buffer_t = (
+        tensors[0].new(math.ceil(buffer_size / tensors[0].element_size())).zero_()
+    )
     buffer = []
 
     def all_reduce_buffer():
         # copy tensors into buffer_t
         offset = 0
         for t in buffer:
             numel = t.numel()
-            buffer_t[offset:offset+numel].copy_(t.view(-1))
+            buffer_t[offset : offset + numel].copy_(t.view(-1))
             offset += numel
 
         # all-reduce and rescale
         torch.distributed.all_reduce(buffer_t[:offset], async_op=False)
         buffer_t.div_(rescale_denom)
 
         # copy all-reduced buffer back into tensors
         offset = 0
         for t in buffer:
             numel = t.numel()
-            t.view(-1).copy_(buffer_t[offset:offset+numel])
+            t.view(-1).copy_(buffer_t[offset : offset + numel])
             offset += numel
 
     filled = 0
     for t in tensors:
         sz = t.numel() * t.element_size()
         # print(filled, sz)
         if sz > buffer_size:
@@ -83,90 +86,93 @@
     if len(buffer) > 0:
         all_reduce_buffer()
 
 
 def all_gather_list(data, max_size=4096):
     """Gathers arbitrary data from all nodes into a list."""
     world_size = torch.distributed.get_world_size()
-    if not hasattr(all_gather_list, '_in_buffer') or \
-            max_size != all_gather_list._in_buffer.size():
+    if (
+        not hasattr(all_gather_list, "_in_buffer")
+        or max_size != all_gather_list._in_buffer.size()
+    ):
         all_gather_list._in_buffer = torch.cuda.ByteTensor(max_size)
         all_gather_list._out_buffers = [
-            torch.cuda.ByteTensor(max_size)
-            for i in range(world_size)
+            torch.cuda.ByteTensor(max_size) for i in range(world_size)
         ]
     in_buffer = all_gather_list._in_buffer
     out_buffers = all_gather_list._out_buffers
 
     enc = pickle.dumps(data)
     enc_size = len(enc)
     if enc_size + 2 > max_size:
-        raise ValueError(
-            'encoded data exceeds max_size: {}'.format(enc_size + 2))
-    assert max_size < 255*256
+        raise ValueError("encoded data exceeds max_size: {}".format(enc_size + 2))
+    assert max_size < 255 * 256
     in_buffer[0] = enc_size // 255  # this encoding works for max_size < 65k
     in_buffer[1] = enc_size % 255
-    in_buffer[2:enc_size+2] = torch.ByteTensor(list(enc))
+    in_buffer[2 : enc_size + 2] = torch.ByteTensor(list(enc))
 
     torch.distributed.all_gather(out_buffers, in_buffer.cuda())
 
     results = []
     for i in range(world_size):
         out_buffer = out_buffers[i]
         size = (255 * out_buffer[0].item()) + out_buffer[1].item()
 
-        bytes_list = bytes(out_buffer[2:size+2].tolist())
+        bytes_list = bytes(out_buffer[2 : size + 2].tolist())
         result = pickle.loads(bytes_list)
         results.append(result)
     return results
 
 
 class ErrorHandler(object):
     """A class that listens for exceptions in children processes and propagates
     the tracebacks to the parent process."""
 
     def __init__(self, error_queue):
-        """ init error handler """
+        """init error handler"""
         import signal
         import threading
+
         self.error_queue = error_queue
         self.children_pids = []
-        self.error_thread = threading.Thread(
-            target=self.error_listener, daemon=True)
+        self.error_thread = threading.Thread(target=self.error_listener, daemon=True)
         self.error_thread.start()
         signal.signal(signal.SIGUSR1, self.signal_handler)
 
     def add_child(self, pid):
-        """ error handler """
+        """error handler"""
         self.children_pids.append(pid)
 
     def error_listener(self):
-        """ error listener """
+        """error listener"""
         (rank, original_trace) = self.error_queue.get()
         self.error_queue.put((rank, original_trace))
         os.kill(os.getpid(), signal.SIGUSR1)
 
     def signal_handler(self, signalnum, stackframe):
-        """ signal handler """
+        """signal handler"""
         for pid in self.children_pids:
             os.kill(pid, signal.SIGINT)  # kill children processes
         (rank, original_trace) = self.error_queue.get()
         msg = """\n\n-- Tracebacks above this line can probably
                  be ignored --\n\n"""
         msg += original_trace
         raise Exception(msg)
 
 
 def consumer(process_fn, opt, device_id, error_queue):  # noqa: E501
     """Run `process_fn` on `device_id` with data from `batch_queue`."""
     try:
         gpu_rank = multi_init(opt, device_id)
         if gpu_rank != opt.gpu_ranks[device_id]:
-            raise AssertionError("An error occurred in \
-                  Distributed initialization")
+            raise AssertionError(
+                "An error occurred in \
+                  Distributed initialization"
+            )
         process_fn(opt, device_id=device_id)
     except KeyboardInterrupt:
         pass  # killed by parent, do nothing
     except Exception:
         # propagate exception to parent process, keeping original traceback
         import traceback
+
         error_queue.put((opt.gpu_ranks[device_id], traceback.format_exc()))
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/earlystopping.py` & `OpenNMT-py-3.1.3/onmt/utils/earlystopping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from enum import Enum
 from onmt.utils.logging import logger
 
 
 class PatienceEnum(Enum):
     IMPROVING = 0
     DECREASING = 1
@@ -27,30 +26,28 @@
         return self._caller(stats)
 
     def _caller(self, stats):
         raise NotImplementedError()
 
 
 class PPLScorer(Scorer):
-
     def __init__(self):
         super(PPLScorer, self).__init__(float("inf"), "ppl")
 
     def is_improving(self, stats):
         return stats.ppl() < self.best_score
 
     def is_decreasing(self, stats):
         return stats.ppl() > self.best_score
 
     def _caller(self, stats):
         return stats.ppl()
 
 
 class AccuracyScorer(Scorer):
-
     def __init__(self):
         super(AccuracyScorer, self).__init__(float("-inf"), "acc")
 
     def is_improving(self, stats):
         return stats.accuracy() > self.best_score
 
     def is_decreasing(self, stats):
@@ -59,41 +56,38 @@
     def _caller(self, stats):
         return stats.accuracy()
 
 
 DEFAULT_SCORERS = [PPLScorer(), AccuracyScorer()]
 
 
-SCORER_BUILDER = {
-    "ppl": PPLScorer,
-    "accuracy": AccuracyScorer
-}
+SCORER_BUILDER = {"ppl": PPLScorer, "accuracy": AccuracyScorer}
 
 
 def scorers_from_opts(opt):
     if opt.early_stopping_criteria is None:
         return DEFAULT_SCORERS
     else:
         scorers = []
         for criterion in set(opt.early_stopping_criteria):
-            assert criterion in SCORER_BUILDER.keys(), \
-                "Criterion {} not found".format(criterion)
+            assert criterion in SCORER_BUILDER.keys(), "Criterion {} not found".format(
+                criterion
+            )
             scorers.append(SCORER_BUILDER[criterion]())
         return scorers
 
 
 class EarlyStopping(object):
-
     def __init__(self, tolerance, scorers=DEFAULT_SCORERS):
         """
-            Callable class to keep track of early stopping.
+        Callable class to keep track of early stopping.
 
-            Args:
-                tolerance(int): number of validation steps without improving
-                scorer(fn): list of scorers to validate performance on dev
+        Args:
+            tolerance(int): number of validation steps without improving
+            scorer(fn): list of scorers to validate performance on dev
         """
 
         self.tolerance = tolerance
         self.stalled_tolerance = self.tolerance
         self.current_tolerance = self.tolerance
         self.early_stopping_scorers = scorers
         self.status = PatienceEnum.IMPROVING
@@ -115,46 +109,50 @@
         :param valid_stats: Statistics of dev set
         """
 
         if self.status == PatienceEnum.STOPPED:
             # Don't do anything
             return
 
-        if all([scorer.is_improving(valid_stats) for scorer
-                in self.early_stopping_scorers]):
+        if all(
+            [scorer.is_improving(valid_stats) for scorer in self.early_stopping_scorers]
+        ):
             self._update_increasing(valid_stats, step)
 
-        elif all([scorer.is_decreasing(valid_stats) for scorer
-                  in self.early_stopping_scorers]):
+        elif all(
+            [
+                scorer.is_decreasing(valid_stats)
+                for scorer in self.early_stopping_scorers
+            ]
+        ):
             self._update_decreasing()
 
         else:
             self._update_stalled()
 
     def _update_stalled(self):
         self.stalled_tolerance -= 1
 
         logger.info(
-            "Stalled patience: {}/{}".format(self.stalled_tolerance,
-                                             self.tolerance))
+            "Stalled patience: {}/{}".format(self.stalled_tolerance, self.tolerance)
+        )
 
         if self.stalled_tolerance == 0:
-            logger.info(
-                "Training finished after stalled validations. Early Stop!"
-            )
+            logger.info("Training finished after stalled validations. Early Stop!")
             self._log_best_step()
 
         self._decreasing_or_stopped_status_update(self.stalled_tolerance)
 
     def _update_increasing(self, valid_stats, step):
         self.current_step_best = step
         for scorer in self.early_stopping_scorers:
             logger.info(
                 "Model is improving {}: {:g} --> {:g}.".format(
-                    scorer.name, scorer.best_score, scorer(valid_stats))
+                    scorer.name, scorer.best_score, scorer(valid_stats)
+                )
             )
             # Update best score of each criteria
             scorer.update(valid_stats)
 
         # Reset tolerance
         self.current_tolerance = self.tolerance
         self.stalled_tolerance = self.tolerance
@@ -164,31 +162,27 @@
 
     def _update_decreasing(self):
         # Decrease tolerance
         self.current_tolerance -= 1
 
         # Log
         logger.info(
-            "Decreasing patience: {}/{}".format(self.current_tolerance,
-                                                self.tolerance)
+            "Decreasing patience: {}/{}".format(self.current_tolerance, self.tolerance)
         )
         # Log
         if self.current_tolerance == 0:
             logger.info("Training finished after not improving. Early Stop!")
             self._log_best_step()
 
         self._decreasing_or_stopped_status_update(self.current_tolerance)
 
     def _log_best_step(self):
-        logger.info("Best model found at step {}".format(
-            self.current_step_best))
+        logger.info("Best model found at step {}".format(self.current_step_best))
 
     def _decreasing_or_stopped_status_update(self, tolerance):
-        self.status = PatienceEnum.DECREASING \
-            if tolerance > 0 \
-            else PatienceEnum.STOPPED
+        self.status = PatienceEnum.DECREASING if tolerance > 0 else PatienceEnum.STOPPED
 
     def is_improving(self):
         return self.status == PatienceEnum.IMPROVING
 
     def has_stopped(self):
         return self.status == PatienceEnum.STOPPED
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/logging.py` & `OpenNMT-py-3.1.3/onmt/utils/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,19 @@
     logger = logging.getLogger("onmt")
     logger.setLevel(log_level)
 
     console_handler = logging.StreamHandler()
     console_handler.setFormatter(log_format)
     logger.handlers = [console_handler]
 
-    if log_file and log_file != '':
+    if log_file and log_file != "":
         if rotate:
             file_handler = RotatingFileHandler(
-                log_file, maxBytes=1000000, backupCount=10)
+                log_file, maxBytes=1000000, backupCount=10
+            )
         else:
             file_handler = logging.FileHandler(log_file)
         file_handler.setLevel(log_file_level)
         file_handler.setFormatter(log_format)
         logger.addHandler(file_handler)
 
     return logger
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/loss.py` & `OpenNMT-py-3.1.3/onmt/utils/loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 import torch.nn.functional as F
 import onmt
 from onmt.modules.sparse_losses import SparsemaxLoss
 from onmt.modules.sparse_activations import LogSparsemax
 from onmt.constants import ModelTask, DefaultTokens
 from onmt.modules.copy_generator import collapse_copy_scores
 from onmt.model_builder import load_test_model
+
 try:
     import ctranslate2
 except ImportError:
-    pass   # this is tested when importing for loading a LM
+    pass  # this is tested when importing for loading a LM
 
 
 class LossCompute(nn.Module):
     """
     Class for managing efficient loss computation. Handles
     accumulating multiple loss computations.
 
@@ -32,19 +33,29 @@
         vocab: target vocab (for copy attention score calculation)
              module that maps the output of the decoder to a
              distribution over the target vocabulary.
         lm_generator (:obj:`ctranslate2.Generator`): LM Generator
         lm_prior_lambda (float): weight of LM model in loss
         lm_prior_tau (float): scaler for LM loss
     """
-    def __init__(self, criterion, generator,
-                 copy_attn=False, lambda_coverage=0.0, lambda_align=0.0,
-                 tgt_shift_index=1, vocab=None, lm_generator=None,
-                 lm_prior_lambda=None, lm_prior_tau=None,
-                 lm_prior_model=None):
+
+    def __init__(
+        self,
+        criterion,
+        generator,
+        copy_attn=False,
+        lambda_coverage=0.0,
+        lambda_align=0.0,
+        tgt_shift_index=1,
+        vocab=None,
+        lm_generator=None,
+        lm_prior_lambda=None,
+        lm_prior_tau=None,
+        lm_prior_model=None,
+    ):
         super(LossCompute, self).__init__()
         self.criterion = criterion
         self.generator = generator
         self.lambda_coverage = lambda_coverage
         self.lambda_align = lambda_align
         self.tgt_shift_index = tgt_shift_index
         self.copy_attn = copy_attn
@@ -59,76 +70,84 @@
         """
         Returns a subclass which wraps around an nn.Module subclass
         (such as nn.NLLLoss) which defines the loss criterion. The LossCompute
         object passes relevant data to a Statistics object which handles
         training/validation logging.
         The Criterion and LossCompute options are triggered by opt settings.
         """
-        device = torch.device("cuda" if onmt.utils.misc.use_gpu(opt)
-                              else "cpu")
+        device = torch.device("cuda" if onmt.utils.misc.use_gpu(opt) else "cpu")
 
         padding_idx = vocab[DefaultTokens.PAD]
         unk_idx = vocab[DefaultTokens.UNK]
 
         if opt.lambda_coverage != 0:
-            assert opt.coverage_attn, "--coverage_attn needs to be set in " \
+            assert opt.coverage_attn, (
+                "--coverage_attn needs to be set in "
                 "order to use --lambda_coverage != 0"
+            )
 
         tgt_shift_idx = 1 if opt.model_task == ModelTask.SEQ2SEQ else 0
 
         if opt.copy_attn:
             criterion = onmt.modules.CopyGeneratorLoss(
-                len(vocab), opt.copy_attn_force,
-                unk_index=unk_idx, ignore_index=padding_idx
+                len(vocab),
+                opt.copy_attn_force,
+                unk_index=unk_idx,
+                ignore_index=padding_idx,
             )
         else:
-            if opt.generator_function == 'sparsemax':
-                criterion = SparsemaxLoss(ignore_index=padding_idx,
-                                          reduction='sum')
+            if opt.generator_function == "sparsemax":
+                criterion = SparsemaxLoss(ignore_index=padding_idx, reduction="sum")
             else:
                 criterion = nn.CrossEntropyLoss(
                     ignore_index=padding_idx,
-                    reduction='sum',
-                    label_smoothing=opt.label_smoothing
+                    reduction="sum",
+                    label_smoothing=opt.label_smoothing,
                 )
 
         lm_prior_lambda = opt.lm_prior_lambda
         lm_prior_tau = opt.lm_prior_tau
         if opt.lm_prior_model:
             if opt.lm_prior_model[-3:] == ".pt":
                 opt.gpu = 0
                 opt.fp32 = False
                 opt.int8 = False
-                _, lm_prior_model, lm_model_opt \
-                    = load_test_model(opt, model_path=opt.lm_prior_model)
+                _, lm_prior_model, lm_model_opt = load_test_model(
+                    opt, model_path=opt.lm_prior_model
+                )
                 lm_prior_model.to(torch.device("cuda", opt.gpu))
                 lm_prior_model.eval()
                 lm_generator = None
             else:
                 lm_prior_model = None
                 try:
                     import ctranslate2
+
                     lm_generator = ctranslate2.Generator(
-                        opt.lm_prior_model, device="cuda",
-                        compute_type="float16")
+                        opt.lm_prior_model, device="cuda", compute_type="float16"
+                    )
                 except ImportError:
                     raise ImportError("Could not import ctranslate2")
         else:
             lm_generator = None
             lm_prior_model = None
 
-        compute = cls(criterion, model.generator,
-                      copy_attn=opt.copy_attn,
-                      lambda_coverage=opt.lambda_coverage,
-                      lambda_align=opt.lambda_align,
-                      tgt_shift_index=tgt_shift_idx,
-                      vocab=vocab, lm_generator=lm_generator,
-                      lm_prior_lambda=lm_prior_lambda,
-                      lm_prior_tau=lm_prior_tau,
-                      lm_prior_model=lm_prior_model)
+        compute = cls(
+            criterion,
+            model.generator,
+            copy_attn=opt.copy_attn,
+            lambda_coverage=opt.lambda_coverage,
+            lambda_align=opt.lambda_align,
+            tgt_shift_index=tgt_shift_idx,
+            vocab=vocab,
+            lm_generator=lm_generator,
+            lm_prior_lambda=lm_prior_lambda,
+            lm_prior_tau=lm_prior_tau,
+            lm_prior_model=lm_prior_model,
+        )
         compute.to(device)
 
         return compute
 
     @property
     def padding_idx(self):
         return self.criterion.ignore_index
@@ -160,17 +179,17 @@
             target: the validate target to compare output with.
             align:
             attns: dictionary of attention distributions
               `(tgt_len, batch, src_len)`
         Returns:
             A tuple with the loss and raw scores.
         """
-        scores = self.generator(self._bottle(output),
-                                self._bottle(attns['copy']),
-                                batch['src_map'])
+        scores = self.generator(
+            self._bottle(output), self._bottle(attns["copy"]), batch["src_map"]
+        )
         loss = self.criterion(scores, align, target).sum()
 
         return loss, scores
 
     def _compute_lm_loss_ct2(self, output, target):
         """
         Compute the loss between MT output and LM output
@@ -186,28 +205,27 @@
         src[src == self.vocab[DefaultTokens.EOS]] = self.padding_idx
         src = src[:, :-1, :]
         src_len = src[:, :, 0].ne(self.padding_idx).sum(1)
         # ct2 expects src with lengths without padding
         lm_scores = self.lm_generator.forward_batch(
             ctranslate2.StorageView.from_array(src[:, :, 0].to(torch.int32)),
             ctranslate2.StorageView.from_array(src_len.to(torch.int32)),
-            return_log_probs=False)
+            return_log_probs=False,
+        )
         lm_scores = torch.as_tensor(lm_scores, device=scores.device)
         # again we use raw probs to rescale with tau and apply log_softmax
         lm_scores = self._bottle(lm_scores) / self.lm_prior_tau
         lm_scores = F.log_softmax(lm_scores.to(torch.float32), dim=-1)
         lm_scores[:, self.vocab[DefaultTokens.UNK]] = -50
         lm_scores[:, self.vocab[DefaultTokens.EOS]] -= 20
         # lm_scores are in log space so log_target=True
-        lm_loss = F.kl_div(scores, lm_scores,
-                           reduction='none',
-                           log_target=True).sum(-1)
+        lm_loss = F.kl_div(scores, lm_scores, reduction="none", log_target=True).sum(-1)
         non_padding = self._bottle(output).ne(self.padding_idx)[:, 0]
         lm_loss = lm_loss.masked_select(non_padding).sum()
-        lm_loss = lm_loss * (self.lm_prior_tau ** 2)
+        lm_loss = lm_loss * (self.lm_prior_tau**2)
         return lm_loss
 
     def _compute_lm_loss(self, output, target):
         """
         Compute the loss between MT output and LM output
         https://github.com/cbaziotis/lm-prior-for-nmt/blob/master
         /fairseq_extension/user/lm_prior/lm_prior.py#L131-L133
@@ -217,38 +235,37 @@
         scores = F.log_softmax(scores.to(torch.float32), dim=-1)
 
         src = target.detach().clone()
         src[src == self.vocab[DefaultTokens.EOS]] = self.padding_idx
         src = src[:, :-1, :]
         src_len = src[:, :, 0].ne(self.padding_idx).sum(1)
         # ct2 expects src with lengths without padding
-        lm_outs, _ = self.lm_prior_model(src, None, src_len,
-                                         with_align=False)
-        lm_scores = self.lm_prior_model.generator(
-            self._bottle(lm_outs)).detach().clone() / self.lm_prior_tau
+        lm_outs, _ = self.lm_prior_model(src, None, src_len, with_align=False)
+        lm_scores = (
+            self.lm_prior_model.generator(self._bottle(lm_outs)).detach().clone()
+            / self.lm_prior_tau
+        )
         # again we use raw probs to rescale with tau and apply log_softmax
         lm_scores = F.log_softmax(lm_scores.to(torch.float32), dim=-1)
         lm_scores[:, self.vocab[DefaultTokens.UNK]] = -50
         lm_scores[:, self.vocab[DefaultTokens.EOS]] -= 20
         # lm_scores are in log space so log_target=True
-        lm_loss = F.kl_div(scores, lm_scores,
-                           reduction='none', log_target=True).sum(-1)
+        lm_loss = F.kl_div(scores, lm_scores, reduction="none", log_target=True).sum(-1)
         non_padding = self._bottle(output).ne(self.padding_idx)[:, 0]
         lm_loss = lm_loss.masked_select(non_padding).sum()
-        lm_loss = lm_loss * (self.lm_prior_tau ** 2)
+        lm_loss = lm_loss * (self.lm_prior_tau**2)
         return lm_loss
 
     def _bottle(self, _v):
         return _v.view(-1, _v.size(2))
 
     def _unbottle(self, _v, batch_size):
         return _v.view(-1, batch_size, _v.size(1))
 
-    def forward(self, batch, output, attns,
-                trunc_start=0, trunc_size=None):
+    def forward(self, batch, output, attns, trunc_start=0, trunc_size=None):
         """Compute the forward loss, supports truncated BPTT for long
         sequences by taking a range in the decoder output sequence to
         back propagate in.
         Range is from `(trunc_start, trunc_start + trunc_size)`.
         Truncation is an approximate efficiency trick to relieve the
         memory required in the RNN buffers.
 
@@ -261,88 +278,91 @@
           trunc_start (int) : starting position of truncation window
           trunc_size (int) : length of truncation window
 
         Returns:
             A tuple with the loss and a :obj:`onmt.utils.Statistics` instance.
         """
         if trunc_size is None:
-            trunc_size = batch['tgt'].size(1) - trunc_start
+            trunc_size = batch["tgt"].size(1) - trunc_start
         # take into account here the tgt_shift_index (0 / 1 = LM/NMT)
-        trunc_range = (trunc_start + self.tgt_shift_index,
-                       trunc_start + trunc_size)
+        trunc_range = (trunc_start + self.tgt_shift_index, trunc_start + trunc_size)
 
-        target = batch['tgt'][:, trunc_range[0]:trunc_range[1],
-                              :]
-        output = output[:, trunc_start:trunc_range[1],
-                        :].contiguous()
+        target = batch["tgt"][:, trunc_range[0] : trunc_range[1], :]
+        output = output[:, trunc_start : trunc_range[1], :].contiguous()
 
         flat_tgt = target[:, :, 0].contiguous().view(-1)
 
         if self.copy_attn:
-            align = batch['alignment'][
-                :, trunc_range[0]:trunc_range[1]
-                ].contiguous().view(-1)
-            loss, scores = self._compute_copy_loss(batch, output, flat_tgt,
-                                                   align, attns)
+            align = (
+                batch["alignment"][:, trunc_range[0] : trunc_range[1]]
+                .contiguous()
+                .view(-1)
+            )
+            loss, scores = self._compute_copy_loss(
+                batch, output, flat_tgt, align, attns
+            )
             scores_data = collapse_copy_scores(
-                self._unbottle(scores.clone(), len(batch['srclen'])),
-                batch, self.vocab, None)
+                self._unbottle(scores.clone(), len(batch["srclen"])),
+                batch,
+                self.vocab,
+                None,
+            )
             scores_data = self._bottle(scores_data)
             # Correct target copy token instead of <unk>
             # tgt[i] = align[i] + len(tgt_vocab)
             # for i such that tgt[i] == 0 and align[i] != 0
             target_data = flat_tgt.clone()
             unk = self.criterion.unk_index
             correct_mask = (target_data == unk) & (align != unk)
             offset_align = align[correct_mask] + len(self.vocab)
             target_data[correct_mask] += offset_align
             scores = scores_data
             flat_tgt = target_data
 
         else:
-
             scores = self.generator(self._bottle(output))
             if isinstance(self.criterion, SparsemaxLoss):
                 scores = LogSparsemax(scores.to(torch.float32), dim=-1)
             loss = self.criterion(scores.to(torch.float32), flat_tgt)
 
             if self.lambda_align != 0.0:
-                align_head = attns['align']
+                align_head = attns["align"]
                 if align_head.dtype != loss.dtype:  # Fix FP16
                     align_head = align_head.to(loss.dtype)
-                align_idx = batch['align']
-                batch_size, pad_tgt_size, _ = batch['tgt'].size()
-                _, pad_src_size, _ = batch['src'].size()
+                align_idx = batch["align"]
+                batch_size, pad_tgt_size, _ = batch["tgt"].size()
+                _, pad_src_size, _ = batch["src"].size()
                 align_matrix_size = [batch_size, pad_tgt_size, pad_src_size]
                 ref_align = onmt.utils.make_batch_align_matrix(
                     align_idx, align_matrix_size, normalize=True
                 )
-                ref_align = ref_align[:, trunc_range[0]:trunc_range[1], :]
+                ref_align = ref_align[:, trunc_range[0] : trunc_range[1], :]
                 if ref_align.dtype != loss.dtype:
                     ref_align = ref_align.to(loss.dtype)
                 align_loss = self._compute_alignement_loss(
-                    align_head=align_head, ref_align=ref_align)
+                    align_head=align_head, ref_align=ref_align
+                )
                 loss += align_loss
 
         if self.lambda_coverage != 0.0:
             coverage_loss = self._compute_coverage_loss(
-                attns['std'], attns['coverage'], flat_tgt)
+                attns["std"], attns["coverage"], flat_tgt
+            )
             loss += coverage_loss
 
         if self.lm_generator is not None:
-            lm_loss = self._compute_lm_loss_ct2(output, batch['tgt'])
+            lm_loss = self._compute_lm_loss_ct2(output, batch["tgt"])
             loss = loss + lm_loss * self.lm_prior_lambda
 
         if self.lm_prior_model is not None:
-            lm_loss = self._compute_lm_loss(output, batch['tgt'])
+            lm_loss = self._compute_lm_loss(output, batch["tgt"])
             loss = loss + lm_loss * self.lm_prior_lambda
 
-        n_sents = len(batch['srclen']) if trunc_start == 0 else 0
-        stats = self._stats(n_sents, loss.sum().item(),
-                            scores, flat_tgt)
+        n_sents = len(batch["srclen"]) if trunc_start == 0 else 0
+        stats = self._stats(n_sents, loss.sum().item(), scores, flat_tgt)
 
         return loss, stats
 
     def _stats(self, bsz, loss, scores, target):
         """
         Args:
             loss (int): the loss computed by the loss criterion.
@@ -355,12 +375,14 @@
         pred = scores.max(1)[1]
         non_padding = target.ne(self.padding_idx)
         num_correct = pred.eq(target).masked_select(non_padding).sum().item()
         num_non_padding = non_padding.sum().item()
         n_batchs = 1 if bsz else 0
         # in the case criterion reduction is None then we need
         # to sum the loss of each sentence in the batch
-        return onmt.utils.Statistics(loss=loss,
-                                     n_batchs=n_batchs,
-                                     n_sents=bsz,
-                                     n_words=num_non_padding,
-                                     n_correct=num_correct)
+        return onmt.utils.Statistics(
+            loss=loss,
+            n_batchs=n_batchs,
+            n_sents=bsz,
+            n_words=num_non_padding,
+            n_correct=num_correct,
+        )
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/misc.py` & `OpenNMT-py-3.1.3/onmt/utils/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,58 +42,64 @@
     """Check if `path` exists, makedirs if not else warning/IOError."""
     if os.path.exists(path):
         if exist_ok:
             log(f"path {path} exists, may overwrite...")
         else:
             raise IOError(f"path {path} exists, stop.")
     else:
-        if os.path.dirname(path) != '':
+        if os.path.dirname(path) != "":
             os.makedirs(os.path.dirname(path), exist_ok=True)
 
 
 def sequence_mask(lengths, max_len=None):
     """
     Creates a boolean mask from sequence lengths.
     """
     batch_size = lengths.numel()
     max_len = max_len or lengths.max()
-    return (torch.arange(0, max_len, device=lengths.device)
-            .type_as(lengths)
-            .repeat(batch_size, 1)
-            .lt(lengths.unsqueeze(1)))
+    return (
+        torch.arange(0, max_len, device=lengths.device)
+        .type_as(lengths)
+        .repeat(batch_size, 1)
+        .lt(lengths.unsqueeze(1))
+    )
 
 
 def tile(x, count, dim=0):
     """
     Tiles x on dimension dim count times.
     """
     perm = list(range(len(x.size())))
     if dim != 0:
         perm[0], perm[dim] = perm[dim], perm[0]
         x = x.permute(perm)
     out_size = list(x.size())
     out_size[0] *= count
     batch = x.size(0)
-    x = x.contiguous().view(batch, -1) \
-         .transpose(0, 1) \
-         .repeat(count, 1) \
-         .transpose(0, 1) \
-         .contiguous() \
-         .view(*out_size)
+    x = (
+        x.contiguous()
+        .view(batch, -1)
+        .transpose(0, 1)
+        .repeat(count, 1)
+        .transpose(0, 1)
+        .contiguous()
+        .view(*out_size)
+    )
     if dim != 0:
         x = x.permute(perm).contiguous()
     return x
 
 
 def use_gpu(opt):
     """
     Creates a boolean if gpu used
     """
-    return (hasattr(opt, 'gpu_ranks') and len(opt.gpu_ranks) > 0) or \
-        (hasattr(opt, 'gpu') and opt.gpu > -1)
+    return (hasattr(opt, "gpu_ranks") and len(opt.gpu_ranks) > 0) or (
+        hasattr(opt, "gpu") and opt.gpu > -1
+    )
 
 
 def set_random_seed(seed, is_cuda):
     """Sets the random seed."""
     if seed > 0:
         torch.manual_seed(seed)
         # this one is needed for Random Shuffler of batches
@@ -114,36 +120,36 @@
     """Returns the list of function arguments name."""
     return inspect.getfullargspec(fun).args
 
 
 def report_matrix(row_label, column_label, matrix):
     header_format = "{:>10.10} " + "{:>10.7} " * len(row_label)
     row_format = "{:>10.10} " + "{:>10.7f} " * len(row_label)
-    output = header_format.format("", *row_label) + '\n'
+    output = header_format.format("", *row_label) + "\n"
     for word, row in zip(column_label, matrix):
         max_index = row.index(max(row))
-        row_format = row_format.replace(
-            "{:>10.7f} ", "{:*>10.7f} ", max_index + 1)
-        row_format = row_format.replace(
-            "{:*>10.7f} ", "{:>10.7f} ", max_index)
-        output += row_format.format(word, *row) + '\n'
+        row_format = row_format.replace("{:>10.7f} ", "{:*>10.7f} ", max_index + 1)
+        row_format = row_format.replace("{:*>10.7f} ", "{:>10.7f} ", max_index)
+        output += row_format.format(word, *row) + "\n"
         row_format = "{:>10.10} " + "{:>10.7f} " * len(row_label)
     return output
 
 
 def check_model_config(model_config, root):
     # we need to check the model path + any tokenizer path
     for model in model_config["models"]:
         model_path = os.path.join(root, model)
         if not os.path.exists(model_path):
             raise FileNotFoundError(
-                "{} from model {} does not exist".format(
-                    model_path, model_config["id"]))
+                "{} from model {} does not exist".format(model_path, model_config["id"])
+            )
     if "tokenizer" in model_config.keys():
         if "params" in model_config["tokenizer"].keys():
             for k, v in model_config["tokenizer"]["params"].items():
                 if k.endswith("path"):
                     tok_path = os.path.join(root, v)
                     if not os.path.exists(tok_path):
                         raise FileNotFoundError(
                             "{} from model {} does not exist".format(
-                                tok_path, model_config["id"]))
+                                tok_path, model_config["id"]
+                            )
+                        )
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/optimizers.py` & `OpenNMT-py-3.1.3/onmt/utils/optimizers.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import operator
 import functools
 from copy import copy
 from math import sqrt
 import types
 import importlib
 from onmt.utils.misc import fn_args
+
 try:
     import apex
 except ImportError:
     pass
 
 
 def build_torch_optimizer(model, opt):
@@ -34,134 +35,120 @@
       opt. The dictionary of options.
 
     Returns:
       A ``torch.optim.Optimizer`` instance.
     """
     params = [p for p in model.parameters() if p.requires_grad]
     betas = [opt.adam_beta1, opt.adam_beta2]
-    if opt.optim == 'sgd':
+    if opt.optim == "sgd":
         optimizer = optim.SGD(params, lr=opt.learning_rate)
-    elif opt.optim == 'adagrad':
+    elif opt.optim == "adagrad":
         optimizer = optim.Adagrad(
             params,
             lr=opt.learning_rate,
-            initial_accumulator_value=opt.adagrad_accumulator_init)
-    elif opt.optim == 'adadelta':
+            initial_accumulator_value=opt.adagrad_accumulator_init,
+        )
+    elif opt.optim == "adadelta":
         optimizer = optim.Adadelta(params, lr=opt.learning_rate)
-    elif opt.optim == 'adafactor':
+    elif opt.optim == "adafactor":
         optimizer = AdaFactor(
-            params,
-            non_constant_decay=True,
-            enable_factorization=True,
-            weight_decay=0)
-    elif opt.optim == 'adam':
-        optimizer = optim.Adam(
-            params,
-            lr=opt.learning_rate,
-            betas=betas,
-            eps=1e-8)
-    elif opt.optim == 'sparseadam':
+            params, non_constant_decay=True, enable_factorization=True, weight_decay=0
+        )
+    elif opt.optim == "adam":
+        optimizer = optim.Adam(params, lr=opt.learning_rate, betas=betas, eps=1e-8)
+    elif opt.optim == "sparseadam":
         dense = []
         sparse = []
         for name, param in model.named_parameters():
             if not param.requires_grad:
                 continue
             # TODO: Find a better way to check for sparse gradients.
-            if 'embed' in name:
+            if "embed" in name:
                 sparse.append(param)
             else:
                 dense.append(param)
         optimizer = MultipleOptimizer(
-            [optim.Adam(
-                dense,
-                lr=opt.learning_rate,
-                betas=betas,
-                eps=1e-8),
-             optim.SparseAdam(
-                 sparse,
-                 lr=opt.learning_rate,
-                 betas=betas,
-                 eps=1e-8)])
-    elif opt.optim == 'fusedadam':
-        optimizer = FusedAdam(
-            params,
-            lr=opt.learning_rate,
-            betas=betas)
+            [
+                optim.Adam(dense, lr=opt.learning_rate, betas=betas, eps=1e-8),
+                optim.SparseAdam(sparse, lr=opt.learning_rate, betas=betas, eps=1e-8),
+            ]
+        )
+    elif opt.optim == "fusedadam":
+        optimizer = FusedAdam(params, lr=opt.learning_rate, betas=betas)
         try:
             import apex
         except ImportError:
             raise ImportError("Could not import apex")
-        if opt.apex_opt_level in ['O0', 'O1', 'O2', 'O3']:
+        if opt.apex_opt_level in ["O0", "O1", "O2", "O3"]:
             # we use apex.amp
             loss_scale = "dynamic" if opt.loss_scale == 0 else opt.loss_scale
             model, optimizer = apex.amp.initialize(
                 [model, model.generator],
                 optimizer,
                 opt_level=opt.apex_opt_level,
                 loss_scale=loss_scale,
-                keep_batchnorm_fp32=None)
+                keep_batchnorm_fp32=None,
+            )
         else:
-            if opt.model_dtype == 'fp16':
+            if opt.model_dtype == "fp16":
                 # In this case use the old FusedAdam with
                 # FP16_optimizer wrapper
                 static_loss_scale = opt.loss_scale
                 dynamic_loss_scale = opt.loss_scale == 0
                 optimizer = apex.contrib.optimizers.FP16_Optimizer(
                     optimizer,
                     static_loss_scale=static_loss_scale,
-                    dynamic_loss_scale=dynamic_loss_scale)
+                    dynamic_loss_scale=dynamic_loss_scale,
+                )
     else:
-        raise ValueError('Invalid optimizer type: ' + opt.optim)
+        raise ValueError("Invalid optimizer type: " + opt.optim)
 
     return optimizer
 
 
 def make_learning_rate_decay_fn(opt):
     """Returns the learning decay function from options."""
-    if opt.decay_method == 'noam':
+    if opt.decay_method == "noam":
         return functools.partial(
-            noam_decay,
-            warmup_steps=opt.warmup_steps,
-            model_size=opt.hidden_size)
-    elif opt.decay_method == 'noamwd':
+            noam_decay, warmup_steps=opt.warmup_steps, model_size=opt.hidden_size
+        )
+    elif opt.decay_method == "noamwd":
         return functools.partial(
             noamwd_decay,
             warmup_steps=opt.warmup_steps,
             model_size=opt.hidden_size,
             rate=opt.learning_rate_decay,
             decay_steps=opt.decay_steps,
-            start_step=opt.start_decay_steps)
-    elif opt.decay_method == 'rsqrt':
-        return functools.partial(
-            rsqrt_decay, warmup_steps=opt.warmup_steps)
+            start_step=opt.start_decay_steps,
+        )
+    elif opt.decay_method == "rsqrt":
+        return functools.partial(rsqrt_decay, warmup_steps=opt.warmup_steps)
     elif opt.start_decay_steps is not None:
         return functools.partial(
             exponential_decay,
             rate=opt.learning_rate_decay,
             decay_steps=opt.decay_steps,
-            start_step=opt.start_decay_steps)
+            start_step=opt.start_decay_steps,
+        )
 
 
 def noam_decay(step, warmup_steps, model_size):
     """Learning rate schedule described in
     https://arxiv.org/pdf/1706.03762.pdf.
     """
-    return (
-        model_size ** (-0.5) *
-        min(step ** (-0.5), step * warmup_steps**(-1.5)))
+    return model_size ** (-0.5) * min(step ** (-0.5), step * warmup_steps ** (-1.5))
 
 
-def noamwd_decay(step, warmup_steps,
-                 model_size, rate, decay_steps, start_step=0):
-    """Learning rate schedule optimized for huge batches
-    """
+def noamwd_decay(step, warmup_steps, model_size, rate, decay_steps, start_step=0):
+    """Learning rate schedule optimized for huge batches"""
     return (
-        model_size ** (-0.5) *
-        min(step ** (-0.5), step * warmup_steps**(-1.5)) *
-        rate ** (max(step - start_step + decay_steps, 0) // decay_steps))
+        model_size ** (-0.5)
+        * min(step ** (-0.5), step * warmup_steps ** (-1.5))
+        * rate ** (max(step - start_step + decay_steps, 0) // decay_steps)
+    )
 
 
 def exponential_decay(step, rate, decay_steps, start_step=0):
     """A standard exponential decay, scaling the learning rate by :obj:`rate`
     every :obj:`decay_steps` steps.
     """
     return rate ** (max(step - start_step + decay_steps, 0) // decay_steps)
@@ -169,48 +156,48 @@
 
 def rsqrt_decay(step, warmup_steps):
     """Decay based on the reciprocal of the step square root."""
     return 1.0 / sqrt(max(step, warmup_steps))
 
 
 class MultipleOptimizer(object):
-    """ Implement multiple optimizers needed for sparse adam """
+    """Implement multiple optimizers needed for sparse adam"""
 
     def __init__(self, op):
-        """ ? """
+        """?"""
         self.optimizers = op
 
     @property
     def param_groups(self):
         param_groups = []
         for optimizer in self.optimizers:
             param_groups.extend(optimizer.param_groups)
         return param_groups
 
     def zero_grad(self, set_to_none=True):
-        """ ? """
+        """?"""
         for op in self.optimizers:
             op.zero_grad(set_to_none)
 
     def step(self):
-        """ ? """
+        """?"""
         for op in self.optimizers:
             op.step()
 
     @property
     def state(self):
-        """ ? """
+        """?"""
         return {k: v for op in self.optimizers for k, v in op.state.items()}
 
     def state_dict(self):
-        """ ? """
+        """?"""
         return [op.state_dict() for op in self.optimizers]
 
     def load_state_dict(self, state_dicts):
-        """ ? """
+        """?"""
         assert len(state_dicts) == len(self.optimizers)
         for i in range(len(state_dicts)):
             self.optimizers[i].load_state_dict(state_dicts[i])
 
 
 class Optimizer(object):
     """
@@ -224,20 +211,17 @@
         optimizer: A ``torch.optim.Optimizer`` instance.
         learning_rate: The initial learning rate.
         learning_rate_decay_fn: An optional callable taking the current step
             as argument and return a learning rate scaling factor.
         max_grad_norm: Clip gradients to this global norm.
     """
 
-    def __init__(self,
-                 optimizer,
-                 learning_rate,
-                 learning_rate_decay_fn=None,
-                 max_grad_norm=None):
-
+    def __init__(
+        self, optimizer, learning_rate, learning_rate_decay_fn=None, max_grad_norm=None
+    ):
         self._optimizer = optimizer
         self._learning_rate = learning_rate
         self._learning_rate_decay_fn = learning_rate_decay_fn
         self._max_grad_norm = max_grad_norm or 0
         self._training_step = 1
         self._decay_step = 1
         self._fp16 = None
@@ -255,56 +239,57 @@
 
         Returns:
           An ``Optimizer`` instance.
         """
         optim_opt = opt
         optim_state_dict = None
 
-        if (opt.train_from and checkpoint is not None and
-                'optim' in checkpoint.keys()):
-            optim = checkpoint['optim']
-            ckpt_opt = checkpoint['opt']
+        if opt.train_from and checkpoint is not None and "optim" in checkpoint.keys():
+            optim = checkpoint["optim"]
+            ckpt_opt = checkpoint["opt"]
             ckpt_state_dict = {}
             if isinstance(optim, Optimizer):  # Backward compatibility.
-                ckpt_state_dict['training_step'] = optim._step + 1
-                ckpt_state_dict['decay_step'] = optim._step + 1
-                ckpt_state_dict['optimizer'] = optim.optimizer.state_dict()
+                ckpt_state_dict["training_step"] = optim._step + 1
+                ckpt_state_dict["decay_step"] = optim._step + 1
+                ckpt_state_dict["optimizer"] = optim.optimizer.state_dict()
             else:
                 ckpt_state_dict = optim
 
-            if opt.reset_optim == 'none':
+            if opt.reset_optim == "none":
                 # Load everything from the checkpoint.
                 optim_opt = ckpt_opt
                 optim_state_dict = ckpt_state_dict
-            elif opt.reset_optim == 'all':
+            elif opt.reset_optim == "all":
                 # Build everything from scratch.
                 pass
-            elif opt.reset_optim == 'states':
+            elif opt.reset_optim == "states":
                 # Reset optimizer, keep options.
                 optim_opt = ckpt_opt
                 optim_state_dict = ckpt_state_dict
-                del optim_state_dict['optimizer']
-            elif opt.reset_optim == 'keep_states':
+                del optim_state_dict["optimizer"]
+            elif opt.reset_optim == "keep_states":
                 # Reset options, keep optimizer.
                 optim_state_dict = ckpt_state_dict
 
         optimizer = cls(
             build_torch_optimizer(model, optim_opt),
             optim_opt.learning_rate,
             learning_rate_decay_fn=make_learning_rate_decay_fn(optim_opt),
-            max_grad_norm=optim_opt.max_grad_norm)
+            max_grad_norm=optim_opt.max_grad_norm,
+        )
         if opt.model_dtype == "fp16":
             if opt.optim == "fusedadam":
-                if opt.apex_opt_level in ['O0', 'O1', 'O2', 'O3']:
+                if opt.apex_opt_level in ["O0", "O1", "O2", "O3"]:
                     optimizer._fp16 = "apex.amp"
                 else:
                     optimizer._fp16 = "legacy"
             else:
                 optimizer._fp16 = "amp"
                 from torch.cuda.amp import GradScaler
+
                 optimizer._scaler = GradScaler()
         if optim_state_dict:
             optimizer.load_state_dict(optim_state_dict)
         return optimizer
 
     @property
     def training_step(self):
@@ -321,26 +306,26 @@
         if self._learning_rate_decay_fn is None:
             return self._learning_rate
         scale = self._learning_rate_decay_fn(self._decay_step)
         return scale * self._learning_rate
 
     def state_dict(self):
         return {
-            'training_step': self._training_step,
-            'decay_step': self._decay_step,
-            'optimizer': self._optimizer.state_dict()
+            "training_step": self._training_step,
+            "decay_step": self._decay_step,
+            "optimizer": self._optimizer.state_dict(),
         }
 
     def load_state_dict(self, state_dict):
-        self._training_step = state_dict['training_step']
+        self._training_step = state_dict["training_step"]
         # State can be partially restored.
-        if 'decay_step' in state_dict:
-            self._decay_step = state_dict['decay_step']
-        if 'optimizer' in state_dict:
-            self._optimizer.load_state_dict(state_dict['optimizer'])
+        if "decay_step" in state_dict:
+            self._decay_step = state_dict["decay_step"]
+        if "optimizer" in state_dict:
+            self._optimizer.load_state_dict(state_dict["optimizer"])
 
     def zero_grad(self, set_to_none=True):
         """Zero the gradients of optimized parameters."""
         self._optimizer.zero_grad()
         # should be: self._optimizer.zero_grad(set_to_none)
         # but apex.amp is not up-to-date:
         # https://github.com/NVIDIA/apex/blob/master/apex/amp/_process_optimizer.py#L367
@@ -370,78 +355,97 @@
         learning_rate = self.learning_rate()
 
         if self.amp:
             self._scaler.unscale_(self._optimizer)
         elif self._fp16 == "legacy":
             if hasattr(self._optimizer, "update_master_grads"):
                 self._optimizer.update_master_grads()
-            if hasattr(self._optimizer, "clip_master_grads") and \
-               self._max_grad_norm > 0:
+            if (
+                hasattr(self._optimizer, "clip_master_grads")
+                and self._max_grad_norm > 0
+            ):
                 self._optimizer.clip_master_grads(self._max_grad_norm)
 
         for group in self._optimizer.param_groups:
-            group['lr'] = learning_rate
+            group["lr"] = learning_rate
             if self._max_grad_norm > 0 and self._fp16 != "legacy":
-                clip_grad_norm_(group['params'], self._max_grad_norm)
+                clip_grad_norm_(group["params"], self._max_grad_norm)
 
         if self.amp:
             # unscaled optimizer's gradients (already done therefore skip),
             # skips optimizer.step() if gradients contain infs/NaNs.
             self._scaler.step(self._optimizer)
             # Updates the scale for next iteration.
             self._scaler.update()
         else:
             self._optimizer.step()
         self._decay_step += 1
         self._training_step += 1
 
+
 # Code below is an implementation of https://arxiv.org/pdf/1804.04235.pdf
 # inspired but modified from https://github.com/DeadAt0m/adafactor-pytorch
 
 
 class AdaFactor(torch.optim.Optimizer):
-
-    def __init__(self, params, lr=None, beta1=0.9, beta2=0.999, eps1=1e-30,
-                 eps2=1e-3, cliping_threshold=1, non_constant_decay=True,
-                 enable_factorization=True, ams_grad=True, weight_decay=0):
-
+    def __init__(
+        self,
+        params,
+        lr=None,
+        beta1=0.9,
+        beta2=0.999,
+        eps1=1e-30,
+        eps2=1e-3,
+        cliping_threshold=1,
+        non_constant_decay=True,
+        enable_factorization=True,
+        ams_grad=True,
+        weight_decay=0,
+    ):
         enable_momentum = beta1 != 0
 
         if non_constant_decay:
             ams_grad = False
 
-        defaults = dict(lr=lr, beta1=beta1, beta2=beta2, eps1=eps1,
-                        eps2=eps2, cliping_threshold=cliping_threshold,
-                        weight_decay=weight_decay, ams_grad=ams_grad,
-                        enable_factorization=enable_factorization,
-                        enable_momentum=enable_momentum,
-                        non_constant_decay=non_constant_decay)
+        defaults = dict(
+            lr=lr,
+            beta1=beta1,
+            beta2=beta2,
+            eps1=eps1,
+            eps2=eps2,
+            cliping_threshold=cliping_threshold,
+            weight_decay=weight_decay,
+            ams_grad=ams_grad,
+            enable_factorization=enable_factorization,
+            enable_momentum=enable_momentum,
+            non_constant_decay=non_constant_decay,
+        )
 
         super(AdaFactor, self).__init__(params, defaults)
 
     def __setstate__(self, state):
         super(AdaFactor, self).__setstate__(state)
 
     def _experimental_reshape(self, shape):
         temp_shape = shape[2:]
         if len(temp_shape) == 1:
-            new_shape = (shape[0], shape[1]*shape[2])
+            new_shape = (shape[0], shape[1] * shape[2])
         else:
             tmp_div = len(temp_shape) // 2 + len(temp_shape) % 2
-            new_shape = (shape[0]*functools.reduce(operator.mul,
-                                                   temp_shape[tmp_div:], 1),
-                         shape[1]*functools.reduce(operator.mul,
-                                                   temp_shape[:tmp_div], 1))
+            new_shape = (
+                shape[0] * functools.reduce(operator.mul, temp_shape[tmp_div:], 1),
+                shape[1] * functools.reduce(operator.mul, temp_shape[:tmp_div], 1),
+            )
         return new_shape, copy(shape)
 
     def _check_shape(self, shape):
-        '''
+        """
         output1 - True - algorithm for matrix, False - vector;
         output2 - need reshape
-        '''
+        """
         if len(shape) > 2:
             return True, True
         elif len(shape) == 2:
             return True, False
         elif len(shape) == 2 and (shape[0] == 1 or shape[1] == 1):
             return False, False
         else:
@@ -451,123 +455,145 @@
         return sqrt(torch.mean(x.pow(2)))
 
     def step(self, closure=None):
         loss = None
         if closure is not None:
             loss = closure()
         for group in self.param_groups:
-            for p in group['params']:
+            for p in group["params"]:
                 if p.grad is None:
                     continue
                 grad = p.grad.data
 
                 if grad.is_sparse:
-                    raise RuntimeError('Adam does not support sparse \
-                                       gradients, use SparseAdam instead')
+                    raise RuntimeError(
+                        "Adam does not support sparse \
+                                       gradients, use SparseAdam instead"
+                    )
 
                 is_matrix, is_need_reshape = self._check_shape(grad.size())
                 new_shape = p.data.size()
-                if is_need_reshape and group['enable_factorization']:
-                    new_shape, old_shape = \
-                        self._experimental_reshape(p.data.size())
+                if is_need_reshape and group["enable_factorization"]:
+                    new_shape, old_shape = self._experimental_reshape(p.data.size())
                     grad = grad.view(new_shape)
 
                 state = self.state[p]
                 if len(state) == 0:
-                    state['step'] = 0
-                    if group['enable_momentum']:
-                        state['exp_avg'] = torch.zeros(new_shape,
-                                                       dtype=torch.float32,
-                                                       device=p.grad.device)
-
-                    if is_matrix and group['enable_factorization']:
-                        state['exp_avg_sq_R'] = \
-                            torch.zeros((1, new_shape[1]),
-                                        dtype=torch.float32,
-                                        device=p.grad.device)
-                        state['exp_avg_sq_C'] = \
-                            torch.zeros((new_shape[0], 1),
-                                        dtype=torch.float32,
-                                        device=p.grad.device)
+                    state["step"] = 0
+                    if group["enable_momentum"]:
+                        state["exp_avg"] = torch.zeros(
+                            new_shape, dtype=torch.float32, device=p.grad.device
+                        )
+
+                    if is_matrix and group["enable_factorization"]:
+                        state["exp_avg_sq_R"] = torch.zeros(
+                            (1, new_shape[1]), dtype=torch.float32, device=p.grad.device
+                        )
+                        state["exp_avg_sq_C"] = torch.zeros(
+                            (new_shape[0], 1), dtype=torch.float32, device=p.grad.device
+                        )
                     else:
-                        state['exp_avg_sq'] = torch.zeros(new_shape,
-                                                          dtype=torch.float32,
-                                                          device=p.grad.device)
-                    if group['ams_grad']:
-                        state['exp_avg_sq_hat'] = \
-                            torch.zeros(new_shape, dtype=torch.float32,
-                                        device=p.grad.device)
-
-                if group['enable_momentum']:
-                    exp_avg = state['exp_avg']
-
-                if is_matrix and group['enable_factorization']:
-                    exp_avg_sq_r = state['exp_avg_sq_R']
-                    exp_avg_sq_c = state['exp_avg_sq_C']
+                        state["exp_avg_sq"] = torch.zeros(
+                            new_shape, dtype=torch.float32, device=p.grad.device
+                        )
+                    if group["ams_grad"]:
+                        state["exp_avg_sq_hat"] = torch.zeros(
+                            new_shape, dtype=torch.float32, device=p.grad.device
+                        )
+
+                if group["enable_momentum"]:
+                    exp_avg = state["exp_avg"]
+
+                if is_matrix and group["enable_factorization"]:
+                    exp_avg_sq_r = state["exp_avg_sq_R"]
+                    exp_avg_sq_c = state["exp_avg_sq_C"]
                 else:
-                    exp_avg_sq = state['exp_avg_sq']
+                    exp_avg_sq = state["exp_avg_sq"]
 
-                if group['ams_grad']:
-                    exp_avg_sq_hat = state['exp_avg_sq_hat']
+                if group["ams_grad"]:
+                    exp_avg_sq_hat = state["exp_avg_sq_hat"]
 
-                state['step'] += 1
-                lr_t = group['lr']
-                lr_t *= max(group['eps2'], self._rms(p.data))
-
-                if group['enable_momentum']:
-                    if group['non_constant_decay']:
-                        beta1_t = group['beta1'] * \
-                                  (1 - group['beta1'] ** (state['step'] - 1)) \
-                                  / (1 - group['beta1'] ** state['step'])
+                state["step"] += 1
+                lr_t = group["lr"]
+                lr_t *= max(group["eps2"], self._rms(p.data))
+
+                if group["enable_momentum"]:
+                    if group["non_constant_decay"]:
+                        beta1_t = (
+                            group["beta1"]
+                            * (1 - group["beta1"] ** (state["step"] - 1))
+                            / (1 - group["beta1"] ** state["step"])
+                        )
                     else:
-                        beta1_t = group['beta1']
+                        beta1_t = group["beta1"]
                     exp_avg.mul_(beta1_t).add_(1 - beta1_t, grad)
 
-                if group['non_constant_decay']:
-                    beta2_t = group['beta2'] * \
-                              (1 - group['beta2'] ** (state['step'] - 1)) / \
-                              (1 - group['beta2'] ** state['step'])
+                if group["non_constant_decay"]:
+                    beta2_t = (
+                        group["beta2"]
+                        * (1 - group["beta2"] ** (state["step"] - 1))
+                        / (1 - group["beta2"] ** state["step"])
+                    )
                 else:
-                    beta2_t = group['beta2']
+                    beta2_t = group["beta2"]
 
-                if is_matrix and group['enable_factorization']:
-                    exp_avg_sq_r.mul_(beta2_t). \
-                        add_(1 - beta2_t, torch.sum(torch.mul(grad, grad).
-                                                    add_(group['eps1']),
-                                                    dim=0, keepdim=True))
-                    exp_avg_sq_c.mul_(beta2_t). \
-                        add_(1 - beta2_t, torch.sum(torch.mul(grad, grad).
-                                                    add_(group['eps1']),
-                                                    dim=1, keepdim=True))
-                    v = torch.mul(exp_avg_sq_c,
-                                  exp_avg_sq_r).div_(torch.sum(exp_avg_sq_r))
+                if is_matrix and group["enable_factorization"]:
+                    exp_avg_sq_r.mul_(beta2_t).add_(
+                        1 - beta2_t,
+                        torch.sum(
+                            torch.mul(grad, grad).add_(group["eps1"]),
+                            dim=0,
+                            keepdim=True,
+                        ),
+                    )
+                    exp_avg_sq_c.mul_(beta2_t).add_(
+                        1 - beta2_t,
+                        torch.sum(
+                            torch.mul(grad, grad).add_(group["eps1"]),
+                            dim=1,
+                            keepdim=True,
+                        ),
+                    )
+                    v = torch.mul(exp_avg_sq_c, exp_avg_sq_r).div_(
+                        torch.sum(exp_avg_sq_r)
+                    )
                 else:
-                    exp_avg_sq.mul_(beta2_t). \
-                        addcmul_(1 - beta2_t, grad, grad). \
-                        add_((1 - beta2_t)*group['eps1'])
+                    exp_avg_sq.mul_(beta2_t).addcmul_(1 - beta2_t, grad, grad).add_(
+                        (1 - beta2_t) * group["eps1"]
+                    )
                     v = exp_avg_sq
 
                 g = grad
-                if group['enable_momentum']:
-                    g = torch.div(exp_avg, 1 - beta1_t ** state['step'])
+                if group["enable_momentum"]:
+                    g = torch.div(exp_avg, 1 - beta1_t ** state["step"])
 
-                if group['ams_grad']:
+                if group["ams_grad"]:
                     torch.max(exp_avg_sq_hat, v, out=exp_avg_sq_hat)
                     v = exp_avg_sq_hat
-                    u = torch.div(g, (torch.div(v, 1 - beta2_t **
-                                  state['step'])).sqrt().add_(group['eps1']))
+                    u = torch.div(
+                        g,
+                        (torch.div(v, 1 - beta2_t ** state["step"]))
+                        .sqrt()
+                        .add_(group["eps1"]),
+                    )
                 else:
                     u = torch.div(g, v.sqrt())
 
-                u.div_(max(1, self._rms(u) / group['cliping_threshold']))
-                p.data.add_(-lr_t * (u.view(old_shape) if is_need_reshape and
-                            group['enable_factorization'] else u))
+                u.div_(max(1, self._rms(u) / group["cliping_threshold"]))
+                p.data.add_(
+                    -lr_t
+                    * (
+                        u.view(old_shape)
+                        if is_need_reshape and group["enable_factorization"]
+                        else u
+                    )
+                )
 
-                if group['weight_decay'] != 0:
-                    p.data.add_(-group['weight_decay'] * lr_t, p.data)
+                if group["weight_decay"] != 0:
+                    p.data.add_(-group["weight_decay"] * lr_t, p.data)
 
         return loss
 
 
 class FusedAdam(torch.optim.Optimizer):
 
     """Implements Adam algorithm. Currently GPU-only.
@@ -589,31 +615,45 @@
             (default: False) NOT SUPPORTED in FusedAdam!
         eps_inside_sqrt (boolean, optional): in the 'update parameters' step,
             adds eps to the bias-corrected second moment estimate before
             evaluating square root instead of adding it to the square root of
             second moment estimate as in the original paper. (default: False)
     """
 
-    def __init__(self, params,
-                 lr=1e-3, bias_correction=True,
-                 betas=(0.9, 0.999), eps=1e-8, eps_inside_sqrt=False,
-                 weight_decay=0., max_grad_norm=0., amsgrad=False):
+    def __init__(
+        self,
+        params,
+        lr=1e-3,
+        bias_correction=True,
+        betas=(0.9, 0.999),
+        eps=1e-8,
+        eps_inside_sqrt=False,
+        weight_decay=0.0,
+        max_grad_norm=0.0,
+        amsgrad=False,
+    ):
         global fused_adam_cuda
         fused_adam_cuda = importlib.import_module("fused_adam_cuda")
 
         if amsgrad:
-            raise RuntimeError('AMSGrad variant not supported.')
-        defaults = dict(lr=lr, bias_correction=bias_correction,
-                        betas=betas, eps=eps, weight_decay=weight_decay,
-                        max_grad_norm=max_grad_norm)
+            raise RuntimeError("AMSGrad variant not supported.")
+        defaults = dict(
+            lr=lr,
+            bias_correction=bias_correction,
+            betas=betas,
+            eps=eps,
+            weight_decay=weight_decay,
+            max_grad_norm=max_grad_norm,
+        )
         super(FusedAdam, self).__init__(params, defaults)
         self.eps_mode = 0 if eps_inside_sqrt else 1
 
-    def step(self, closure=None, grads=None, output_params=None,
-             scale=1., grad_norms=None):
+    def step(
+        self, closure=None, grads=None, output_params=None, scale=1.0, grad_norms=None
+    ):
         """Performs a single optimization step.
 
         Arguments:
             closure (callable, optional): A closure that reevaluates the model
                 and returns the loss.
             grads (list of tensors, optional): weight gradient to use for the
                 optimizer update. If gradients have type torch.half, parameters
@@ -626,93 +666,100 @@
                 by before applying to weights. (default: 1)
         """
         loss = None
         if closure is not None:
             loss = closure()
 
         if grads is None:
-            grads_group = [None]*len(self.param_groups)
+            grads_group = [None] * len(self.param_groups)
         # backward compatibility
         # assuming a list/generator of parameter means single group
         elif isinstance(grads, types.GeneratorType):
             grads_group = [grads]
         elif type(grads[0]) != list:
             grads_group = [grads]
         else:
             grads_group = grads
 
         if output_params is None:
-            output_params_group = [None]*len(self.param_groups)
+            output_params_group = [None] * len(self.param_groups)
         elif isinstance(output_params, types.GeneratorType):
             output_params_group = [output_params]
         elif type(output_params[0]) != list:
             output_params_group = [output_params]
         else:
             output_params_group = output_params
 
         if grad_norms is None:
-            grad_norms = [None]*len(self.param_groups)
+            grad_norms = [None] * len(self.param_groups)
 
-        for group, grads_this_group, output_params_this_group, \
-            grad_norm in zip(self.param_groups, grads_group,
-                             output_params_group, grad_norms):
+        for group, grads_this_group, output_params_this_group, grad_norm in zip(
+            self.param_groups, grads_group, output_params_group, grad_norms
+        ):
             if grads_this_group is None:
-                grads_this_group = [None]*len(group['params'])
+                grads_this_group = [None] * len(group["params"])
             if output_params_this_group is None:
-                output_params_this_group = [None]*len(group['params'])
+                output_params_this_group = [None] * len(group["params"])
 
             # compute combined scale factor for this group
             combined_scale = scale
-            if group['max_grad_norm'] > 0:
+            if group["max_grad_norm"] > 0:
                 # norm is in fact norm*scale
-                clip = ((grad_norm / scale) + 1e-6) / group['max_grad_norm']
+                clip = ((grad_norm / scale) + 1e-6) / group["max_grad_norm"]
                 if clip > 1:
                     combined_scale = clip * scale
 
-            bias_correction = 1 if group['bias_correction'] else 0
+            bias_correction = 1 if group["bias_correction"] else 0
 
-            for p, grad, output_param in zip(group['params'],
-                                             grads_this_group,
-                                             output_params_this_group):
+            for p, grad, output_param in zip(
+                group["params"], grads_this_group, output_params_this_group
+            ):
                 # note: p.grad should not ever be set for correct operation of
                 # mixed precision optimizer that sometimes sends None gradients
                 if p.grad is None and grad is None:
                     continue
                 if grad is None:
                     grad = p.grad.data
                 if grad.is_sparse:
-                    raise RuntimeError('FusedAdam does not support sparse \
+                    raise RuntimeError(
+                        "FusedAdam does not support sparse \
                                        gradients, please consider \
-                                       SparseAdam instead')
+                                       SparseAdam instead"
+                    )
 
                 state = self.state[p]
 
                 # State initialization
                 if len(state) == 0:
-                    state['step'] = 0
+                    state["step"] = 0
                     # Exponential moving average of gradient values
-                    state['exp_avg'] = torch.zeros_like(p.data)
+                    state["exp_avg"] = torch.zeros_like(p.data)
                     # Exponential moving average of squared gradient values
-                    state['exp_avg_sq'] = torch.zeros_like(p.data)
+                    state["exp_avg_sq"] = torch.zeros_like(p.data)
 
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-                beta1, beta2 = group['betas']
+                exp_avg, exp_avg_sq = state["exp_avg"], state["exp_avg_sq"]
+                beta1, beta2 = group["betas"]
 
-                state['step'] += 1
+                state["step"] += 1
 
-                out_p = torch.tensor([], dtype=torch.float) if \
-                    output_param is None else output_param
-                fused_adam_cuda.adam(p.data,
-                                     out_p,
-                                     exp_avg,
-                                     exp_avg_sq,
-                                     grad,
-                                     group['lr'],
-                                     beta1,
-                                     beta2,
-                                     group['eps'],
-                                     combined_scale,
-                                     state['step'],
-                                     self.eps_mode,
-                                     bias_correction,
-                                     group['weight_decay'])
+                out_p = (
+                    torch.tensor([], dtype=torch.float)
+                    if output_param is None
+                    else output_param
+                )
+                fused_adam_cuda.adam(
+                    p.data,
+                    out_p,
+                    exp_avg,
+                    exp_avg_sq,
+                    grad,
+                    group["lr"],
+                    beta1,
+                    beta2,
+                    group["eps"],
+                    combined_scale,
+                    state["step"],
+                    self.eps_mode,
+                    bias_correction,
+                    group["weight_decay"],
+                )
         return loss
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/parse.py` & `OpenNMT-py-3.1.3/onmt/utils/parse.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,69 +17,79 @@
         if not os.path.isfile(file_path):
             raise IOError(f"Please check path of your {info} file!")
 
     @classmethod
     def _validate_data(cls, opt):
         """Parse corpora specified in data field of YAML file."""
         import yaml
+
         default_transforms = opt.transforms
         if len(default_transforms) != 0:
             logger.info(f"Default transforms: {default_transforms}.")
         corpora = yaml.safe_load(opt.data)
 
         for cname, corpus in corpora.items():
             # Check Transforms
-            _transforms = corpus.get('transforms', None)
+            _transforms = corpus.get("transforms", None)
             if _transforms is None:
-                logger.info(f"Missing transforms field for {cname} data, "
-                            f"set to default: {default_transforms}.")
-                corpus['transforms'] = default_transforms
+                logger.info(
+                    f"Missing transforms field for {cname} data, "
+                    f"set to default: {default_transforms}."
+                )
+                corpus["transforms"] = default_transforms
             # Check path
-            path_src = corpus.get('path_src', None)
-            path_tgt = corpus.get('path_tgt', None)
+            path_src = corpus.get("path_src", None)
+            path_tgt = corpus.get("path_tgt", None)
             if path_src is None:
-                raise ValueError(f'Corpus {cname} src path is required.'
-                                 'tgt path is also required for non language'
-                                 ' modeling tasks.')
+                raise ValueError(
+                    f"Corpus {cname} src path is required."
+                    "tgt path is also required for non language"
+                    " modeling tasks."
+                )
             else:
                 opt.data_task = ModelTask.SEQ2SEQ
                 if path_tgt is None:
                     logger.debug(
                         "path_tgt is None, it should be set unless the task"
                         " is language modeling"
                     )
                     opt.data_task = ModelTask.LANGUAGE_MODEL
                     # tgt is src for LM task
                     corpus["path_tgt"] = path_src
                     corpora[cname] = corpus
                     path_tgt = path_src
-                cls._validate_file(path_src, info=f'{cname}/path_src')
-                cls._validate_file(path_tgt, info=f'{cname}/path_tgt')
-            path_align = corpus.get('path_align', None)
+                cls._validate_file(path_src, info=f"{cname}/path_src")
+                cls._validate_file(path_tgt, info=f"{cname}/path_tgt")
+            path_align = corpus.get("path_align", None)
             if path_align is None:
-                if hasattr(opt, 'lambda_align') and opt.lambda_align > 0.0:
-                    raise ValueError(f'Corpus {cname} alignment file path are '
-                                     'required when lambda_align > 0.0')
-                corpus['path_align'] = None
+                if hasattr(opt, "lambda_align") and opt.lambda_align > 0.0:
+                    raise ValueError(
+                        f"Corpus {cname} alignment file path are "
+                        "required when lambda_align > 0.0"
+                    )
+                corpus["path_align"] = None
             else:
-                cls._validate_file(path_align, info=f'{cname}/path_align')
+                cls._validate_file(path_align, info=f"{cname}/path_align")
             # Check weight
-            weight = corpus.get('weight', None)
+            weight = corpus.get("weight", None)
             if weight is None:
                 if cname != CorpusName.VALID:
-                    logger.warning(f"Corpus {cname}'s weight should be given."
-                                   " We default it to 1 for you.")
-                corpus['weight'] = 1
+                    logger.warning(
+                        f"Corpus {cname}'s weight should be given."
+                        " We default it to 1 for you."
+                    )
+                corpus["weight"] = 1
 
             # Check features
             if opt.n_src_feats > 0:
-                if 'inferfeats' not in corpus["transforms"]:
+                if "inferfeats" not in corpus["transforms"]:
                     raise ValueError(
                         "'inferfeats' transform is required "
-                        "when setting source features")
+                        "when setting source features"
+                    )
 
         logger.info(f"Parsed {len(corpora)} corpora from -data.")
         opt.data = corpora
 
     @classmethod
     def _validate_transforms_opts(cls, opt):
         """Check options used by transforms."""
@@ -88,62 +98,71 @@
                 transform_cls._validate_options(opt)
 
     @classmethod
     def _get_all_transform(cls, opt):
         """Should only called after `_validate_data`."""
         all_transforms = set(opt.transforms)
         for cname, corpus in opt.data.items():
-            _transforms = set(corpus['transforms'])
+            _transforms = set(corpus["transforms"])
             if len(_transforms) != 0:
                 all_transforms.update(_transforms)
-        if hasattr(opt, 'lambda_align') and opt.lambda_align > 0.0:
-            if not all_transforms.isdisjoint(
-                    {'sentencepiece', 'bpe', 'onmt_tokenize'}):
-                raise ValueError('lambda_align is not compatible with'
-                                 ' on-the-fly tokenization.')
-            if not all_transforms.isdisjoint(
-                    {'tokendrop', 'prefix', 'bart'}):
-                raise ValueError('lambda_align is not compatible yet with'
-                                 ' potentiel token deletion/addition.')
+        if hasattr(opt, "lambda_align") and opt.lambda_align > 0.0:
+            if not all_transforms.isdisjoint({"sentencepiece", "bpe", "onmt_tokenize"}):
+                raise ValueError(
+                    "lambda_align is not compatible with" " on-the-fly tokenization."
+                )
+            if not all_transforms.isdisjoint({"tokendrop", "prefix", "bart"}):
+                raise ValueError(
+                    "lambda_align is not compatible yet with"
+                    " potentiel token deletion/addition."
+                )
         opt._all_transform = all_transforms
 
     @classmethod
     def _get_all_transform_translate(cls, opt):
         opt._all_transform = opt.transforms
 
     @classmethod
     def _validate_vocab_opts(cls, opt, build_vocab_only=False):
         """Check options relate to vocab."""
 
         if build_vocab_only:
             if not opt.share_vocab:
-                assert opt.tgt_vocab, \
-                    "-tgt_vocab is required if not -share_vocab."
+                assert opt.tgt_vocab, "-tgt_vocab is required if not -share_vocab."
             return
         # validation when train:
-        cls._validate_file(opt.src_vocab, info='src vocab')
+        cls._validate_file(opt.src_vocab, info="src vocab")
         if not opt.share_vocab:
-            cls._validate_file(opt.tgt_vocab, info='tgt vocab')
+            cls._validate_file(opt.tgt_vocab, info="tgt vocab")
 
         if opt.dump_transforms:
-            assert opt.save_data, "-save_data should be set if set \
+            assert (
+                opt.save_data
+            ), "-save_data should be set if set \
                 -dump_transforms."
         # Check embeddings stuff
         if opt.both_embeddings is not None:
-            assert (opt.src_embeddings is None
-                    and opt.tgt_embeddings is None), \
-                "You don't need -src_embeddings or -tgt_embeddings \
+            assert (
+                opt.src_embeddings is None and opt.tgt_embeddings is None
+            ), "You don't need -src_embeddings or -tgt_embeddings \
                 if -both_embeddings is set."
 
-        if any([opt.both_embeddings is not None,
+        if any(
+            [
+                opt.both_embeddings is not None,
                 opt.src_embeddings is not None,
-                opt.tgt_embeddings is not None]):
-            assert opt.embeddings_type is not None, \
-                "You need to specify an -embedding_type!"
-            assert opt.save_data, "-save_data should be set if use \
+                opt.tgt_embeddings is not None,
+            ]
+        ):
+            assert (
+                opt.embeddings_type is not None
+            ), "You need to specify an -embedding_type!"
+            assert (
+                opt.save_data
+            ), "-save_data should be set if use \
                 pretrained embeddings."
 
     @classmethod
     def _validate_language_model_compatibilities_opts(cls, opt):
         if opt.model_task != ModelTask.LANGUAGE_MODEL:
             return
 
@@ -156,24 +175,26 @@
         assert (
             opt.decoder_type == "transformer"
         ), "Only transformer decoder is supported for LM task"
 
     @classmethod
     def _validate_source_features_opts(cls, opt):
         if opt.src_feats_defaults is not None:
-            assert (
-                opt.n_src_feats == len(opt.src_feats_defaults.split("￨"))
+            assert opt.n_src_feats == len(
+                opt.src_feats_defaults.split("￨")
             ), "The number source features defaults does not match \
                 -n_src_feats"
 
     @classmethod
     def validate_prepare_opts(cls, opt, build_vocab_only=False):
         """Validate all options relate to prepare (data/transform/vocab)."""
         if opt.n_sample != 0:
-            assert opt.save_data, "-save_data should be set if \
+            assert (
+                opt.save_data
+            ), "-save_data should be set if \
                 want save samples."
         cls._validate_data(opt)
         cls._get_all_transform(opt)
         cls._validate_transforms_opts(opt)
         cls._validate_vocab_opts(opt, build_vocab_only=build_vocab_only)
         cls._validate_source_features_opts(opt)
 
@@ -182,22 +203,24 @@
         cls._validate_language_model_compatibilities_opts(opt)
 
 
 class ArgumentParser(cfargparse.ArgumentParser, DataOptsCheckerMixin):
     """OpenNMT option parser powered with option check methods."""
 
     def __init__(
-            self,
-            config_file_parser_class=cfargparse.YAMLConfigFileParser,
-            formatter_class=cfargparse.ArgumentDefaultsHelpFormatter,
-            **kwargs):
+        self,
+        config_file_parser_class=cfargparse.YAMLConfigFileParser,
+        formatter_class=cfargparse.ArgumentDefaultsHelpFormatter,
+        **kwargs,
+    ):
         super(ArgumentParser, self).__init__(
             config_file_parser_class=config_file_parser_class,
             formatter_class=formatter_class,
-            **kwargs)
+            **kwargs,
+        )
 
     @classmethod
     def defaults(cls, *args):
         """Get default arguments added to a parser by all ``*args``."""
         dummy_parser = cls()
         for callback in args:
             callback(dummy_parser)
@@ -207,17 +230,17 @@
     @classmethod
     def update_model_opts(cls, model_opt):
         if model_opt.word_vec_size > 0:
             model_opt.src_word_vec_size = model_opt.word_vec_size
             model_opt.tgt_word_vec_size = model_opt.word_vec_size
 
         # Backward compatibility with "fix_word_vecs_*" opts
-        if hasattr(model_opt, 'fix_word_vecs_enc'):
+        if hasattr(model_opt, "fix_word_vecs_enc"):
             model_opt.freeze_word_vecs_enc = model_opt.fix_word_vecs_enc
-        if hasattr(model_opt, 'fix_word_vecs_dec'):
+        if hasattr(model_opt, "fix_word_vecs_dec"):
             model_opt.freeze_word_vecs_dec = model_opt.fix_word_vecs_dec
 
         if model_opt.layers > 0:
             model_opt.enc_layers = model_opt.layers
             model_opt.dec_layers = model_opt.layers
 
         if model_opt.hidden_size > 0:
@@ -232,104 +255,113 @@
         if model_opt.alignment_layer is None:
             model_opt.alignment_layer = -2
             model_opt.lambda_align = 0.0
             model_opt.full_context_alignment = False
 
     @classmethod
     def validate_model_opts(cls, model_opt):
-        assert model_opt.model_type in ["text"], \
+        assert model_opt.model_type in ["text"], (
             "Unsupported model type %s" % model_opt.model_type
+        )
 
         # encoder and decoder should be same sizes
         same_size = model_opt.enc_hid_size == model_opt.dec_hid_size
-        assert same_size, \
-            "The encoder and decoder rnns must be the same size for now"
+        assert same_size, "The encoder and decoder rnns must be the same size for now"
 
-        assert model_opt.rnn_type != "SRU" or model_opt.gpu_ranks, \
-            "Using SRU requires -gpu_ranks set."
+        assert (
+            model_opt.rnn_type != "SRU" or model_opt.gpu_ranks
+        ), "Using SRU requires -gpu_ranks set."
         if model_opt.share_embeddings:
             if model_opt.model_type != "text":
-                raise AssertionError(
-                    "--share_embeddings requires --model_type text.")
+                raise AssertionError("--share_embeddings requires --model_type text.")
         if model_opt.lambda_align > 0.0:
-            assert model_opt.decoder_type == 'transformer', \
-                "Only transformer is supported to joint learn alignment."
-            assert model_opt.alignment_layer < model_opt.dec_layers and \
-                model_opt.alignment_layer >= -model_opt.dec_layers, \
-                "N° alignment_layer should be smaller than number of layers."
-            logger.info("Joint learn alignment at layer [{}] "
-                        "with {} heads in full_context '{}'.".format(
-                            model_opt.alignment_layer,
-                            model_opt.alignment_heads,
-                            model_opt.full_context_alignment))
+            assert (
+                model_opt.decoder_type == "transformer"
+            ), "Only transformer is supported to joint learn alignment."
+            assert (
+                model_opt.alignment_layer < model_opt.dec_layers
+                and model_opt.alignment_layer >= -model_opt.dec_layers
+            ), "N° alignment_layer should be smaller than number of layers."
+            logger.info(
+                "Joint learn alignment at layer [{}] "
+                "with {} heads in full_context '{}'.".format(
+                    model_opt.alignment_layer,
+                    model_opt.alignment_heads,
+                    model_opt.full_context_alignment,
+                )
+            )
 
         if model_opt.feat_merge == "concat" and model_opt.feat_vec_size > 0:
             assert (
-                (model_opt.feat_vec_size * model_opt.n_src_feats)
-                + model_opt.src_word_vec_size == model_opt.hidden_size), \
-                "(feat_vec_size * n_src_feats) + " \
-                "src_word_vec_size should be equal to hidden_size with " \
+                model_opt.feat_vec_size * model_opt.n_src_feats
+            ) + model_opt.src_word_vec_size == model_opt.hidden_size, (
+                "(feat_vec_size * n_src_feats) + "
+                "src_word_vec_size should be equal to hidden_size with "
                 "-feat_merge concat mode."
+            )
 
-        if model_opt.position_encoding and \
-                model_opt.max_relative_positions != 0:
+        if model_opt.position_encoding and model_opt.max_relative_positions != 0:
             raise ValueError(
                 "Cannot use absolute and relative position encoding at the"
                 "same time. Use either --position_encoding=true for legacy"
                 "absolute position encoding or --max_realtive_positions with"
                 " -1 for Rotary, or > 0 for Relative Position Representations"
-                "as in https://arxiv.org/pdf/1803.02155.pdf")
+                "as in https://arxiv.org/pdf/1803.02155.pdf"
+            )
 
     @classmethod
     def ckpt_model_opts(cls, ckpt_opt):
         # Load default opt values, then overwrite with the opts in
         # the checkpoint. That way, if there are new options added,
         # the defaults are used.
         opt = cls.defaults(opts.model_opts)
         opt.__dict__.update(ckpt_opt.__dict__)
         return opt
 
     @classmethod
     def validate_train_opts(cls, opt):
-
         if torch.cuda.is_available() and not opt.gpu_ranks:
             logger.warn("You have a CUDA device, should run with -gpu_ranks")
         if opt.world_size < len(opt.gpu_ranks):
             raise AssertionError(
-                  "parameter counts of -gpu_ranks must be less or equal "
-                  "than -world_size.")
-        if opt.world_size == len(opt.gpu_ranks) and \
-                min(opt.gpu_ranks) > 0:
+                "parameter counts of -gpu_ranks must be less or equal "
+                "than -world_size."
+            )
+        if opt.world_size == len(opt.gpu_ranks) and min(opt.gpu_ranks) > 0:
             raise AssertionError(
-                  "-gpu_ranks should have master(=0) rank "
-                  "unless -world_size is greater than len(gpu_ranks).")
-
-        assert len(opt.dropout) == len(opt.dropout_steps), \
-            "Number of dropout values must match accum_steps values"
-
-        assert len(opt.attention_dropout) == len(opt.dropout_steps), \
-            "Number of attention_dropout values must match accum_steps values"
-
-        assert len(opt.accum_count) == len(opt.accum_steps), \
-            'Number of accum_count values must match number of accum_steps'
+                "-gpu_ranks should have master(=0) rank "
+                "unless -world_size is greater than len(gpu_ranks)."
+            )
+
+        assert len(opt.dropout) == len(
+            opt.dropout_steps
+        ), "Number of dropout values must match accum_steps values"
+
+        assert len(opt.attention_dropout) == len(
+            opt.dropout_steps
+        ), "Number of attention_dropout values must match accum_steps values"
+
+        assert len(opt.accum_count) == len(
+            opt.accum_steps
+        ), "Number of accum_count values must match number of accum_steps"
 
         if opt.update_vocab:
-            assert opt.train_from, \
-                "-update_vocab needs -train_from option"
-            assert opt.reset_optim in ['states', 'all'], \
-                '-update_vocab needs -reset_optim "states" or "all"'
+            assert opt.train_from, "-update_vocab needs -train_from option"
+            assert opt.reset_optim in [
+                "states",
+                "all",
+            ], '-update_vocab needs -reset_optim "states" or "all"'
 
     @classmethod
     def validate_translate_opts(cls, opt):
         if opt.gold_align:
-            assert opt.report_align, \
-                "-report_align should be enabled with -gold_align"
-            assert not opt.replace_unk, \
-                "-replace_unk option can not be used with -gold_align enabled"
-            assert opt.tgt, \
-                "-tgt should be specified with -gold_align"
+            assert opt.report_align, "-report_align should be enabled with -gold_align"
+            assert (
+                not opt.replace_unk
+            ), "-replace_unk option can not be used with -gold_align enabled"
+            assert opt.tgt, "-tgt should be specified with -gold_align"
 
     @classmethod
     def validate_translate_opts_dynamic(cls, opt):
         # It comes from training
         # TODO: needs to be added as inference opt
         opt.share_vocab = False
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/report_manager.py` & `OpenNMT-py-3.1.3/onmt/utils/report_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,37 +6,36 @@
 
 from onmt.utils.logging import logger
 
 
 def build_report_manager(opt, gpu_rank):
     if opt.tensorboard and gpu_rank <= 0:
         from torch.utils.tensorboard import SummaryWriter
-        if not hasattr(opt, 'tensorboard_log_dir_dated'):
+
+        if not hasattr(opt, "tensorboard_log_dir_dated"):
             opt.tensorboard_log_dir_dated = (
-                opt.tensorboard_log_dir +
-                datetime.now().strftime("/%b-%d_%H-%M-%S")
+                opt.tensorboard_log_dir + datetime.now().strftime("/%b-%d_%H-%M-%S")
             )
         writer = SummaryWriter(opt.tensorboard_log_dir_dated, comment="Unmt")
     else:
         writer = None
 
-    report_mgr = ReportMgr(opt.report_every, start_time=-1,
-                           tensorboard_writer=writer)
+    report_mgr = ReportMgr(opt.report_every, start_time=-1, tensorboard_writer=writer)
     return report_mgr
 
 
 class ReportMgrBase(object):
     """
     Report Manager Base class
     Inherited classes should override:
         * `_report_training`
         * `_report_step`
     """
 
-    def __init__(self, report_every, start_time=-1.):
+    def __init__(self, report_every, start_time=-1.0):
         """
         Args:
             report_every(int): Report status every this many sentences
             start_time(float): manually set report start time. Negative values
                 means that you will need to set it later or use `start()`
         """
         self.report_every = report_every
@@ -44,122 +43,115 @@
 
     def start(self):
         self.start_time = time.time()
 
     def log(self, *args, **kwargs):
         logger.info(*args, **kwargs)
 
-    def report_training(self, step, num_steps, learning_rate, patience,
-                        report_stats, multigpu=False):
+    def report_training(
+        self, step, num_steps, learning_rate, patience, report_stats, multigpu=False
+    ):
         """
         This is the user-defined batch-level traing progress
         report function.
         Args:
             step(int): current step count.
             num_steps(int): total number of batches.
             learning_rate(float): current learning rate.
             report_stats(Statistics): old Statistics instance.
         Returns:
             report_stats(Statistics): updated Statistics instance.
         """
         if self.start_time < 0:
-            raise ValueError("""ReportMgr needs to be started
-                                (set 'start_time' or use 'start()'""")
+            raise ValueError(
+                """ReportMgr needs to be started
+                                (set 'start_time' or use 'start()'"""
+            )
 
         if step % self.report_every == 0:
             if multigpu:
-                report_stats = \
-                    onmt.utils.Statistics.all_gather_stats(report_stats)
+                report_stats = onmt.utils.Statistics.all_gather_stats(report_stats)
             self._report_training(
-                step, num_steps, learning_rate, patience, report_stats)
+                step, num_steps, learning_rate, patience, report_stats
+            )
             return onmt.utils.Statistics()
         else:
             return report_stats
 
     def _report_training(self, *args, **kwargs):
-        """ To be overridden """
+        """To be overridden"""
         raise NotImplementedError()
 
-    def report_step(self, lr, patience, step, train_stats=None,
-                    valid_stats=None):
+    def report_step(self, lr, patience, step, train_stats=None, valid_stats=None):
         """
         Report stats of a step
 
         Args:
             lr(float): current learning rate
             patience(int): current patience
             step(int): current step
             train_stats(Statistics): training stats
             valid_stats(Statistics): validation stats
         """
         self._report_step(
-            lr, patience, step,
-            valid_stats=valid_stats, train_stats=train_stats)
+            lr, patience, step, valid_stats=valid_stats, train_stats=train_stats
+        )
 
     def _report_step(self, *args, **kwargs):
         raise NotImplementedError()
 
 
 class ReportMgr(ReportMgrBase):
-    def __init__(self, report_every, start_time=-1., tensorboard_writer=None):
+    def __init__(self, report_every, start_time=-1.0, tensorboard_writer=None):
         """
         A report manager that writes statistics on standard output as well as
         (optionally) TensorBoard
 
         Args:
             report_every(int): Report status every this many sentences
             tensorboard_writer(:obj:`tensorboard.SummaryWriter`):
                 The TensorBoard Summary writer to use or None
         """
         super(ReportMgr, self).__init__(report_every, start_time)
         self.tensorboard_writer = tensorboard_writer
 
-    def maybe_log_tensorboard(self, stats, prefix, learning_rate,
-                              patience, step):
+    def maybe_log_tensorboard(self, stats, prefix, learning_rate, patience, step):
         if self.tensorboard_writer is not None:
             stats.log_tensorboard(
-                prefix, self.tensorboard_writer, learning_rate, patience, step)
+                prefix, self.tensorboard_writer, learning_rate, patience, step
+            )
 
-    def _report_training(self, step, num_steps, learning_rate, patience,
-                         report_stats):
+    def _report_training(self, step, num_steps, learning_rate, patience, report_stats):
         """
         See base class method `ReportMgrBase.report_training`.
         """
-        report_stats.output(step, num_steps,
-                            learning_rate, self.start_time)
-        self.maybe_log_tensorboard(report_stats,
-                                   "progress",
-                                   learning_rate,
-                                   patience,
-                                   step)
+        report_stats.output(step, num_steps, learning_rate, self.start_time)
+        self.maybe_log_tensorboard(
+            report_stats, "progress", learning_rate, patience, step
+        )
         report_stats = onmt.utils.Statistics()
 
         return report_stats
 
-    def _report_step(self, lr, patience, step,
-                     valid_stats=None, train_stats=None):
+    def _report_step(self, lr, patience, step, valid_stats=None, train_stats=None):
         """
         See base class method `ReportMgrBase.report_step`.
         """
         if train_stats is not None:
-            self.log('Train perplexity: %g' % train_stats.ppl())
-            self.log('Train accuracy: %g' % train_stats.accuracy())
-            self.log('Sentences processed: %g' % train_stats.n_sents)
-            self.log('Average bsz: %4.0f/%4.0f/%2.0f' %
-                     (train_stats.n_src_words / train_stats.n_batchs,
-                      train_stats.n_words / train_stats.n_batchs,
-                      train_stats.n_sents / train_stats.n_batchs))
-
-            self.maybe_log_tensorboard(train_stats,
-                                       "train",
-                                       lr,
-                                       patience,
-                                       step)
+            self.log("Train perplexity: %g" % train_stats.ppl())
+            self.log("Train accuracy: %g" % train_stats.accuracy())
+            self.log("Sentences processed: %g" % train_stats.n_sents)
+            self.log(
+                "Average bsz: %4.0f/%4.0f/%2.0f"
+                % (
+                    train_stats.n_src_words / train_stats.n_batchs,
+                    train_stats.n_words / train_stats.n_batchs,
+                    train_stats.n_sents / train_stats.n_batchs,
+                )
+            )
+
+            self.maybe_log_tensorboard(train_stats, "train", lr, patience, step)
         if valid_stats is not None:
-            self.log('Validation perplexity: %g' % valid_stats.ppl())
-            self.log('Validation accuracy: %g' % valid_stats.accuracy())
+            self.log("Validation perplexity: %g" % valid_stats.ppl())
+            self.log("Validation accuracy: %g" % valid_stats.accuracy())
 
-            self.maybe_log_tensorboard(valid_stats,
-                                       "valid",
-                                       lr,
-                                       patience,
-                                       step)
+            self.maybe_log_tensorboard(valid_stats, "valid", lr, patience, step)
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/scoring_utils.py` & `OpenNMT-py-3.1.3/onmt/utils/scoring_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from onmt.constants import DefaultTokens
 from onmt.inputters.text_utils import _addcopykeys, tensorify, text_sort_key
 from onmt.inputters.inputter import IterOnDevice
 from onmt.transforms import get_transforms_cls, make_transforms, TransformPipe
 from itertools import repeat
 
 
-class ScoringPreparator():
+class ScoringPreparator:
     """Allow the calculation of metrics via the Trainer's
-     training_eval_handler method.
+    training_eval_handler method.
     """
+
     def __init__(self, vocabs, opt):
         self.vocabs = vocabs
         self.opt = opt
         if self.opt.dump_preds is not None:
             if not os.path.exists(self.opt.dump_preds):
                 os.makedirs(self.opt.dump_preds)
         self.transforms = opt.transforms
@@ -42,39 +43,46 @@
         """
         vocab = self.vocabs[side]
         batch_side = batch[side]
         nb_sentences = batch_side.shape[0]
         nb_tokens_per_sentence = batch_side.shape[1]
         nb_feats = batch_side.shape[2] - 1
 
-        indices_to_remove = [vocab.lookup_token(token)
-                             for token in [DefaultTokens.PAD,
-                                           DefaultTokens.EOS,
-                                           DefaultTokens.BOS]]
+        indices_to_remove = [
+            vocab.lookup_token(token)
+            for token in [DefaultTokens.PAD, DefaultTokens.EOS, DefaultTokens.BOS]
+        ]
         transformed_sentences = []
         for i in range(nb_sentences):
-            tokens = [vocab.lookup_index(batch_side[i, t, 0])
-                      for t in range(nb_tokens_per_sentence)
-                      if batch_side[i, t, 0] not in indices_to_remove]
+            tokens = [
+                vocab.lookup_index(batch_side[i, t, 0])
+                for t in range(nb_tokens_per_sentence)
+                if batch_side[i, t, 0] not in indices_to_remove
+            ]
             transformed_sentences.append(tokens)
 
         if nb_feats > 0:
             transformed_feats = []
             for i_feat in range(nb_feats):
                 fv = self.vocabs["src_feats"][i_feat]
-                indices_to_remove = [fv.lookup_token(token)
-                                     for token in [DefaultTokens.PAD,
-                                                   DefaultTokens.EOS,
-                                                   DefaultTokens.BOS]]
+                indices_to_remove = [
+                    fv.lookup_token(token)
+                    for token in [
+                        DefaultTokens.PAD,
+                        DefaultTokens.EOS,
+                        DefaultTokens.BOS,
+                    ]
+                ]
                 transformed_feat = []
                 for i in range(nb_sentences):
-                    tokens = [fv.lookup_index(batch_side[i, t, i_feat+1])
-                              for t in range(nb_tokens_per_sentence)
-                              if batch_side[i, t, i_feat+1]
-                              not in indices_to_remove]
+                    tokens = [
+                        fv.lookup_index(batch_side[i, t, i_feat + 1])
+                        for t in range(nb_tokens_per_sentence)
+                        if batch_side[i, t, i_feat + 1] not in indices_to_remove
+                    ]
                     transformed_feat.append(tokens)
                 transformed_feats.append(transformed_feat)
         else:
             transformed_feats = [repeat(None)]
 
         return transformed_sentences, transformed_feats
 
@@ -84,27 +92,24 @@
         Args:
             batch: batch yielded from `DynamicDatasetIter` object
         Returns:
             transformed_batch(list): A list of examples
         with the fields "src" and "tgt"
         """
 
-        transformed_srcs, transformed_src_feats = \
-            self.ids_to_tokens_batch_side(batch, 'src')
-        transformed_tgts, _ = \
-            self.ids_to_tokens_batch_side(batch, 'tgt')
+        transformed_srcs, transformed_src_feats = self.ids_to_tokens_batch_side(
+            batch, "src"
+        )
+        transformed_tgts, _ = self.ids_to_tokens_batch_side(batch, "tgt")
 
         transformed_batch = []
-        for src, tgt, *src_feats in zip(transformed_srcs,
-                                        transformed_tgts,
-                                        *transformed_src_feats):
-            ex = {
-                "src": src,
-                "tgt": tgt
-            }
+        for src, tgt, *src_feats in zip(
+            transformed_srcs, transformed_tgts, *transformed_src_feats
+        ):
+            ex = {"src": src, "tgt": tgt}
             if src_feats[0] is not None:
                 ex["src_feats"] = src_feats
             transformed_batch.append(ex)
 
         return transformed_batch
 
     def translate(self, model, transformed_batches, gpu_rank, step, mode):
@@ -121,15 +126,15 @@
         Returns:
             preds (list): Detokenized predictions
             texts_ref (list): Detokenized target sentences
         """
         model_opt = self.opt
         parser = ArgumentParser()
         translate_opts(parser)
-        base_args = (["-model", "dummy"] + ["-src", "dummy"])
+        base_args = ["-model", "dummy"] + ["-src", "dummy"]
         opt = parser.parse_args(base_args)
         opt.gpu = gpu_rank
         ArgumentParser.validate_translate_opts(opt)
         ArgumentParser.update_model_opts(model_opt)
         ArgumentParser.validate_model_opts(model_opt)
         scorer = GNMTGlobalScorer.from_opt(opt)
         out_file = codecs.open(os.devnull, "w", "utf-8")
@@ -138,66 +143,70 @@
             self.vocabs,
             opt,
             model_opt,
             global_scorer=scorer,
             out_file=out_file,
             report_align=opt.report_align,
             report_score=False,
-            logger=None)
+            logger=None,
+        )
         # translate
         preds = []
         raw_sources = []
         raw_refs = []
         for batch in transformed_batches:
             # for validation we build an infer_iter per batch
             # in order to avoid oom issues because there is no
             # batching strategy in `textbatch_to_tensor`
             numeric = []
             for i, ex in enumerate(batch):
                 if ex is not None:
-                    raw_sources.append(ex['src'])
-                    raw_refs.append(ex['tgt'])
-                    if isinstance(ex['src'], bytes):
-                        ex['src'] = ex['src'].decode("utf-8")
-                    idxs = translator.vocabs['src'](ex['src'])
-                    num_ex = {'src': {'src': " ".join(ex['src']),
-                              'src_ids': idxs},
-                              'srclen': len(ex['src']),
-                              'tgt': None,
-                              'indices': i,
-                              'align': None}
+                    raw_sources.append(ex["src"])
+                    raw_refs.append(ex["tgt"])
+                    if isinstance(ex["src"], bytes):
+                        ex["src"] = ex["src"].decode("utf-8")
+                    idxs = translator.vocabs["src"](ex["src"])
+                    num_ex = {
+                        "src": {"src": " ".join(ex["src"]), "src_ids": idxs},
+                        "srclen": len(ex["src"]),
+                        "tgt": None,
+                        "indices": i,
+                        "align": None,
+                    }
                     if "src_feats" in ex:
-                        fs_idxs = [fv(f) for fv, f in
-                                   zip(translator.vocabs["src_feats"],
-                                       ex["src_feats"])]
+                        fs_idxs = [
+                            fv(f)
+                            for fv, f in zip(
+                                translator.vocabs["src_feats"], ex["src_feats"]
+                            )
+                        ]
                         num_ex["src"]["feats"] = fs_idxs
                     num_ex = _addcopykeys(translator.vocabs["src"], num_ex)
-                    num_ex["src"]["src"] = ex['src']
+                    num_ex["src"]["src"] = ex["src"]
                     numeric.append(num_ex)
             numeric.sort(key=text_sort_key, reverse=True)
             infer_iter = [tensorify(self.vocabs, numeric)]
             infer_iter = IterOnDevice(infer_iter, opt.gpu)
-            _, preds_ = translator._translate(
-                        infer_iter, transform=self.transform)
+            _, preds_ = translator._translate(infer_iter, transform=self.transform)
             preds += preds_
 
         # apply_reverse refs
         if self.transforms:
             texts_ref = self.transform.batch_apply_reverse(raw_refs)
 
             # flatten preds
             preds = [item for preds_ in preds for item in preds_]
         else:
             texts_ref = [" ".join(raw_ref) for raw_ref in raw_refs]
             preds = [" ".join(preds_) for preds_ in preds]
 
         # save results
         if len(preds) > 0 and self.opt.scoring_debug:
-            path = os.path.join(self.opt.dump_preds,
-                                "preds.{}_step_{}.{}".format(
-                                    mode, step, "txt"))
+            path = os.path.join(
+                self.opt.dump_preds, "preds.{}_step_{}.{}".format(mode, step, "txt")
+            )
             with open(path, "a") as file:
                 for i in range(len(preds)):
                     file.write("SOURCE: {}\n".format(raw_sources[i]))
                     file.write("REF: {}\n".format(texts_ref[i]))
                     file.write("PRED: {}\n\n".format(preds[i]))
         return preds, texts_ref
```

### Comparing `OpenNMT-py-3.1.2/onmt/utils/statistics.py` & `OpenNMT-py-3.1.3/onmt/utils/statistics.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,17 @@
     Currently calculates:
 
     * accuracy
     * perplexity
     * elapsed time
     """
 
-    def __init__(self, loss=0, n_batchs=0, n_sents=0,
-                 n_words=0, n_correct=0, computed_metrics={}):
+    def __init__(
+        self, loss=0, n_batchs=0, n_sents=0, n_words=0, n_correct=0, computed_metrics={}
+    ):
         self.loss = loss
         self.n_batchs = n_batchs
         self.n_sents = n_sents
         self.n_words = n_words
         self.n_correct = n_correct
         self.n_src_words = 0
         self.computed_metrics = computed_metrics
@@ -88,27 +89,27 @@
         self.n_correct += stat.n_correct
         self.computed_metrics = stat.computed_metrics
 
         if update_n_src_words:
             self.n_src_words += stat.n_src_words
 
     def accuracy(self):
-        """ compute accuracy """
+        """compute accuracy"""
         return 100 * (self.n_correct / self.n_words)
 
     def xent(self):
-        """ compute cross entropy """
+        """compute cross entropy"""
         return self.loss / self.n_words
 
     def ppl(self):
-        """ compute perplexity """
+        """compute perplexity"""
         return math.exp(min(self.loss / self.n_words, 100))
 
     def elapsed_time(self):
-        """ compute elapsed time """
+        """compute elapsed time"""
         return time.time() - self.start_time
 
     def output(self, step, num_steps, learning_rate, start):
         """Write out statistics to stdout.
 
         Args:
            step (int): current step
@@ -116,35 +117,44 @@
            start (int): start time of step.
         """
         t = self.elapsed_time()
         step_fmt = "%2d" % step
         if num_steps > 0:
             step_fmt = "%s/%5d" % (step_fmt, num_steps)
         logger.info(
-            ("Step %s; acc: %2.1f; ppl: %5.1f; xent: %2.1f; " +
-             "lr: %7.5f; sents: %7.0f; bsz: %4.0f/%4.0f/%2.0f; " +
-             "%3.0f/%3.0f tok/s; %6.0f sec;")
-            % (step_fmt,
-               self.accuracy(),
-               self.ppl(),
-               self.xent(),
-               learning_rate,
-               self.n_sents,
-               self.n_src_words / self.n_batchs,
-               self.n_words / self.n_batchs,
-               self.n_sents / self.n_batchs,
-               self.n_src_words / (t + 1e-5),
-               self.n_words / (t + 1e-5),
-               time.time() - start) +
-            "".join([" {}: {}".format(k, round(v, 2))
-                     for k, v in self.computed_metrics.items()]))
+            (
+                "Step %s; acc: %2.1f; ppl: %5.1f; xent: %2.1f; "
+                + "lr: %7.5f; sents: %7.0f; bsz: %4.0f/%4.0f/%2.0f; "
+                + "%3.0f/%3.0f tok/s; %6.0f sec;"
+            )
+            % (
+                step_fmt,
+                self.accuracy(),
+                self.ppl(),
+                self.xent(),
+                learning_rate,
+                self.n_sents,
+                self.n_src_words / self.n_batchs,
+                self.n_words / self.n_batchs,
+                self.n_sents / self.n_batchs,
+                self.n_src_words / (t + 1e-5),
+                self.n_words / (t + 1e-5),
+                time.time() - start,
+            )
+            + "".join(
+                [
+                    " {}: {}".format(k, round(v, 2))
+                    for k, v in self.computed_metrics.items()
+                ]
+            )
+        )
         sys.stdout.flush()
 
     def log_tensorboard(self, prefix, writer, learning_rate, patience, step):
-        """ display statistics to tensorboard """
+        """display statistics to tensorboard"""
         t = self.elapsed_time()
         writer.add_scalar(prefix + "/xent", self.xent(), step)
         writer.add_scalar(prefix + "/ppl", self.ppl(), step)
         for k, v in self.computed_metrics.items():
             writer.add_scalar(prefix + "/" + k, round(v, 4), step)
         writer.add_scalar(prefix + "/accuracy", self.accuracy(), step)
         writer.add_scalar(prefix + "/tgtper", self.n_words / t, step)
```

### Comparing `OpenNMT-py-3.1.2/setup.py` & `OpenNMT-py-3.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='OpenNMT-py',
-    description='A python implementation of OpenNMT',
+    name="OpenNMT-py",
+    description="A python implementation of OpenNMT",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    version='3.1.2',
+    long_description_content_type="text/markdown",
+    version="3.1.3",
     packages=find_packages(),
     project_urls={
         "Documentation": "http://opennmt.net/OpenNMT-py/",
         "Forum": "http://forum.opennmt.net/",
         "Gitter": "https://gitter.im/OpenNMT/OpenNMT-py",
-        "Source": "https://github.com/OpenNMT/OpenNMT-py/"
+        "Source": "https://github.com/OpenNMT/OpenNMT-py/",
     },
     python_requires=">=3.8",
     install_requires=[
         "torch>=1.13,<2",
         "configargparse",
         "ctranslate2>=3.2,<4",
         "tensorboard>=2.3",
         "flask",
         "waitress",
         "pyonmttok>=1.35,<2",
         "pyyaml",
         "sacrebleu",
         "rapidfuzz",
         "pyahocorasick",
-        "gcld3"
+        "fasttext-wheel",
     ],
     entry_points={
         "console_scripts": [
             "onmt_server=onmt.bin.server:main",
             "onmt_train=onmt.bin.train:main",
             "onmt_translate=onmt.bin.translate:main",
             "onmt_translate_dynamic=onmt.bin.translate_dynamic:main",
             "onmt_release_model=onmt.bin.release_model:main",
             "onmt_average_models=onmt.bin.average_models:main",
-            "onmt_build_vocab=onmt.bin.build_vocab:main"
+            "onmt_build_vocab=onmt.bin.build_vocab:main",
         ],
-    }
+    },
 )
```

