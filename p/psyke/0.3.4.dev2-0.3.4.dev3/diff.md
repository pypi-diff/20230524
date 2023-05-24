# Comparing `tmp/psyke-0.3.4.dev2.tar.gz` & `tmp/psyke-0.3.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.3.4.dev2.tar", last modified: Sat May 20 18:43:39 2023, max compression
+gzip compressed data, was "psyke-0.3.4.dev3.tar", last modified: Wed May 24 12:06:53 2023, max compression
```

## Comparing `psyke-0.3.4.dev2.tar` & `psyke-0.3.4.dev3.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 18:43:38.000000 psyke-0.3.4.dev2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.015039 psyke-0.3.4.dev2/psyke/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-20 18:43:32.000000 psyke-0.3.4.dev2/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/hypercubic/gridrex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/extraction/trepan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke/gui/controller/
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/controller/Controller.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/controller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.015039 psyke-0.3.4.dev2/psyke/gui/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.015039 psyke-0.3.4.dev2/psyke/gui/libs/garden/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.023039 psyke-0.3.4.dev2/psyke/gui/libs/garden/garden.matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-20 18:43:32.000000 psyke-0.3.4.dev2/psyke/gui/libs/garden/garden.matplotlib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 18:43:32.000000 psyke-0.3.4.dev2/psyke/gui/libs/garden/garden.matplotlib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-20 18:43:32.000000 psyke-0.3.4.dev2/psyke/gui/libs/garden/garden.matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50930 2023-05-20 18:43:32.000000 psyke-0.3.4.dev2/psyke/gui/libs/garden/garden.matplotlib/backend_kivy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-05-20 18:43:32.000000 psyke-0.3.4.dev2/psyke/gui/libs/garden/garden.matplotlib/backend_kivyagg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.023039 psyke-0.3.4.dev2/psyke/gui/model/
--rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/model/Model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.023039 psyke-0.3.4.dev2/psyke/gui/view/
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/view/DataPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/view/ExtractorPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/view/FeaturePanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/view/PlotPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/view/PredictorPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/view/TheoryPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/view/View.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/view/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/view/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/gui/view/style.kv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.023039 psyke-0.3.4.dev2/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.023039 psyke-0.3.4.dev2/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.023039 psyke-0.3.4.dev2/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.023039 psyke-0.3.4.dev2/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.023039 psyke-0.3.4.dev2/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.019039 psyke-0.3.4.dev2/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-20 18:43:38.000000 psyke-0.3.4.dev2/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-20 18:43:39.000000 psyke-0.3.4.dev2/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:43:38.000000 psyke-0.3.4.dev2/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:43:38.000000 psyke-0.3.4.dev2/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-20 18:43:38.000000 psyke-0.3.4.dev2/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 18:43:38.000000 psyke-0.3.4.dev2/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.015039 psyke-0.3.4.dev2/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.023039 psyke-0.3.4.dev2/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.023039 psyke-0.3.4.dev2/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-20 18:42:07.000000 psyke-0.3.4.dev2/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-20 18:42:11.000000 psyke-0.3.4.dev2/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 18:42:11.000000 psyke-0.3.4.dev2/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-20 18:42:11.000000 psyke-0.3.4.dev2/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:39.027039 psyke-0.3.4.dev2/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-20 18:42:11.000000 psyke-0.3.4.dev2/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.670873 psyke-0.3.4.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-24 12:06:53.670873 psyke-0.3.4.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 12:06:53.000000 psyke-0.3.4.dev3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.658873 psyke-0.3.4.dev3/psyke/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-24 12:06:46.000000 psyke-0.3.4.dev3/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/hypercubic/gridrex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/extraction/trepan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/gui/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/controller/Controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/controller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.658873 psyke-0.3.4.dev3/psyke/gui/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.658873 psyke-0.3.4.dev3/psyke/gui/libs/garden/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/gui/libs/garden/garden.matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-24 12:06:46.000000 psyke-0.3.4.dev3/psyke/gui/libs/garden/garden.matplotlib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 12:06:46.000000 psyke-0.3.4.dev3/psyke/gui/libs/garden/garden.matplotlib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-24 12:06:46.000000 psyke-0.3.4.dev3/psyke/gui/libs/garden/garden.matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50930 2023-05-24 12:06:46.000000 psyke-0.3.4.dev3/psyke/gui/libs/garden/garden.matplotlib/backend_kivy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-05-24 12:06:46.000000 psyke-0.3.4.dev3/psyke/gui/libs/garden/garden.matplotlib/backend_kivyagg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke/gui/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/model/Model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/psyke/gui/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/view/DataPanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/view/ExtractorPanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/view/FeaturePanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/view/PlotPanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/view/PredictorPanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/view/TheoryPanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/view/View.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/view/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/view/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/gui/view/style.kv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.662873 psyke-0.3.4.dev3/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-24 12:06:53.000000 psyke-0.3.4.dev3/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-24 12:06:53.000000 psyke-0.3.4.dev3/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:06:53.000000 psyke-0.3.4.dev3/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:06:53.000000 psyke-0.3.4.dev3/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 12:06:53.000000 psyke-0.3.4.dev3/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 12:06:53.000000 psyke-0.3.4.dev3/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:06:53.670873 psyke-0.3.4.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.658873 psyke-0.3.4.dev3/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.666873 psyke-0.3.4.dev3/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.670873 psyke-0.3.4.dev3/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.670873 psyke-0.3.4.dev3/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-24 12:05:26.000000 psyke-0.3.4.dev3/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.670873 psyke-0.3.4.dev3/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-24 12:05:30.000000 psyke-0.3.4.dev3/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.670873 psyke-0.3.4.dev3/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-24 12:05:30.000000 psyke-0.3.4.dev3/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.670873 psyke-0.3.4.dev3/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-24 12:05:30.000000 psyke-0.3.4.dev3/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:06:53.670873 psyke-0.3.4.dev3/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-24 12:05:30.000000 psyke-0.3.4.dev3/test/resources/tests/__init__.py
```

### Comparing `psyke-0.3.4.dev2/LICENSE` & `psyke-0.3.4.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/PKG-INFO` & `psyke-0.3.4.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.3.4.dev2
+Version: 0.3.4.dev3
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.3.4.dev2/README.md` & `psyke-0.3.4.dev3/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/__init__.py` & `psyke-0.3.4.dev3/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/clustering/__init__.py` & `psyke-0.3.4.dev3/psyke/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/clustering/cream/__init__.py` & `psyke-0.3.4.dev3/psyke/clustering/cream/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/clustering/exact/__init__.py` & `psyke-0.3.4.dev3/psyke/clustering/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/clustering/utils.py` & `psyke-0.3.4.dev3/psyke/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/cart/__init__.py` & `psyke-0.3.4.dev3/psyke/extraction/cart/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/cart/predictor.py` & `psyke-0.3.4.dev3/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/hypercubic/__init__.py` & `psyke-0.3.4.dev3/psyke/extraction/hypercubic/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.3.4.dev3/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.3.4.dev3/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.3.4.dev3/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.3.4.dev3/psyke/extraction/hypercubic/hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.3.4.dev3/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/hypercubic/strategy.py` & `psyke-0.3.4.dev3/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/hypercubic/utils.py` & `psyke-0.3.4.dev3/psyke/extraction/hypercubic/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/real/__init__.py` & `psyke-0.3.4.dev3/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/real/utils.py` & `psyke-0.3.4.dev3/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/trepan/__init__.py` & `psyke-0.3.4.dev3/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/extraction/trepan/utils.py` & `psyke-0.3.4.dev3/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/__init__.py` & `psyke-0.3.4.dev3/psyke/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/controller/Controller.py` & `psyke-0.3.4.dev3/psyke/gui/controller/Controller.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/libs/garden/garden.matplotlib/LICENSE` & `psyke-0.3.4.dev3/psyke/gui/libs/garden/garden.matplotlib/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/libs/garden/garden.matplotlib/__init__.py` & `psyke-0.3.4.dev3/psyke/gui/libs/garden/garden.matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/libs/garden/garden.matplotlib/backend_kivy.py` & `psyke-0.3.4.dev3/psyke/gui/libs/garden/garden.matplotlib/backend_kivy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/libs/garden/garden.matplotlib/backend_kivyagg.py` & `psyke-0.3.4.dev3/psyke/gui/libs/garden/garden.matplotlib/backend_kivyagg.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/model/Model.py` & `psyke-0.3.4.dev3/psyke/gui/model/Model.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/model/__init__.py` & `psyke-0.3.4.dev3/psyke/gui/model/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/view/DataPanel.py` & `psyke-0.3.4.dev3/psyke/gui/view/DataPanel.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/view/ExtractorPanel.py` & `psyke-0.3.4.dev3/psyke/gui/view/ExtractorPanel.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/view/FeaturePanel.py` & `psyke-0.3.4.dev3/psyke/gui/view/FeaturePanel.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/view/PlotPanel.py` & `psyke-0.3.4.dev3/psyke/gui/view/PlotPanel.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/view/PredictorPanel.py` & `psyke-0.3.4.dev3/psyke/gui/view/PredictorPanel.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/view/TheoryPanel.py` & `psyke-0.3.4.dev3/psyke/gui/view/TheoryPanel.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/view/View.py` & `psyke-0.3.4.dev3/psyke/gui/view/View.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/view/__init__.py` & `psyke-0.3.4.dev3/psyke/gui/view/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/view/layout.py` & `psyke-0.3.4.dev3/psyke/gui/view/layout.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/gui/view/plot.py` & `psyke-0.3.4.dev3/psyke/gui/view/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/schema/__init__.py` & `psyke-0.3.4.dev3/psyke/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/tuning/__init__.py` & `psyke-0.3.4.dev3/psyke/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/tuning/crash/__init__.py` & `psyke-0.3.4.dev3/psyke/tuning/crash/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/tuning/pedro/__init__.py` & `psyke-0.3.4.dev3/psyke/tuning/pedro/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/utils/__init__.py` & `psyke-0.3.4.dev3/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/utils/dataframe.py` & `psyke-0.3.4.dev3/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/utils/logic.py` & `psyke-0.3.4.dev3/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/utils/metrics.py` & `psyke-0.3.4.dev3/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/utils/plot.py` & `psyke-0.3.4.dev3/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke/utils/sorted.py` & `psyke-0.3.4.dev3/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/psyke.egg-info/PKG-INFO` & `psyke-0.3.4.dev3/psyke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.3.4.dev2
+Version: 0.3.4.dev3
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.3.4.dev2/psyke.egg-info/SOURCES.txt` & `psyke-0.3.4.dev3/psyke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/setup.py` & `psyke-0.3.4.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/__init__.py` & `psyke-0.3.4.dev3/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/extraction/cart/test_cart.py` & `psyke-0.3.4.dev3/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.3.4.dev3/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.3.4.dev3/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/extraction/real/test_real.py` & `psyke-0.3.4.dev3/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/extraction/real/test_rule.py` & `psyke-0.3.4.dev3/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/extraction/trepan/test_node.py` & `psyke-0.3.4.dev3/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/extraction/trepan/test_split.py` & `psyke-0.3.4.dev3/test/psyke/extraction/trepan/test_split.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.3.4.dev3/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/utils/test_prune.py` & `psyke-0.3.4.dev3/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/utils/test_simplify.py` & `psyke-0.3.4.dev3/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.3.4.dev3/test/psyke/utils/test_simplify_formatter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.4.dev2/test/resources/tests/__init__.py` & `psyke-0.3.4.dev3/test/resources/tests/__init__.py`

 * *Files identical despite different names*

