# Comparing `tmp/ragraph-1.17.1.tar.gz` & `tmp/ragraph-1.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragraph-1.17.1.tar", max compression
+gzip compressed data, was "ragraph-1.18.0.tar", max compression
```

## Comparing `ragraph-1.17.1.tar` & `ragraph-1.18.0.tar`

### file list

```diff
@@ -1,135 +1,136 @@
--rw-r--r--   0        0        0    35400 2023-05-02 10:06:24.073175 ragraph-1.17.1/LICENSE.rst
--rw-r--r--   0        0        0     1781 2023-05-02 10:06:24.073175 ragraph-1.17.1/README.rst
--rw-r--r--   0        0        0     2357 2023-05-02 10:06:24.076176 ragraph-1.17.1/pyproject.toml
--rw-r--r--   0        0        0       72 2023-05-02 10:06:24.076176 ragraph-1.17.1/ragraph/__init__.py
--rw-r--r--   0        0        0      100 2023-05-02 10:06:24.076176 ragraph-1.17.1/ragraph/analysis/__init__.py
--rw-r--r--   0        0        0    19876 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/_classes.py
--rw-r--r--   0        0        0     7901 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/_utils.py
--rw-r--r--   0        0        0     1142 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/bus/__init__.py
--rw-r--r--   0        0        0     3743 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/bus/_gamma.py
--rw-r--r--   0        0        0     1613 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/cluster/__init__.py
--rw-r--r--   0        0        0    13777 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/cluster/_markov.py
--rw-r--r--   0        0        0     3438 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/cluster/_tarjan.py
--rw-r--r--   0        0        0      503 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/comparison/__init__.py
--rw-r--r--   0        0        0     5548 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/comparison/_delta.py
--rw-r--r--   0        0        0     4722 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/comparison/_sigma.py
--rw-r--r--   0        0        0     1706 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/comparison/utils.py
--rw-r--r--   0        0        0    19484 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/compatibility/__init__.py
--rw-r--r--   0        0        0     2729 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/compatibility/bdd.py
--rw-r--r--   0        0        0     1227 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/heuristics/__init__.py
--rw-r--r--   0        0        0     3368 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/heuristics/_johnson.py
--rw-r--r--   0        0        0     5157 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/heuristics/_markov_gamma.py
--rw-r--r--   0        0        0     1787 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/__init__.py
--rw-r--r--   0        0        0    10956 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_axis.py
--rw-r--r--   0        0        0     5226 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_genetic.py
--rw-r--r--   0        0        0     3010 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_markov.py
--rw-r--r--   0        0        0      840 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_name.py
--rw-r--r--   0        0        0     3750 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_scc_tearing.py
--rw-r--r--   0        0        0     1713 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_tarjan.py
--rw-r--r--   0        0        0     7133 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/metrics.py
--rw-r--r--   0        0        0     5256 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/utils.py
--rw-r--r--   0        0        0     1336 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/analysis/similarity/__init__.py
--rw-r--r--   0        0        0     3036 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/analysis/similarity/_jaccard.py
--rw-r--r--   0        0        0     9582 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/analysis/similarity/_similarity.py
--rw-r--r--   0        0        0     1824 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/analysis/similarity/utils.py
--rw-r--r--   0        0        0     9963 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/colors/__init__.py
--rw-r--r--   0        0        0     5320 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/colors/cubehelix.py
--rw-r--r--   0        0        0      774 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/colors/utils.py
--rw-r--r--   0        0        0     1663 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/datasets/__init__.py
--rw-r--r--   0        0        0      673 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/datasets/aircraft_engine/__init__.py
--rw-r--r--   0        0        0    28938 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv
--rw-r--r--   0        0        0      977 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv
--rw-r--r--   0        0        0     1035 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/datasets/architecture_integral/__init__.py
--rw-r--r--   0        0        0     1364 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_integral/architecture_integral_edges.csv
--rw-r--r--   0        0        0      352 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_integral/architecture_integral_nodes.csv
--rw-r--r--   0        0        0     1048 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_mix/__init__.py
--rw-r--r--   0        0        0     2264 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_mix/architecture_mix_edges.csv
--rw-r--r--   0        0        0      352 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_mix/architecture_mix_nodes.csv
--rw-r--r--   0        0        0     1043 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_modular/__init__.py
--rw-r--r--   0        0        0     2722 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_modular/architecture_modular_edges.csv
--rw-r--r--   0        0        0      351 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_modular/architecture_modular_nodes.csv
--rw-r--r--   0        0        0      813 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control/__init__.py
--rw-r--r--   0        0        0     5778 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control/climate_control_edges.csv
--rw-r--r--   0        0        0      632 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control/climate_control_nodes.csv
--rw-r--r--   0        0        0      374 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control_mg/__init__.py
--rw-r--r--   0        0        0     5778 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv
--rw-r--r--   0        0        0     1441 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv
--rw-r--r--   0        0        0      460 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/compatibility/__init__.py
--rw-r--r--   0        0        0      564 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/compatibility/compatibility_edges.csv
--rw-r--r--   0        0        0       83 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/compatibility/compatibility_nodes.csv
--rw-r--r--   0        0        0      431 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/design/__init__.py
--rw-r--r--   0        0        0      872 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/design/design_edges.csv
--rw-r--r--   0        0        0      384 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/design/design_nodes.csv
--rw-r--r--   0        0        0       57 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/eefde_lock/__init__.py
--rw-r--r--   0        0        0    24347 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/eefde_lock/eefde_lock_edges.csv
--rw-r--r--   0        0        0     1047 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/eefde_lock/eefde_lock_nodes.csv
--rw-r--r--   0        0        0      998 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator175/__init__.py
--rw-r--r--   0        0        0   103961 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator175/elevator175_edges.csv
--rw-r--r--   0        0        0     7255 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator175/elevator175_nodes.csv
--rw-r--r--   0        0        0      995 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator45/__init__.py
--rw-r--r--   0        0        0    29033 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator45/elevator45_edges.csv
--rw-r--r--   0        0        0     1887 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator45/elevator45_nodes.csv
--rw-r--r--   0        0        0     1148 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/esl/__init__.py
--rw-r--r--   0        0        0       75 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/esl/pump/__init__.py
--rw-r--r--   0        0        0     3523 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/esl/pump/pump.esl
--rw-r--r--   0        0        0     1868 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/ford_hood/__init__.py
--rw-r--r--   0        0        0    30483 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/ford_hood/ford_hood_edges.csv
--rw-r--r--   0        0        0     3339 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/ford_hood/ford_hood_nodes.csv
--rw-r--r--   0        0        0     1461 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/kodak3d/__init__.py
--rw-r--r--   0        0        0     6660 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/kodak3d/kodak3d_edges.csv
--rw-r--r--   0        0        0     1134 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/kodak3d/kodak3d_nodes.csv
--rw-r--r--   0        0        0      216 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/ledsip/__init__.py
--rw-r--r--   0        0        0   210027 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/ledsip/ledsip_edges.csv
--rw-r--r--   0        0        0    50840 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/ledsip/ledsip_nodes.csv
--rw-r--r--   0        0        0       74 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/localbus/__init__.py
--rw-r--r--   0        0        0      723 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/localbus/localbus_edges.csv
--rw-r--r--   0        0        0       27 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/localbus/localbus_nodes.csv
--rw-r--r--   0        0        0       76 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/overlap/__init__.py
--rw-r--r--   0        0        0      149 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/overlap/overlap_edges.csv
--rw-r--r--   0        0        0       15 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/overlap/overlap_nodes.csv
--rw-r--r--   0        0        0     3167 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/pathfinder/__init__.py
--rw-r--r--   0        0        0    17741 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/pathfinder/pathfinder_edges.csv
--rw-r--r--   0        0        0     1084 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/pathfinder/pathfinder_nodes.csv
--rw-r--r--   0        0        0      307 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/shaja8/__init__.py
--rw-r--r--   0        0        0      243 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/shaja8/shaja8_edges.csv
--rw-r--r--   0        0        0       21 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/shaja8/shaja8_nodes.csv
--rw-r--r--   0        0        0      224 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/similarity/__init__.py
--rw-r--r--   0        0        0      872 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/similarity/similarity_edges.csv
--rw-r--r--   0        0        0      360 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/similarity/similarity_nodes.csv
--rw-r--r--   0        0        0      253 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/tarjans8/__init__.py
--rw-r--r--   0        0        0      199 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/tarjans8/tarjans8_edges.csv
--rw-r--r--   0        0        0       21 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/tarjans8/tarjans8_nodes.csv
--rw-r--r--   0        0        0     1493 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/ucav/__init__.py
--rw-r--r--   0        0        0     5183 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/ucav/ucav_edges.csv
--rw-r--r--   0        0        0     1141 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/ucav/ucav_nodes.csv
--rw-r--r--   0        0        0     4372 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/edge.py
--rw-r--r--   0        0        0    23032 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/generic.py
--rw-r--r--   0        0        0    39432 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/graph.py
--rw-r--r--   0        0        0       80 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/io/__init__.py
--rw-r--r--   0        0        0    11755 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/archimate/__init__.py
--rw-r--r--   0        0        0    48350 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/archimate/archimate3_Model.xsd
--rw-r--r--   0        0        0      461 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/archimate/bare.xml
--rw-r--r--   0        0        0     8836 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/archimate/xml.xsd
--rw-r--r--   0        0        0     6745 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/canopy.py
--rw-r--r--   0        0        0    13730 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/csv.py
--rw-r--r--   0        0        0      229 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/esl.py
--rw-r--r--   0        0        0     4146 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/json.py
--rw-r--r--   0        0        0     5081 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/matrix.py
--rw-r--r--   0        0        0     1819 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/xml/XMI-Canonical.xsd
--rw-r--r--   0        0        0     9246 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/io/xml/__init__.py
--rw-r--r--   0        0        0      358 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/io/xml/bare.xml
--rw-r--r--   0        0        0     4332 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/io/xml/ragraph.xsd
--rw-r--r--   0        0        0     1270 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/io/yaml.py
--rw-r--r--   0        0        0     7862 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/node.py
--rw-r--r--   0        0        0     4325 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/__init__.py
--rw-r--r--   0        0        0      507 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/components/__init__.py
--rw-r--r--   0        0        0     1178 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/components/blank.py
--rw-r--r--   0        0        0     3822 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/components/labels.py
--rw-r--r--   0        0        0     9115 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/components/legend.py
--rw-r--r--   0        0        0    20779 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/components/piemap.py
--rw-r--r--   0        0        0     6765 2023-05-02 10:06:24.087176 ragraph-1.17.1/ragraph/plot/components/tree.py
--rw-r--r--   0        0        0    28046 2023-05-02 10:06:24.087176 ragraph-1.17.1/ragraph/plot/generic.py
--rw-r--r--   0        0        0     9811 2023-05-02 10:06:24.087176 ragraph-1.17.1/ragraph/plot/svg.py
--rw-r--r--   0        0        0     9274 2023-05-02 10:06:24.087176 ragraph-1.17.1/ragraph/plot/utils.py
--rw-r--r--   0        0        0     3088 2023-05-02 10:06:24.087176 ragraph-1.17.1/ragraph/utils.py
--rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 ragraph-1.17.1/PKG-INFO
+-rw-r--r--   0        0        0    35400 2023-05-17 09:45:08.443721 ragraph-1.18.0/LICENSE.rst
+-rw-r--r--   0        0        0     1781 2023-05-17 09:45:08.443721 ragraph-1.18.0/README.rst
+-rw-r--r--   0        0        0     2357 2023-05-17 09:45:08.447721 ragraph-1.18.0/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-05-17 09:45:08.447721 ragraph-1.18.0/ragraph/__init__.py
+-rw-r--r--   0        0        0      100 2023-05-17 09:45:08.447721 ragraph-1.18.0/ragraph/analysis/__init__.py
+-rw-r--r--   0        0        0    19876 2023-05-17 09:45:08.447721 ragraph-1.18.0/ragraph/analysis/_classes.py
+-rw-r--r--   0        0        0     7901 2023-05-17 09:45:08.447721 ragraph-1.18.0/ragraph/analysis/_utils.py
+-rw-r--r--   0        0        0     1142 2023-05-17 09:45:08.447721 ragraph-1.18.0/ragraph/analysis/bus/__init__.py
+-rw-r--r--   0        0        0     3743 2023-05-17 09:45:08.447721 ragraph-1.18.0/ragraph/analysis/bus/_gamma.py
+-rw-r--r--   0        0        0     1613 2023-05-17 09:45:08.447721 ragraph-1.18.0/ragraph/analysis/cluster/__init__.py
+-rw-r--r--   0        0        0    13777 2023-05-17 09:45:08.447721 ragraph-1.18.0/ragraph/analysis/cluster/_markov.py
+-rw-r--r--   0        0        0     3438 2023-05-17 09:45:08.447721 ragraph-1.18.0/ragraph/analysis/cluster/_tarjan.py
+-rw-r--r--   0        0        0      503 2023-05-17 09:45:08.447721 ragraph-1.18.0/ragraph/analysis/comparison/__init__.py
+-rw-r--r--   0        0        0     5548 2023-05-17 09:45:08.447721 ragraph-1.18.0/ragraph/analysis/comparison/_delta.py
+-rw-r--r--   0        0        0     4722 2023-05-17 09:45:08.448722 ragraph-1.18.0/ragraph/analysis/comparison/_sigma.py
+-rw-r--r--   0        0        0     1706 2023-05-17 09:45:08.448722 ragraph-1.18.0/ragraph/analysis/comparison/utils.py
+-rw-r--r--   0        0        0    19484 2023-05-17 09:45:08.448722 ragraph-1.18.0/ragraph/analysis/compatibility/__init__.py
+-rw-r--r--   0        0        0     2729 2023-05-17 09:45:08.448722 ragraph-1.18.0/ragraph/analysis/compatibility/bdd.py
+-rw-r--r--   0        0        0     1227 2023-05-17 09:45:08.448722 ragraph-1.18.0/ragraph/analysis/heuristics/__init__.py
+-rw-r--r--   0        0        0     3368 2023-05-17 09:45:08.448722 ragraph-1.18.0/ragraph/analysis/heuristics/_johnson.py
+-rw-r--r--   0        0        0     5157 2023-05-17 09:45:08.448722 ragraph-1.18.0/ragraph/analysis/heuristics/_markov_gamma.py
+-rw-r--r--   0        0        0     1787 2023-05-17 09:45:08.448722 ragraph-1.18.0/ragraph/analysis/sequence/__init__.py
+-rw-r--r--   0        0        0    10956 2023-05-17 09:45:08.448722 ragraph-1.18.0/ragraph/analysis/sequence/_axis.py
+-rw-r--r--   0        0        0     5226 2023-05-17 09:45:08.448722 ragraph-1.18.0/ragraph/analysis/sequence/_genetic.py
+-rw-r--r--   0        0        0     3010 2023-05-17 09:45:08.448722 ragraph-1.18.0/ragraph/analysis/sequence/_markov.py
+-rw-r--r--   0        0        0      840 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/analysis/sequence/_name.py
+-rw-r--r--   0        0        0     3750 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/analysis/sequence/_scc_tearing.py
+-rw-r--r--   0        0        0     1713 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/analysis/sequence/_tarjan.py
+-rw-r--r--   0        0        0     7133 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/analysis/sequence/metrics.py
+-rw-r--r--   0        0        0     5256 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/analysis/sequence/utils.py
+-rw-r--r--   0        0        0     1336 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/analysis/similarity/__init__.py
+-rw-r--r--   0        0        0     3036 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/analysis/similarity/_jaccard.py
+-rw-r--r--   0        0        0     9582 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/analysis/similarity/_similarity.py
+-rw-r--r--   0        0        0     1824 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/analysis/similarity/utils.py
+-rw-r--r--   0        0        0     9963 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/colors/__init__.py
+-rw-r--r--   0        0        0     5320 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/colors/cubehelix.py
+-rw-r--r--   0        0        0      774 2023-05-17 09:45:08.449722 ragraph-1.18.0/ragraph/colors/utils.py
+-rw-r--r--   0        0        0     1663 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/aircraft_engine/__init__.py
+-rw-r--r--   0        0        0    28938 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv
+-rw-r--r--   0        0        0      977 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv
+-rw-r--r--   0        0        0     1035 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/architecture_integral/__init__.py
+-rw-r--r--   0        0        0     1364 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/architecture_integral/architecture_integral_edges.csv
+-rw-r--r--   0        0        0      352 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/architecture_integral/architecture_integral_nodes.csv
+-rw-r--r--   0        0        0     1048 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/architecture_mix/__init__.py
+-rw-r--r--   0        0        0     2264 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/architecture_mix/architecture_mix_edges.csv
+-rw-r--r--   0        0        0      352 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/architecture_mix/architecture_mix_nodes.csv
+-rw-r--r--   0        0        0     1043 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/architecture_modular/__init__.py
+-rw-r--r--   0        0        0     2722 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/architecture_modular/architecture_modular_edges.csv
+-rw-r--r--   0        0        0      351 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/architecture_modular/architecture_modular_nodes.csv
+-rw-r--r--   0        0        0      813 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/climate_control/__init__.py
+-rw-r--r--   0        0        0     5778 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/climate_control/climate_control_edges.csv
+-rw-r--r--   0        0        0      632 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/climate_control/climate_control_nodes.csv
+-rw-r--r--   0        0        0      374 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/climate_control_mg/__init__.py
+-rw-r--r--   0        0        0     5778 2023-05-17 09:45:08.450722 ragraph-1.18.0/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv
+-rw-r--r--   0        0        0     1441 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv
+-rw-r--r--   0        0        0      460 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/compatibility/__init__.py
+-rw-r--r--   0        0        0      564 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/compatibility/compatibility_edges.csv
+-rw-r--r--   0        0        0       83 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/compatibility/compatibility_nodes.csv
+-rw-r--r--   0        0        0      431 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/design/__init__.py
+-rw-r--r--   0        0        0      872 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/design/design_edges.csv
+-rw-r--r--   0        0        0      384 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/design/design_nodes.csv
+-rw-r--r--   0        0        0       57 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/eefde_lock/__init__.py
+-rw-r--r--   0        0        0    24347 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/eefde_lock/eefde_lock_edges.csv
+-rw-r--r--   0        0        0     1047 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/eefde_lock/eefde_lock_nodes.csv
+-rw-r--r--   0        0        0      998 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/elevator175/__init__.py
+-rw-r--r--   0        0        0   103961 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/elevator175/elevator175_edges.csv
+-rw-r--r--   0        0        0     7255 2023-05-17 09:45:08.451722 ragraph-1.18.0/ragraph/datasets/elevator175/elevator175_nodes.csv
+-rw-r--r--   0        0        0      995 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/elevator45/__init__.py
+-rw-r--r--   0        0        0    29033 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/elevator45/elevator45_edges.csv
+-rw-r--r--   0        0        0     1887 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/elevator45/elevator45_nodes.csv
+-rw-r--r--   0        0        0     1148 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/esl/__init__.py
+-rw-r--r--   0        0        0       75 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/esl/pump/__init__.py
+-rw-r--r--   0        0        0     3523 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/esl/pump/pump.esl
+-rw-r--r--   0        0        0     1868 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/ford_hood/__init__.py
+-rw-r--r--   0        0        0    30483 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/ford_hood/ford_hood_edges.csv
+-rw-r--r--   0        0        0     3339 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/ford_hood/ford_hood_nodes.csv
+-rw-r--r--   0        0        0     1461 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/kodak3d/__init__.py
+-rw-r--r--   0        0        0     6660 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/kodak3d/kodak3d_edges.csv
+-rw-r--r--   0        0        0     1134 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/kodak3d/kodak3d_nodes.csv
+-rw-r--r--   0        0        0      216 2023-05-17 09:45:08.452722 ragraph-1.18.0/ragraph/datasets/ledsip/__init__.py
+-rw-r--r--   0        0        0   210027 2023-05-17 09:45:08.453722 ragraph-1.18.0/ragraph/datasets/ledsip/ledsip_edges.csv
+-rw-r--r--   0        0        0    50840 2023-05-17 09:45:08.453722 ragraph-1.18.0/ragraph/datasets/ledsip/ledsip_nodes.csv
+-rw-r--r--   0        0        0       74 2023-05-17 09:45:08.453722 ragraph-1.18.0/ragraph/datasets/localbus/__init__.py
+-rw-r--r--   0        0        0      723 2023-05-17 09:45:08.453722 ragraph-1.18.0/ragraph/datasets/localbus/localbus_edges.csv
+-rw-r--r--   0        0        0       27 2023-05-17 09:45:08.453722 ragraph-1.18.0/ragraph/datasets/localbus/localbus_nodes.csv
+-rw-r--r--   0        0        0       76 2023-05-17 09:45:08.453722 ragraph-1.18.0/ragraph/datasets/overlap/__init__.py
+-rw-r--r--   0        0        0      149 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/overlap/overlap_edges.csv
+-rw-r--r--   0        0        0       15 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/overlap/overlap_nodes.csv
+-rw-r--r--   0        0        0     3167 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/pathfinder/__init__.py
+-rw-r--r--   0        0        0    17741 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/pathfinder/pathfinder_edges.csv
+-rw-r--r--   0        0        0     1084 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/pathfinder/pathfinder_nodes.csv
+-rw-r--r--   0        0        0      307 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/shaja8/__init__.py
+-rw-r--r--   0        0        0      243 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/shaja8/shaja8_edges.csv
+-rw-r--r--   0        0        0       21 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/shaja8/shaja8_nodes.csv
+-rw-r--r--   0        0        0      224 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/similarity/__init__.py
+-rw-r--r--   0        0        0      872 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/similarity/similarity_edges.csv
+-rw-r--r--   0        0        0      360 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/similarity/similarity_nodes.csv
+-rw-r--r--   0        0        0      253 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/tarjans8/__init__.py
+-rw-r--r--   0        0        0      199 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/tarjans8/tarjans8_edges.csv
+-rw-r--r--   0        0        0       21 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/tarjans8/tarjans8_nodes.csv
+-rw-r--r--   0        0        0     1493 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/ucav/__init__.py
+-rw-r--r--   0        0        0     5183 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/ucav/ucav_edges.csv
+-rw-r--r--   0        0        0     1141 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/datasets/ucav/ucav_nodes.csv
+-rw-r--r--   0        0        0     4372 2023-05-17 09:45:08.454722 ragraph-1.18.0/ragraph/edge.py
+-rw-r--r--   0        0        0    23032 2023-05-17 09:45:08.455722 ragraph-1.18.0/ragraph/generic.py
+-rw-r--r--   0        0        0    39432 2023-05-17 09:45:08.455722 ragraph-1.18.0/ragraph/graph.py
+-rw-r--r--   0        0        0       80 2023-05-17 09:45:08.455722 ragraph-1.18.0/ragraph/io/__init__.py
+-rw-r--r--   0        0        0    11755 2023-05-17 09:45:08.455722 ragraph-1.18.0/ragraph/io/archimate/__init__.py
+-rw-r--r--   0        0        0    48350 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/archimate/archimate3_Model.xsd
+-rw-r--r--   0        0        0      461 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/archimate/bare.xml
+-rw-r--r--   0        0        0     8836 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/archimate/xml.xsd
+-rw-r--r--   0        0        0     6745 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/canopy.py
+-rw-r--r--   0        0        0    13730 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/csv.py
+-rw-r--r--   0        0        0      229 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/esl.py
+-rw-r--r--   0        0        0     5925 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/grip.py
+-rw-r--r--   0        0        0     4146 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/json.py
+-rw-r--r--   0        0        0     5081 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/matrix.py
+-rw-r--r--   0        0        0     1819 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/xml/XMI-Canonical.xsd
+-rw-r--r--   0        0        0     9246 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/xml/__init__.py
+-rw-r--r--   0        0        0      358 2023-05-17 09:45:08.456722 ragraph-1.18.0/ragraph/io/xml/bare.xml
+-rw-r--r--   0        0        0     4332 2023-05-17 09:45:08.457722 ragraph-1.18.0/ragraph/io/xml/ragraph.xsd
+-rw-r--r--   0        0        0     1270 2023-05-17 09:45:08.457722 ragraph-1.18.0/ragraph/io/yaml.py
+-rw-r--r--   0        0        0     7862 2023-05-17 09:45:08.457722 ragraph-1.18.0/ragraph/node.py
+-rw-r--r--   0        0        0     4325 2023-05-17 09:45:08.457722 ragraph-1.18.0/ragraph/plot/__init__.py
+-rw-r--r--   0        0        0      507 2023-05-17 09:45:08.457722 ragraph-1.18.0/ragraph/plot/components/__init__.py
+-rw-r--r--   0        0        0     1178 2023-05-17 09:45:08.457722 ragraph-1.18.0/ragraph/plot/components/blank.py
+-rw-r--r--   0        0        0     3822 2023-05-17 09:45:08.457722 ragraph-1.18.0/ragraph/plot/components/labels.py
+-rw-r--r--   0        0        0     9115 2023-05-17 09:45:08.457722 ragraph-1.18.0/ragraph/plot/components/legend.py
+-rw-r--r--   0        0        0    20779 2023-05-17 09:45:08.457722 ragraph-1.18.0/ragraph/plot/components/piemap.py
+-rw-r--r--   0        0        0     6765 2023-05-17 09:45:08.457722 ragraph-1.18.0/ragraph/plot/components/tree.py
+-rw-r--r--   0        0        0    28046 2023-05-17 09:45:08.458722 ragraph-1.18.0/ragraph/plot/generic.py
+-rw-r--r--   0        0        0     9811 2023-05-17 09:45:08.458722 ragraph-1.18.0/ragraph/plot/svg.py
+-rw-r--r--   0        0        0     9274 2023-05-17 09:45:08.458722 ragraph-1.18.0/ragraph/plot/utils.py
+-rw-r--r--   0        0        0     3088 2023-05-17 09:45:08.458722 ragraph-1.18.0/ragraph/utils.py
+-rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 ragraph-1.18.0/PKG-INFO
```

### Comparing `ragraph-1.17.1/LICENSE.rst` & `ragraph-1.18.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/README.rst` & `ragraph-1.18.0/README.rst`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/pyproject.toml` & `ragraph-1.18.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ragraph"
-version = "1.17.1"
+version = "1.18.0"
 description = "Ratio graph handling in Python."
 authors = ["Ratio Innovations B.V. <info@ratio-case.nl>"]
 license = "GPL-3.0-or-later"
 documentation = "https://ragraph.ratio-case.nl"
 readme = "README.rst"
 repository = "https://gitlab.com/ratio-case-os/python/ragraph"
 homepage = "https://ragraph.ratio-case.nl"
```

### Comparing `ragraph-1.17.1/ragraph/analysis/_classes.py` & `ragraph-1.18.0/ragraph/analysis/_classes.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/_utils.py` & `ragraph-1.18.0/ragraph/analysis/_utils.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/bus/__init__.py` & `ragraph-1.18.0/ragraph/analysis/bus/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/bus/_gamma.py` & `ragraph-1.18.0/ragraph/analysis/bus/_gamma.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/cluster/__init__.py` & `ragraph-1.18.0/ragraph/analysis/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/cluster/_markov.py` & `ragraph-1.18.0/ragraph/analysis/cluster/_markov.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/cluster/_tarjan.py` & `ragraph-1.18.0/ragraph/analysis/cluster/_tarjan.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/comparison/_delta.py` & `ragraph-1.18.0/ragraph/analysis/comparison/_delta.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/comparison/_sigma.py` & `ragraph-1.18.0/ragraph/analysis/comparison/_sigma.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/comparison/utils.py` & `ragraph-1.18.0/ragraph/analysis/comparison/utils.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/compatibility/__init__.py` & `ragraph-1.18.0/ragraph/analysis/compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/compatibility/bdd.py` & `ragraph-1.18.0/ragraph/analysis/compatibility/bdd.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/heuristics/__init__.py` & `ragraph-1.18.0/ragraph/analysis/heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/heuristics/_johnson.py` & `ragraph-1.18.0/ragraph/analysis/heuristics/_johnson.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/heuristics/_markov_gamma.py` & `ragraph-1.18.0/ragraph/analysis/heuristics/_markov_gamma.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/sequence/__init__.py` & `ragraph-1.18.0/ragraph/analysis/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/sequence/_axis.py` & `ragraph-1.18.0/ragraph/analysis/sequence/_axis.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/sequence/_genetic.py` & `ragraph-1.18.0/ragraph/analysis/sequence/_genetic.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/sequence/_markov.py` & `ragraph-1.18.0/ragraph/analysis/sequence/_markov.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/sequence/_name.py` & `ragraph-1.18.0/ragraph/analysis/sequence/_name.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/sequence/_scc_tearing.py` & `ragraph-1.18.0/ragraph/analysis/sequence/_scc_tearing.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/sequence/_tarjan.py` & `ragraph-1.18.0/ragraph/analysis/sequence/_tarjan.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/sequence/metrics.py` & `ragraph-1.18.0/ragraph/analysis/sequence/metrics.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/sequence/utils.py` & `ragraph-1.18.0/ragraph/analysis/sequence/utils.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/similarity/__init__.py` & `ragraph-1.18.0/ragraph/analysis/similarity/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/similarity/_jaccard.py` & `ragraph-1.18.0/ragraph/analysis/similarity/_jaccard.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/similarity/_similarity.py` & `ragraph-1.18.0/ragraph/analysis/similarity/_similarity.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/analysis/similarity/utils.py` & `ragraph-1.18.0/ragraph/analysis/similarity/utils.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/colors/__init__.py` & `ragraph-1.18.0/ragraph/colors/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/colors/cubehelix.py` & `ragraph-1.18.0/ragraph/colors/cubehelix.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/colors/utils.py` & `ragraph-1.18.0/ragraph/colors/utils.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/__init__.py` & `ragraph-1.18.0/ragraph/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/aircraft_engine/__init__.py` & `ragraph-1.18.0/ragraph/datasets/aircraft_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv` & `ragraph-1.18.0/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv` & `ragraph-1.18.0/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/architecture_integral/__init__.py` & `ragraph-1.18.0/ragraph/datasets/architecture_integral/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/architecture_integral/architecture_integral_edges.csv` & `ragraph-1.18.0/ragraph/datasets/architecture_integral/architecture_integral_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/architecture_mix/__init__.py` & `ragraph-1.18.0/ragraph/datasets/architecture_mix/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/architecture_mix/architecture_mix_edges.csv` & `ragraph-1.18.0/ragraph/datasets/architecture_mix/architecture_mix_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/architecture_modular/__init__.py` & `ragraph-1.18.0/ragraph/datasets/architecture_modular/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/architecture_modular/architecture_modular_edges.csv` & `ragraph-1.18.0/ragraph/datasets/architecture_modular/architecture_modular_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/climate_control/__init__.py` & `ragraph-1.18.0/ragraph/datasets/climate_control/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/climate_control/climate_control_edges.csv` & `ragraph-1.18.0/ragraph/datasets/climate_control/climate_control_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/climate_control/climate_control_nodes.csv` & `ragraph-1.18.0/ragraph/datasets/climate_control/climate_control_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv` & `ragraph-1.18.0/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv` & `ragraph-1.18.0/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/compatibility/compatibility_edges.csv` & `ragraph-1.18.0/ragraph/datasets/compatibility/compatibility_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/design/design_edges.csv` & `ragraph-1.18.0/ragraph/datasets/design/design_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/eefde_lock/eefde_lock_edges.csv` & `ragraph-1.18.0/ragraph/datasets/eefde_lock/eefde_lock_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/eefde_lock/eefde_lock_nodes.csv` & `ragraph-1.18.0/ragraph/datasets/eefde_lock/eefde_lock_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/elevator175/__init__.py` & `ragraph-1.18.0/ragraph/datasets/elevator175/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/elevator175/elevator175_edges.csv` & `ragraph-1.18.0/ragraph/datasets/elevator175/elevator175_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/elevator175/elevator175_nodes.csv` & `ragraph-1.18.0/ragraph/datasets/elevator175/elevator175_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/elevator45/__init__.py` & `ragraph-1.18.0/ragraph/datasets/elevator45/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/elevator45/elevator45_edges.csv` & `ragraph-1.18.0/ragraph/datasets/elevator45/elevator45_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/elevator45/elevator45_nodes.csv` & `ragraph-1.18.0/ragraph/datasets/elevator45/elevator45_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/esl/__init__.py` & `ragraph-1.18.0/ragraph/datasets/esl/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/esl/pump/pump.esl` & `ragraph-1.18.0/ragraph/datasets/esl/pump/pump.esl`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/ford_hood/__init__.py` & `ragraph-1.18.0/ragraph/datasets/ford_hood/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/ford_hood/ford_hood_edges.csv` & `ragraph-1.18.0/ragraph/datasets/ford_hood/ford_hood_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/ford_hood/ford_hood_nodes.csv` & `ragraph-1.18.0/ragraph/datasets/ford_hood/ford_hood_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/kodak3d/__init__.py` & `ragraph-1.18.0/ragraph/datasets/kodak3d/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/kodak3d/kodak3d_edges.csv` & `ragraph-1.18.0/ragraph/datasets/kodak3d/kodak3d_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/kodak3d/kodak3d_nodes.csv` & `ragraph-1.18.0/ragraph/datasets/kodak3d/kodak3d_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/ledsip/ledsip_edges.csv` & `ragraph-1.18.0/ragraph/datasets/ledsip/ledsip_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/ledsip/ledsip_nodes.csv` & `ragraph-1.18.0/ragraph/datasets/ledsip/ledsip_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/localbus/localbus_edges.csv` & `ragraph-1.18.0/ragraph/datasets/localbus/localbus_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/pathfinder/__init__.py` & `ragraph-1.18.0/ragraph/datasets/pathfinder/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/pathfinder/pathfinder_edges.csv` & `ragraph-1.18.0/ragraph/datasets/pathfinder/pathfinder_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/pathfinder/pathfinder_nodes.csv` & `ragraph-1.18.0/ragraph/datasets/pathfinder/pathfinder_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/similarity/similarity_edges.csv` & `ragraph-1.18.0/ragraph/datasets/similarity/similarity_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/ucav/__init__.py` & `ragraph-1.18.0/ragraph/datasets/ucav/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/ucav/ucav_edges.csv` & `ragraph-1.18.0/ragraph/datasets/ucav/ucav_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/datasets/ucav/ucav_nodes.csv` & `ragraph-1.18.0/ragraph/datasets/ucav/ucav_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/edge.py` & `ragraph-1.18.0/ragraph/edge.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/generic.py` & `ragraph-1.18.0/ragraph/generic.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/graph.py` & `ragraph-1.18.0/ragraph/graph.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/io/archimate/__init__.py` & `ragraph-1.18.0/ragraph/io/archimate/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/io/archimate/archimate3_Model.xsd` & `ragraph-1.18.0/ragraph/io/archimate/archimate3_Model.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/io/archimate/xml.xsd` & `ragraph-1.18.0/ragraph/io/archimate/xml.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/io/canopy.py` & `ragraph-1.18.0/ragraph/io/canopy.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/io/csv.py` & `ragraph-1.18.0/ragraph/io/csv.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/io/json.py` & `ragraph-1.18.0/ragraph/io/json.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/io/matrix.py` & `ragraph-1.18.0/ragraph/io/matrix.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/io/xml/XMI-Canonical.xsd` & `ragraph-1.18.0/ragraph/io/xml/XMI-Canonical.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/io/xml/__init__.py` & `ragraph-1.18.0/ragraph/io/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/io/xml/ragraph.xsd` & `ragraph-1.18.0/ragraph/io/xml/ragraph.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/io/yaml.py` & `ragraph-1.18.0/ragraph/io/yaml.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/node.py` & `ragraph-1.18.0/ragraph/node.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/plot/__init__.py` & `ragraph-1.18.0/ragraph/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/plot/components/blank.py` & `ragraph-1.18.0/ragraph/plot/components/blank.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/plot/components/labels.py` & `ragraph-1.18.0/ragraph/plot/components/labels.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/plot/components/legend.py` & `ragraph-1.18.0/ragraph/plot/components/legend.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/plot/components/piemap.py` & `ragraph-1.18.0/ragraph/plot/components/piemap.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/plot/components/tree.py` & `ragraph-1.18.0/ragraph/plot/components/tree.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/plot/generic.py` & `ragraph-1.18.0/ragraph/plot/generic.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/plot/svg.py` & `ragraph-1.18.0/ragraph/plot/svg.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/plot/utils.py` & `ragraph-1.18.0/ragraph/plot/utils.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/ragraph/utils.py` & `ragraph-1.18.0/ragraph/utils.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.1/PKG-INFO` & `ragraph-1.18.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragraph
-Version: 1.17.1
+Version: 1.18.0
 Summary: Ratio graph handling in Python.
 Home-page: https://ragraph.ratio-case.nl
 License: GPL-3.0-or-later
 Author: Ratio Innovations B.V.
 Author-email: info@ratio-case.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

