# Comparing `tmp/squirrel_datasets_core-0.3.1.dev22854.tar.gz` & `tmp/squirrel_datasets_core-0.3.1.dev577398.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squirrel_datasets_core-0.3.1.dev22854.tar", max compression
+gzip compressed data, was "squirrel_datasets_core-0.3.1.dev577398.tar", max compression
```

## Comparing `squirrel_datasets_core-0.3.1.dev22854.tar` & `squirrel_datasets_core-0.3.1.dev577398.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11347 2023-05-24 06:42:45.722647 squirrel_datasets_core-0.3.1.dev22854/LICENSE
--rw-r--r--   0        0        0     5115 2023-05-24 06:42:45.722647 squirrel_datasets_core-0.3.1.dev22854/README.md
--rw-r--r--   0        0        0     2526 2023-05-24 06:53:34.187967 squirrel_datasets_core-0.3.1.dev22854/pyproject.toml
--rw-r--r--   0        0        0       89 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/__init__.py
--rw-r--r--   0        0        0     2793 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/AutoML/README.rst
--rw-r--r--   0        0        0      636 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/AutoML/__init__.py
--rw-r--r--   0        0        0     3487 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/AutoML/driver.py
--rw-r--r--   0        0        0        0 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/__init__.py
--rw-r--r--   0        0        0     2147 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/adult_dataset/README.rst
--rw-r--r--   0        0        0      410 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/adult_dataset/__init__.py
--rw-r--r--   0        0        0     2154 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/adult_dataset/driver.py
--rw-r--r--   0        0        0     2024 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/allenai_c4/README.rst
--rw-r--r--   0        0        0      441 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/allenai_c4/__init__.py
--rw-r--r--   0        0        0     4071 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/allenai_c4/allenai_c4_multilingual.py
--rw-r--r--   0        0        0    11361 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/allenai_c4/constants.py
--rw-r--r--   0        0        0     1937 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/bdd100k/README.rst
--rw-r--r--   0        0        0      139 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/bdd100k/__init__.py
--rw-r--r--   0        0        0     3957 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/bdd100k/driver.py
--rw-r--r--   0        0        0     2042 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/california_housing/README.rst
--rw-r--r--   0        0        0      619 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/california_housing/__init__.py
--rw-r--r--   0        0        0     1430 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/california_housing/driver.py
--rw-r--r--   0        0        0     2300 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/camvid/README.rst
--rw-r--r--   0        0        0      135 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/camvid/__init__.py
--rw-r--r--   0        0        0     4061 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/camvid/driver.py
--rw-r--r--   0        0        0     1590 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/cc100/README.rst
--rw-r--r--   0        0        0      394 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/cc100/__init__.py
--rw-r--r--   0        0        0     3188 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/cc100/cc100.py
--rw-r--r--   0        0        0     6352 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/cc100/constants.py
--rw-r--r--   0        0        0     1806 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/conceptual_captions/README.rst
--rw-r--r--   0        0        0      445 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/conceptual_captions/__init__.py
--rw-r--r--   0        0        0     4157 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/conceptual_captions/driver.py
--rw-r--r--   0        0        0     2374 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/ds_bowl_2018/README.rst
--rw-r--r--   0        0        0      180 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/ds_bowl_2018/__init__.py
--rw-r--r--   0        0        0     3788 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/ds_bowl_2018/driver.py
--rw-r--r--   0        0        0      761 2023-05-24 06:42:45.730647 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/fem_simulations/README.rst
--rw-r--r--   0        0        0     5783 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/fem_simulations/__init__.py
--rw-r--r--   0        0        0     1914 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/hugging_face/__init__.py
--rw-r--r--   0        0        0     1528 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/imagenet/README.rst
--rw-r--r--   0        0        0      286 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/imagenet/__init__.py
--rw-r--r--   0        0        0    10812 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/imagenet/driver.py
--rw-r--r--   0        0        0     3208 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/kaggle_casting_quality/README.rst
--rw-r--r--   0        0        0      336 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/kaggle_casting_quality/__init__.py
--rw-r--r--   0        0        0     1910 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/kaggle_casting_quality/driver.py
--rw-r--r--   0        0        0     3426 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/monthly_german_tweets/README.rst
--rw-r--r--   0        0        0      189 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/monthly_german_tweets/__init__.py
--rw-r--r--   0        0        0     2324 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/monthly_german_tweets/driver.py
--rw-r--r--   0        0        0        0 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/railsem19/__init__.py
--rw-r--r--   0        0        0     8076 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/railsem19/railsem19_preprocessing.py
--rw-r--r--   0        0        0      709 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/torchvision/__init__.py
--rw-r--r--   0        0        0     1539 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/driver/__init__.py
--rw-r--r--   0        0        0     1549 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/driver/deeplake.py
--rw-r--r--   0        0        0     1466 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/driver/hub.py
--rw-r--r--   0        0        0      961 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/driver/huggingface.py
--rw-r--r--   0        0        0     4003 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/driver/torchvision.py
--rw-r--r--   0        0        0       78 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/io/__init__.py
--rw-r--r--   0        0        0     1002 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/io/io.py
--rw-r--r--   0        0        0     2422 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/parse_dataset_cards.py
--rw-r--r--   0        0        0        0 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/preprocessing/__init__.py
--rw-r--r--   0        0        0     4155 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/preprocessing/save_shards.py
--rw-r--r--   0        0        0      224 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/py.typed
--rw-r--r--   0        0        0      193 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/spark/__init__.py
--rw-r--r--   0        0        0      331 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/spark/dummy_df.py
--rw-r--r--   0        0        0     4405 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/spark/setup_spark.py
--rw-r--r--   0        0        0     2361 2023-05-24 06:42:45.734648 squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/squirrel_plugin.py
--rw-r--r--   0        0        0     6806 1970-01-01 00:00:00.000000 squirrel_datasets_core-0.3.1.dev22854/PKG-INFO
+-rw-r--r--   0        0        0    11347 2023-03-27 12:10:19.022080 squirrel_datasets_core-0.3.1.dev577398/LICENSE
+-rw-r--r--   0        0        0     5115 2023-03-27 12:10:19.022080 squirrel_datasets_core-0.3.1.dev577398/README.md
+-rw-r--r--   0        0        0     2527 2023-03-27 12:20:39.787250 squirrel_datasets_core-0.3.1.dev577398/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/__init__.py
+-rw-r--r--   0        0        0     2793 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/AutoML/README.rst
+-rw-r--r--   0        0        0      636 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/AutoML/__init__.py
+-rw-r--r--   0        0        0     3487 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/AutoML/driver.py
+-rw-r--r--   0        0        0        0 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/__init__.py
+-rw-r--r--   0        0        0     2147 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/adult_dataset/README.rst
+-rw-r--r--   0        0        0      410 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/adult_dataset/__init__.py
+-rw-r--r--   0        0        0     2154 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/adult_dataset/driver.py
+-rw-r--r--   0        0        0     2024 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/allenai_c4/README.rst
+-rw-r--r--   0        0        0      441 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/allenai_c4/__init__.py
+-rw-r--r--   0        0        0     4071 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/allenai_c4/allenai_c4_multilingual.py
+-rw-r--r--   0        0        0    11361 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/allenai_c4/constants.py
+-rw-r--r--   0        0        0     1937 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/bdd100k/README.rst
+-rw-r--r--   0        0        0      139 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/bdd100k/__init__.py
+-rw-r--r--   0        0        0     3957 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/bdd100k/driver.py
+-rw-r--r--   0        0        0     2042 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/california_housing/README.rst
+-rw-r--r--   0        0        0      619 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/california_housing/__init__.py
+-rw-r--r--   0        0        0     1430 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/california_housing/driver.py
+-rw-r--r--   0        0        0     2300 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/camvid/README.rst
+-rw-r--r--   0        0        0      135 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/camvid/__init__.py
+-rw-r--r--   0        0        0     4061 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/camvid/driver.py
+-rw-r--r--   0        0        0     1590 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/cc100/README.rst
+-rw-r--r--   0        0        0      394 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/cc100/__init__.py
+-rw-r--r--   0        0        0     3188 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/cc100/cc100.py
+-rw-r--r--   0        0        0     6352 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/cc100/constants.py
+-rw-r--r--   0        0        0     1806 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/conceptual_captions/README.rst
+-rw-r--r--   0        0        0      445 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/conceptual_captions/__init__.py
+-rw-r--r--   0        0        0     4157 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/conceptual_captions/driver.py
+-rw-r--r--   0        0        0     2374 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/ds_bowl_2018/README.rst
+-rw-r--r--   0        0        0      180 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/ds_bowl_2018/__init__.py
+-rw-r--r--   0        0        0     3788 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/ds_bowl_2018/driver.py
+-rw-r--r--   0        0        0      761 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/fem_simulations/README.rst
+-rw-r--r--   0        0        0     5783 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/fem_simulations/__init__.py
+-rw-r--r--   0        0        0     1914 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/hugging_face/__init__.py
+-rw-r--r--   0        0        0     1528 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/imagenet/README.rst
+-rw-r--r--   0        0        0      286 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/imagenet/__init__.py
+-rw-r--r--   0        0        0    10812 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/imagenet/driver.py
+-rw-r--r--   0        0        0     3208 2023-03-27 12:10:19.030080 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/kaggle_casting_quality/README.rst
+-rw-r--r--   0        0        0      336 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/kaggle_casting_quality/__init__.py
+-rw-r--r--   0        0        0     1910 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/kaggle_casting_quality/driver.py
+-rw-r--r--   0        0        0     3426 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/monthly_german_tweets/README.rst
+-rw-r--r--   0        0        0      189 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/monthly_german_tweets/__init__.py
+-rw-r--r--   0        0        0     2324 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/monthly_german_tweets/driver.py
+-rw-r--r--   0        0        0        0 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/railsem19/__init__.py
+-rw-r--r--   0        0        0     8076 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/railsem19/railsem19_preprocessing.py
+-rw-r--r--   0        0        0      709 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/torchvision/__init__.py
+-rw-r--r--   0        0        0     1539 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/utils.py
+-rw-r--r--   0        0        0        0 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/driver/__init__.py
+-rw-r--r--   0        0        0     1549 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/driver/deeplake.py
+-rw-r--r--   0        0        0     1466 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/driver/hub.py
+-rw-r--r--   0        0        0      961 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/driver/huggingface.py
+-rw-r--r--   0        0        0     4003 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/driver/torchvision.py
+-rw-r--r--   0        0        0       78 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/io/__init__.py
+-rw-r--r--   0        0        0     1002 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/io/io.py
+-rw-r--r--   0        0        0     2422 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/parse_dataset_cards.py
+-rw-r--r--   0        0        0        0 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4155 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/preprocessing/save_shards.py
+-rw-r--r--   0        0        0      224 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/py.typed
+-rw-r--r--   0        0        0      193 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/spark/__init__.py
+-rw-r--r--   0        0        0      331 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/spark/dummy_df.py
+-rw-r--r--   0        0        0     4405 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/spark/setup_spark.py
+-rw-r--r--   0        0        0     2361 2023-03-27 12:10:19.034081 squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/squirrel_plugin.py
+-rw-r--r--   0        0        0     6857 1970-01-01 00:00:00.000000 squirrel_datasets_core-0.3.1.dev577398/PKG-INFO
```

### Comparing `squirrel_datasets_core-0.3.1.dev22854/LICENSE` & `squirrel_datasets_core-0.3.1.dev577398/LICENSE`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/README.md` & `squirrel_datasets_core-0.3.1.dev577398/README.md`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/pyproject.toml` & `squirrel_datasets_core-0.3.1.dev577398/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squirrel-datasets-core"
-version = "0.3.1-dev22854"
+version = "0.3.1-dev577398"
 description = "Squirrel public datasets collection"
 authors = ["Merantix Momentum"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "squirrel_datasets_core", from = "src"}]
 homepage = "https://merantix-momentum.com/technology/squirrel/"
 repository = "https://github.com/merantix-momentum/squirrel-datasets-core"
```

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/AutoML/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/AutoML/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/AutoML/__init__.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/AutoML/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/AutoML/driver.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/AutoML/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/adult_dataset/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/adult_dataset/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/adult_dataset/driver.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/adult_dataset/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/allenai_c4/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/allenai_c4/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/allenai_c4/allenai_c4_multilingual.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/allenai_c4/allenai_c4_multilingual.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/allenai_c4/constants.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/allenai_c4/constants.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/bdd100k/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/bdd100k/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/bdd100k/driver.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/bdd100k/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/california_housing/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/california_housing/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/california_housing/__init__.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/california_housing/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/california_housing/driver.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/california_housing/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/camvid/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/camvid/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/camvid/driver.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/camvid/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/cc100/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/cc100/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/cc100/cc100.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/cc100/cc100.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/cc100/constants.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/cc100/constants.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/conceptual_captions/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/conceptual_captions/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/conceptual_captions/driver.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/conceptual_captions/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/ds_bowl_2018/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/ds_bowl_2018/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/ds_bowl_2018/driver.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/ds_bowl_2018/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/fem_simulations/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/fem_simulations/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/fem_simulations/__init__.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/fem_simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/hugging_face/__init__.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/imagenet/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/imagenet/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/imagenet/driver.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/imagenet/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/kaggle_casting_quality/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/kaggle_casting_quality/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/kaggle_casting_quality/driver.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/kaggle_casting_quality/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/monthly_german_tweets/README.rst` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/monthly_german_tweets/README.rst`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/monthly_german_tweets/driver.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/monthly_german_tweets/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/railsem19/railsem19_preprocessing.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/railsem19/railsem19_preprocessing.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/torchvision/__init__.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/torchvision/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/datasets/utils.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/driver/deeplake.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/driver/deeplake.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/driver/hub.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/driver/hub.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/driver/huggingface.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/driver/huggingface.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/driver/torchvision.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/driver/torchvision.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/io/io.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/io/io.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/parse_dataset_cards.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/parse_dataset_cards.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/preprocessing/save_shards.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/preprocessing/save_shards.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/spark/setup_spark.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/spark/setup_spark.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/src/squirrel_datasets_core/squirrel_plugin.py` & `squirrel_datasets_core-0.3.1.dev577398/src/squirrel_datasets_core/squirrel_plugin.py`

 * *Files identical despite different names*

### Comparing `squirrel_datasets_core-0.3.1.dev22854/PKG-INFO` & `squirrel_datasets_core-0.3.1.dev577398/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: squirrel-datasets-core
-Version: 0.3.1.dev22854
+Version: 0.3.1.dev577398
 Summary: Squirrel public datasets collection
 Home-page: https://merantix-momentum.com/technology/squirrel/
 License: Apache 2.0
 Author: Merantix Momentum
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Provides-Extra: all
 Provides-Extra: deeplake
 Provides-Extra: hub
 Provides-Extra: huggingface
 Provides-Extra: preprocessing
 Provides-Extra: torchvision
```

