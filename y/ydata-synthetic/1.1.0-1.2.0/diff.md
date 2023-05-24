# Comparing `tmp/ydata-synthetic-1.1.0.tar.gz` & `tmp/ydata-synthetic-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydata-synthetic-1.1.0.tar", last modified: Mon Mar 27 07:39:01 2023, max compression
+gzip compressed data, was "ydata-synthetic-1.2.0.tar", last modified: Wed May 24 06:53:51 2023, max compression
```

## Comparing `ydata-synthetic-1.1.0.tar` & `ydata-synthetic-1.2.0.tar`

### file list

```diff
@@ -1,98 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-03-27 07:38:58.000000 ydata-synthetic-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-03-27 07:38:58.000000 ydata-synthetic-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8655 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6248 2023-03-27 07:38:58.000000 ydata-synthetic-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-27 07:39:01.000000 ydata-synthetic-1.1.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.679450 ydata-synthetic-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.679450 ydata-synthetic-1.1.0/src/ydata_synthetic/postprocessing/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/postprocessing/regular/
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5464 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/base_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/regular/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/regular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8210 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4519 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/regular/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/timeseries/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/timeseries/stock.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/timeseries/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/
--rw-r--r--   0 runner    (1001) docker     (122)     4196 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/About.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/
--rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2947 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/functions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/functions/generate.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/functions/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/run.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11134 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cgan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8357 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cgan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cramergan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cramergan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8733 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cramergan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/ctgan/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/ctgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14115 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/ctgan/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cwgangp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cwgangp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8916 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/dragan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/dragan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7839 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/dragan/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/vanillagan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/vanillagan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6693 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/wgan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/wgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8112 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/wgan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/wgangp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/wgangp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8389 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/wgangp/model.py
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/saving_keras.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/timeseries/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/timeseries/timegan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/timeseries/timegan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13785 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/tests/custom_layers/
--rw-r--r--   0 runner    (1001) docker     (122)     3315 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (122)     3368 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     4346 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/utils/gumbel_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.687450 ydata-synthetic-1.1.0/src/ydata_synthetic/utils/misc/
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-03-27 07:38:59.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/utils/misc/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-27 07:39:01.000000 ydata-synthetic-1.1.0/src/ydata_synthetic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:39:01.683450 ydata-synthetic-1.1.0/src/ydata_synthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8655 2023-03-27 07:39:01.000000 ydata-synthetic-1.1.0/src/ydata_synthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3294 2023-03-27 07:39:01.000000 ydata-synthetic-1.1.0/src/ydata_synthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-27 07:39:01.000000 ydata-synthetic-1.1.0/src/ydata_synthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-03-27 07:39:01.000000 ydata-synthetic-1.1.0/src/ydata_synthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-27 07:39:01.000000 ydata-synthetic-1.1.0/src/ydata_synthetic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9582 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7127 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-24 06:53:50.000000 ydata-synthetic-1.2.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.688075 ydata-synthetic-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.688075 ydata-synthetic-1.2.0/src/ydata_synthetic/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.688075 ydata-synthetic-1.2.0/src/ydata_synthetic/postprocessing/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/postprocessing/regular/
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5464 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/base_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8210 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4519 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/stock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/
+-rw-r--r--   0 runner    (1001) docker     (122)     4196 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/About.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/
+-rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2947 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/run.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cgan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8358 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cgan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cramergan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cramergan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8740 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cramergan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14122 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cwgangp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cwgangp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/dragan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/dragan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/dragan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/gmm/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/gmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3804 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/gmm/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/vanillagan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/vanillagan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8119 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgangp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgangp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8396 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgangp/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/saving_keras.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/timegan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/timegan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13792 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.688075 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/custom_layers/
+-rw-r--r--   0 runner    (1001) docker     (122)     3315 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)     3368 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4346 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/gumbel_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/misc/
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/misc/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.688075 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9582 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/top_level.txt
```

### Comparing `ydata-synthetic-1.1.0/LICENSE` & `ydata-synthetic-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/PKG-INFO` & `ydata-synthetic-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-synthetic
-Version: 1.1.0
+Version: 1.2.0
 Summary: Synthetic data generation methods with different synthetization methods.
 Home-page: https://github.com/ydataai/ydata-synthetic
 Author: YData
 Author-email: community@ydata.ai
 License: https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE
 Description: ![](https://img.shields.io/github/workflow/status/ydataai/ydata-synthetic/prerelease)
         ![](https://img.shields.io/pypi/status/ydata-synthetic)
@@ -16,33 +16,38 @@
         <p align="center"><img width="200" src="https://user-images.githubusercontent.com/3348134/177604157-11181f6c-57e5-44b1-8f6c-774edbba5512.png" alt="Synthetic Data Logo"></p>
         
         Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/mw7xjJ7b7s)
         
         # YData Synthetic
         A package to generate synthetic tabular and time-series data leveraging the state of the art generative models.
         
-        ## 🎊 We have **big news**: v1.0.0 is here
-        > We have exciting news for you. The new version of `ydata-synthetic` include new and exciting features:
+        ## 🎊 The exciting features:
+        > These are must try features when it comes to synthetic data generation:
+          > - A new streamlit app that delivers the synthetic data generation experience with a UI interface. A low code experience for the quick generation of synthetic data
+          > - A new fast synthetic data generation model based on Gaussian Mixture. So you can quickstart in the world of synthetic data generation without the need for a GPU.
           > - A conditional architecture for tabular data: CTGAN, which will make the process of synthetic data generation easier and with higher quality!
-          > - A new streamlit app that delivers the synthetic data generation experience with a UI interface
-        
+          
         ## Synthetic data
         ### What is synthetic data?
         Synthetic data is artificially generated data that is not collected from real world events. It replicates the statistical components of real data without containing any identifiable information, ensuring individuals' privacy.
         
         ### Why Synthetic Data?
         Synthetic data can be used for many applications:
-          - Privacy
+          - Privacy compliance for data-sharing and Machine Learning development
           - Remove bias
           - Balance datasets
           - Augment datasets
         
         # ydata-synthetic
-        This repository contains material related with Generative Adversarial Networks for synthetic data generation, in particular regular tabular data and time-series.
-        It consists a set of different GANs architectures developed using Tensorflow 2.0. Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
+        This repository contains material related with architectures and models for synthetic data, from Generative Adversarial Networks (GANs) to Gaussian Mixtures.
+        The repo includes a full ecosystem for synthetic data generation, that includes different models for the generation of synthetic structure data and time-series.
+        All the Deep Learning models are implemented leveraging Tensorflow 2.0.
+        Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
+        
+        Are you ready to learn more about synthetic data and the bext-practices for synthetic data generation?
         
         ## Quickstart
         The source code is currently hosted on GitHub at: https://github.com/ydataai/ydata-synthetic
         
         Binary installers for the latest released version are available at the [Python Package Index (PyPI).](https://pypi.org/project/ydata-synthetic/)
         ```commandline
         pip install ydata-synthetic
@@ -54,15 +59,15 @@
         The streamlit app is available form *v1.0.0* onwards, and supports the following flows:
         - Train a synthesizer model
         - Generate & profile synthetic data samples
         
         #### Installation
         
         ```commandline
-        pip install ydata-syntehtic[streamlit]
+        pip install ydata-synthetic[streamlit]
         ```
         #### Quickstart
         Use the code snippet below in a python file (Jupyter Notebooks are not supported):
         ```python
         from ydata_synthetic import streamlit_app
         
         streamlit_app.run()
@@ -82,15 +87,15 @@
           - CRAMER
           - CTGAN
         
         [![Watch the video](assets/streamlit_app.png)](https://youtu.be/ep0PhwsFx0A)
         
         ### Examples
         Here you can find usage examples of the package and models to synthesize tabular data.
-          
+          - Fast tabular data synthesis on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/Fast_Adult_Census_Income_Data.ipynb)
           - Tabular synthetic data generation with CTGAN on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/CTGAN_Adult_Census_Income_Data.ipynb)
           - Time Series synthetic data generation with TimeGAN on stock dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/timeseries/TimeGAN_Synthetic_stock_data.ipynb)
           - More examples are continuously added and can be found in `/examples` directory.
         
         ### Datasets for you to experiment
         Here are some example datasets for you to try with the synthesizers:
         #### Tabular datasets
@@ -110,14 +115,15 @@
           - [CGAN (Conditional GAN)](https://arxiv.org/abs/1411.1784)
           - [WGAN (Wasserstein GAN)](https://arxiv.org/abs/1701.07875)
           - [WGAN-GP (Wassertein GAN with Gradient Penalty)](https://arxiv.org/abs/1704.00028)
           - [DRAGAN (On Convergence and stability of GANS)](https://arxiv.org/pdf/1705.07215.pdf)
           - [Cramer GAN (The Cramer Distance as a Solution to Biased Wasserstein Gradients)](https://arxiv.org/abs/1705.10743)
           - [CWGAN-GP (Conditional Wassertein GAN with Gradient Penalty)](https://cameronfabbri.github.io/papers/conditionalWGAN.pdf)
           - [CTGAN (Conditional Tabular GAN)](https://arxiv.org/pdf/1907.00503.pdf)
+          - [Gaussian Mixture](https://towardsdatascience.com/gaussian-mixture-models-explained-6986aaf5a95)
         
         ### Sequential data
           - [TimeGAN](https://papers.nips.cc/paper/2019/file/c9efe5f26cd17ba6216bbe2a7d26d490-Paper.pdf)
         
         ## Contributing
         We are open to collaboration! If you want to start contributing you only need to:
           1. Search for an issue in which you would like to work. Issues for newcomers are labeled with good first issue.
```

### Comparing `ydata-synthetic-1.1.0/README.md` & `ydata-synthetic-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,33 +8,38 @@
 <p align="center"><img width="200" src="https://user-images.githubusercontent.com/3348134/177604157-11181f6c-57e5-44b1-8f6c-774edbba5512.png" alt="Synthetic Data Logo"></p>
 
 Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/mw7xjJ7b7s)
 
 # YData Synthetic
 A package to generate synthetic tabular and time-series data leveraging the state of the art generative models.
 
-## 🎊 We have **big news**: v1.0.0 is here
-> We have exciting news for you. The new version of `ydata-synthetic` include new and exciting features:
+## 🎊 The exciting features:
+> These are must try features when it comes to synthetic data generation:
+  > - A new streamlit app that delivers the synthetic data generation experience with a UI interface. A low code experience for the quick generation of synthetic data
+  > - A new fast synthetic data generation model based on Gaussian Mixture. So you can quickstart in the world of synthetic data generation without the need for a GPU.
   > - A conditional architecture for tabular data: CTGAN, which will make the process of synthetic data generation easier and with higher quality!
-  > - A new streamlit app that delivers the synthetic data generation experience with a UI interface
-
+  
 ## Synthetic data
 ### What is synthetic data?
 Synthetic data is artificially generated data that is not collected from real world events. It replicates the statistical components of real data without containing any identifiable information, ensuring individuals' privacy.
 
 ### Why Synthetic Data?
 Synthetic data can be used for many applications:
-  - Privacy
+  - Privacy compliance for data-sharing and Machine Learning development
   - Remove bias
   - Balance datasets
   - Augment datasets
 
 # ydata-synthetic
-This repository contains material related with Generative Adversarial Networks for synthetic data generation, in particular regular tabular data and time-series.
-It consists a set of different GANs architectures developed using Tensorflow 2.0. Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
+This repository contains material related with architectures and models for synthetic data, from Generative Adversarial Networks (GANs) to Gaussian Mixtures.
+The repo includes a full ecosystem for synthetic data generation, that includes different models for the generation of synthetic structure data and time-series.
+All the Deep Learning models are implemented leveraging Tensorflow 2.0.
+Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
+
+Are you ready to learn more about synthetic data and the bext-practices for synthetic data generation?
 
 ## Quickstart
 The source code is currently hosted on GitHub at: https://github.com/ydataai/ydata-synthetic
 
 Binary installers for the latest released version are available at the [Python Package Index (PyPI).](https://pypi.org/project/ydata-synthetic/)
 ```commandline
 pip install ydata-synthetic
@@ -46,15 +51,15 @@
 The streamlit app is available form *v1.0.0* onwards, and supports the following flows:
 - Train a synthesizer model
 - Generate & profile synthetic data samples
 
 #### Installation
 
 ```commandline
-pip install ydata-syntehtic[streamlit]
+pip install ydata-synthetic[streamlit]
 ```
 #### Quickstart
 Use the code snippet below in a python file (Jupyter Notebooks are not supported):
 ```python
 from ydata_synthetic import streamlit_app
 
 streamlit_app.run()
@@ -74,15 +79,15 @@
   - CRAMER
   - CTGAN
 
 [![Watch the video](assets/streamlit_app.png)](https://youtu.be/ep0PhwsFx0A)
 
 ### Examples
 Here you can find usage examples of the package and models to synthesize tabular data.
-  
+  - Fast tabular data synthesis on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/Fast_Adult_Census_Income_Data.ipynb)
   - Tabular synthetic data generation with CTGAN on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/CTGAN_Adult_Census_Income_Data.ipynb)
   - Time Series synthetic data generation with TimeGAN on stock dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/timeseries/TimeGAN_Synthetic_stock_data.ipynb)
   - More examples are continuously added and can be found in `/examples` directory.
 
 ### Datasets for you to experiment
 Here are some example datasets for you to try with the synthesizers:
 #### Tabular datasets
@@ -102,14 +107,15 @@
   - [CGAN (Conditional GAN)](https://arxiv.org/abs/1411.1784)
   - [WGAN (Wasserstein GAN)](https://arxiv.org/abs/1701.07875)
   - [WGAN-GP (Wassertein GAN with Gradient Penalty)](https://arxiv.org/abs/1704.00028)
   - [DRAGAN (On Convergence and stability of GANS)](https://arxiv.org/pdf/1705.07215.pdf)
   - [Cramer GAN (The Cramer Distance as a Solution to Biased Wasserstein Gradients)](https://arxiv.org/abs/1705.10743)
   - [CWGAN-GP (Conditional Wassertein GAN with Gradient Penalty)](https://cameronfabbri.github.io/papers/conditionalWGAN.pdf)
   - [CTGAN (Conditional Tabular GAN)](https://arxiv.org/pdf/1907.00503.pdf)
+  - [Gaussian Mixture](https://towardsdatascience.com/gaussian-mixture-models-explained-6986aaf5a95)
 
 ### Sequential data
   - [TimeGAN](https://papers.nips.cc/paper/2019/file/c9efe5f26cd17ba6216bbe2a7d26d490-Paper.pdf)
 
 ## Contributing
 We are open to collaboration! If you want to start contributing you only need to:
   1. Search for an issue in which you would like to work. Issues for newcomers are labeled with good first issue.
```

### Comparing `ydata-synthetic-1.1.0/setup.py` & `ydata-synthetic-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/base_processor.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/base_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/regular/processor.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/timeseries/stock.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/stock.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/preprocessing/timeseries/utils.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/About.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/About.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/functions/generate.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/generate.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/streamlit_app/pages/functions/train.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/train.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/gan.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 "Implements a GAN BaseModel synthesizer, not meant to be directly instantiated."
+from abc import ABC, abstractmethod
 from collections import namedtuple
 from typing import List, Optional, Union
 
+import pandas as pd
 import tqdm
 
 from numpy import array, vstack, ndarray
 from numpy.random import normal
 from pandas.api.types import is_float_dtype, is_integer_dtype
 from pandas import DataFrame
 from pandas import concat
@@ -36,27 +38,65 @@
 
 _train_parameters = ['cache_prefix', 'label_dim', 'epochs', 'sample_interval', 
                      'labels', 'n_clusters', 'epsilon', 'log_frequency']
 
 ModelParameters = namedtuple('ModelParameters', _model_parameters, defaults=_model_parameters_df)
 TrainParameters = namedtuple('TrainParameters', _train_parameters, defaults=('', None, 300, 50, None, 10, 0.005, True))
 
+@typechecked
+class BaseModel(ABC):
+    """
+    Abstract class for synthetic data generation nmodels
+
+    The main methods are train (for fitting the synthesizer), save/load and sample (generating synthetic records).
+
+    """
+    __MODEL__ = None
+
+    @abstractmethod
+    def fit(self, data: Union[DataFrame, array],
+                  num_cols: Optional[List[str]] = None,
+                  cat_cols: Optional[List[str]] = None):
+        """
+        ### Description:
+        Trains and fit a synthesizer model to a given input dataset.
+
+        ### Args:
+        `data` (Union[DataFrame, array]): Training data
+        `num_cols` (Optional[List[str]]) : List with the names of the categorical columns
+        `cat_cols` (Optional[List[str]]): List of names of categorical columns
+
+        ### Returns:
+        **self:** *object*
+            Fitted synthesizer
+        """
+        ...
+    @abstractmethod
+    def sample(self, n_samples:int) -> pd.DataFrame:
+        assert n_samples>0, "Please insert a value bigger than 0 for n_samples parameter."
+        ...
+
+    @classmethod
+    def load(cls, path: str):
+        ...
+
+    @abstractmethod
+    def save(self, path: str):
+        ...
 
 # pylint: disable=R0902
 @typechecked
-class BaseModel():
+class BaseGANModel(BaseModel):
     """
     Base class of GAN synthesizer models.
     The main methods are train (for fitting the synthesizer), save/load and sample (obtain synthetic records).
     Args:
         model_parameters (ModelParameters):
             Set of architectural parameters for model definition.
     """
-    __MODEL__ = None
-
     def __init__(
             self,
             model_parameters: ModelParameters
     ):
         gpu_devices = tfconfig.list_physical_devices('GPU')
         if len(gpu_devices) > 0:
             try:
@@ -80,15 +120,15 @@
         self.generator_dims = model_parameters.generator_dims
         self.critic_dims = model_parameters.critic_dims
         self.l2_scale = model_parameters.l2_scale
         self.latent_dim = model_parameters.latent_dim
         self.gp_lambda = model_parameters.gp_lambda
         self.pac = model_parameters.pac
 
-        self.processor = None
+        self.processor=None
         if self.__MODEL__ in RegularModels.__members__ or \
             self.__MODEL__ == CTGANDataProcessor.SUPPORTED_MODEL:
             self.tau = model_parameters.tau_gs
 
     # pylint: disable=E1101
     def __call__(self, inputs, **kwargs):
         return self.model(inputs=inputs, **kwargs)
@@ -179,16 +219,16 @@
         """
         #Save only the generator?
         if self.__MODEL__=='WGAN' or self.__MODEL__=='WGAN_GP' or self.__MODEL__=='CWGAN_GP':
             del self.critic
         make_keras_picklable()
         dump(self, path)
 
-    @staticmethod
-    def load(path):
+    @classmethod
+    def load(cls, path):
         """
         ### Description:
         Loads a saved synthesizer from a pickle.
 
         ### Args:
         `path` (str): Path to read the synthesizer pickle from.
         """
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/loss.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/loss.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cgan/model.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cgan/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from tensorflow import dtypes
 from keras import Model
 from keras.layers import (Dense, Dropout, Input, concatenate)
 from keras.optimizers import Adam
 
 #Import ydata synthetic classes
 from ....synthesizers import TrainParameters
-from ....synthesizers.gan import ConditionalModel
+from ....synthesizers.base import ConditionalModel
 
 class CGAN(ConditionalModel):
     "CGAN model for discrete conditions"
 
     __MODEL__='CGAN'
 
     def __init__(self, model_parameters):
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cramergan/model.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cramergan/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from keras import  Model
 from keras.layers import (Dense, Dropout, Input)
 from keras.optimizers import Adam
 from tqdm import trange
 
 #Import ydata synthetic classes
 from ....synthesizers import TrainParameters
-from ....synthesizers.gan import BaseModel
+from ....synthesizers.base import BaseGANModel
 from ....synthesizers.loss import Mode, gradient_penalty
 
-class CRAMERGAN(BaseModel):
+class CRAMERGAN(BaseGANModel):
 
     __MODEL__='CRAMERGAN'
 
     def __init__(self, model_parameters, gradient_penalty_weight=10):
         """Create a base CramerGAN.
 
         Based according to the WGAN paper - https://arxiv.org/pdf/1705.10743.pdf
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/ctgan/model.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from keras import Model
 
 import tensorflow_probability as tfp
 from ydata_synthetic.synthesizers.regular.ctgan.utils \
     import ConditionalLoss, RealDataSampler, ConditionalSampler
  
 from ydata_synthetic.synthesizers.loss import gradient_penalty, Mode as ModeGP
-from ydata_synthetic.synthesizers.gan import BaseModel, ModelParameters, TrainParameters
+from ydata_synthetic.synthesizers.base import BaseGANModel, ModelParameters, TrainParameters
 from ydata_synthetic.preprocessing.regular.ctgan_processor import CTGANDataProcessor
 
-class CTGAN(BaseModel):
+class CTGAN(BaseGANModel):
     """
     Conditional Tabular GAN model.
     Based on the paper https://arxiv.org/abs/1907.00503.
 
     Args:
         model_parameters: Parameters used to create the CTGAN model.
     """
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from tensorflow import dtypes, GradientTape, reduce_sum, reduce_mean, sqrt, random
 from keras import Model
 from keras.layers import (Dense, Dropout, Input, concatenate, LeakyReLU)
 from keras.optimizers import Adam
 
 #Import ydata synthetic classes
 from ....synthesizers import TrainParameters
-from ....synthesizers.gan import ConditionalModel
+from ....synthesizers.base import ConditionalModel
 from ....synthesizers.regular.wgangp.model import WGAN_GP
 
 class CWGANGP(ConditionalModel, WGAN_GP):
 
     __MODEL__='CWGAN_GP'
 
     def __init__(self, model_parameters,
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/dragan/model.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/dragan/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 import tensorflow as tf
 import tqdm
 from keras import Model, initializers
 from keras.layers import Dense, Dropout, Input
 from keras.optimizers import Adam
 
 #Import ydata synthetic classes
-from ....synthesizers.gan import BaseModel
+from ....synthesizers.base import BaseGANModel
 from ....synthesizers.loss import Mode, gradient_penalty
 
-class DRAGAN(BaseModel):
+class DRAGAN(BaseGANModel):
 
     __MODEL__='DRAGAN'
 
     def __init__(self, model_parameters, n_discriminator, gradient_penalty_weight=10):
         # As recommended in DRAGAN paper - https://arxiv.org/abs/1705.07215
         self.n_discriminator = n_discriminator
         self.gradient_penalty_weight = gradient_penalty_weight
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/model.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,46 +11,54 @@
 from ydata_synthetic.synthesizers.regular.cgan.model import CGAN
 from ydata_synthetic.synthesizers.regular.wgan.model import WGAN
 from ydata_synthetic.synthesizers.regular.wgangp.model import WGAN_GP
 from ydata_synthetic.synthesizers.regular.cwgangp.model import CWGANGP
 from ydata_synthetic.synthesizers.regular.cramergan.model import CRAMERGAN
 from ydata_synthetic.synthesizers.regular.dragan.model import DRAGAN
 from ydata_synthetic.synthesizers.regular.ctgan.model import CTGAN
+from ydata_synthetic.synthesizers.regular.gmm.model import GMM
 
 
 @unique
 class Model(Enum):
     VANILLA = 'gan'
     CONDITIONAL = 'cgan'
     WASSERTEIN =  'wgan'
     WASSERTEINGP ='wgangp'
     CWASSERTEINGP = 'cwgangp'
     CRAMER = 'cramer'
     DEEPREGRET = 'dragan'
     CONDITIONALTABULAR = 'ctgan'
+    FAST = 'fast'
 
     __MAPPING__ = {
         VANILLA : VanilllaGAN,
         CONDITIONAL: CGAN,
         WASSERTEIN: WGAN,
         WASSERTEINGP: WGAN_GP,
         CWASSERTEINGP: CWGANGP,
         CRAMER: CRAMERGAN,
         DEEPREGRET: DRAGAN,
-        CONDITIONALTABULAR: CTGAN
+        CONDITIONALTABULAR: CTGAN,
+        FAST: GMM
     }
 
     @property
     def function(self):
         return self.__MAPPING__[self.value]
 
 class RegularSynthesizer():
     "Abstraction class "
-    def __new__(cls, modelname: str, model_parameters, **kwargs):
-        return Model(modelname).function(model_parameters, **kwargs)
+    def __new__(cls, modelname: str, model_parameters =None, **kwargs):
+        model = None
+        if Model(modelname) == Model.FAST:
+            model=Model(modelname).function(**kwargs)
+        else:
+            model=Model(modelname).function(model_parameters, **kwargs)
+        return model
 
     @staticmethod
     def load(path):
         """
         ### Description:
         Loads a saved synthesizer from a pickle.
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 
 import tensorflow as tf
 from keras.layers import Input, Dense, Dropout
 from keras import Model
 from keras.optimizers import Adam
 
 #Import ydata synthetic classes
-from ....synthesizers.gan import BaseModel
+from ....synthesizers.base import BaseGANModel
 from ....synthesizers import TrainParameters
-from ....utils.gumbel_softmax import GumbelSoftmaxActivation
 
-class VanilllaGAN(BaseModel):
+class VanilllaGAN(BaseGANModel):
 
     __MODEL__='GAN'
 
     def __init__(self, model_parameters):
         super().__init__(model_parameters)
 
     def define_gan(self, activation_info: Optional[NamedTuple]):
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/wgan/model.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgan/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import keras.backend as K
 from keras import Model
 from keras.layers import Dense, Dropout, Input
 from keras.optimizers import Adam
 
 #Import ydata synthetic classes
 from ....synthesizers import TrainParameters
-from ....synthesizers.gan import BaseModel
+from ....synthesizers.base import BaseGANModel
 
 #Auxiliary Keras backend class to calculate the Random Weighted average
 #https://stackoverflow.com/questions/58133430/how-to-substitute-keras-layers-merge-merge-in-tensorflow-keras
 class RandomWeightedAverage(tf.keras.layers.Layer):
     def __init__(self, batch_size):
         super().__init__()
         self.batch_size = batch_size
@@ -29,15 +29,15 @@
     def call(self, inputs, **kwargs):
         alpha = tf.random_uniform((self.batch_size, 1, 1, 1))
         return (alpha * inputs[0]) + ((1 - alpha) * inputs[1])
 
     def compute_output_shape(self, input_shape):
         return input_shape[0]
 
-class WGAN(BaseModel):
+class WGAN(BaseGANModel):
 
     __MODEL__='WGAN'
 
     def __init__(self, model_parameters, n_critic, clip_value=0.01):
         # As recommended in WGAN paper - https://arxiv.org/abs/1701.07875
         # WGAN-GP - WGAN with Gradient Penalty
         self.n_critic = n_critic
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/regular/wgangp/model.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgangp/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import tensorflow as tf
 from keras import Model
 from keras.layers import Dense, Dropout, Input
 from keras.optimizers import Adam
 
 #Import ydata synthetic classes
 from ....synthesizers import TrainParameters
-from ....synthesizers.gan import BaseModel
+from ....synthesizers.base import BaseGANModel
 
-class WGAN_GP(BaseModel):
+class WGAN_GP(BaseGANModel):
 
     __MODEL__='WGAN_GP'
 
     def __init__(self, model_parameters, n_generator:int=1, n_critic:int=1, gradient_penalty_weight:int=10):
         # As recommended in WGAN paper - https://arxiv.org/abs/1701.07875
         # WGAN-GP - WGAN with Gradient Penalty
         self.n_critic = n_critic
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/saving_keras.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/saving_keras.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from tensorflow import data as tfdata
 from tensorflow import nn
 from keras import (Model, Sequential, Input)
 from keras.layers import (GRU, LSTM, Dense)
 from keras.optimizers import Adam
 from keras.losses import (BinaryCrossentropy, MeanSquaredError)
 
-from ....synthesizers.gan import BaseModel
+from ....synthesizers.base import BaseGANModel
 
 def make_net(model, n_layers, hidden_units, output_units, net_type='GRU'):
     if net_type=='GRU':
         for i in range(n_layers):
             model.add(GRU(units=hidden_units,
                       return_sequences=True,
                       name=f'GRU_{i + 1}'))
@@ -29,15 +29,15 @@
 
     model.add(Dense(units=output_units,
                     activation='sigmoid',
                     name='OUT'))
     return model
 
 
-class TimeGAN(BaseModel):
+class TimeGAN(BaseGANModel):
 
     __MODEL__='TimeGAN'
 
     def __init__(self, model_parameters, hidden_dim, seq_len, n_seq, gamma):
         self.seq_len=seq_len
         self.n_seq=n_seq
         self.hidden_dim=hidden_dim
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/utils/cache.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/utils/gumbel_softmax.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/utils/gumbel_softmax.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic/utils/misc/colormaps.py` & `ydata-synthetic-1.2.0/src/ydata_synthetic/utils/misc/colormaps.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic.egg-info/PKG-INFO` & `ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-synthetic
-Version: 1.1.0
+Version: 1.2.0
 Summary: Synthetic data generation methods with different synthetization methods.
 Home-page: https://github.com/ydataai/ydata-synthetic
 Author: YData
 Author-email: community@ydata.ai
 License: https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE
 Description: ![](https://img.shields.io/github/workflow/status/ydataai/ydata-synthetic/prerelease)
         ![](https://img.shields.io/pypi/status/ydata-synthetic)
@@ -16,33 +16,38 @@
         <p align="center"><img width="200" src="https://user-images.githubusercontent.com/3348134/177604157-11181f6c-57e5-44b1-8f6c-774edbba5512.png" alt="Synthetic Data Logo"></p>
         
         Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/mw7xjJ7b7s)
         
         # YData Synthetic
         A package to generate synthetic tabular and time-series data leveraging the state of the art generative models.
         
-        ## 🎊 We have **big news**: v1.0.0 is here
-        > We have exciting news for you. The new version of `ydata-synthetic` include new and exciting features:
+        ## 🎊 The exciting features:
+        > These are must try features when it comes to synthetic data generation:
+          > - A new streamlit app that delivers the synthetic data generation experience with a UI interface. A low code experience for the quick generation of synthetic data
+          > - A new fast synthetic data generation model based on Gaussian Mixture. So you can quickstart in the world of synthetic data generation without the need for a GPU.
           > - A conditional architecture for tabular data: CTGAN, which will make the process of synthetic data generation easier and with higher quality!
-          > - A new streamlit app that delivers the synthetic data generation experience with a UI interface
-        
+          
         ## Synthetic data
         ### What is synthetic data?
         Synthetic data is artificially generated data that is not collected from real world events. It replicates the statistical components of real data without containing any identifiable information, ensuring individuals' privacy.
         
         ### Why Synthetic Data?
         Synthetic data can be used for many applications:
-          - Privacy
+          - Privacy compliance for data-sharing and Machine Learning development
           - Remove bias
           - Balance datasets
           - Augment datasets
         
         # ydata-synthetic
-        This repository contains material related with Generative Adversarial Networks for synthetic data generation, in particular regular tabular data and time-series.
-        It consists a set of different GANs architectures developed using Tensorflow 2.0. Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
+        This repository contains material related with architectures and models for synthetic data, from Generative Adversarial Networks (GANs) to Gaussian Mixtures.
+        The repo includes a full ecosystem for synthetic data generation, that includes different models for the generation of synthetic structure data and time-series.
+        All the Deep Learning models are implemented leveraging Tensorflow 2.0.
+        Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
+        
+        Are you ready to learn more about synthetic data and the bext-practices for synthetic data generation?
         
         ## Quickstart
         The source code is currently hosted on GitHub at: https://github.com/ydataai/ydata-synthetic
         
         Binary installers for the latest released version are available at the [Python Package Index (PyPI).](https://pypi.org/project/ydata-synthetic/)
         ```commandline
         pip install ydata-synthetic
@@ -54,15 +59,15 @@
         The streamlit app is available form *v1.0.0* onwards, and supports the following flows:
         - Train a synthesizer model
         - Generate & profile synthetic data samples
         
         #### Installation
         
         ```commandline
-        pip install ydata-syntehtic[streamlit]
+        pip install ydata-synthetic[streamlit]
         ```
         #### Quickstart
         Use the code snippet below in a python file (Jupyter Notebooks are not supported):
         ```python
         from ydata_synthetic import streamlit_app
         
         streamlit_app.run()
@@ -82,15 +87,15 @@
           - CRAMER
           - CTGAN
         
         [![Watch the video](assets/streamlit_app.png)](https://youtu.be/ep0PhwsFx0A)
         
         ### Examples
         Here you can find usage examples of the package and models to synthesize tabular data.
-          
+          - Fast tabular data synthesis on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/Fast_Adult_Census_Income_Data.ipynb)
           - Tabular synthetic data generation with CTGAN on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/CTGAN_Adult_Census_Income_Data.ipynb)
           - Time Series synthetic data generation with TimeGAN on stock dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/timeseries/TimeGAN_Synthetic_stock_data.ipynb)
           - More examples are continuously added and can be found in `/examples` directory.
         
         ### Datasets for you to experiment
         Here are some example datasets for you to try with the synthesizers:
         #### Tabular datasets
@@ -110,14 +115,15 @@
           - [CGAN (Conditional GAN)](https://arxiv.org/abs/1411.1784)
           - [WGAN (Wasserstein GAN)](https://arxiv.org/abs/1701.07875)
           - [WGAN-GP (Wassertein GAN with Gradient Penalty)](https://arxiv.org/abs/1704.00028)
           - [DRAGAN (On Convergence and stability of GANS)](https://arxiv.org/pdf/1705.07215.pdf)
           - [Cramer GAN (The Cramer Distance as a Solution to Biased Wasserstein Gradients)](https://arxiv.org/abs/1705.10743)
           - [CWGAN-GP (Conditional Wassertein GAN with Gradient Penalty)](https://cameronfabbri.github.io/papers/conditionalWGAN.pdf)
           - [CTGAN (Conditional Tabular GAN)](https://arxiv.org/pdf/1907.00503.pdf)
+          - [Gaussian Mixture](https://towardsdatascience.com/gaussian-mixture-models-explained-6986aaf5a95)
         
         ### Sequential data
           - [TimeGAN](https://papers.nips.cc/paper/2019/file/c9efe5f26cd17ba6216bbe2a7d26d490-Paper.pdf)
         
         ## Contributing
         We are open to collaboration! If you want to start contributing you only need to:
           1. Search for an issue in which you would like to work. Issues for newcomers are labeled with good first issue.
```

### Comparing `ydata-synthetic-1.1.0/src/ydata_synthetic.egg-info/SOURCES.txt` & `ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py
 src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py
 src/ydata_synthetic/streamlit_app/pages/functions/__init__.py
 src/ydata_synthetic/streamlit_app/pages/functions/generate.py
 src/ydata_synthetic/streamlit_app/pages/functions/load_data.py
 src/ydata_synthetic/streamlit_app/pages/functions/train.py
 src/ydata_synthetic/synthesizers/__init__.py
-src/ydata_synthetic/synthesizers/gan.py
+src/ydata_synthetic/synthesizers/base.py
 src/ydata_synthetic/synthesizers/loss.py
 src/ydata_synthetic/synthesizers/saving_keras.py
 src/ydata_synthetic/synthesizers/regular/__init__.py
 src/ydata_synthetic/synthesizers/regular/model.py
 src/ydata_synthetic/synthesizers/regular/cgan/__init__.py
 src/ydata_synthetic/synthesizers/regular/cgan/model.py
 src/ydata_synthetic/synthesizers/regular/cramergan/__init__.py
@@ -44,14 +44,16 @@
 src/ydata_synthetic/synthesizers/regular/ctgan/__init__.py
 src/ydata_synthetic/synthesizers/regular/ctgan/model.py
 src/ydata_synthetic/synthesizers/regular/ctgan/utils.py
 src/ydata_synthetic/synthesizers/regular/cwgangp/__init__.py
 src/ydata_synthetic/synthesizers/regular/cwgangp/model.py
 src/ydata_synthetic/synthesizers/regular/dragan/__init__.py
 src/ydata_synthetic/synthesizers/regular/dragan/model.py
+src/ydata_synthetic/synthesizers/regular/gmm/__init__.py
+src/ydata_synthetic/synthesizers/regular/gmm/model.py
 src/ydata_synthetic/synthesizers/regular/vanillagan/__init__.py
 src/ydata_synthetic/synthesizers/regular/vanillagan/model.py
 src/ydata_synthetic/synthesizers/regular/wgan/__init__.py
 src/ydata_synthetic/synthesizers/regular/wgan/model.py
 src/ydata_synthetic/synthesizers/regular/wgangp/__init__.py
 src/ydata_synthetic/synthesizers/regular/wgangp/model.py
 src/ydata_synthetic/synthesizers/timeseries/__init__.py
```

