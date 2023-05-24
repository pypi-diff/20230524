# Comparing `tmp/medkit_lib-0.5.0.tar.gz` & `tmp/medkit_lib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medkit_lib-0.5.0.tar", max compression
+gzip compressed data, was "medkit_lib-0.6.0.tar", max compression
```

## Comparing `medkit_lib-0.5.0.tar` & `medkit_lib-0.6.0.tar`

### file list

```diff
@@ -1,121 +1,124 @@
--rw-r--r--   0        0        0     1077 2023-03-23 15:19:08.254089 medkit_lib-0.5.0/LICENSE
--rw-r--r--   0        0        0     1098 2023-03-23 15:19:08.254089 medkit_lib-0.5.0/README.md
--rw-r--r--   0        0        0      173 2023-04-04 06:31:49.436370 medkit_lib-0.5.0/medkit/__init__.py
--rw-r--r--   0        0        0       61 2023-03-23 15:19:08.258090 medkit_lib-0.5.0/medkit/audio/__init__.py
--rw-r--r--   0        0        0      248 2023-04-04 06:31:49.436370 medkit_lib-0.5.0/medkit/audio/preprocessing/__init__.py
--rw-r--r--   0        0        0     2236 2023-03-23 15:19:08.258090 medkit_lib-0.5.0/medkit/audio/preprocessing/downmixer.py
--rw-r--r--   0        0        0     2460 2023-03-23 15:19:08.258090 medkit_lib-0.5.0/medkit/audio/preprocessing/power_normalizer.py
--rw-r--r--   0        0        0     2482 2023-04-21 12:33:02.946744 medkit_lib-0.5.0/medkit/audio/preprocessing/resampler.py
--rw-r--r--   0        0        0      250 2023-04-04 06:31:49.440370 medkit_lib-0.5.0/medkit/audio/segmentation/__init__.py
--rw-r--r--   0        0        0     6530 2023-04-21 12:33:02.946744 medkit_lib-0.5.0/medkit/audio/segmentation/pa_speaker_detector.py
--rw-r--r--   0        0        0     7416 2023-04-21 12:33:02.946744 medkit_lib-0.5.0/medkit/audio/segmentation/webrtc_voice_detector.py
--rw-r--r--   0        0        0      554 2023-04-04 06:31:49.460371 medkit_lib-0.5.0/medkit/audio/transcription/__init__.py
--rw-r--r--   0        0        0     7168 2023-03-23 15:19:08.258090 medkit_lib-0.5.0/medkit/audio/transcription/doc_transcriber.py
--rw-r--r--   0        0        0     3821 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/audio/transcription/hf_transcriber_function.py
--rw-r--r--   0        0        0     4562 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/audio/transcription/sb_transcriber_function.py
--rw-r--r--   0        0        0     4776 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/audio/transcription/transcribed_document.py
--rw-r--r--   0        0        0     1489 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/__init__.py
--rw-r--r--   0        0        0     7827 2023-04-20 16:18:05.215523 medkit_lib-0.5.0/medkit/core/_prov_graph.py
--rw-r--r--   0        0        0     1200 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/annotation.py
--rw-r--r--   0        0        0     4665 2023-03-28 15:25:00.537196 medkit_lib-0.5.0/medkit/core/annotation_container.py
--rw-r--r--   0        0        0     2969 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/core/attribute.py
--rw-r--r--   0        0        0     3052 2023-03-28 15:25:00.537196 medkit_lib-0.5.0/medkit/core/attribute_container.py
--rw-r--r--   0        0        0      514 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/__init__.py
--rw-r--r--   0        0        0     3718 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/annotation.py
--rw-r--r--   0        0        0     1534 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/annotation_container.py
--rw-r--r--   0        0        0    10898 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/audio_buffer.py
--rw-r--r--   0        0        0     4016 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/document.py
--rw-r--r--   0        0        0      963 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/operation.py
--rw-r--r--   0        0        0      973 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/span.py
--rw-r--r--   0        0        0     1750 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/collection.py
--rw-r--r--   0        0        0      575 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/conversion.py
--rw-r--r--   0        0        0      475 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/data_item.py
--rw-r--r--   0        0        0     4719 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/dict_conv.py
--rw-r--r--   0        0        0     3951 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/doc_pipeline.py
--rw-r--r--   0        0        0      825 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/document.py
--rw-r--r--   0        0        0       96 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/id.py
--rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/operation.py
--rw-r--r--   0        0        0     1042 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/operation_desc.py
--rw-r--r--   0        0        0    13044 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/pipeline.py
--rw-r--r--   0        0        0     1470 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/prov_store.py
--rw-r--r--   0        0        0    10886 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/prov_tracer.py
--rw-r--r--   0        0        0     2396 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/store.py
--rw-r--r--   0        0        0      883 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/__init__.py
--rw-r--r--   0        0        0     8728 2023-04-04 06:31:49.484372 medkit_lib-0.5.0/medkit/core/text/annotation.py
--rw-r--r--   0        0        0     5316 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/annotation_container.py
--rw-r--r--   0        0        0     4854 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/document.py
--rw-r--r--   0        0        0     1334 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/entity_attribute_container.py
--rw-r--r--   0        0        0     3244 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/core/text/entity_norm_attribute.py
--rw-r--r--   0        0        0     6471 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/operation.py
--rw-r--r--   0        0        0     3147 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/span.py
--rw-r--r--   0        0        0    18208 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/span_utils.py
--rw-r--r--   0        0        0    11691 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/utils.py
--rw-r--r--   0        0        0     1462 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/utils.py
--rw-r--r--   0        0        0      401 2023-04-04 06:31:49.484372 medkit_lib-0.5.0/medkit/io/__init__.py
--rw-r--r--   0        0        0    16195 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/_brat_utils.py
--rw-r--r--   0        0        0    21166 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/io/brat.py
--rw-r--r--   0        0        0      649 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/medkit_json/__init__.py
--rw-r--r--   0        0        0     1235 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/medkit_json/_common.py
--rw-r--r--   0        0        0     5506 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/medkit_json/audio.py
--rw-r--r--   0        0        0     5496 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/medkit_json/text.py
--rw-r--r--   0        0        0    12123 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/rttm.py
--rw-r--r--   0        0        0     7750 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/io/spacy.py
--rw-r--r--   0        0        0      152 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/text/__init__.py
--rw-r--r--   0        0        0      590 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/text/context/__init__.py
--rw-r--r--   0        0        0     9128 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/context/family_detector.py
--rw-r--r--   0        0        0      790 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/text/context/family_detector_default_rules.yml
--rw-r--r--   0        0        0    14243 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/context/hypothesis_detector.py
--rw-r--r--   0        0        0      905 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/context/hypothesis_detector_example_rules.yml
--rw-r--r--   0        0        0   307270 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/context/hypothesis_detector_example_verbs.yml
--rw-r--r--   0        0        0     9134 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/context/negation_detector.py
--rw-r--r--   0        0        0     4101 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/context/negation_detector_default_rules.yml
--rw-r--r--   0        0        0     1320 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/ner/__init__.py
--rw-r--r--   0        0        0     3795 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/ner/adicap_norm_attribute.py
--rw-r--r--   0        0        0    11470 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/ner/date_attribute.py
--rw-r--r--   0        0        0     5527 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/ner/duckling_matcher.py
--rw-r--r--   0        0        0     6534 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/ner/hf_entity_matcher.py
--rw-r--r--   0        0        0     8109 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/ner/hf_entity_matcher_trainable.py
--rw-r--r--   0        0        0     6396 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/ner/hf_tokenization_utils.py
--rw-r--r--   0        0        0     5215 2023-04-04 06:31:49.488372 medkit_lib-0.5.0/medkit/text/ner/iamsystem_matcher.py
--rw-r--r--   0        0        0    12917 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/ner/quick_umls_matcher.py
--rw-r--r--   0        0        0    12788 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/ner/regexp_matcher.py
--rw-r--r--   0        0        0    22942 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/ner/regexp_matcher_default_rules.yml
--rw-r--r--   0        0        0     5154 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/ner/tnm_attribute.py
--rw-r--r--   0        0        0    17079 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/ner/umls_coder_normalizer.py
--rw-r--r--   0        0        0     2791 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/ner/umls_norm_attribute.py
--rw-r--r--   0        0        0     5468 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/ner/umls_semgroups_v04.txt
--rw-r--r--   0        0        0     4365 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/ner/umls_utils.py
--rw-r--r--   0        0        0       89 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/postprocessing/__init__.py
--rw-r--r--   0        0        0     3302 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/postprocessing/attribute_duplicator.py
--rw-r--r--   0        0        0     2953 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/preprocessing/__init__.py
--rw-r--r--   0        0        0     5393 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/preprocessing/eds_cleaner.py
--rw-r--r--   0        0        0     3157 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/preprocessing/normalizer.py
--rw-r--r--   0        0        0      202 2023-04-04 06:31:49.492373 medkit_lib-0.5.0/medkit/text/relations/__init__.py
--rw-r--r--   0        0        0     9639 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/relations/syntactic_relation_extractor.py
--rw-r--r--   0        0        0      404 2023-04-04 06:31:49.496373 medkit_lib-0.5.0/medkit/text/segmentation/__init__.py
--rw-r--r--   0        0        0    13452 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/segmentation/default_section_definition.yml
--rw-r--r--   0        0        0      389 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/segmentation/default_syntagma_definition.yml
--rw-r--r--   0        0        0     3731 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/segmentation/rush_sentence_tokenizer.py
--rw-r--r--   0        0        0    23436 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv
--rw-r--r--   0        0        0     6800 2023-04-20 16:18:05.223523 medkit_lib-0.5.0/medkit/text/segmentation/section_tokenizer.py
--rw-r--r--   0        0        0     4765 2023-04-05 07:40:19.924515 medkit_lib-0.5.0/medkit/text/segmentation/sentence_tokenizer.py
--rw-r--r--   0        0        0     4876 2023-04-20 16:18:05.223523 medkit_lib-0.5.0/medkit/text/segmentation/syntagma_tokenizer.py
--rw-r--r--   0        0        0      669 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/spacy/__init__.py
--rw-r--r--   0        0        0     4203 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/spacy/displacy_utils.py
--rw-r--r--   0        0        0     5765 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/spacy/doc_pipeline.py
--rw-r--r--   0        0        0    15636 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/spacy/edsnlp.py
--rw-r--r--   0        0        0     5136 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/spacy/pipeline.py
--rw-r--r--   0        0        0    18167 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/spacy/spacy_utils.py
--rw-r--r--   0        0        0      180 2023-04-04 06:31:49.500373 medkit_lib-0.5.0/medkit/text/translation/__init__.py
--rw-r--r--   0        0        0    15478 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/translation/hf_translator.py
--rw-r--r--   0        0        0      204 2023-04-04 06:31:49.552376 medkit_lib-0.5.0/medkit/tools/__init__.py
--rw-r--r--   0        0        0     1198 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/tools/hf_utils.py
--rw-r--r--   0        0        0     5443 2023-03-23 15:19:08.278091 medkit_lib-0.5.0/medkit/tools/save_prov_to_dot.py
--rw-r--r--   0        0        0      765 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/training/__init__.py
--rw-r--r--   0        0        0     3822 2023-03-23 15:19:08.278091 medkit_lib-0.5.0/medkit/training/callbacks.py
--rw-r--r--   0        0        0     1987 2023-04-20 16:18:05.231523 medkit_lib-0.5.0/medkit/training/trainable_component.py
--rw-r--r--   0        0        0    11628 2023-04-20 16:18:05.231523 medkit_lib-0.5.0/medkit/training/trainer.py
--rw-r--r--   0        0        0      755 2023-03-23 15:19:08.278091 medkit_lib-0.5.0/medkit/training/trainer_config.py
--rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.278091 medkit_lib-0.5.0/medkit/training/utils.py
--rw-r--r--   0        0        0     3764 2023-05-02 15:41:31.551957 medkit_lib-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4879 1970-01-01 00:00:00.000000 medkit_lib-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-23 15:19:08.254089 medkit_lib-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1098 2023-03-23 15:19:08.254089 medkit_lib-0.6.0/README.md
+-rw-r--r--   0        0        0      173 2023-04-04 06:31:49.436370 medkit_lib-0.6.0/medkit/__init__.py
+-rw-r--r--   0        0        0       61 2023-03-23 15:19:08.258090 medkit_lib-0.6.0/medkit/audio/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-04 06:31:49.436370 medkit_lib-0.6.0/medkit/audio/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2236 2023-03-23 15:19:08.258090 medkit_lib-0.6.0/medkit/audio/preprocessing/downmixer.py
+-rw-r--r--   0        0        0     2460 2023-03-23 15:19:08.258090 medkit_lib-0.6.0/medkit/audio/preprocessing/power_normalizer.py
+-rw-r--r--   0        0        0     2482 2023-04-21 12:33:02.946744 medkit_lib-0.6.0/medkit/audio/preprocessing/resampler.py
+-rw-r--r--   0        0        0      250 2023-04-04 06:31:49.440370 medkit_lib-0.6.0/medkit/audio/segmentation/__init__.py
+-rw-r--r--   0        0        0     6530 2023-04-21 12:33:02.946744 medkit_lib-0.6.0/medkit/audio/segmentation/pa_speaker_detector.py
+-rw-r--r--   0        0        0     7416 2023-04-21 12:33:02.946744 medkit_lib-0.6.0/medkit/audio/segmentation/webrtc_voice_detector.py
+-rw-r--r--   0        0        0      554 2023-04-04 06:31:49.460371 medkit_lib-0.6.0/medkit/audio/transcription/__init__.py
+-rw-r--r--   0        0        0     7168 2023-03-23 15:19:08.258090 medkit_lib-0.6.0/medkit/audio/transcription/doc_transcriber.py
+-rw-r--r--   0        0        0     3821 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/audio/transcription/hf_transcriber_function.py
+-rw-r--r--   0        0        0     4562 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/audio/transcription/sb_transcriber_function.py
+-rw-r--r--   0        0        0     4776 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/audio/transcription/transcribed_document.py
+-rw-r--r--   0        0        0     1489 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/__init__.py
+-rw-r--r--   0        0        0     7827 2023-04-20 16:18:05.215523 medkit_lib-0.6.0/medkit/core/_prov_graph.py
+-rw-r--r--   0        0        0     1200 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/annotation.py
+-rw-r--r--   0        0        0     4665 2023-03-28 15:25:00.537196 medkit_lib-0.6.0/medkit/core/annotation_container.py
+-rw-r--r--   0        0        0     2969 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/core/attribute.py
+-rw-r--r--   0        0        0     3052 2023-03-28 15:25:00.537196 medkit_lib-0.6.0/medkit/core/attribute_container.py
+-rw-r--r--   0        0        0      514 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/__init__.py
+-rw-r--r--   0        0        0     3718 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/annotation.py
+-rw-r--r--   0        0        0     1534 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/annotation_container.py
+-rw-r--r--   0        0        0    10898 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/audio_buffer.py
+-rw-r--r--   0        0        0     4016 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/document.py
+-rw-r--r--   0        0        0      963 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/operation.py
+-rw-r--r--   0        0        0      973 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/audio/span.py
+-rw-r--r--   0        0        0     1750 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/collection.py
+-rw-r--r--   0        0        0      575 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/conversion.py
+-rw-r--r--   0        0        0      475 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/data_item.py
+-rw-r--r--   0        0        0     4719 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/dict_conv.py
+-rw-r--r--   0        0        0     3951 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/doc_pipeline.py
+-rw-r--r--   0        0        0      825 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/document.py
+-rw-r--r--   0        0        0       96 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/id.py
+-rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/operation.py
+-rw-r--r--   0        0        0     1042 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/operation_desc.py
+-rw-r--r--   0        0        0    13044 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/pipeline.py
+-rw-r--r--   0        0        0     1470 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/prov_store.py
+-rw-r--r--   0        0        0    10886 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/prov_tracer.py
+-rw-r--r--   0        0        0     2396 2023-03-23 15:19:08.262090 medkit_lib-0.6.0/medkit/core/store.py
+-rw-r--r--   0        0        0      883 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/__init__.py
+-rw-r--r--   0        0        0     8728 2023-04-04 06:31:49.484372 medkit_lib-0.6.0/medkit/core/text/annotation.py
+-rw-r--r--   0        0        0     5316 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/annotation_container.py
+-rw-r--r--   0        0        0     4854 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/document.py
+-rw-r--r--   0        0        0     1334 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/entity_attribute_container.py
+-rw-r--r--   0        0        0     3244 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/core/text/entity_norm_attribute.py
+-rw-r--r--   0        0        0     6471 2023-05-22 15:41:00.683311 medkit_lib-0.6.0/medkit/core/text/operation.py
+-rw-r--r--   0        0        0     3147 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/span.py
+-rw-r--r--   0        0        0    18208 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/span_utils.py
+-rw-r--r--   0        0        0    11691 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/text/utils.py
+-rw-r--r--   0        0        0     1462 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/core/utils.py
+-rw-r--r--   0        0        0      401 2023-04-04 06:31:49.484372 medkit_lib-0.6.0/medkit/io/__init__.py
+-rw-r--r--   0        0        0    16195 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/_brat_utils.py
+-rw-r--r--   0        0        0    21166 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/io/brat.py
+-rw-r--r--   0        0        0      649 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/medkit_json/__init__.py
+-rw-r--r--   0        0        0     1235 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/medkit_json/_common.py
+-rw-r--r--   0        0        0     5506 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/medkit_json/audio.py
+-rw-r--r--   0        0        0     5496 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/medkit_json/text.py
+-rw-r--r--   0        0        0    12123 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/io/rttm.py
+-rw-r--r--   0        0        0     7750 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/io/spacy.py
+-rw-r--r--   0        0        0      152 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/text/__init__.py
+-rw-r--r--   0        0        0      590 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/text/context/__init__.py
+-rw-r--r--   0        0        0     9128 2023-04-20 16:18:05.219523 medkit_lib-0.6.0/medkit/text/context/family_detector.py
+-rw-r--r--   0        0        0      790 2023-03-23 15:19:08.266090 medkit_lib-0.6.0/medkit/text/context/family_detector_default_rules.yml
+-rw-r--r--   0        0        0    14243 2023-04-20 16:18:05.219523 medkit_lib-0.6.0/medkit/text/context/hypothesis_detector.py
+-rw-r--r--   0        0        0      905 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/context/hypothesis_detector_example_rules.yml
+-rw-r--r--   0        0        0   307270 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/context/hypothesis_detector_example_verbs.yml
+-rw-r--r--   0        0        0     9134 2023-04-20 16:18:05.219523 medkit_lib-0.6.0/medkit/text/context/negation_detector.py
+-rw-r--r--   0        0        0     4101 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/context/negation_detector_default_rules.yml
+-rw-r--r--   0        0        0      304 2023-05-23 14:37:42.934717 medkit_lib-0.6.0/medkit/text/metrics/__init__.py
+-rw-r--r--   0        0        0     9422 2023-05-23 14:37:42.934717 medkit_lib-0.6.0/medkit/text/metrics/ner.py
+-rw-r--r--   0        0        0     1320 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/ner/__init__.py
+-rw-r--r--   0        0        0     3795 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/ner/adicap_norm_attribute.py
+-rw-r--r--   0        0        0    11470 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/ner/date_attribute.py
+-rw-r--r--   0        0        0     5527 2023-04-20 16:18:05.219523 medkit_lib-0.6.0/medkit/text/ner/duckling_matcher.py
+-rw-r--r--   0        0        0     6534 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/ner/hf_entity_matcher.py
+-rw-r--r--   0        0        0     8175 2023-05-23 14:37:42.934717 medkit_lib-0.6.0/medkit/text/ner/hf_entity_matcher_trainable.py
+-rw-r--r--   0        0        0     7082 2023-05-23 14:37:42.934717 medkit_lib-0.6.0/medkit/text/ner/hf_tokenization_utils.py
+-rw-r--r--   0        0        0     5993 2023-05-23 16:01:44.808582 medkit_lib-0.6.0/medkit/text/ner/iamsystem_matcher.py
+-rw-r--r--   0        0        0    13006 2023-05-05 09:01:47.817716 medkit_lib-0.6.0/medkit/text/ner/quick_umls_matcher.py
+-rw-r--r--   0        0        0    12788 2023-04-20 16:18:05.219523 medkit_lib-0.6.0/medkit/text/ner/regexp_matcher.py
+-rw-r--r--   0        0        0    22942 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/ner/regexp_matcher_default_rules.yml
+-rw-r--r--   0        0        0     5154 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/ner/tnm_attribute.py
+-rw-r--r--   0        0        0    17079 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/ner/umls_coder_normalizer.py
+-rw-r--r--   0        0        0     2791 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/ner/umls_norm_attribute.py
+-rw-r--r--   0        0        0     5468 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/ner/umls_semgroups_v04.txt
+-rw-r--r--   0        0        0     4365 2023-03-23 15:19:08.270090 medkit_lib-0.6.0/medkit/text/ner/umls_utils.py
+-rw-r--r--   0        0        0       89 2023-05-23 14:37:42.934717 medkit_lib-0.6.0/medkit/text/postprocessing/__init__.py
+-rw-r--r--   0        0        0     3302 2023-05-23 14:37:42.938717 medkit_lib-0.6.0/medkit/text/postprocessing/attribute_duplicator.py
+-rw-r--r--   0        0        0     2953 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/preprocessing/__init__.py
+-rw-r--r--   0        0        0     5393 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/preprocessing/eds_cleaner.py
+-rw-r--r--   0        0        0     3157 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/preprocessing/normalizer.py
+-rw-r--r--   0        0        0      202 2023-04-04 06:31:49.492373 medkit_lib-0.6.0/medkit/text/relations/__init__.py
+-rw-r--r--   0        0        0     9639 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/relations/syntactic_relation_extractor.py
+-rw-r--r--   0        0        0      475 2023-05-05 09:23:06.369871 medkit_lib-0.6.0/medkit/text/segmentation/__init__.py
+-rw-r--r--   0        0        0    13452 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/segmentation/default_section_definition.yml
+-rw-r--r--   0        0        0      629 2023-05-05 09:23:06.369871 medkit_lib-0.6.0/medkit/text/segmentation/default_syntagma_definition.yml
+-rw-r--r--   0        0        0     3731 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/segmentation/rush_sentence_tokenizer.py
+-rw-r--r--   0        0        0    23436 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv
+-rw-r--r--   0        0        0     8836 2023-05-15 07:18:23.883719 medkit_lib-0.6.0/medkit/text/segmentation/section_tokenizer.py
+-rw-r--r--   0        0        0     4765 2023-04-05 07:40:19.924515 medkit_lib-0.6.0/medkit/text/segmentation/sentence_tokenizer.py
+-rw-r--r--   0        0        0     5798 2023-05-15 07:18:23.883719 medkit_lib-0.6.0/medkit/text/segmentation/syntagma_tokenizer.py
+-rw-r--r--   0        0        0     1821 2023-05-05 09:23:06.377871 medkit_lib-0.6.0/medkit/text/segmentation/tokenizer_utils.py
+-rw-r--r--   0        0        0      669 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/spacy/__init__.py
+-rw-r--r--   0        0        0     4203 2023-03-23 15:19:08.274090 medkit_lib-0.6.0/medkit/text/spacy/displacy_utils.py
+-rw-r--r--   0        0        0     5765 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/spacy/doc_pipeline.py
+-rw-r--r--   0        0        0    15636 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/spacy/edsnlp.py
+-rw-r--r--   0        0        0     5136 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/spacy/pipeline.py
+-rw-r--r--   0        0        0    18167 2023-04-21 08:20:44.049464 medkit_lib-0.6.0/medkit/text/spacy/spacy_utils.py
+-rw-r--r--   0        0        0      180 2023-04-04 06:31:49.500373 medkit_lib-0.6.0/medkit/text/translation/__init__.py
+-rw-r--r--   0        0        0    15478 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/text/translation/hf_translator.py
+-rw-r--r--   0        0        0      204 2023-04-04 06:31:49.552376 medkit_lib-0.6.0/medkit/tools/__init__.py
+-rw-r--r--   0        0        0     1198 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/tools/hf_utils.py
+-rw-r--r--   0        0        0     5443 2023-03-23 15:19:08.278091 medkit_lib-0.6.0/medkit/tools/save_prov_to_dot.py
+-rw-r--r--   0        0        0      765 2023-04-21 12:33:02.950744 medkit_lib-0.6.0/medkit/training/__init__.py
+-rw-r--r--   0        0        0     3822 2023-03-23 15:19:08.278091 medkit_lib-0.6.0/medkit/training/callbacks.py
+-rw-r--r--   0        0        0     1987 2023-04-20 16:18:05.231523 medkit_lib-0.6.0/medkit/training/trainable_component.py
+-rw-r--r--   0        0        0    11628 2023-05-23 14:37:42.938717 medkit_lib-0.6.0/medkit/training/trainer.py
+-rw-r--r--   0        0        0      755 2023-03-23 15:19:08.278091 medkit_lib-0.6.0/medkit/training/trainer_config.py
+-rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.278091 medkit_lib-0.6.0/medkit/training/utils.py
+-rw-r--r--   0        0        0     3875 2023-05-24 10:16:38.055392 medkit_lib-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5047 1970-01-01 00:00:00.000000 medkit_lib-0.6.0/PKG-INFO
```

### Comparing `medkit_lib-0.5.0/LICENSE` & `medkit_lib-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/README.md` & `medkit_lib-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/audio/preprocessing/downmixer.py` & `medkit_lib-0.6.0/medkit/audio/preprocessing/downmixer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/audio/preprocessing/power_normalizer.py` & `medkit_lib-0.6.0/medkit/audio/preprocessing/power_normalizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/audio/preprocessing/resampler.py` & `medkit_lib-0.6.0/medkit/audio/preprocessing/resampler.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/audio/segmentation/pa_speaker_detector.py` & `medkit_lib-0.6.0/medkit/audio/segmentation/pa_speaker_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/audio/segmentation/webrtc_voice_detector.py` & `medkit_lib-0.6.0/medkit/audio/segmentation/webrtc_voice_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/audio/transcription/__init__.py` & `medkit_lib-0.6.0/medkit/audio/transcription/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/audio/transcription/doc_transcriber.py` & `medkit_lib-0.6.0/medkit/audio/transcription/doc_transcriber.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/audio/transcription/hf_transcriber_function.py` & `medkit_lib-0.6.0/medkit/audio/transcription/hf_transcriber_function.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/audio/transcription/sb_transcriber_function.py` & `medkit_lib-0.6.0/medkit/audio/transcription/sb_transcriber_function.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/audio/transcription/transcribed_document.py` & `medkit_lib-0.6.0/medkit/audio/transcription/transcribed_document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/__init__.py` & `medkit_lib-0.6.0/medkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/_prov_graph.py` & `medkit_lib-0.6.0/medkit/core/_prov_graph.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/annotation.py` & `medkit_lib-0.6.0/medkit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/annotation_container.py` & `medkit_lib-0.6.0/medkit/core/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/attribute.py` & `medkit_lib-0.6.0/medkit/core/attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/attribute_container.py` & `medkit_lib-0.6.0/medkit/core/attribute_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/audio/__init__.py` & `medkit_lib-0.6.0/medkit/core/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/audio/annotation.py` & `medkit_lib-0.6.0/medkit/core/audio/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/audio/annotation_container.py` & `medkit_lib-0.6.0/medkit/core/audio/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/audio/audio_buffer.py` & `medkit_lib-0.6.0/medkit/core/audio/audio_buffer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/audio/document.py` & `medkit_lib-0.6.0/medkit/core/audio/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/audio/operation.py` & `medkit_lib-0.6.0/medkit/core/audio/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/audio/span.py` & `medkit_lib-0.6.0/medkit/core/audio/span.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/collection.py` & `medkit_lib-0.6.0/medkit/core/collection.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/conversion.py` & `medkit_lib-0.6.0/medkit/core/conversion.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/dict_conv.py` & `medkit_lib-0.6.0/medkit/core/dict_conv.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/doc_pipeline.py` & `medkit_lib-0.6.0/medkit/core/doc_pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/document.py` & `medkit_lib-0.6.0/medkit/core/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/operation.py` & `medkit_lib-0.6.0/medkit/core/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/operation_desc.py` & `medkit_lib-0.6.0/medkit/core/operation_desc.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/pipeline.py` & `medkit_lib-0.6.0/medkit/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/prov_store.py` & `medkit_lib-0.6.0/medkit/core/prov_store.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/prov_tracer.py` & `medkit_lib-0.6.0/medkit/core/prov_tracer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/store.py` & `medkit_lib-0.6.0/medkit/core/store.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/text/__init__.py` & `medkit_lib-0.6.0/medkit/core/text/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/text/annotation.py` & `medkit_lib-0.6.0/medkit/core/text/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/text/annotation_container.py` & `medkit_lib-0.6.0/medkit/core/text/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/text/document.py` & `medkit_lib-0.6.0/medkit/core/text/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/text/entity_attribute_container.py` & `medkit_lib-0.6.0/medkit/core/text/entity_attribute_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/text/entity_norm_attribute.py` & `medkit_lib-0.6.0/medkit/core/text/entity_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/text/operation.py` & `medkit_lib-0.6.0/medkit/core/text/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/text/span.py` & `medkit_lib-0.6.0/medkit/core/text/span.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/text/span_utils.py` & `medkit_lib-0.6.0/medkit/core/text/span_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/text/utils.py` & `medkit_lib-0.6.0/medkit/core/text/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/core/utils.py` & `medkit_lib-0.6.0/medkit/core/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/io/_brat_utils.py` & `medkit_lib-0.6.0/medkit/io/_brat_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/io/brat.py` & `medkit_lib-0.6.0/medkit/io/brat.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/io/medkit_json/__init__.py` & `medkit_lib-0.6.0/medkit/io/medkit_json/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/io/medkit_json/_common.py` & `medkit_lib-0.6.0/medkit/io/medkit_json/_common.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/io/medkit_json/audio.py` & `medkit_lib-0.6.0/medkit/io/medkit_json/audio.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/io/medkit_json/text.py` & `medkit_lib-0.6.0/medkit/io/medkit_json/text.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/io/rttm.py` & `medkit_lib-0.6.0/medkit/io/rttm.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/io/spacy.py` & `medkit_lib-0.6.0/medkit/io/spacy.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/context/__init__.py` & `medkit_lib-0.6.0/medkit/text/context/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/context/family_detector.py` & `medkit_lib-0.6.0/medkit/text/context/family_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/context/family_detector_default_rules.yml` & `medkit_lib-0.6.0/medkit/text/context/family_detector_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/context/hypothesis_detector.py` & `medkit_lib-0.6.0/medkit/text/context/hypothesis_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/context/hypothesis_detector_example_rules.yml` & `medkit_lib-0.6.0/medkit/text/context/hypothesis_detector_example_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/context/hypothesis_detector_example_verbs.yml` & `medkit_lib-0.6.0/medkit/text/context/hypothesis_detector_example_verbs.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/context/negation_detector.py` & `medkit_lib-0.6.0/medkit/text/context/negation_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/context/negation_detector_default_rules.yml` & `medkit_lib-0.6.0/medkit/text/context/negation_detector_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/__init__.py` & `medkit_lib-0.6.0/medkit/text/ner/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/adicap_norm_attribute.py` & `medkit_lib-0.6.0/medkit/text/ner/adicap_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/date_attribute.py` & `medkit_lib-0.6.0/medkit/text/ner/date_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/duckling_matcher.py` & `medkit_lib-0.6.0/medkit/text/ner/duckling_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/hf_entity_matcher.py` & `medkit_lib-0.6.0/medkit/text/ner/hf_entity_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/hf_entity_matcher_trainable.py` & `medkit_lib-0.6.0/medkit/text/ner/hf_entity_matcher_trainable.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,17 @@
 
     def save(self, path: Union[str, Path]):
         state_dict = self._model.state_dict()
         self._model.save_pretrained(path, state_dict=state_dict)
         self._tokenizer.save_pretrained(path)
 
     def load(self, path: Union[str, Path]):
-        tokenizer = transformers.AutoTokenizer.from_pretrained(path, use_fast=True)
+        tokenizer = transformers.AutoTokenizer.from_pretrained(
+            path, use_fast=True, model_max_length=self.tokenizer_max_length
+        )
 
         if not isinstance(tokenizer, transformers.PreTrainedTokenizerFast):
             raise ValueError(
                 "This operation only works with model that have a fast tokenizer. Check"
                 " the hugging face documentation to find the required tokenizer"
             )
 
@@ -199,11 +201,11 @@
         # Easier finetunning
         if sorted(config.label2id.keys()) != sorted(label_to_id.keys()):
             logger.warning(
                 f"""The operation model seems to have different labels.
             PreTrained with labels: {sorted(config.label2id.keys())}, new labels
             {sorted(label_to_id.keys())}. Ignoring the model labels as result."""
             )
-            config.label2id = {label: idx for idx, label in label_to_id.items()}
-            config.id2label = {idx: label for idx, label in label_to_id.items()}
+            config.label2id = {label: idx for label, idx in label_to_id.items()}
+            config.id2label = {idx: label for label, idx in label_to_id.items()}
 
         return config
```

### Comparing `medkit_lib-0.5.0/medkit/text/ner/hf_tokenization_utils.py` & `medkit_lib-0.6.0/medkit/text/ner/hf_tokenization_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -49,14 +49,49 @@
     all_labels = [f"{prefix}-{label}" for label in labels for prefix in scheme]
 
     for idx, label in enumerate(all_labels):
         label_to_id[label] = idx + 1
     return label_to_id
 
 
+def create_entity_tags(
+    nb_tags: int, label: str, tagging_scheme: Literal["bilou", "iob2"]
+) -> List[str]:
+    """Create a list of tags representing one entity
+
+    Parameters
+    ----------
+    nb_tags:
+        Total of tags to create
+    label:
+        Entity label
+    tagging_scheme:
+        Scheme to use in the conversion, "iob2" follows the BIO scheme.
+
+    Returns
+    -------
+    tags: List[str]:
+        Tags representing the entity
+
+    Examples
+    --------
+    >>> create_entity_tags(nb_tags=3, label="corporation", tagging_scheme="bilou")
+    ['B-corporation', 'I-corporation', 'L-corporation']
+    """
+    tags = [f"I-{label}"] * nb_tags
+    if len(tags) == 1:
+        prefix = "U" if tagging_scheme == "bilou" else "B"
+        tags[0] = f"{prefix}-{label}"
+    else:
+        tags[0] = f"B-{label}"
+        prefix = "L" if tagging_scheme == "bilou" else "I"
+        tags[-1] = f"{prefix}-{label}"
+    return tags
+
+
 def transform_entities_to_tags(
     text_encoding: EncodingFast,
     entities: List[Entity],
     tagging_scheme: Literal["bilou", "iob2"] = "bilou",
 ) -> List[str]:
     """
     Transform entities from a encoded document to a list of BILOU/IOB2 tags.
@@ -119,25 +154,20 @@
                 tokens_entity.add(token_id)
 
         tokens_entity = sorted(list(tokens_entity))
 
         if not tokens_entity:
             continue
 
-        if len(tokens_entity) == 1:
-            prefix = "U" if tagging_scheme == "bilou" else "B"
-            tags[tokens_entity[0]] = f"{prefix}-{label}"
-        else:
-            tags[tokens_entity[0]] = f"B-{label}"
-            prefix = "L" if tagging_scheme == "bilou" else "I"
-            tags[tokens_entity[-1]] = f"{prefix}-{label}"
-
-            inside_tokens = tokens_entity[1:-1]
-            for token_idx in inside_tokens:
-                tags[token_idx] = f"I-{label}"
+        entity_tags = create_entity_tags(
+            nb_tags=len(tokens_entity), label=label, tagging_scheme=tagging_scheme
+        )
+
+        for token_idx, tag in zip(tokens_entity, entity_tags):
+            tags[token_idx] = tag
     return tags
 
 
 def align_and_map_tokens_with_tags(
     text_encoding: EncodingFast,
     tags: List[str],
     tag_to_id: Dict[str, int],
```

### Comparing `medkit_lib-0.5.0/medkit/text/ner/iamsystem_matcher.py` & `medkit_lib-0.6.0/medkit/text/ner/iamsystem_matcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     Entity annotator and linker based on iamsystem library
     """
 
     def __init__(
         self,
         matcher: IS_Matcher,
         label_provider: Optional[LabelProvider] = None,
+        attrs_to_copy: Optional[List[str]] = None,
         name: Optional[str] = None,
         uid: Optional[str] = None,
     ):
         """
         Instantiate the operation supporting the iamsystem matcher
 
         Parameters
@@ -86,25 +87,34 @@
         label_provider
             Callable providing the output label to set for detected entity.
             As iamsystem matcher may return several keywords for an annotation,
             we have to know how to provide only one entity label whatever the
             number of matched keywords.
             In medkit, normalization attributes are used for representing detected
             keywords.
+        attrs_to_copy:
+            Labels of the attributes that should be copied from the input segment
+            to the created entity. Useful for propagating context attributes
+            (negation, antecedent, etc).
         name
             Name describing the matcher (defaults to the class name)
         uid
             Identifier of the operation
         """
         # Pass all arguments to super (remove self)
         init_args = locals()
         init_args.pop("self")
         super().__init__(**init_args)
+
+        if attrs_to_copy is None:
+            attrs_to_copy = []
+
         self.matcher = matcher
         self.label_provider = label_provider or DefaultLabelProvider()
+        self.attrs_to_copy = attrs_to_copy
 
     def run(self, segments: List[Segment]) -> List[Entity]:
         entities = []
         for segment in segments:
             anns = self.matcher.annot_text(segment.text)
             for ann in anns:
                 entities.append(self._create_entity_from_iamsystem_ann(ann, segment))
@@ -138,14 +148,23 @@
         entity = Entity(
             label=ent_label,
             text=text,
             spans=spans,
             metadata=metadata,
         )
 
+        # Copy inherited attributes
+        for label in self.attrs_to_copy:
+            for attr in segment.attrs.get(label=label):
+                copied_attr = attr.copy()
+                entity.attrs.add(copied_attr)
+                # handle provenance
+                if self._prov_tracer is not None:
+                    self._prov_tracer.add_prov(copied_attr, self.description, [attr])
+
         if self._prov_tracer is not None:
             self._prov_tracer.add_prov(
                 entity, self.description, source_data_items=[segment]
             )
 
         # create normalization attributes
         for kw in ann.keywords:
```

### Comparing `medkit_lib-0.5.0/medkit/text/ner/quick_umls_matcher.py` & `medkit_lib-0.6.0/medkit/text/ner/quick_umls_matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,18 +86,21 @@
     on a different environment if a similar install is available.
     """
 
     _install_paths: Dict[_QuickUMLSInstall, str] = {}
     _semtype_to_semgroup: Optional[Dict[str, str]] = None
 
     DEFAULT_LABEL_MAPPING: Dict[str, str] = {
+        "ACTI": "activity",
         "ANAT": "anatomy",
         "CHEM": "chemical",
+        "CONC": "concept",
         "DEVI": "device",
         "DISO": "disorder",
+        "GENE": "genes_sequence",
         "GEOG": "geographic_area",
         "LIVB": "living_being",
         "OBJC": "object",
         "PHEN": "phenomenon",
         "PHYS": "physiology",
         "PROC": "procedure",
     }
```

### Comparing `medkit_lib-0.5.0/medkit/text/ner/regexp_matcher.py` & `medkit_lib-0.6.0/medkit/text/ner/regexp_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/regexp_matcher_default_rules.yml` & `medkit_lib-0.6.0/medkit/text/ner/regexp_matcher_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/tnm_attribute.py` & `medkit_lib-0.6.0/medkit/text/ner/tnm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/umls_coder_normalizer.py` & `medkit_lib-0.6.0/medkit/text/ner/umls_coder_normalizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/umls_norm_attribute.py` & `medkit_lib-0.6.0/medkit/text/ner/umls_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/umls_semgroups_v04.txt` & `medkit_lib-0.6.0/medkit/text/ner/umls_semgroups_v04.txt`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/ner/umls_utils.py` & `medkit_lib-0.6.0/medkit/text/ner/umls_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/postprocessing/attribute_duplicator.py` & `medkit_lib-0.6.0/medkit/text/postprocessing/attribute_duplicator.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/preprocessing/__init__.py` & `medkit_lib-0.6.0/medkit/text/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/preprocessing/eds_cleaner.py` & `medkit_lib-0.6.0/medkit/text/preprocessing/eds_cleaner.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/preprocessing/normalizer.py` & `medkit_lib-0.6.0/medkit/text/preprocessing/normalizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/relations/syntactic_relation_extractor.py` & `medkit_lib-0.6.0/medkit/text/relations/syntactic_relation_extractor.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/segmentation/default_section_definition.yml` & `medkit_lib-0.6.0/medkit/text/segmentation/default_section_definition.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/segmentation/rush_sentence_tokenizer.py` & `medkit_lib-0.6.0/medkit/text/segmentation/rush_sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv` & `medkit_lib-0.6.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/segmentation/section_tokenizer.py` & `medkit_lib-0.6.0/medkit/text/segmentation/section_tokenizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
 
 __all__ = ["SectionModificationRule", "SectionTokenizer"]
 
 import dataclasses
 import pathlib
-from typing import Dict, List, Optional, Tuple
+from typing import Dict, Iterable, List, Optional, Tuple
 from typing_extensions import Literal
 import yaml
 
 from flashtext import KeywordProcessor
 
 from medkit.core.text import Segment, SegmentationOperation, span_utils
+from medkit.text.segmentation.tokenizer_utils import lstrip, rstrip
 
 
 _DEFAULT_SECTION_DEFINITION_RULES = (
     pathlib.Path(__file__).parent / "default_section_definition.yml"
 )
 
 
 @dataclasses.dataclass(frozen=True)
 class DefaultConfig:
     output_label: str = "SECTION"
+    strip_chars: str = ".;,?! \n\r\t"
 
 
 @dataclasses.dataclass
 class SectionModificationRule:
     section_name: str
     new_section_name: str
     other_sections: List[str]
@@ -34,15 +36,16 @@
 class SectionTokenizer(SegmentationOperation):
     """Section segmentation annotator based on keyword rules"""
 
     def __init__(
         self,
         section_dict: Dict[str, List[str]],
         output_label: str = DefaultConfig.output_label,
-        section_rules: Tuple[SectionModificationRule] = (),
+        section_rules: Iterable[SectionModificationRule] = (),
+        strip_chars: str = DefaultConfig.strip_chars,
         uid: Optional[str] = None,
     ):
         """
         Initialize the Section Tokenizer
 
         Parameters
         ----------
@@ -50,23 +53,29 @@
             Dictionary containing the section name as key and the list of mappings
             as value (cf. content of default_section_dict.yml as example)
         output_label
             Segment label to use for annotation output. Default is SECTION.
         section_rules
             List of rules for modifying a section name according its order to the other
             sections.
+        strip_chars
+            The list of characters to strip at the beginning of the returned segment.
+            Default: '.;,?! \n\r\t' (cf. DefaultConfig)
+        uid: str, Optional
+            Identifier of the tokenizer
         """
         # Pass all arguments to super (remove self)
         init_args = locals()
         init_args.pop("self")
         super().__init__(**init_args)
 
         self.output_label = output_label
         self.section_dict = section_dict
-        self.section_rules = section_rules
+        self.section_rules = tuple(section_rules)
+        self.strip_chars = strip_chars
         self.keyword_processor = KeywordProcessor(case_sensitive=True)
         self.keyword_processor.add_keywords_from_dict(section_dict)
 
     def run(self, segments: List[Segment]) -> List[Segment]:
         """
         Return sections detected in `segments`.
 
@@ -104,19 +113,31 @@
         for index, section in enumerate(match):
             name = new_sections.get(index, section[0])
             if index != len(match) - 1:
                 ranges = [(section[1], match[index + 1][1])]
             else:
                 ranges = [(section[1], len(segment.text))]
 
+            # Remove extra characters at beginning of the detected segments
+            # and white spaces at end of the text
+            strip_ranges = []
+            for start, end in ranges:
+                text, new_start = lstrip(
+                    segment.text[start:end], start, self.strip_chars
+                )
+                text, new_end = rstrip(text, end)
+                if len(text) == 0:  # empty segment
+                    continue
+                strip_ranges.append((new_start, new_end))
+
             # Extract medkit spans from relative spans (i.e., ranges)
             text, spans = span_utils.extract(
                 text=segment.text,
                 spans=segment.spans,
-                ranges=ranges,
+                ranges=strip_ranges,
             )
 
             # add section name in metadata
             metadata = dict(name=name)
             section = Segment(
                 label=self.output_label,
                 spans=spans,
@@ -166,28 +187,28 @@
             section_rules=section_rules,
         )
         return section_tokenizer
 
     @staticmethod
     def load_section_definition(
         filepath: pathlib.Path, encoding: Optional[str] = None
-    ) -> Tuple[Dict[str, List[str]], Tuple[SectionModificationRule]]:
+    ) -> Tuple[Dict[str, List[str]], Tuple[SectionModificationRule, ...]]:
         """
         Load the sections definition stored in a yml file
 
         Parameters
         ----------
         filepath:
             Path to a yml file containing the sections(name + mappings) and rules
         encoding:
             Encoding of the file to open
 
         Returns
         -------
-        Tuple[Dict[str, List[str]], Tuple[SectionModificationRule]]
+        Tuple[Dict[str, List[str]], Tuple[SectionModificationRule, ...]]
             Tuple containing:
             - the dictionary where key is the section name and value is the list of all
             equivalent strings.
             - the list of section modification rules.
             These rules allow to rename some sections according their order
         """
 
@@ -196,7 +217,36 @@
 
         section_dict = config["sections"]
         section_rules = tuple(
             SectionModificationRule(**rule) for rule in config["rules"]
         )
 
         return section_dict, section_rules
+
+    @staticmethod
+    def save_section_definition(
+        section_dict: Dict[str, List[str]],
+        section_rules: Iterable[SectionModificationRule],
+        filepath: pathlib.Path,
+        encoding: Optional[str] = None,
+    ):
+        """
+        Save section yaml definition file
+
+        Parameters
+        ----------
+        section_dict
+            Dictionary containing the section name as key and the list of mappings
+            as value (cf. content of default_section_dict.yml as example)
+        section_rules
+            List of rules for modifying a section name according its order to the other
+            sections.
+        filepath
+            Path to the file to save
+        encoding
+            File encoding. Default: None
+        """
+        with open(filepath, mode="w", encoding=encoding) as f:
+            data = {"sections": section_dict, "rules": []}
+            for rule in section_rules:
+                data["rules"].append(dataclasses.asdict(rule))
+            yaml.safe_dump(data, f, allow_unicode=True, encoding=encoding)
```

### Comparing `medkit_lib-0.5.0/medkit/text/segmentation/sentence_tokenizer.py` & `medkit_lib-0.6.0/medkit/text/segmentation/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/spacy/__init__.py` & `medkit_lib-0.6.0/medkit/text/spacy/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/spacy/displacy_utils.py` & `medkit_lib-0.6.0/medkit/text/spacy/displacy_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/spacy/doc_pipeline.py` & `medkit_lib-0.6.0/medkit/text/spacy/doc_pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/spacy/edsnlp.py` & `medkit_lib-0.6.0/medkit/text/spacy/edsnlp.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/spacy/pipeline.py` & `medkit_lib-0.6.0/medkit/text/spacy/pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/spacy/spacy_utils.py` & `medkit_lib-0.6.0/medkit/text/spacy/spacy_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/text/translation/hf_translator.py` & `medkit_lib-0.6.0/medkit/text/translation/hf_translator.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/tools/hf_utils.py` & `medkit_lib-0.6.0/medkit/tools/hf_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/tools/save_prov_to_dot.py` & `medkit_lib-0.6.0/medkit/tools/save_prov_to_dot.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/training/__init__.py` & `medkit_lib-0.6.0/medkit/training/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/training/callbacks.py` & `medkit_lib-0.6.0/medkit/training/callbacks.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/training/trainable_component.py` & `medkit_lib-0.6.0/medkit/training/trainable_component.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/training/trainer.py` & `medkit_lib-0.6.0/medkit/training/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             total_loss_epoch += loss.item()
 
             if config.do_metrics_in_training and self.metrics_computer is not None:
                 prepared_batch = self.metrics_computer.prepare_batch(
                     model_output, input_batch
                 )
                 for key, values in prepared_batch.items():
-                    data_for_metrics[key].append(values)
+                    data_for_metrics[key].extend(values)
 
             self.callback.on_step_end(
                 step, nb_batches=len(self.train_dataloader), phase="train"
             )
 
         total_loss_epoch /= len(self.train_dataloader)
         metrics["loss"] = total_loss_epoch
@@ -208,15 +208,15 @@
                 total_loss_epoch += loss.item()
 
                 if self.metrics_computer is not None:
                     prepared_batch = self.metrics_computer.prepare_batch(
                         model_output, input_batch
                     )
                     for key, values in prepared_batch.items():
-                        data_for_metrics[key].append(values)
+                        data_for_metrics[key].extend(values)
 
                 self.callback.on_step_end(
                     step, nb_batches=len(eval_dataloader), phase="eval"
                 )
 
         total_loss_epoch /= len(self.eval_dataloader)
         metrics["loss"] = total_loss_epoch
```

### Comparing `medkit_lib-0.5.0/medkit/training/trainer_config.py` & `medkit_lib-0.6.0/medkit/training/trainer_config.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/medkit/training/utils.py` & `medkit_lib-0.6.0/medkit/training/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.5.0/pyproject.toml` & `medkit_lib-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medkit-lib"
-version = "0.5.0"
+version = "0.6.0"
 description = "A Python library for a learning health system"
 readme = "README.md"
 repository = "https://gitlab.inria.fr/heka/medkit/"
 documentation = "https://heka.gitlabpages.inria.fr/medkit/"
 authors = ["HeKA Research Team"]
 maintainers = [
     "medkit-maintainers <medkit-maintainers@inria.fr>"
@@ -54,14 +54,15 @@
 sentencepiece = {version = "*", optional = true}
 spacy = {version = "^3.4", optional = true}
 speechbrain = {version = "^0.5", optional = true}
 torch = {version ="^1.0", optional = true}
 torchaudio = {version ="^0.12", optional = true}
 transformers = {version = "^4.21", optional = true}
 webrtcvad = {version = "^2.0", optional = true}
+seqeval = {version = "^1.2.2", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 pytest-cov = "*"
 pytest-mock = "*"
 pre-commit = "*"
 
@@ -91,14 +92,15 @@
 hf-translator = [
     "sacremoses",  # needed by default model "Helsinki-NLP/opus-mt-fr-en"
     "sentencepiece",
     "torch",
     "transformers"
 ]
 hf-utils = ["transformers"]
+metrics-ner = ["seqeval","transformers","torch"]
 pa-speaker-detector = [
     "torch",
     "pyannote-audio",
 ]
 quick-umls = [
     "packaging",  # needed to check quickumls version
     "quickumls",
@@ -130,14 +132,15 @@
     "pandas",
     "PyRuSH",
     "quickumls",
     "resampy",
     "sacremoses",
     "sentencepiece",
     "spacy",
+    "seqeval",
     "torch",
     "torchaudio",
     "transformers",
     "webrtcvad",
 ]
 
 [build-system]
@@ -147,13 +150,13 @@
 
 [tool.black]
 line-length = 88
 preview = true
 extend-exclude = ".venv"
 
 [tool.poetry-dynamic-versioning]
-enable = false
+enable = true
 vcs = "git"
 dirty = true
 pattern = "(?P<base>\\d+(\\.\\d+)*)"
 latest-tag = true
 style = "semver"
```

### Comparing `medkit_lib-0.5.0/PKG-INFO` & `medkit_lib-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medkit-lib
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python library for a learning health system
 Home-page: https://gitlab.inria.fr/heka/medkit/
 License: MIT
 Author: HeKA Research Team
 Maintainer: medkit-maintainers
 Maintainer-email: medkit-maintainers@inria.fr
 Requires-Python: >=3.7.1,<4.0
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Provides-Extra: edsnlp
 Provides-Extra: hf-entity-matcher
 Provides-Extra: hf-transcriber-function
 Provides-Extra: hf-translator
 Provides-Extra: hf-utils
+Provides-Extra: metrics-ner
 Provides-Extra: optional
 Provides-Extra: pa-speaker-detector
 Provides-Extra: quick-umls
 Provides-Extra: resampler
 Provides-Extra: rush-sentence-tokenizer
 Provides-Extra: sb-transcriber-function
 Provides-Extra: spacy
@@ -49,22 +50,23 @@
 Requires-Dist: pyaml
 Requires-Dist: pyannote-audio (>=2.1,<3.0) ; extra == "pa-speaker-detector"
 Requires-Dist: quickumls (>=1.4,<2.0) ; extra == "quick-umls" or extra == "optional"
 Requires-Dist: requests
 Requires-Dist: resampy (>=0.4,<0.5) ; extra == "resampler" or extra == "optional"
 Requires-Dist: sacremoses ; extra == "hf-translator" or extra == "optional"
 Requires-Dist: sentencepiece ; extra == "hf-translator" or extra == "optional"
+Requires-Dist: seqeval (>=1.2.2,<2.0.0) ; extra == "metrics-ner" or extra == "optional"
 Requires-Dist: smart-open
 Requires-Dist: soundfile
 Requires-Dist: spacy (>=3.4,<4.0) ; extra == "spacy" or extra == "syntactic-relation-extractor" or extra == "optional"
 Requires-Dist: speechbrain (>=0.5,<0.6) ; extra == "sb-transcriber-function"
-Requires-Dist: torch (>=1.0,<2.0) ; extra == "hf-entity-matcher" or extra == "hf-translator" or extra == "pa-speaker-detector" or extra == "sb-transcriber-function" or extra == "training" or extra == "umls-coder-normalizer" or extra == "optional"
+Requires-Dist: torch (>=1.0,<2.0) ; extra == "hf-entity-matcher" or extra == "hf-translator" or extra == "metrics-ner" or extra == "pa-speaker-detector" or extra == "sb-transcriber-function" or extra == "training" or extra == "umls-coder-normalizer" or extra == "optional"
 Requires-Dist: torchaudio (>=0.12,<0.13) ; extra == "hf-transcriber-function" or extra == "optional"
 Requires-Dist: tqdm
-Requires-Dist: transformers (>=4.21,<5.0) ; extra == "hf-entity-matcher" or extra == "hf-transcriber-function" or extra == "hf-translator" or extra == "hf-utils" or extra == "sb-transcriber-function" or extra == "umls-coder-normalizer" or extra == "optional"
+Requires-Dist: transformers (>=4.21,<5.0) ; extra == "hf-entity-matcher" or extra == "hf-transcriber-function" or extra == "hf-translator" or extra == "hf-utils" or extra == "metrics-ner" or extra == "sb-transcriber-function" or extra == "umls-coder-normalizer" or extra == "optional"
 Requires-Dist: typing-extensions
 Requires-Dist: webrtcvad (>=2.0,<3.0) ; extra == "webrtc-voice-detector" or extra == "optional"
 Requires-Dist: wheel
 Project-URL: Documentation, https://heka.gitlabpages.inria.fr/medkit/
 Project-URL: Repository, https://gitlab.inria.fr/heka/medkit/
 Description-Content-Type: text/markdown
```

