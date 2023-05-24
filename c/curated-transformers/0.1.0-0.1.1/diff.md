# Comparing `tmp/curated-transformers-0.1.0.tar.gz` & `tmp/curated-transformers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-transformers-0.1.0.tar", last modified: Fri May  5 11:55:56 2023, max compression
+gzip compressed data, was "curated-transformers-0.1.1.tar", last modified: Wed May 24 07:10:38 2023, max compression
```

## Comparing `curated-transformers-0.1.0.tar` & `curated-transformers-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      101 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)      773 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      460 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.113939 curated-transformers-0.1.0/curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      313 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/_compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4688 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.113939 curated-transformers-0.1.0/curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      194 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      583 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/activations.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/albert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2362 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/albert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)      949 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/albert/layer_group.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2258 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/attention.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3795 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/bert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/bert/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1738 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/bert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4774 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/bert/layer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1239 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/curated_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10980 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/hf_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1556 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/output.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/roberta/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/roberta/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1780 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/roberta/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1881 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/scalar_weight.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1254 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)       94 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/tests/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      280 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/models/albert/test_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2969 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/models/test_hf_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1441 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/models/test_torchscript.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/tests/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tokenization/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.113939 curated-transformers-0.1.0/curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)      773 2023-05-05 11:55:56.000000 curated-transformers-0.1.0/curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1869 2023-05-05 11:55:56.000000 curated-transformers-0.1.0/curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-05 11:55:56.000000 curated-transformers-0.1.0/curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       36 2023-05-05 11:55:56.000000 curated-transformers-0.1.0/curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-05-05 11:55:56.000000 curated-transformers-0.1.0/curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-05 11:55:55.000000 curated-transformers-0.1.0/curated_transformers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)      612 2023-05-05 11:55:56.121939 curated-transformers-0.1.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      101 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)      933 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      620 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.767744 curated-transformers-0.1.1/curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      313 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/_compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4688 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.767744 curated-transformers-0.1.1/curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      194 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      583 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/activations.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/albert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2362 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/albert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      949 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/albert/layer_group.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2258 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/attention.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3795 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/bert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/bert/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1738 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/bert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4774 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/bert/layer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1239 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/curated_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10980 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/hf_util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1556 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/output.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/roberta/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/roberta/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1780 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/roberta/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1881 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/models/scalar_weight.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1254 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       94 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/tests/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      280 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/models/albert/test_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2969 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/models/test_hf_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1441 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/models/test_torchscript.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/tests/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.771744 curated-transformers-0.1.1/curated_transformers/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/curated_transformers/tokenization/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 07:10:38.767744 curated-transformers-0.1.1/curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)      933 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1869 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-24 07:10:38.000000 curated-transformers-0.1.1/curated_transformers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)      589 2023-05-24 07:10:38.775744 curated-transformers-0.1.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-05-24 07:10:27.000000 curated-transformers-0.1.1/setup.py
```

### Comparing `curated-transformers-0.1.0/LICENSE` & `curated-transformers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/PKG-INFO` & `curated-transformers-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Curated transformer models
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -18,14 +18,18 @@
 
 - ALBERT
 - BERT
 - CamemBERT
 - RoBERTa
 - XLM-RoBERTa
 
+spaCy integration for curated transformers is provided by the
+[`spacy-curated-transformers`](https://github.com/explosion/spacy-curated-transformers)
+package.
+
 ## ⚠️ Warning: experimental package
 
 This package is experimental and it is possible that models and APIs will
 change in incompatible ways.
 
 ## ⏳ Install
```

### Comparing `curated-transformers-0.1.0/curated_transformers/errors.py` & `curated-transformers-0.1.1/curated_transformers/errors.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/activations.py` & `curated-transformers-0.1.1/curated_transformers/models/activations.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/albert/config.py` & `curated-transformers-0.1.1/curated_transformers/models/albert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/albert/encoder.py` & `curated-transformers-0.1.1/curated_transformers/models/albert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/albert/layer_group.py` & `curated-transformers-0.1.1/curated_transformers/models/albert/layer_group.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/attention.py` & `curated-transformers-0.1.1/curated_transformers/models/attention.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/bert/config.py` & `curated-transformers-0.1.1/curated_transformers/models/bert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/bert/embeddings.py` & `curated-transformers-0.1.1/curated_transformers/models/bert/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/bert/encoder.py` & `curated-transformers-0.1.1/curated_transformers/models/bert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/bert/layer.py` & `curated-transformers-0.1.1/curated_transformers/models/bert/layer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/curated_transformer.py` & `curated-transformers-0.1.1/curated_transformers/models/curated_transformer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/embeddings.py` & `curated-transformers-0.1.1/curated_transformers/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/hf_util.py` & `curated-transformers-0.1.1/curated_transformers/models/hf_util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/output.py` & `curated-transformers-0.1.1/curated_transformers/models/output.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/roberta/config.py` & `curated-transformers-0.1.1/curated_transformers/models/roberta/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/roberta/embeddings.py` & `curated-transformers-0.1.1/curated_transformers/models/roberta/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/roberta/encoder.py` & `curated-transformers-0.1.1/curated_transformers/models/roberta/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/models/scalar_weight.py` & `curated-transformers-0.1.1/curated_transformers/models/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/tests/conftest.py` & `curated-transformers-0.1.1/curated_transformers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/tests/models/test_hf_model.py` & `curated-transformers-0.1.1/curated_transformers/tests/models/test_hf_model.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers/tests/models/test_torchscript.py` & `curated-transformers-0.1.1/curated_transformers/tests/models/test_torchscript.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/curated_transformers.egg-info/PKG-INFO` & `curated-transformers-0.1.1/curated_transformers.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Curated transformer models
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -18,14 +18,18 @@
 
 - ALBERT
 - BERT
 - CamemBERT
 - RoBERTa
 - XLM-RoBERTa
 
+spaCy integration for curated transformers is provided by the
+[`spacy-curated-transformers`](https://github.com/explosion/spacy-curated-transformers)
+package.
+
 ## ⚠️ Warning: experimental package
 
 This package is experimental and it is possible that models and APIs will
 change in incompatible ways.
 
 ## ⏳ Install
```

### Comparing `curated-transformers-0.1.0/curated_transformers.egg-info/SOURCES.txt` & `curated-transformers-0.1.1/curated_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.1.0/setup.cfg` & `curated-transformers-0.1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [metadata]
-version = 0.1.0
+version = 0.1.1
 description = Curated transformer models
 url = https://github.com/explosion/curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 zip_safe = true
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
-	cutlery>=0.0.3,<0.1.0
 	torch>=1.12.0
 
 [bdist_wheel]
 universal = true
 
 [sdist]
 formats = gztar
```

